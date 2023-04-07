# 🌐 네트워크

## 1. HTTP가 무엇인가요?

<details>
<summary>1번 정답</summary>
<div markdown="1">
 http는 HyperText Transfer Protocol의 약자로 서버 클라이언트 모델을 따르면서 request/response 구조로 웹 상에서 정보를 주고받을 수 있는 프로토콜입니다.<br>
 TCP/IP 기반으로 작동하며, Connectionless와 Stateless의 특징을 가지고 있습니다.
</div>
</details>
<hr>

## 2.http의 Connectionless와 Stateless 특징에 대해서 설명해 주세요

<details>
<summary>2번 정답</summary>
<div markdown="1">
http는 서버에 연결 후 요청에 응답을 받고나면 연결을 끊는데 이러한 특징을 connectionless라고 합니다.<br>
그리고 연결을 끊었기 때문에 이전의 상태를 알 수 없어서 stateless의 특징도 갖게 됩니다.
</div>
</details>
<hr>

## 3. http와 https를 비교하여 설명해 보세요

<details>
<summary>3번 정답</summary>
<div markdown="1">
http와 https 모두 인터넷 통신을 위한 프로토콜이지만 몇 가지 차이점이 있습니다.<br>
먼저 가장 큰 차이점은 보안성입니다. http는 평문 통신으로 암호화되지 않은 데이터를 주고 받기 때문에 보안에 취약하다는 단점이 있습니다. 반면 https는 ssl/tls 프로토콜을 사용하여 데이터를 암호화하여 전송하기 때문에 보안성이 높습니다.<br>
두 번째는 포트번호입니다. http는  80번 포트 https는 443포트를 사용합니다.<br>
세 번째는 인증서입니다. https는 ssl/tls 인증서를 사용하여 신원을 보호합니다.<br>
네 번째는 속도입니다. https는 암호화된 데이터를 전송하기 때문에 http에 비해 속도가 느립니다.<br>
다섯 번째는 검색 엔진 최적화입니다. https는 검색 엔진 최적화를 위해 google에서 우선적으로 검색되는 경향이 있습니다.<br>
<br>
요약하자면 https는 보안성이 높지만 암호화 과정때문에 속도가 느리고, https는 반대로 보안성은 낮지만 속도가 빠릅니다.

</div>
</details>
<hr>

## 4. http request method 중 GET 과 POST를 비교해서 설명해 보세요

<details>
<summary>4번 정답</summary>
<div markdown="1">
GET 메서드는 클라이언트가 서버에게 리소스 조회를 요청할 때 사용하는 메서드입니다.<br>
POST 메서드는 서버에게 데이터를 생성을 요청할 때 사용하는 메서드입니다.<br>
<br>
GET 메서드는 URL 뒤에 Query String을 추가해서 데이터를 전달하고, POST 메서드는 전달할 데이터를 Body 부분에 포함시켜 통신합니다.
<br>
GET 메서드는 요청하는 데이터가 URL에 노출되어 있어서 보안상 취약할 수 있지만, 캐시를 이용하여 빠른 속도로 데이터를 받아올 수 있습니다.<br>
반면 POST는 데이터가 본문에 담겨 전달되므로 비교적 보안성이 높으나 캐시가 없어서 GET보다 느릴 수 있습니다.
</div>
</details>
<hr>

## 5. http request method 중 PUT 과 PATCH를 비교해서 설명해 보세요

<details>
<summary>5번 정답</summary>
<div markdown="1">
PUT과 PATCH는 데이터를 수정할 때 사용되며, 비슷한 기능을 수행하지만 약간의 차이가 있습니다.<br>
PUT은 전체 데이터를 수정할 때 사용되며, 클라이언트가 전체 데이터를 보내면 서버는 해당 데이터로 완전히 대체됩니다.<br>
반면, PATCH는 부분적인 수정을 할 때 사용되며 클라이언트가 변경하고자 하는 필드만 보내면 서버는 해당 필드만 수정하고 나머지는 그대로 유지합니다.
</div>
</details>
<hr>

## 6. Naver를 주소창에 쳤을 대 화면에 나오기까지의 과정을 설명해 보세요

<details>
<summary>6번 정답</summary>
<div markdown="1">
1. 사용자가 주소창에 브라우저에 해당 url를 입력합니다.<br>
2. 브라우저는 DNS(Domain Name System) 서버에 "naver.com"도메인명의 IP 주소를 요청합니다.<br>
3. DNS 서버는 "naver.com" 도메인명에 해당하는 IP 주소를 응답합니다.<br>
4. 클라이언트의 브라우저는 해당 IP 주소로 HTTP 요청 메시지를 보냅니다.<br>
5. 네이버 서버는 클라이언트의 요청을 받아 해당 요청에 대한 HTTP 응답 메시지를 생성합니다.<br>
6. 생성된 HTTP 응답 메시지를 서버에서 클라이언트의 브라우저로 전송합니다.<br>
7. 클라이언트의 브라우저는 전송받은 HTTP 응답 메시지를 해석하여 사용자에게 네이버 웹사이트를 표시합니다.<br>
</div>
</details>
<hr>

