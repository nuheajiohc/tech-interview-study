# 🌐 네트워크

## 1. OSI 7계층은 네트워크에서 통신이 일어나는 과정을 7단계로 나눈 것입니다. 이 때 계층을 나눈 이유는 무엇일까요?
<details>
<summary>1번 정답</summary>
<div markdown="1">      
중요한 목적은 표준과 학습 도구라 할 수 있다.<br>
표준화를 통해 이질적인 포트 문제나 프로토콜 등으로 인한 문제를 해결하여 비용을 절감했다.<br>
또한, 계층별의 기능과 통신 과정을 단계별로 나누어서 쉽게 알 수 있고, <strong><em>특정한 곳에 이상이 생기면 그 단계만 수정할 수 있기 때문에 편리하다.</em></strong><br>
<a href="https://github.com/WooVictory/Ready-For-Tech-Interview/blob/master/Network/OSI%207%20%EA%B3%84%EC%B8%B5.md">참고1</a>
<a href="https://steady-coding.tistory.com/504">참고2</a>
</div>
</details>
<hr>

## 2. OSI 계층에서 전송 계층에 속하는 프로토콜과 전송 계층의 역할에 대해 말해보세요.
<details>
<summary>2번 정답</summary>
<div markdown="1">      
<strong>TCP/UDP 프로토콜</strong><br>
<strong><em>데이터가 제대로 도착했는지 확인</em></strong>하고 전송된 데이터의 목적지가 <strong><em>어떤 애플리케이션인지 식별</em></strong>합니다.<br>
<a href="https://github.com/gyoogle/tech-interview-for-developer/blob/master/Computer%20Science/Network/OSI%207%20%EA%B3%84%EC%B8%B5.md">참고1</a>
<a href="https://velog.io/@april_5/%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC-%EA%B5%AC%EC%A1%B0-%EC%9D%B4%ED%95%B4-%EC%A0%84%EC%86%A1-%EA%B3%84%EC%B8%B5-%EC%8B%A0%EB%A2%B0%ED%95%A0-%EC%88%98-%EC%9E%88%EB%8A%94-%EB%8D%B0%EC%9D%B4%ED%84%B0-%EC%A0%84%EC%86%A1%ED%95%98%EA%B8%B0">참고2</a>
</div>
</details>
<hr>

## 3. TCP와 UDP의 공통점과 차이점에 대해 말해보세요.
<details>
<summary>3번 정답</summary>
<div markdown="1">      
공통점<br>
<strong><em>1. 전송 계층에서 사용되는 프로토콜</em></strong><br>
2. 포트 번호를 이용하여 주소를 지정하는 것<br>
3. 데이터 오류검사를 위한 체크섬 존재<br>
차이점<br>
<strong><em>TCP는 신뢰성 있는 데이터 전송을 지원하는 연결 지향형 프로토콜</em></strong>로 데이터를 송신할때마다 확인 응답을 주고 받는 절차를 통해 신뢰성이 있지만<br> 반면 <strong><em>UDP는 비연결 지향적 프로토콜</em></strong>로 연결 과정이 없기 때문에 신뢰성이 떨어지지만 TCP보다 빠른 전송을 할 수 있다.<br><br>
※ 중요 부분이므로 참고외에 더 공부할 것!<br>
<a href="https://s-mile-y.tistory.com/9">참고1</a>
</div>
</details>
<hr>

