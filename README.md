## CS 메모
---
### 인터넷
- 인터넷의 동작 원리

수천 마일 떨어진 곳에 위치할 수도 있는 데이터센터에 영상이 저장되어 있다. 이 데이터가 어떻게 휴대폰이나 노트북에 전송될까. 위성은 지연이 심하다. 데이터센터와 장치 사이에 연결되는 광섬유 케이블의 복잡한 네트워크를 통해 이행된다. 어떻게 되냐. IP주소. 인터넷에 연결된 모든 장치는 ip주소라는 고유한 식별 번호가 있다.ip주소는 집 주소와 같다. isp 인터넷 서비스 공급자 장치의 ip 주소를 결정한다. 데이터 센터의 서버에도 ip 주소가 있다. 서버는 웹사이트에 저장하므로 서버의 ip주소를 알기만 해도 모든 웹사이트에 접속할 수 있다. 사람이 ip주소를 기억하긴 어려우므로 youtube.com같은 도메인 이름을 이용한다. 사람들이 도메인 이름을 입력해서 요청하면 인터넷은 어디에서 그에 해당하는 ip주소를 가져올까. 인터넷은 dns라는 거대한 전화번호부를 사용한다. 인터넷 서비스 공급자 혹은 다른 조직이 dns 서버를 관리할 수 있다. 도메인 이름을 입력하면 브라우저가 해당 ip 주소를 얻기 위해 dns 서버에 요청을 보낸다. ip주소를 받은 후 브라우저는 해당 요청을 데이터센터, 각 서버로 전달한다. 서버가 특정 웹사이트에 대한 요청을 받으면 데이터의 흐름이 시작된다. 데이터는 광섬유케이블을 통해 디지털 형식으로 전송되며 , 광펄스의 형태로 전송된다. 이런 광케이블 네트워크를 유지하고 구축하는 기업들(구글, 버라이즌, AT&T 등)이 있다. 배에서 쟁기를 떨어뜨려 바다 깊숙히 위치하게 한 뒤 이 쟁기로 해저의 광섬유 케이블이 깔리게 될 도랑을  판다. 빛을 전달하는 광케이블은 해저를 가로질러 여러분의 집에 라우터까지 연결되어 있다. 라우터는 이러한 빛 신호를 전기 신호로 변환한다. 그다음 이더넷 케이블을 사용하여 노트북에 전기 신호를 전송한다. 셀룰러 데이터를 사용하여 인터넷에 접속한다면 광케이블에서의 신호는 기지국으로 보내져야하고 기지국에서 그 신호를 전자파 형태로 여러분의 휴대폰에 보내게 된다. 인터넷은 세계적인 네트워크이기 때문에 ip주소 부여, 도메인 이름 등록 등과 같은 조직의 존재가 중요해졌다. 이것은 미국에 위치한 ICANN이라는 기관이 관리한다. 인터넷의 데이터 전송을 효율적으로 만드는 것은 0과1로 이루어진 패킷이라고 알려진 작은 덩어리로 잘라내어 전송하는 방법이다. 이러한 0과1의 흐름이 패킷으로 구성되어 휴대폰을 향해 라우팅된다. 모든 패킷이 동일한 경로를 통해 라우팅 될 필요는 없으며 각 패킷은 독립적으로 해당 시점에 사용 가능한 최상의 경로를 사용한다. 휴대폰에 도달하게 되면 패킷이 시퀀스 번호에 따라 조립된다. 인터넷에서도 데이터패킷의 복잡한 흐름을 관리하기 위해 프로토콜 이라는 것을 사용함. 프로토콜은 데이터 패킷 변한, 각 패킷에 대한 발신처 및 수신처 주소 첨부, 라우터의 규칙 설정을 한다. 응용 프로그램마다 사용되는 프로토콜이 다르다.