## 7. 쿠키와 세션을 비교하여 설명해 보세요

<details>
<summary>7번 정답</summary>
<div markdown="1">
쿠키와 세션은 모두 클라이언트와 서버간의 상태를 유지하기 위한 메커니즘입니다.<br>
하지만 쿠키와 세션은 상태를 유지하는 방법이 다릅니다.<br>
1. 저장위치 : 쿠키는 상태를 브라우저에 저장하며, 세션은 서버 측에 저장합니다.<br>
2. 저장내용 : 쿠키는 클라이언트 측에 작은 양의 데이터를 저장할 수 있고, 세션은 보통 쿠키에 저장된 세션 ID와 같은 식별자를 사용하여 서버 측에 데이터를 저장할 수 있습니다.<br>
3. 보안 : 쿠키는 클라이언트 측에 저장되므로 보안에 취약하고, 세션은 서버 측에 저장되므로 상대적으로 안전합니다.<br>
4. 만료 시점 : 쿠키는 만료일이 지나면 자동으로 삭제되고, 세션은 세션 ID를 사용하여 서버 측에서 삭제할 수 있습니다.<br>
<br>
즉, 쿠키는 클라이언트 측에서 간단한 정보를 저장하고, 세션은 서버 측에서 보다 복잡한 정보를 저장합니다. 또한, 세션은 쿠키보다 보안적으로 더 안전합니다.

</div>
</details>
<hr>

## 8. stateful 서비스와 stateless 서비스의 차이를 설명해 주세요

<details>
<summary>8번 정답</summary>
<div markdown="1">
stateful서비스는 클라이언트와 서버의 연결을 유지하며 , 이전 상태 정보를 유지합니다. 예를 들어, FTP서비스에서 데이터 전송을 할 때 TCP/IP 연결을 유지하면서 파일을 전송하고 상태 정보를 유지합니다.<br>
반면 stateless서비스는 클라이언트와 서버의 연결을 유지하지 않고, 상태정보도 저장하지 않습니다. 예를 들어, HTTP 서비스가 있습니다.<br>
<br>
stateful 서비스는 상태 정보를 유지해야 하므로, 클라이언트와 서버 간의 부하가 크고 확장성이 낮습니다. 하지만 상태정보를 유지하기때문에 일관성을 유지하기 쉽습니다.<br>
 반면 stateless 서비스는 연결을 유지하지 않으므로, 확장성이 높고 부하가 적습니다. 하지만 상태를 저장하지 않기에 일관성 유지가 어렵습니다.
</div>
</details>
<hr>

## 9. HTTP/1.0 HTTP/1.1 HTTP/2.0 HTTP/3.0에 대해서 설명해 주세요

<details>
<summary>9번 정답</summary>
<div markdown="1">
1. HTTP/1.0
- <strong>최초의 HTTP 버전</strong>으로, 1996년에 등장했습니다.<br>
- <strong>하나의 요청에 대해 하나의 응답</strong>을 받아야 했으며, 캐싱 기능이 부족하여 성능이 떨어졌습니다.<br>
- 보안 기능이 부족하여 보안에 취약합니다.<br>
<br>
2. HTTP/1.1<br>
<br>
- 1999년에 등장한 <strong>HTTP의 개선 버전</strong>입니다.<br>
- <strong>하나의 연결로 여러 개의 요청을 처리</strong>할 수 있도록 개선되었습니다.<br>
 이를 통해 <strong>병렬로 요청과 응답을 처리</strong>할 수 있게 되어 성능이 개선되었습니다.<br>
- <strong>캐싱 기능이 개선되었으며, 보안 기능도 개선</strong>되었습니다.<br>
<br>
3. HTTP/2.0<br>
<br>
- 2015년에 등장한 <strong>HTTP의 최신 버전</strong>입니다.<br>
- 요청과 응답을 이진화하여 처리하므로, 처리 속도가 빨라지고 대역폭을 효율적으로 사용할 수 있게 됩니다.<br>
- <strong>하나의 연결로 여러 개의 요청과 응답을 처리하는 기능이 개선</strong>되었습니다.<br>
- <strong>보안 기능이 강화</strong>되었습니다.<br>
<br>
4. HTTP/3.0<br>
<br>
- <strong>현재 개발 중인 HTTP의 최신 버전</strong>입니다.<br>
- <strong>UDP 프로토콜을 기반</strong>으로 하여, 연결 설정과 데이터 전송을 병렬</strong>로 처리할 수 있습니다.<br>
- <strong>TCP의 문제점을 보완하여, 연결이 끊기더라도 빠른 데이터 전송이 가능</strong>합니다.<br>
- 보안 기능이 강화되었습니다.<br>
<br>
따라서, HTTP 버전이 높아질수록 성능과 보안 기능이 개선되며, 최신 버전을 사용함으로써 더 나은 웹 환경을 제공할 수 있습니다.<br>

</div>
</details>
<hr>

