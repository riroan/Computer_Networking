## 1.1.1 구성요소로 본 인터넷

### 인터넷

수십억 개의 컴퓨팅 장치를 연결하는 컴퓨터 네트워크

컴퓨팅 장치: 데스크톱 PC, 리눅스 워크스테이션, 서버, 스마트폰, 태블릿

컴퓨팅 장치는 **호스트**(host), **종단 시스템**(end system)이라고도 한다.

### 종단 시스템

종단 시스템은 통신 링크(communication link), 패킷 스위치(packet switch)의 네트워크로 연결된다.

통신 링크: 동축케이블, 구리선, 광케이블, 라디오 스펙트럼

단위는 bps (bit per second)

### 패킷

네트워크로 보내는 데이터 단위

데이터를 **세그먼트**로 나누고 해당 세그먼트에 **헤더**를 붙여 **패킷**으로 만든다.

### 패킷 스위치

패킷을 전달하는 장치, **라우터**와 **링크 계층 스위치**를 가장 많이 사용한다.

패킷이 송신 종단 시스템에서 수신 종단 시스템까지 거쳐온 통신 링크와 패킷 스위치를 **경로**(route, path)라고 한다.

### ISP

종단 시스템은 ISP(Internet Service Provider)로부터 네트워크 접속을 제공받는다.

ISP는 회사, 가정, 법인, 대학등에 인터넷 접속을 제공하며 KT, SK 브로드밴드, LG U+가 있다. ([참고](https://namu.wiki/w/%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EC%A0%9C%EA%B3%B5%EC%82%AC%EC%97%85%EC%9E%90))

각 ISP는 패킷 스위치와 통신 링크로 이루어진 네트워크이다.

ISP도 상위 ISP에 의해 연결된다.
