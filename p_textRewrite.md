사용자는 'baseTexts' (기존 텍스트 정보)와 'newTexts' (새로 작성할 텍스트 정보) 객체를 제공합니다.

작업 지시:
1.  입력된 `baseTexts`와 `newTexts` JSON 객체를 분석합니다. 두 객체는 동일한 키 구조 ('templateTopic/userTopic', 'textTone', 'copyBlocks')를 가집니다.
2.  `baseTexts`의 `templateTopic`, `textTone`, 그리고 `copyBlocks` 내 각 "Item [x/y]" 텍스트의 내용, 스타일, 길이, 구조를 파악합니다.
3.  `newTexts`의 `userTopic`과 `textTone`을 목표로 삼아, `newTexts.copyBlocks`의 각 "Item [x/y]: # ToDo" 항목을 채워야 합니다.
4.  각 "Item [x/y]"를 작성할 때, **`baseTexts.copyBlocks`의 동일한 "Item [x/y]" 텍스트**를 참고하여 스타일, 글자 수, 문장 구조를 최대한 유지하되, 내용은 `newTexts`의 주제와 톤에 맞게 창의적으로 재작성합니다. **기존 표현을 그대로 사용하지 마세요.**
5.  결과는 반드시 사용자가 요청한 특정 JSON 형식 ('newTexts' 키 포함)으로 반환해야 합니다. 'copyBlocks' 배열의 모든 "# ToDo" 값이 실제 텍스트로 채워져야 합니다.
6.  'copyBlocks' 배열 내 각 텍스트 항목 앞에는 반드시 "Item [x/y]:" 포맷을 유지해야 합니다.
7.  JSON 데이터 외에 다른 텍스트나 마크다운 코드블록을 포함하지 마세요. 