## 10. JWT로 로그인 하는 방식을 설명해보세요

<details>
<summary>10번 정답</summary>
<div markdown="1">
JWT는 JSON Web Token의 약자로 사용자 인증 정보를 안전하게 전송하기 위한 방법 중 하나입니다.<br>
JWT를 사용하여 로그인하는 방식은 다음과 같습니다.<br>
<br>
1. 클라이언트에서 사용자가 로그인할 때, 서버에 사용자의 로그인 정보를 보냅니다.<br>
2. 서버는 사용자가 입력한 로그인 정보를 검증합니다.<br>
3. 검증이 성공하면, 서버는 JWT를 발급하여 클라이언트에게 전달합니다.<br>
4. 클라이언트는 이후 요청에 대해 JWT를 함께 전송합니다.<br>
5. 서버는 JWT를 검증하여, 요청이 유효한지 확인합니다.<br>
6. JWT가 검증되면, 서버는 요청에 대한 응답을 반환합니다.<br>
<br>
JWT는 서명된 정보를 가지고 있으므로, 클라이언트에서 JWT를 조작하여 인증을 획득하는 것은 불가능합니다.<br>
 따라서, JWT를 사용하여 로그인하는 방식은 보안적으로 안전하며, 사용자의 인증 정보를 안전하게 전송할 수 있습니다.<br>
<br>
JWT를 사용한 로그인 방식은 많은 웹 서비스에서 사용되고 있으며, 다양한 프로그래밍 언어와 프레임워크에서 지원하고 있습니다.

</div>
</details>
<hr>

## 11. OAuth로 로그인 하는 방식을 설명해 보세요

<details>
<summary>11번 정답</summary>
<div markdown="1">
OAuth는 Open Authorization의 약자로 사용자가 다른 애플리케이션에서 사용하는 서비스에 대해 권한을 부여할 수 있도록 하는 인터넷 표준 프로토콜입니다.<br>
<br>
1. 클라이언트 애플리케이션에서 사용자가 다른 서비스에 로그인하도록 요청합니다.<br>
2. 사용자는 다른 서비스에 로그인하고, 클라이언트 애플리케이션에서 요청한 권한을 부여합니다.<br>
3. 다른 서비스는 클라이언트 애플리케이션에 대한 액세스 토큰을 발급하고, 이를 클라이언트 애플리케이션에 반환합니다.<br>
4. 클라이언트 애플리케이션은 이후 요청에 대해 액세스 토큰을 함께 전송합니다.<br>
5. 서비스는 액세스 토큰을 검증하여, 요청이 유효한지 확인합니다.<br>
6. 액세스 토큰이 검증되면, 서비스는 요청에 대한 응답을 반환합니다.<br>
<br>
OAuth를 사용하여 로그인하는 방식은 사용자가 다른 서비스의 인증 정보를 클라이언트 애플리케이션과 공유하지 않아도 되므로, 보안적으로 안전합니다.<br>
 또한, OAuth를 사용하면 사용자가 한 번 로그인하면, 다른 서비스들에서도 로그인할 필요 없이 액세스 토큰만으로 인증이 가능하므로 사용자 경험을 향상시킬 수 있습니다.<br>
<br>
OAuth를 사용한 로그인 방식은 많은 웹 서비스에서 사용되고 있으며, 다양한 프로그래밍 언어와 프레임워크에서 지원하고 있습니다.<br>

</div>
</details>
<hr>

## 12. CORS에 대해서 설명해 주세요

<details>
<summary>12번 정답</summary>
<div markdown="1">
CORS(Cross-Origin Resource Sharing)란, 웹 브라우저에서 실행되는 JavaScript에서 다른 출처의 리소스에 접근하는 것을 제한하는 보안 정책입니다.<br>
 다른 출처의 리소스를 요청하는 것을 "Cross-Origin Request"라고 하며, 기본적으로 브라우저는 이를 보안상의 이유로 차단합니다.<br>
<br>
CORS를 사용하면, 웹 애플리케이션에서 다른 출처의 리소스에 접근할 수 있도록 브라우저에서 설정을 변경할 수 있습니다.<br>
 이를 위해서는, 서버에서 CORS 정책을 설정해야 합니다.<br>
  서버에서 Access-Control-Allow-Origin 헤더를 설정하면, 브라우저는 해당 출처의 리소스에 접근할 수 있도록 허용합니다.<br>
<br>
CORS는 보안상의 이유로 브라우저에서 제한하는 것이기 때문에, 서버 사이드에서는 별도의 제한이 없습니다. 따라서, 서버 측에서는 CORS를 사용하지 않아도 됩니다.<br>
<br>
CORS를 사용하여 다른 출처의 리소스에 접근하는 것은 보안에 대한 고민이 필요합니다.<br>
외부 출처에서 제공하는 리소스를 사용할 경우, 해당 리소스가 악성 스크립트나 코드를 포함하고 있을 가능성이 있으므로, 신뢰할 수 있는 출처에서만 사용하는 것이 좋습니다.

</div>
</details>
<hr>

# 보충 필요