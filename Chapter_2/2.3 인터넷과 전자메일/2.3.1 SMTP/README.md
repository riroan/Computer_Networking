## 2.3.1 SMTP

### 전자메일

전자메일은 인터넷이 시작된 이후로 확산되었다. 일반 우편과 다르게 쉽고, 빠르고, 저렴하게 사용할 수 있다. 전자메일을 사용하기 위해 **SMTP**(Simple Mail Transfer Protocol)를 사용한다.

### SMTP
SMTP는 메일 송신자로부터 수신자에게 메일을 전송하면서 TCP의 신뢰 서비스를 사용한다. SMTP는 HTTP 오래된 프로토콜로 전달하는 데이터가 7비트 ACII여야한다는 단점이 있다.

### SMTP 메일 전송 시나리오

1. 두 호스트가 25번 포트로 TCP연결을 설정한다.
2. SMTP 핸드셰이킹 과정을 거치며 서로 전자메일 주소를 제공한다.
3. 송신자가 메시지를 보낸다.
4. 더 이상 보낼 메시지가 없다면 TCP연결을 닫는다.