- HTTP
HTTP(HyperText Transfer Protocol)는 W3 상에서 정보를 주고받을 수 있는 프로토콜이다. 주로 HTML 문서를 주고받는 데에 쓰인다. 주로 TCP를 사용하고 HTTP/3 부터는 UDP를 사용하며, 80번 포트를 사용한다.
HTTP는 클라이언트와 서버 사이에 이루어지는 요청/응답(request/response) 프로토콜이다. 예를 들면, 클라이언트인 웹 브라우저가 HTTP를 통하여 서버로부터 웹페이지(HTML)나 그림 정보를 요청하면, 서버는 이 요청에 응답하여 필요한 정보를 해당 사용자에게 전달하게 된다. 이 정보가 모니터와 같은 출력 장치를 통해 사용자에게 나타나는 것이다.
HTTP를 통해 전달되는 자료는 http:로 시작하는 URL(인터넷 주소)로 조회할 수 있다.
- 브라우저
- DNS
도메인 네임 시스템(Domain Name System, DNS)은 호스트의 도메인 이름을 호스트의 네트워크 주소로 바꾸거나 그 반대의 변환을 수행할 수 있도록 하기 위해 개발되었다. 특정 컴퓨터(또는 네트워크로 연결된 임의의 장치)의 주소를 찾기 위해, 사람이 이해하기 쉬운 도메인 이름을 숫자로 된 식별 번호(IP 주소)로 변환해 준다. 도메인 네임 시스템은 흔히 "전화번호부"에 비유된다. 인터넷 도메인 주소 체계로서 TCP/IP의 응용에서, www.example.com과 같은 주 컴퓨터의 도메인 이름을 192.168.1.0과 같은 IP 주소로 변환하고 라우팅 정보를 제공하는 분산형 데이터베이스 시스템이다.
인터넷은 2개의 주요 이름공간을 관리하는데, 하나는 도메인 네임 계층[1], 다른 하나는 인터넷 프로토콜(IP) 주소 공간이다. 도메인 네임 시스템은 도메인 네임 계층을 관리하며 해당 네임 계층과 주소 공간 간의 변환 서비스를 제공한다. 인터넷 네임 서버와 통신 프로토콜은 도메인 네임 시스템을 구현한다. DNS 네임 서버는 도메인을 위한 DNS 레코드를 저장하는 서버이다. DNS 네임 서버는 데이터베이스에 대한 쿼리의 응답 정보와 함께 응답한다.
- 도메인
- 호스팅
### 운영체제
- 터미널
- 프로세스
- 스레드
- 메모리
- 입출력
- 네트워크
### 데이터베이스
- 옛날엔 데이터를 개별 파일로 관리하고 있었다. 그러나 데이터 중복, 싱크에 문제가 있었다. 데이터를 한 곳에 모아놓을 필요성이 생김. 동시성, 성능, 보안에 신경 써야함. 이걸 관리해주는게 DBMS이다. 관리시스템을 통해서만 데이터에 손을 댈 수 있게 하고 이 손을 댈 때 쓰는게 SQL이다.
- 스키마는 표들을 그룹핑하는 일종의 폴더다.
- 관계형 데이터베이스의 핵심은 JOIN
### API
### 캐싱
### 웹보안
### CI/CD
### 쿠키
- 웹사이트 접속시 유저의 개인장치에 다운로드 되고 브라우저에 저장되는 작은 텍스트 파일이다.
- 일종의 정보파일이며 사용자의 인증을 도와준다. 인증 외에도 보안, 환경설정, 마케팅, 성능 등에 활용한다.
- 웹사이트에서 사용자의 방문에 관한 정보를 기억하여 다음번에 사이트에 방문했을 때 번거로운 작업을 피하고 더 유용하게 사이트를 활용할 수 있다. (예. 회원제로 운영되는 웹사이트에서 쿠키를 사용할 경우 이용자는 처음 들어갈 때 ID와 비밀번호를 입력하면 다른 페이지를 방문할 때마다 ID와 비밀번호를 다시 입력할 필요가 없다. 그러나 쿠키를 사용하지 않으면 이용자는 동일 웹사이트에서 다른 서비스 페이지를 방문할 때마다 회원정보를 계속 입력해야 하는 불편함이 있다.)
- 쿠키는 도메인에 따라 제한됨.(예. 구글이 준 쿠키는 구글에만 보내지게 됨)
- 유효기간이 있다. 서버가 정한 기간에 따라 다름.
- 세션 쿠키(session cookies)와 지속적 쿠키(persistent cookies)가 있다. 세션 쿠키는 유저가 사이트를 떠날 때까지 유저의 기기에 남아있는 임시적인 쿠키이다. 지속적 쿠키는 유저가 수동으로 삭제하기 전까지 남아있는 등 더 오랜기간 동안 유저의 컴퓨터에 저장된다.
---
### 캐시
- 다음 방문 시 페이지를 빠르게 열 수 있도록 이미지 등 페이지의 일부를 기억함.
---
### 세션과 토큰
- 세션은 서버의 메모리에 생성되는 저장 공간이다. 세션은 고유ID가 있다. 
---
### SQL
- 데이터베이스 관리 시스템(DBMS)에 질의하는 명령어
