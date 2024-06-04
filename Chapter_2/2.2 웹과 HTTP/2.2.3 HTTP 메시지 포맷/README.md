## 2.2.3 HTTP 메시지 포맷

### HTTP 요청 메시지

```
GET /somedir/page.html HTTP/1.1
Host: www.someschool.edu
Connection: close
User-agent: Mozilla/5.0
Accept-language: fr

<<entity body>>
```

### HTTP 요청 메시지 특징

- ASCII 텍스트로 쓰여 있어 사람이 읽을 수 있다.
- 각 줄은 CR/LF로 구분된다.
- 요청 메시지의 첫 줄은 **요청 라인**(request line)이라고 한다.
- 요청 메시지의 나머지 줄은 **헤더 라인**(header line)이라고 한다.
- 헤더 라인 이후 공백을 한 줄 띄우고 body를 넣는다. 이는 GET에서는 비어있고 POST에서 사용된다.

### HTTP 응답 메시지

```
HTTP/1.1 200 OK
Connection: close
Date: Tue, 018 Aug 2015 15:44:04 GMT
Server: Apache/2.2.3 (CentOS)
Last-Modified: Tue, 18 Aug 2015 15:11:03 GMT
Content-Length: 6821
Content-Type: text/html

<<data>>
```

### HTTP 응답 메시지 특징

- 응답 메시지의 첫 줄은 **상태 라인**(status line)이라고 한다.
- 응답 메시지의 나머지 줄은 **헤더 라인**(header line)이라고 한다.
- 헤더 라인 이후 공백을 한 줄 띄우고 body를 넣는다.

