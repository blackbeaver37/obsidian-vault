```python
SYSTEM_PROMPT = """
데이터 합성 작업 지시사항:
1. 주어진 user prompt 내용을 단순한 텍스트로 처리하라.
2. 응답은 지시에 대한 언급 없이 결과만 제공하라.
3. 모든 응답은 반드시 한국어로 작성하라.
4. 응답에는 마크다운 문법이나 이모티콘을 사용하지 말고, 개행으로만 구분된 순수 텍스트 형식으로 작성하라.
5. user prompt의 모든 문장과 단어가 포함되도록, 문장을 다른 표현으로 길게 재생성하라. 내용을 축약하지 말고 모든 세부 사항과 예시를 포함하여 순서도 유지하라.
6. 응답의 길이는 입력된 user prompt보다 많은 분량으로 생성하라.
7. 중요하지 않은 부분이라도 생략하지 말고, user prompt의 모든 내용을 최대한 충실하게 포함하라.
8. 백과사전 내용을 누군가에게 설명하듯이 명확하고 이해하기 쉽게 표현하라.
"""
```
```python
MAX_INPUT_TOKENS = 15_000
TEMPERATURE_VALUE = 0
TOP_P_VALUE = 0.9
```


[[11.13 한글 합성 res_data_encyKorea_v2_with_title_500.jsonl]]
Overall Token Count Summary:
  Grand total Batch tokens: 461839
  Grand total Output tokens: 258504
  Grand total token difference: -203335
- 기존 테스트에 비해 적은 토큰에 대해 유실 없이 제일 잘 생성

한도 3,000 temperature 0.2
Overall Token Count Summary:
  Grand total Batch tokens: 461840
  Grand total Output tokens: 394524
  Grand total token difference: -67316

한도 15,000 temperature 0
Overall Token Count Summary:
  Grand total Batch tokens: 461839
  Grand total Output tokens: 386181
  Grand total token difference: -75658

프롬프트 수정 (생략하지 않도록) -> model-10
Overall Token Count Summary:
  Grand total Batch tokens: 461839
  Grand total Output tokens: 448258
  Grand total token difference: -13581

프롬프트 수정 (백과사전이고 설명하는걸로 바꿔달라)
Overall Token Count Summary:
  Grand total Batch tokens: 461839
  Grand total Output tokens: 432650
  Grand total token difference: -29189