## 4. TCP/IP 4계층에 대해 말해보세요.
<details>
<summary>4번 정답</summary>
<div markdown="1">      
4계층 : 애플리케이션 계층<br>
- 사양자와 가장 가까운 계층으로, 사용자-소프트웨어 간 소통을 담당하는 계층<br>
- 프로토콜 : HTTP, HTTPS, FTP, SSH, Telenet, DNS 등<br>
3계층 : 전송 계층<br>
- 데이터의 실제 송수신을 담당<br>
- 프로토콜 : TCP, UDP 등<br>
2계층 : 인터넷 계층<br>
- 경로 검색을 해주는 계층(라우팅)<br>
- 프로토콜 : IP, ARP, ICMP, RARP 등<br>
1계층 : 네트워크 액세스 계층/네트워크 인터페이스 계층<br>
- 데이터를 전기신호로 변환한 뒤, 물리적 주소인 MAC 주소를 사용해, 알맞은 기기로 데이터를 전달하는 계층<br>
- 프로토콜 : Ethernet, Wi-Fi, PPP 등<br>
<a href="https://github.com/devham76/tech-interview-study/blob/master/contents/network.md#TCP/IP-%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C-%EC%8A%A4%ED%83%9D-4%EA%B3%84%EC%B8%B5%EC%9C%BC%EB%A1%9C-%EA%B5%AC%EB%B6%84%EC%A7%93%EA%B3%A0-%EC%84%A4%EB%AA%85%ED%95%98%EB%9D%BC">참고1</a>
<a href="https://wooono.tistory.com/507">참고2</a>
</div>
</details>
<hr>

## 5. 3-way handshake와 4-way handshake에 대해 간단하게 말해보세요. (연결 과정 X, 무슨 과정인가?)
<details>
<summary>5번 정답</summary>
<div markdown="1">      
3-way handshake<br>
- TCP/IP 프로토콜을 이용해서 통신을 하는 응용프로그램이 데이터를 전송하기 전에 먼저 정확한 전송을 보장하기 위해 <strong><em>상대방 컴퓨터와 사전에 세션을 수립하는 과정</em></strong><br>
4-way handshake<br>
- <strong><em>세션을 종료하기 위해 수행되는 과정</em></strong><br><br>
※ 연결 과정에 대해서도 같이 공부하기!<br>
<a href="https://jeongkyun-it.tistory.com/180">참고1</a>
</div>
</details>
<hr>

## 6. 3-way handshake와 4-way handshake의 단계가 차이나는 이유는?
<details>
<summary>6번 정답</summary>
<div markdown="1">      
Client가 데이터 전송을 마쳤다고 하더라도 <strong><em>Server는 아직 보낼 데이터가 남아 있을 수 있기 때문에 일단 FIN에 대한 ACK만 보내고, 데이터를 모두 전송한 후에 자신도 FIN 메세지를 보내기 때문</em></strong>이다.<br>
<a href="https://jeongkyun-it.tistory.com/180">참고1</a>
</div>
</details>
<hr>

## 7. 3-way handshake는 왜 2-way가 아니라 3-way일까?
<details>
<summary>7번 정답</summary>
<div markdown="1">      
TCP는 <strong><em>양방향성 연결</em></strong>이기 때문에 클라이언트에서 서버에게 자신의 존재를 알리고 패킷을 보낼 수 있는 것처럼 서버에서도 클라이언트에게 자신의 존재를 알리고 패킷을 보낼 수 있다는 신호를 보내야 하기 때문이다.<br>
<a href="https://github.com/WooVictory/Ready-For-Tech-Interview/blob/master/Network/3%20way%20handshake.md">참고1</a>
</div>
</details>
<hr>


## 8. 4-way handshake에서 TIME_WAIT을 하는 이유는?
<details>
<summary>8번 정답</summary>
<div markdown="1">      
<strong><em>클라이언트가 전송한 패킷이 Routing 지연이나 패킷 유실로 인한 재전송으로 서버 측에 늦게 도착하는 상황에서 패킷이 유실되는 것을 방지</em></strong>하기 위해서이다.<br>
<a href="https://hpjang.tistory.com/4">참고1</a>
</div>
</details>
<hr>

## 9. HTTP 동작에 대해 설명해보세요.
<details>
<summary>9번 정답</summary>
<div markdown="1">      
<strong><em>Client가 브라우저를 통해 URI을 통해 특정 요청(Request)을 보내면, Server는 해당 요청(Request)을 받아 처리를 하여 Client에게 응답(Response)을 하는 형태</em></strong><br>
<a href="https://github.com/devsungmin/Ready-For-Tech-Interview/blob/master/Network/HTTP%EB%8F%99%EC%9E%91%EA%B3%BC%EC%A0%95%EA%B3%BC%20HTTP%20Method%2C%20%EC%83%81%ED%83%9C%EC%BD%94%EB%93%9C.md">참고1</a>
</div>
</details>
<hr>

