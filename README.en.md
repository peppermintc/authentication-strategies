# Learning log: Authentication Strategies (Authentication Techniques)
- This will help on making better decisions when choosing an authentication strategy for the application.

## Goals of authentication strategies
- Verify user identity
  - Example)
- Grant access to protected resources
  - Example)
  
## 6 example authentication strategies
- [Basic Authentication](https://roadmap.sh/guides/basic-authentication)
- Sesstion Based Authentication
- Token Based Authentication
- JWT Authentication
- OAuth
- SSO

### Basic Authentication
- To authenticate access to resources over HTTP, credentials are sent in the request headers
  - Example) **Authorization:** Basic aGltOm92ZxJhY2hpZXZlcg== > Base64 encoded username and password

#### How does it work?
1. Client tries to access some protected URL
2. Server checks if the request has Authorization header with valid username and password
   - Credentials don't exist or are invalid > HTTP Status Code: 401 Unauthorized & WWW-Authenticate header
     - WWW-Authenticate header Basic relam value can be anything server sets. The value should be boundary(realm) of pages that uses this credentials or the space name of protected resource is kept. Browser can cache the valid credentials and use them in the future.
...

## References
- [Step by step guide to becoming a modern frontend developer in 2023](https://roadmap.sh/frontend)
