## 2.2.1 HTTP 개요

### HTTP

**HTTP**(HyperText Transfer Protocol)는 클라이언트와 서버 프로그램으로 구현된다. 두 프로그램은 HTTP 메시지를 교환하여 통신한다.

HTTP는 TCP를 사용하여 통신한다.

HTTP 서버는 클라이언트의 정보를 저장하지 않으므로 **비상태 프로토콜**(stateless protocol)이라고 한다.

### 웹 페이지

**웹 페이지**(web-page)는 기본 HTML파일과 이미지나 텍스트같은 참조 객체들로 이루어진다. 기본 HTML은 페이지 내부의 다른 객체를 URL로 참조한다.

`http://www.abc.com/abcd` 라는 URL이 있으면 `http://www.abc.com`은 호스트 이름이고 `/abcd`는 객체의 경로이다.

### 웹 브라우저

**웹 브라우저**(web-browser)는 HTTP의 클라이언트를 구현한 것이다.

### 웹 서버

**웹 서버**(web-server)는 HTTP의 서버를 구현한 것이다.