## 10. HTTP Status Code 중 4xx는 어떠한 코드인가?
<details>
<summary>10번 정답</summary>
<div markdown="1">
<strong><em>클라이언트 요청 오류</em></strong><br>      
- 클라이언에서 서버에 잘못된 요청을 보내 서버가 요청을 해결할 수 없을때 발생하는 코드이며, <strong><em>클라이언트측에서 발생하는 코드</em></strong><br>
<a href="https://github.com/devsungmin/Ready-For-Tech-Interview/blob/master/Network/HTTP%EB%8F%99%EC%9E%91%EA%B3%BC%EC%A0%95%EA%B3%BC%20HTTP%20Method%2C%20%EC%83%81%ED%83%9C%EC%BD%94%EB%93%9C.md">참고1</a>
</div>
</details>
<hr>

## 11. HTTP Method 중 HEAD에 대해 말해보세요.
<details>
<summary>11번 정답</summary>
<div markdown="1">
GET메소드와 방식은 동일하지만, <strong><em>응답에 BODY가 없고 응답 코드와 HEAD만 응답하는데 사용</em></strong>되는 메소드<br>
<a href="https://github.com/devsungmin/Ready-For-Tech-Interview/blob/master/Network/HTTP%EB%8F%99%EC%9E%91%EA%B3%BC%EC%A0%95%EA%B3%BC%20HTTP%20Method%2C%20%EC%83%81%ED%83%9C%EC%BD%94%EB%93%9C.md">참고1</a>
</div>
</details>
<hr>

## 12. Web Server와 WAS의 차이점에 대해 말해보세요.
<details>
<summary>12번 정답</summary>
<div markdown="1">
Web Server<br>
- HTTP 프로토콜을 기반으로 Client가 웹 브라우저에서 어떠한 요청을 하면 그 요청을 받아 <strong><em>정적 컨테츠를 제공하는 서버</em></strong><br>
- 정적 컨텐츠 : HTML, CSS, 이미지, 파일 등 즉시 응답 가능한 컨텐츠<br>
WAS(Web Application Server)<br>
-  <strong><em>DB 조회 혹은 다양한 로직 처리를 요구하는 동적 컨텐츠를 제공</em></strong>하기 위해 만들어진 Application 서버<br>
<a href="https://code-lab1.tistory.com/199">참고1</a>
<a href="https://velog.io/@gillog/Web-Server%EC%99%80-Web-Application-Server%EC%9D%98-%EC%B0%A8%EC%9D%B4">참고2</a>
</div>
</details>
<hr>


## 13. Web Server와 WAS를 분리하는 이유는 무엇인가?
<details>
<summary>13번 정답</summary>
<div markdown="1">
1. <strong><em>서버 부하 방지</em></strong><br>
- WAS와 웹 서버는 분리하여 서버의 부하를 방지해야 한다. WAS는 DB 조회나 다양한 로직을 처리하고, 단순한 정적 컨텐츠는 웹 서버에서 처리해줘야한다. 만약 정적 컨텐츠까지 WAS가 처리한담녀 부하가 커지게 되고, 수행 속도가 느려질 것이다.<br>
2. <strong><em>보안 강화</em></strong><br>
- SSL에 대한 암호화, 복호화 처리에 웹 서버를 사용 가능<br>
3. <strong><em>여러 대의 WAS 연결 가능</em></strong><br>
- 로드 밸런싱을 위해 웹 사버를 사용할 수 있다. 여러 개의 서버를 사용하는 대용량 웹 어플리케이션의 경우 웹 서버와 WAS를 분리하여 무중단 운영을 위한 장애 극복에 쉽게 대응할 수 있다.<br>
4. <strong><em>여러 웹 어플리케이션 서비스 가능</em></strong><br>
- 하나의 서버에서 PHP, JAVA 애플리케이션을 함께 사용할 수 있다.<br>
<a href="https://code-lab1.tistory.com/199">참고1</a>
</div>
</details>
<hr>