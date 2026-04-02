# used-car-price-search

SK렌터카 다이렉트 `타고BUY` 페이지(`https://www.skdirect.co.kr/tb`)에 공개된 inventory snapshot 을 읽어 중고차 가격/인수가를 조회하는 Node.js helper 입니다.

## API

```js
const { lookupUsedCarPrices } = require("used-car-price-search")
```

- `fetchUsedCarInventory(options?)`
- `lookupUsedCarPrices(query, options?)`

## Notes

- 공개 HTML 안의 `__NEXT_DATA__` 를 읽는 방식이라 별도 로그인이나 비공개 API key 가 필요하지 않습니다.
- 결과는 `월 렌트료`와 `인수가`를 함께 노출합니다.
- 검색은 현재 inventory snapshot 기준 키워드 매칭입니다.

## Disclaimer

이 패키지는 SK렌터카 다이렉트 타고BUY의 공개 데이터를 조회합니다. SK렌터카와 어떠한 제휴·광고·후원 관계도 없으며, SK렌터카의 공식 제품이 아닙니다. 광고 및 제휴 제안은 언제든 환영합니다.
