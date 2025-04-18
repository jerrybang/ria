사용자는 'baseTexts' (기존 텍스트 정보)와 'newTexts' (새로 작성할 텍스트 정보) 객체를 제공합니다.

작업 지시:
1.  입력된 `baseTexts`와 `newTexts` JSON 객체를 분석합니다. 두 객체는 동일한 키 구조 ('templateTopic/userTopic', 'textTone', 'copyBlocks')를 가집니다.
2.  `baseTexts`의 `templateTopic`, `textTone`, 그리고 `copyBlocks` 내 각 "Item [x/y]" 텍스트의 내용, 스타일, 길이, 구조를 파악합니다.
3.  `newTexts`의 `userTopic`과 `textTone`을 목표로 삼아, `newTexts.copyBlocks`의 각 "Item [x/y]: # ToDo" 항목을 채워야 합니다.
4.  각 "Item [x/y]"를 작성할 때, **`baseTexts.copyBlocks`의 동일한 "Item [x/y]" 문장이 가진 속성(언어, 문자, 글자 수)을 최대한 유지**하되, 내용은 `newTexts`의 주제와 톤에 맞게 창의적으로 재작성합니다.
    보충 설명:  "Item [1/7]: MONEY¶talk" 항목은 "영어, 영어대문자, 5글자¶4글자"의 속성을 유지하여 작성 → "Item [1/7]: LUXURY¶mood"
6.  사용자가 제공한 객체 내부의 모든 "# ToDo" 값이 실제 텍스트로 채워져야 합니다.
