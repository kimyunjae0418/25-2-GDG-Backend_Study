1. Spring Boot 애플리케이션을 실행하고, 브라우저에 localhost:8080 을 입력했을 때 나오는 Whitelabel Error Page 스크린샷
<img width="845" height="961" alt="스크린샷 2025-09-30 오후 5 50 30" src="https://github.com/user-attachments/assets/15a71c57-36a0-4914-9266-fe29cde78612" />

2. 작성한 온라인 쇼핑몰 프로젝트 API 명세서
# 상품(Product)
- POST   /products
- GET    /products
- GET    /products/{productId}
- PATCH  /products/{productId}
- DELETE /products/{productId}

# 주문(Order)
- POST   /orders
- GET    /orders
- GET    /orders/{orderId}
- POST   /orders/{orderId}/cancel
