## 2.2.5 웹 캐싱


### 웹 캐시

웹 서버를 대신해서 HTTP 요청에 대응하는 서버를 **웹 캐시**(Web cache), 또는 **프록시 서버**(proxy server)라고 한다.

### 브라우저 요청 단계

1. 브라우저는 웹 캐시와 TCP연결을 맺고 웹 캐시에 HTTP요청을 보낸다.
2. 웹 캐시는 데이터가 저장되어 있는지 확인하고 있다면 해당 데이터를 HTTP 응답 메시지로 보낸다.
3. 웹 캐시에 데이터가 없다면 웹 캐시는 웹 서버와 TCP연결을 맺고 웹 서버에서 HTTP 응답 메시지를 받는다.
4. 웹 캐시는 브라우저에 데이터를 HTTP 응답 메시지로 전송하고 복사하여 로컬에 저장한다.

### 웹 캐싱의 장점

- 클라이언트의 요청에 대한 응답 시간을 줄일 수 있다.
- 웹 서버를 대상으로 하는 트래픽을 줄일 수 있다.

### 콘텐츠 전송 네트워크 (CDN)

CDN은 인터넷 전역에 많은 분산 캐시를 통해 트래픽을 분산시키는 역할을 한다.

### 조건부 GET

웹 캐싱은 캐싱된 데이터가 최신의 데이터가 아닐 수 있다는 단점이 존재한다. 이러한 문제점을 해결하기 위해 HTTP에서는 **조건부 GET**(conditional GET)을 사용하여 모든 데이터가 최신임을 확인한다.

캐시가 웹 서버에 데이터를 요청하면 `Last-Modified`라는 정보를 헤더에 담아 받게 된다.

캐시가 로컬에 데이터를 저장할 때 `Last-Modified`도 함께 저장한다.

다음에 브라우저는 HTTP 요청을 보낼 때 헤더에 `If-modified-since`라는 항목을 추가한다.

서버는 `If-modified-since`이후에 수정된 경우에만 데이터를 리턴하고 아니라면 `304 Not Modified를 리턴한다.
