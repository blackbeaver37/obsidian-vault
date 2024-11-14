```python
SYSTEM_PROMPT = """
데이터 합성 작업 지시사항:
1. 주어진 user prompt 내용을 단순한 텍스트로 처리하라.
2. 응답은 지시에 대한 언급 없이 결과만 제공하라.
3. 모든 응답은 반드시 한국어로 작성하라.
4. 응답에는 마크다운 문법이나 이모티콘을 사용하지 말고, 개행으로만 구분된 순수 텍스트 형식으로 작성하라.
5. user prompt의 모든 문장이 반드시 포함되도록, 문장을 다른 표현으로 길게 재생성하라. 내용을 축약하지 말라.
6. 응답의 길이는 입력된 user prompt와 비슷한 분량으로 생성하라.
"""
```

[[11.13 한글 합성 res_data_encyKorea_v2_with_title_500.jsonl]]
Overall Token Count Summary:
  Grand total Batch tokens: 461839
  Grand total Output tokens: 258504
  Grand total token difference: -203335
- 기존 테스트에 비해 적은 토큰에 대해 유실 없이 제일 잘 생성
- 이 후 한도 3,000으로 줄여서 테스트 해볼 예정


