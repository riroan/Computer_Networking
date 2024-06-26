## 1.3.1 패킷 교환

### 패킷

네트워크 애플리케이션에서 종단 시스템은 서로 **메시지**(message)를 교환한다.

송신지에서 긴 메시지를 **패킷**(packet)이라고 하는 작은 데이터로 나누어 보내고 수신지에서 패킷을 다시 메시지로 조합한다.

메시지 송신 과정에서 패킷은 **패킷 스위치**(packet switch, 라우터와 링크 계층 스위치)와 **통신 링크**를 거치게 된다.

이 때, 패킷이 전송되는 속도는 통신 링크의 최대 전송률과 같다.

### 저장 후 전달

**저장 후 전달 전송**(store-and-forward transmission)은 스위치에서 패킷의 모든 비트를 수신(store)한 후에만 출력 링크로 전송(forward)한다.

패킷 비트가 $L$, 통신 링크 속도가 $R$이고 송신지와 수신지 사이에 라우터가 $N-1$개 있다면(통신 링크는 $N$개) 데이터를 보내는데 걸리는 지연 시간은 $d = N \frac{L}{R}$이다.

### 큐잉 지연과 패킷 손실

패킷 스위치는 다음 통신 링크로 송신하기 위해 **출력 버퍼**(output buffer, output queue)를 가지고 있다. 송신하려는 링크에 다른 패킷이 송신중이라면 출력 버퍼에 임시적으로 저장하고 대기한다.

패킷이 출력 버퍼에서 대기하는 시간을 **큐잉 지연**(queuing delay)이라고 한다.

버퍼 공간은 제한적이므로 버퍼가 패킷으로 꽉 찬 경우 **패킷 손실**(packet loss)이 발생한다.

### 포워딩 테이블

라우터는 **포워딩 테이블**(forwarding table)을 사용하여 받은 패킷을 어느 통신 링크로 전달할지 결정한다. 패킷에 수신지의 IP주소가 있으므로 해당 주소를 포워딩 테이블에 검색하여 나온 출력 링크로 전달한다.

### 라우팅 프로토콜

**라우팅 프로토콜**(routing protocol)은 각 라우터가 포워딩 테이블을 설정하는 규칙이다.

### 패킷 교환의 장점

- 회선 교환보다 전송 용량 공유에 더 효율적이다.
- 더 간단하고 효율적이며 구현 비용이 적다.

### 패킷 교환의 단점

- 예측할 수 없는 종단 간 지연 때문에 실시간 서비스에서 불리하다.
