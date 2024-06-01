## 1.3.3 네트워크의 네트워크

### 네트워크의 네트워크

ISP가 종단 시스템을 연결하는 것처럼 ISP도 무언가에 의해 연결되어야 한다. 이를 **네트워크의 네트워크**(network of network)라고 한다.

한 가지 방법은 ISP를 다른 ISP로 연결시키는 것이다. 여기서 ISP를 연결하는 ISP를 **글로벌 ISP**(global ISP)라고 한다.

### 네트워크 구조 1

모든 ISP를 하나의 글로벌 ISP와 연결한 구조

### 네트워크 구조 2

네트워크 구조 1에서 글로벌 ISP가 여러 개인 구조, 다중 글로벌 ISP라고 한다.

사용자는 여러 글로벌 ISP에서 가격과 서비스를 비교하며 선택할 수 있다.

### 네트워크 구조 3

ISP를 계층화한 구조

접속 ISP -> 지역 ISP -> 글로벌 ISP 같이 다중계층구조를 이루며 오늘날의 인터넷과 유사하다.

### 네트워크 구조 4

네트워크 구조 3에서 PoP(points of presence), 멀티홈(multi-homing), 피어링(peering), IXP(Internet exchange point)를 추가한 구조

PoP: 네트워크 내에 있는 하나 이상의 접속점, 모든 계층에 존재한다. [참고](http://www.ktword.co.kr/test/view/view.php?no=1759)

멀티홈: 네트워크 상의 한 노드가 여러 네트워크에 연결하는 형상 [참고](http://www.ktword.co.kr/test/view/view.php?no=3118)

피어링: 상위 계층 ISP를 통하지 않고 같은 계층의 ISP에 송수신할 수 있도록 연결

IXP: 다중 ISP들이 피어링하여 만나는 장소

### 네트워크 구조 5

네트워크 구조 4에서 **콘텐츠 제공자 네트워크**(content-provider network)가 추가된 구조

현재 구글에서 콘텐츠 제공자 네트워크를 제공하고 하위 ISP와 직접 연결한다.
