
  # 푸드팡 파트너 API

  푸드팡 파트너사를 위한 주문 연동 API 문서입니다.

  ## 시작하기

  API 사용을 위해 푸드팡에서 발급해드린 `API Key`와 `API Secret`을 준비하세요.
  모든 요청은 `Content-Type: application/json`을 사용합니다.

  ## 인증

  두 가지 방식 중 하나를 선택해 사용합니다.

  **Basic Auth (권장)**
  Authorization: Basic base64(keyId:secret)

  **Custom Header**
  X-Api-Key: pac_xxx
  X-Api-Secret: pas_xxx

  ## 제공 기능

  | 기능 | 설명 |
  |------|------|
  | 인증 확인 | 발급된 키로 인증 상태 확인 |
  | 상품 조회 | 주문 가능한 상품 목록 조회 |
  | 주문 생성 | 상품을 선택해 주문 등록 |

  ## 참고

  - [에러코드](error-codes.md) — 응답 코드별 의미 확인
  - API 버전: `v1`
  - Base URL

  | 환경 | URL |
  |------|-----|
  | Production | `https://admin.foodpang.co/admin/api/partner/v1` |
  | TEST | `https://inhouse.foodpang.co/pa/api/partner/v1` |
  
  Base URL은 실제 운영 URL로 맞춰주세요.