# computer_network_final
computer_network_final

```
9장 연결하기
케이블 광대역

케이블 텔레비전 네트워크를 통한 인터넷 서비스 제공
모뎀 : 변조기(modulator)/복조기(demodulator)의 약자

케이블 모뎀 : 디지털 신호를 아날로그 신호로 변조
케이블 모뎀 종단 시스템 : 아날로그 신호를 디지털 신호로 변환

동적 호스트 구성 프로토콜을 지원해서 사용자에게 동적 ip를 할당하기도 함

디지털 가입자 회선(Digital Subscriber Line) DSL : 기존의 전화 회선 상에서 고속 디지털 통신을 지원

LAN : 한 건물, 또는 좁은 지역 내 연결
WAN : 더 먼 지리적 거리에 걸쳐 전송
LAN은 일반회사,조직 WAN은 통신 사업자

LAN : 계층2 스위치 계층1 허브/중계기, 고속, 학교 네트워크, 근거리
WAN : 계층3 라우터, ATM, Frame Relay 스위치, 상대적 저속, 인터넷, 원거리

접속점 AP(Acess Point)
인터넷과 같은 유선 기반 구조와의 연결을 담당하는 장치

무선 이더넷 : 물리, 데이터링크(MAC, LLC) 계층 포함 매체접근 방식 CSMA/CA

무선 랜 MAC 매체접근방식 = CSMA/CA 충돌회피 충돌감지X

A->B RTS(Request to send)(제어용프레임) RTS는 다른 노드들이 감지X
B준비->CTS(Clear to send)를 A에게 전송 이때 다른 노드들이 CTS를 감지
C단말이 보낼 것이 있지만 전송을 대기(충돌 회피) C에게 A는 Hidden Terminal
A에게 C는 Hidden Terminal

ISM(Industrial, Scientific, and medical)를 위한 대역

무선 랜 기본 구성 단위
BSS(Basic Service Set) : 고정과 이동하는 무선국과 접근점

Ad hoc network : AP없이 네트워크 구성
Infrastrcutured network bss: AP를 가진 BSS

ESS(Extended Service Set) AP를 가진 2개 이상의 BSS로 구성
분산시스템(Distribution System) : BSS의 AP들을 연결

무선랜 프레임포맷
지속/ID : DUR 데이터 지속시간 RTS : 얼마만큼받겠구나를 계산 대기
프레임 전달 시나리오에 따라 4개의 주소공간이 사용(1수신자,2송신자,3,4)
802.11 보안
WEP (Wired Equivalent Privacy) : 기존 유선 네트워크와 동등한 수준의 보안성을 제공하기 위해 설계
유선 동등 프라이버시

기밀유지 :도청 방지
무결성 : 데이터가 변경되지않았음을 보장
인증 : 통신 당사자가 누구인지, 네트워크에서 작동하는 데 필요한 권한이 있는 지 확인
WEP은 현재 취약해서 사용 X 
현재는 WPA2 별도의 인증서버를 사용 AES암호 사용

모바일 IP 

기존의 IP 프로토콜을 확장해서 이동 중에 인터넷을 사용할 수 있게 하는 프로토콜
한 네트워크에서 다른 네트워크로 가면 IP주소가 변경되어야 함
하지만 이동단말이 통신을 계속하려면 클라이언트, 서버 IP, 포트번호가 변경되서는 안됌

네트워크 계층에 같은 계층의 헤더인 home adrees와 foreign adress를 덧붙이는 터널링을 한다. 삼각 라우팅을 해서 자신의 홈 네트워크의 주소를 변경시키지 않고도 통신이 가능하다.

블루투스 PAN <- AD hoc network = AP가 없음 10M의 짧은 거리에서 통신

전화 접속 네트워크 PPP프로토콜  포인트 투 포인트 연결 (점대점 연결)	

링크 제어 프로토콜 LCP : 링크 설정
인증 프로토콜 AP : 사용자의 신원을 증명
네트워크 제어 프로토콜 NCP : 협상하고자 하는 네트워크 계층 프로토콜과 링크 수립, 유지 종료

PPP에서의 다중화
데이터그램을 하나 이상 전송할 수 있어야함, 데이터그램을 전송하는 것이 주 목적

허브(물리 계층 이더넷) -> 필터링,라우터X 수신하고 재전송만 함
브릿지(데이터링크계층) -> 물리주소로 패킷 필터링, 전송, 목적지 주소가 전송이아니라면 모든 테이블에 전송
링크계층 스위치 -> 처음에 빈 스위치테이블을 브로드캐스트 학습해서 결국에는 다 채워짐, 필터링, MAC 검사
스위치 방식 두가지
컷 스루 : 목적지 얻자마자 전송 시작
저장 및 전송 : 오류검사해서 있으면 대기, 없으면 전송

1. 전화선을 통해 IP 데이터그램을 전송하는 데 사용되는 주요 프로토콜은?
ppp 포인트 투 포인트 프로토콜

2. 가정용으로 사용할 수 있는 유선 기반 광대역 기술 2가지 설명

케이블 광대역
DSL 디지털 가입자 회선
3. 광대역 네트워크 기술 4가지 설명
프레임 릴레이, HDLC, ISDN 및 ATM 네 가지 일반적인 WAN 기술

4. 독립 기본 서비스 집합 무선 네트워크의 다른 이름?
애드 혹 네트워크

5. 허브와 스위치의 차이점 
허브는 전통적인 이더넷 케이블처럼 환경을 생성해 모든 메시지를 모든 포트에 전송해서 모든 컴퓨터가 모든 메시지를 볼 수 있습니다. 스위치는 물리 주소 테이블을 유지하고 의도한 컴퓨터에만 메시지를 전송합니다.

1. 전화 연결 접속의 단점 나열
전화 접속 연결은 DSL이나 케이블 모뎀과 같은 광대역 연결보다 훨씬 더 느립니다. 전화 접속 연결 중에는 전화를 사용할 수 없고 사용이후에 네트워크 연결이 끊기므로 인터넷 사용이 불편해짐.

10장 이름확인

모든 IP 주소를 기억하는 것은 비효율 초기에는 호스트 파일을 이용해서 이름 확인을 함
파일이 커지거나 대규모일 때 비효율적, 관리자는 hosts.txt 파일을 지속적으로 관리해줘야 했음
계층적 이름 확인 시스템이 필요했음 -> DNS의 탄생


DNS(Domain Name System) 이름공간을 도메인이라고 하는 계층적 엔티티로 분할
DNS 최상단은 루트
루트 밑에 최상위 도메인 TLD (TOP-LEVEL-DOMAIN)이라고 하는 그룹이 있음

최대 63자 아래노드에서 위노드(루트)까지 위에서 아래로 읽혀지고 루트는 null 즉 마지막 문자는 .dot이 된다.
하위 도메인의 권한을 다른 이름 서버에 위임할 수 있다.
이름 확인 권한은 트리를 통해 위임되고 지정된 도메인 관리자는 해당 도메인 호스트에 대한 이름-주소 매핑 제어권을 가질 수 있다.

일반적으로는 재귀적 방법 모르면 바로넘어감 최상위->하위->하위->하위
반복적 방법 없으면 근처 이름 서버에 쿼리 과정을 시작

2개 이상의 서버를 선택해야함
주 이름 서버, 보조 이름 서버

존 전송 : 보조 서버는 주 서버의 존 파일에서 정보를 가져옴
존(zone) : 이름 서버가 책임을 가지거나 권한을 가지는 영역
이름서버가 도메인에 대한 책임을 맡고 이를 더 작은 도메인으로 나누지 않았다면 도메인 = 영역

존 파일 -> 자원 레코드로 구성되어있음 name, type, class, ttl, rdlength, rdata

DNS 보안 확장 
DNS쿼리 응답이 존을 관리하는 실제 DNS 서버에서 왔다는 것을 보장하는 수단이 필요함
DNSSEC : DNS 데이터를 검증하기 위한 시스템을 제공

DNS 유틸리티
이름확인을 제공하는 모든 네트워크 유틸리티를 사용해서 네트워크가 올바르게 이름을 사용하는지 확인 가능
Ping, NSLookup

동적 DNS
새로운 IP주소가 DHCP를 통해 새로이 할당
DNS 서버는 반드시 사용중인 IP를 알아낼 방법이 있어야 한다는 의미

NetBIOS IBM이 개발한 이름확인시스템 
TCP/IP를 사용하지 않는 네트워크를 위해 개발 But DNS를 사용하는 것이 바람직
NetBIOS는 브로드캐스트를 통해 작동하기 때문에 소규모에서는 불필요
 
FQDN Fully Qualified Domain Name = 호스트+도메인 .으로 연결
PQDN Partically Qualified Domain Name = 하위도메인

1. 별칭에 사용되는 리소스 레코드의 유형
CNAME: A 레코드에 명시된 별칭을 이름으로 매핑하는 데 사용

2. DS 리소스 레코드와 DNSKEY 리소스 레코드는 왜 다른 서버에 저장되어 있습니까?
DNSSEC은 하위 영역과 함께 저장된 DNSKEY 리소스 레코드를 식별하고 인증하기 위해 상위 영역에 저장된 DS 리소스 레코드를 사용합니다. 상위 영역에 DS 레코드를 저장하면 쿼리가 응답의 신뢰성을 확인하는 데 필요한 신뢰 체인을 통과할 수 있도록 합니다.

11장 TCP/IP 보안

초기 방화벽 패킷 필터 ->　IP주소 및 TCP와 UDP 포트 번호를 주시

방화벽 기능이 종종 라우터에 내장되어 있음
네트워크 통로에 위치한 장치로 인바운드 패킷 헤더를 검사, 수락 또는 거부

첫 번째 룰셋 외부에서 접근하는 모든 ᅟᅵᆺ스템에 내부의 IP주소 80번 포트에 대한 접근을 허용
두 번째 룰셋 명백히 허용하지 않은 서비스에 대한 거부를 적용 명시 허용 X -> 모두 차단

패킷 필터 방화벽 한계 -> 바이러스는 파일 등을 통해 감염되므로 방화벽이 영향을 미치기 어려움
일부 웜은 막을 수 있지만 정상적이 ㄴ서비스 포트에 대해 웜이 공격을 시도할 때는 막을 수 없음

응용 레벨 게이트웨이(Proxy Server)

응용-레벨 트래픽의 증개자 역할 수행 응용레벨에서 들어오는 모든 트래픽을 로깅하고 감사
별도 프록시 서버를 구축, 내부와 외부 2개의 연결이 요구되며 그에 따른 처리량 증가
외부와 내부 네트워크 간의 직접적인 패킷 교환을 허용하지 않는다. 중개인 역할
	
DMZ : 많은 기관이 FTP, 이메일 인터넷으로 접근할 수 있는 다른 시스템을 유지
방화벽 간의 공간
DMZ의 주 목적은 무엇입니까?

DMZ의 목적은 내부 네트워크보다는 접근이 더 용이하지만 개방형 인터넷보다는 보호된 중간 수준의 보안 영역을 제공하는 것입니다.

1. 프록시 서버는 어떻게 웹 브라우저의 응답 속도를 높입니까?
많은 프록시 서버가 이전에 방문한 웹 페이지를 캐시합니다. 콘텐츠 캐싱이라고 하는 기술은 프록시 서버가 페이지를 로컬로 제공하도록 허용

2. 업데이트하는 것이 왜 중요한가?
시스템을 안전하게 유지하려고

3. 스크립트에 사용자의 입력 문자열의 유형과 길이를 확인하는 단계를 추가해야 하는 이유?
오버런하는 버퍼 오버플로 공격을 방지할 수 있는 중요한 방법

12장 구성하기

네트워크에 연결하기 위해서는 네트워크 정보를 설정해줘야 함

IP주소, 서브넷 마스크, 게이트웨이 주소, DNS 서버 주소. 호스트 이름

정적과 동적 IP 중 선택

정적 IP 주소 단점 : 더 많은 구성(개별적 구성), 더 많은 주소(현재 네트워크와 상관없이 사용), 유연성 감소(다른 서브네트워크 할당->수동 재구성)

DHCP는 디스크 없는 컴퓨터를 부팅할 때 사용하던 BOOTP라고 하는 초기 프로토콜에서 시작

DHCP(Dynamic Host Configuration Protocol) : 호스트에 동적으로 ip 주소를 할당하기 위해 사용하는 응용 계층 프로토콜

DHCP 서버가 호스트에 제공하는 중요 정보

호스트에 할당할 IP주소, 라우터 주소, DNS 서버 주소, Prefix

각 클라이언트는 주소에 대해 제한된 임대 기간을 가짐

만료되었을 때 더 이상 사용하지 않는다면 해당 주소는 다른 클라이언트에게 할당할 수 있음
DHCP의 임대 기능은 네트워크가 일반적으로 클라이언트 수만큼 IP주소가 많이 필요하지 않다는 효과를 가져옴

DHCP 메시지 포맷 : TAG, LENGTH, VALUE(Option), UDP 프로토콜 사용 TCP/IP 지정안해줘도됌


DHCP 동작 절차

DISCOVER(브로드) - OFFER - REQUEST - ACK

IP주소 합의 수많은 DHCP 중에 하나 68, 67 DISCOVER 
67 68 주소사용하라고 DHCP 서버가 제안
68 67 쓰겠다고 요청
너 IP주소 67이라고 승인

DHCP 작동원리

라우터는 일반적으로 브로드캐스트를 다른 네트워크로 전송하지 않는데
DHCP 작동하려면 중개자가 DHCP 프로세스를 도와주어야함 <- 릴레이 에이전트
릴레이에이전트는 정적IP DHCP 서버의 IP 알고 있고 데이터그램 항상 송수신 가능
릴레이에이전트는 DHCP 클라이언트와 동일한 네트워크이므로 브로드캐스트를 통해 DHCP 클라이언트와 통신 
라우터 자체에 DHCP 서버를 배치

네트워크 주소 변환(Network Adress Translation) NAT

사설 IP와 공인 IP 주소간 매핑 기능
NAT는 로컬네트워크의 모든 세부 내용을 가리고 실제로 로컬 네트워크의 존재를 숨김
로컬 컴퓨터가 인터넷 자원 연결하려고 하면 NAT 장치가 대신 연결 
인터넷 자원에서 받은 모든 패킷은 로컬 네트워크의 주소 체계로 변환되고 연결을 시작한 로컬 컴퓨터로 전송

NAT장치는 로컬 네트워크를 알아내는 것을 막기 때문에 보안 향상
외부에서 NAT장치는 인터넷에 연결된 단일 호스트로 보임
로컬 네트워크의 주소를 알아내더라도 로컬 주소 지정 체계가 인터넷 주소공간과 인접X
일부 IP 주소는 사설 IP 주소 영역으로 예약되어있음

사설IP와 공인IP의 변환 과정은 NAT 테이블을 참조함

Newtork address and port translation <- 네트워크 주소와 포트 

제로 구성
IPv4LL 링크 로컬 주소 지정 = 자동 사설 IP 주소 지정(APIPA) Automatic Private IP Addressing
정적 주소가 없고 동적 주소를 받을 수 없다면 자체적으로(라우팅이 불가능한) ip 주소를 지정함
로컬 네트워크에서 성공적으로 통신할 수 있는 상태가 됨
주소 라우팅이 불가능 -> 인터넷 x, 로컬 네트워크를 벗어난 자원 접근 x
	
제로콘프(Zeroconf)

IPv4LL의 철학 확장 소규모 로컬 네트워크를 위한 거의 완전한 네트워크 환경의 가능성 제공
애플 매킨토시 사에서 Bongjour라는 이름으로 구현
링크 로컬 주소 지정, 멀티캐스트 DNS, DNS 서비스 검색 
멀티캐스트 DNS에서 각 컴퓨터는 자신만의 DNS 내부 테이블을 유지
	
1. 다른 네트워크의 DHCP 서버로부터 한 네트워크의 DHCP 클라이언트가 IP 주소를 임대받기 위해 요구되는 것
DHCP 릴레이 에이전트

2. DNS-SD는 주로 어떤 DNS 레코드에 의존?
PTR레코드를 통해 서비스 인스턴트의 찾아보기 목록 조합을 도와주고 SRV 레코드를 사용해 서비스의 DNS 호스트 이름과 포트 번호를 획득, TXT 레코드는 서비스에 대한 부가 정보 부여

13장 IPv6: 차세대

왜 새로운 ip를 쓸까 -> IPv4의 부족한 주소 공간 해결책으로 제안
IPv6 주소 길이는 128비트 공간 -> 2의 128승

IPv6 헤더 형식 

헤더길이->40byte 고정

flow label -> 같은 특성을 공유하는 패킷들의 흐름은 flow table을 참조해서 빠르게 보냄
flow의 식별 - 소스 주소와 flow label의 조합을 이용 
ex) 실시간 비디오, 비디오 전송을 위한 자원 예약에 사용 RTP, RSVP와 함께 사용된다.

IPv6 확장 헤더

전송 경로를 따라 중간 노드가 처리
홉 바이 홉 확장 헤더 : 데이터 정렬과 옵션 지정 일부 패딩 + (65535바이트보다 큰 페이로드 처리) 라우터를 거칠때마다 처리해야하는 옵션 처리
라우팅 확장 헤더	: 데이터그램이 목적지까지 가는 경로 상의 라우터를 명시 

(수신지)목적지 확장 헤더 : 선택적 정보를 목적지 노드에 연결

인증 확장 헤더 : 송신자의 인증과 데이터 무결성을 제공

ESP(Encrypted Security Payload header) 확장 헤더 : 페이로드의 암호화를 통한 기밀성을 제공

프래그먼트 확장 헤더 : IPv4의 fragmentation 기능에 해당
MTU보다 작은 조각으로 나누어 전달된 데이터그램을 재조립하는데 필요한 정보를 포함

IPv6 주소 지정

영역 앞에 있는 0은 생략 가능
연속되는 영역이 0으로만 구성 -> 더블 콜론
주소당 한번만 가능, CIDR 표기 가능

2001:0DB8:0000:CD30:0000:0000:0000:0000/60
2001:0DB8:0:CD30::/60

유니캐스트 주소(단일 인터페이스를 정의)
애니캐스트 주소(하나의 주소를 공유하는 컴퓨터들의 집합을 정의, 애니캐스트 주소 패킷은 가장 도달 가능한 한 구성원에게만 전송됨
멀티캐스트 주소

불특정 ::/128 할당되면 안 되며 주소가 없음을 의미
루프백 ::1/128 자기 자신에게 패킷 진단 주소
패핑된 IPv4 ::FFFF/96 
멀티캐스트 FF00::/8   호스트 그룹 식별
링크로컬유니캐스트 FE80::/10 
범용 유니 (그외모든것)

global routing prefix, subnet identifier, interface identifier

global routing prefix + subnet identifier = network address 48 + 16 = 64
interface identifier = host address 64 

링크 로컬 주소 FE80::/10

라우터를 통과하지 않고 로컬 네트워크 세그먼트 간 통신에만 사용
수동 구성 단계 없이 로컬 네트워크 세그먼트에서 통신하도록 허용
더 큰 규모X 연결하려면 라우팅 가능한 자신만의 IP를 가지거나 동적 주소를 수신하기 위한 
DHCP 장치에 접근할 수 있어야 함

자동 구성

Interface identifier 인터페이스 식별자 
이더넷 MAC 주소 매핑을 통해 생성
호스트가 자기를 위해 링크 로컬 주소를 생성함
생성주소를 네트워크 상 다른 호스트가 사용하고 있는 지 중복 확인 
Neighbor solicitation/ neighbor advertisement 메시지이용

라우터로부터 글로벌 라우팅 프리픽스와 서브넷 식별자를 구하여
router solicitation/router advertisement 메시지 이용한 인터페이스 식별자와 결합함
-> 글로벌 유니캐스트 주소

이런 중복 주소를 검출하는 과정-> 중복 주소 검출 (Duplicate Address Detection)

노화된 IPv4 인프라의 균일 서비스 품질 요구를 해결
ip 데이터그램이 기다리면서 우선순위를 지정
차별화된 서비스 수준으로 우선순위 지정을 지원하도록 설계
트래픽 클래스와 흐름 레이블 필드는 데이터그램에 포함된 유형과 데이터의 우선순위를 지정하는 수단을 제공
트래픽 클래스 Type of service <- TOS 
흐름 레이블 FLOW label 

IPv4-mapped IPv6

169.219.13.133 -> ::FFFF:A9DB:0D85 -> ::FFFF:169.219.13.133 (IPv4 IPv6 혼합 가능)

IPv6 터널 : IPv4 내에 IPv6를 캡슐화하는 것(터널링과 비슷)
6in4 - 고정된 터널 종단점간에 IPv6 트래픽 전달
6to4 - 6to4 릴레이 서버는 해당 IPv6 주소를 받아서 IPv4를 추출하고 IPv4 패킷 내에 IPv6 패킷을 캡슐화한뒤 목적지에 보낸다. 목적지에서 패킷은 애니캐스트 주소에서 동작하는 6to4 릴레이로 전송된 후 원본 IPv6 패킷이 추출되어 전달됨

TSP (Ternerl Setup Protocol) 터널 셋업 프로토콜

IPv6 네트워크 엔드포인트는 TSP 서버와 계약
연결가능한 엔드 포인트와 매개변수를 협상해서 연결될 수 있도록 함

1. 멀티캐스트가 브로드캐스트보다 더 효율적인 이유
네트워크 세그먼트의 모든 호스트는 해당 정보와 관련이 없어도 브로드캐스트를 읽습니다.
멀티캐스트는 로컬 네트워크에 작은 하위 집합을 포함할 수 있는 호스트 그룹으로 수신자를 제한하기 때문

2. 왜 IPv6 자동 구성이 IPv4 제로콘프 자동 구성보다 더 안정적?
IPv6 자동 구성은 고유 물리 주소 기반으로 주소를 생성 다음 호스트는 자동 구성된 주소를 가정하기 위해 중복 주소를 확인 이 단계는 주소 충돌의 가능성을 줄입니다.

3. 6to4를 위해 예약된 IPv6 주소 접두사는?
IPv6 접두사 FF02::/16과 관련 멀티캐스트

14장 클래식 도구

연결 문제 : 프로토콜 장애 또는 잘못된 구성, 회선 문제, 잘못된 이름 확인, 과도한 트래픽

TCP/IP 올바르게 구성되었는지 확인 유틸리티
Ping
구성 정보 유틸리티, ipconfig, ifconfig
arp

회선 문제 : ping, 허브 스위치 라우터 케이블이 올바르게 꽂혀 있는지 확인

DNS 서버 문제 : IP 주소로는 대상에 도달할 수 있지만 호스트 이름으로는 도달할 수 없음

네트워크 성능 문제

traceroute : ICMP 프로토콜 사용해서 데이터그램이 통과하는 경로를 추적
netstat : ip, tcp, udp 및 icmp 프로토콜과 관련된 통계 및 연결 상태 표시

텔넷 : 가상 터미널 서비스를 위한 표준 응용 프로토콜, 원격 로그인 서비스 제공
텔넷 서버와 클라이언트 간의 상호작용을 정의하는 규칙 시스템 프로토콜
원격 사용자가 입력한 명령어가 다른 컴퓨터의 입력이 되는 수단을 제공
telnet hostname

보안성이 부족해서 ssh(secure shell)을 대체하여 사용

버클리 원격 유틸리티 r*

보안 셸 telnet을 대체하기위해서 설계된 프로토콜 : ssh, scp, sftp

네트워크 관리 : 네트워크 구성요소를 감시, 시험, 구성, 문제 해결

SNMP 단순 망 관리 프로토콜 (Simple Network Management protocol)
원격 모니터 (RMON, Remote Monitioring) 이용


단순 망 관리 프로토콜

네트워크에서 원격 장치를 관리하고 모니터링하기 위해서 설계
관리자가 snmp를 사용해 컴퓨터 및 다른 장치를 관리하고 모니터링할 수 있는 단일 워크스테이션을 원격으로 운영

네트워크 모니터 : snmp 관리 소프트웨어를 가진 컴퓨터
노드 : 네트워크에 있는 장치
커뮤니티 : 노드 그룹

에이전트라고 불리는 프로그램이 작동해 모니터에서 실행 중인 관리 시스템과 통신

snmp : 관리 정보 베이스(Management information base MIB)의 매개변수를 사용해 에이전트로부터 정보를 요청하고
구성 설정을 변경

SNMP 주소 공간 - MIB

루트에서 시작해서 계층 구조를 통해 진행

1. 웹 서핑 중 페이지 로딩이 멈췄을 때 해야할 해결 도구
일부 원격 사이트를 핑하는 것
2. ARP 캐시의 콘텐츠를 보여주는 명령어
arp -a
3. TCP를 통해 어떤 호스트가 연결되었는지 어떻게 볼 수 있나?
netstat -p tcp
4. ROUTE 버전은 라우팅 테이블 옵션이 없다 어떤 유틸 사용?
netstat -r 라우팅 테이블 확인
5. 텔넷 대신 SSH 선호하는 이유
SSH는 암호화를 제공하고 텔넷보다 더 안전한 보호 장치 제공
15장 클래식 서비스

FTP 

원격 호스트로의 파일 전달, TCP 프로토콜 사용, 

포트 2개 사용

데이터 연결용 20번 사용

제어 연결용 21번 사용

동작 절차 -> 21번으로 제어 연결 통해 인증 획득 20번으로 데이터 전달 전달 후 TCP 연결 종료
다른 파일 전송을 위해 새로운 데이터용 TCP 연결 20번을 설정

파일의 유형을 반드시 명시해야함
파일 기본 전송 모드는 아스키
단순 텍스트 -> 아스키
워드 또는 그래픽, 프로그램 파일 -> 바이너리

단순 파일 전송 프로토콜 (Trivial File Transfer protocol) TFTP
클라이언트와 TFTP 데몬을 실행하고 있는 TFTP 서버간 파일 전송

UDP를 전송 수단 FTP와는 다르게 로그인할 필요 X
디렉터리 컨텐츠 나열, 생성, 삭제 FTP처럼 로그인 허용X

파일 및 프린트 서비스

네트워크 파일 시스템(NFS) : 유닉스/리눅스에서 사용되는 프로토콜
마운팅이라는 프로세스를 거쳐야함, RFC 원격 프로시저 호출, 운영체제 등과 독립적으로 설계


공용 인터넷 파일 시스템/서버 메시지 블록 :CIFS/SMB 윈도의 클라이언트에 원격으로 파일 접근 사용 프로토콜

SMB는 클라이언트와 서버 기반 설계, 도스나 윈도우에서 파일, 장치를 공유하는데 사용
윈도에서 파일을 공유할 때마다 컴퓨터가 CIFS 서버의 역할을 하도록 구성

경량 디렉터리 접근 프로토콜 LDAP (Light Directory Access Protocol)
대규모 네트워크에서 다양한 자원에 대해 균일하고 효율적으로 관리
tcp포트에서 수신, 다양한 정보를 포함

LDAP 이름 공간 

계층적으로 구성, 각 엔트리는 고유한 식별 이름 DN을 가짐
DN은 콤마로 분리된 하나 이상의상대 식별 이름(RDN)으로 구성됨

식별 이름(RDN) 
구별되는 속성을 이름 내 RDN 요소로 사용 가능

이름 값과 관련된 두 글자 속성 유형

도메인 구성 요소 (dc) domainComponenont : 중첩  컨테이너 체인의 항목, 도메인이름
조직 단위 (ou) organizationalUnitName : 컨테이너 그룹화 항목명
정식 이름 (cn) canonicalName) : 인간친화적이름 

디렉터리 정보는 LDAP 서버에 URL 형태로 전달됨
특정 속성을 명시하려면 물음표로 묶음

원격 제어

원격 제어 프로토콜과 유틸리티로 사용자가 일반적인 그래픽 테스크톱 작업을 통해 원격 시스템을 제어
GUI 기반 원격제어는 시만텍의 pcAnywhere와 네토비아의 팀북트 같은 도구에 의해 대중화

윈도우는 원격 데스크톱 프로토콜 (RDP remote desktop protocol)
유닉스/리눅스 시스템은 X-Sever 기능의 기본 버전 o
가상 네트워크 컴퓨팅(VNC Virtual Network Computing) 및 노머신의 nx가 편리 

gui 기반 원격 접근 도구는 키보드 및 마우스 명령을 리다이렉팅

1. FTP의 put와 mput의 차이점
put은 파일을 서버에 업로드하는 명령 mput은 단일 명령줄로 여러 파일을 업로드 가능

2. TFTP를 사용해 디렉터리 파일 나열 가능?
불가능 TFTP는 파일 전송만 가능

3. 유닉스/리눅스 삼바 파일 서버 파일 서비스 프로토콜
삼바는 원래 SMB를 위한 오픈 소스 서버 CIFS는 개방형 표준 삼바는 CIFS를 지원

16장 인터넷 자세히 살펴보기

인터넷의 구조 : 공용 및 사설 네트워크의 다계층 시스템이다.

인터넷에서 일어나는 일 : 클라이언트-서버 통신

피어 투 피어 통신 : 클라이언트가 서버의 역할을 하는 개념

인터넷 세계 : DNS 서버, 웹 서버, 이메일 서버, FTP 서버, SSH 원격 접근 서버가 서로 연결되어있다.

URL(Locator 자원 위치 표준)은 URI(Uniform Resource Idenfier)의 한 형식
스킴(file, ftp, http, https, ldap, mailto, telnet): // userInfo @ host :port path?query#fragment

userInfo (user, password) 유저정보 아이디 패스워드
host : 호스트
port_number : 포트번호

쿼리 구성 요소 : 스크립트 및 웹에서 네트워크 서비스로 정보를 전달하기 위해 사용

해시# 기호 다음은 보조 리소스를 지정 
프래그먼트가 지정되면 서버는 리소스 내에서 프래그먼트를 찾음

URN(Name) : 얘는 단순히 식별하기 위한 용도임

urn:<namespace-identifier>:<namespace-specific-string>

17장 HTTP, HTML 및 월드 와이드 웹

web : 1989년 유럽원자핵연구소에서 제안
월드 와이드 웹 www 프로토콜은 하이퍼텍스트 전송 프로토콜(HTTP)

hypertext : 텍스트의 문서, 이미지 링크를 포함하는 문서
markup언어 : 태그 등을 이용해서 데이터 구조 명기

웹 사이트는 페이지와 링크의 통합 시스템

http -> 전송계층 프로토콜 (tcp) request, response 메시지로 구성
웰논포트번호 80번 이용 

데이터 전송 request 데이터 응답 response 하면 연결 끊음 비연결성
자원 낭비를 막기위해서 1.1부터는 연결을 끊음

요청메시지 method로 시작 url , version 버전에 따라 구조가 조금씩다름
헤더 : 헤더이름 value(body의 압축 정보 중 하나)
blank line : 한 칸 쉼 전까지가 헤더임을 명시해주기위해 띄움 
바디 : post 같은 건 정보를 넘겨줘야 해서 바디에 씀
응답메시지는 version으로 시작 상태코드 phrase(설명)

http/2는 조금 더 좋아졌다.
메서드나 구문은 그대로

http1과 비교해서 2가 가진 장점 3가지

http/2는 1. 서버가 여러 연결을 처리할 수 있고 2. 헤더 정보를 압축하고 3. 서버 푸시 응답 서버에서 요청을 기다리기보다 요청을 직접 예상해서 콘텐츠를 푸시

스크립팅

script : 컴파일없이 실행될 수 있는 명령어의 집합(대본)

스크립팅 : 서버 사이드 스크립트, 클라이언트 사이드 스크립트

서버 사이드 스크립트 
클라이언트 입력을 서버가 받아서 처리

CGI(Common Gateway Interface) : 양식에 기반한 입력을 받아 처리하고 html형식으로 출력하기 위해 개발, 서버와 애플 간에 데이터를 주고 받는 방식

클라이언트 사이드 스크립트 : 새로고침했는데 바뀐 부분만 제공하는 거 할 수 있음 다 안고치고 

웹 브라우저 : 제어기 + 클라이언트 프로토콜 + 해석기

Controller 제어기 - 키보드, 마우스 입력받아 클라이언트 프로그램을 사용해서 웹 문서에 접근함

클라이언트 프로토콜 : 응응계층 프로토콜 : http, ftp, smtp

Interpreter : 웹 문서 해석

보안이 추가된 https와 ssl/tls 소켓 계층/ 전송 계층 보안으로 통신할 수 있도록 디지털 서명 및 인증서 지원을 제공해야 함

시맨틱 웹 : 의미를 가지는 태그

RDF 자원 기술 프레임워크 (Resource Description Framework)
resource (URI를 갖는 모든 것 웹 페이지, 이미지, 동영상 등)
Description(자원들의 속성)
Framework(문법, 언어, 모델)

마이크로포맷 (완전한 문장구조와 구문 구조를 표현하려고 하지 않음)
사람 친화적(human readable)

XHTML = XML + HTML

HTML과 비슷하지만 더 엄격

비표준 플러그인 같은 기술이 난립, 비호환성
 
HTML5 (범용성 표준이 필요하다) 

새로운 웹 표준 HTML5

19장 추적

웹 사이트가 지속적으로 클라이언트와 관계를 유지하는 중요한 방법은 브라우저 크키 또는 http 쿠키를 통해서 통신하는 것

쿠키는 웹 서버가 클라이언트 컴퓨터에 저장한 정보의 일부

쿠키는 컴퓨터에 작은 텍스트 파일의 형태로 저장

세션 쿠키 : 메모리에 존재하고 세션 기간 동안만 남아 있음(휘발성)

영구 쿠키 : 세션 동안 살아있고 지정된 만료 날짜까지 지속 (추적 쿠키라고도 한다)

추적 세부 사항 추가 가능 : 경로에 대한 쿠키를 반환하도록 명령
기간을 줘서 세션 쿠키가 아닌 영구 쿠기가 되도록 명령

secure 속성 https 연결을 통해 전송되어야 함을 명시함
HTTPOnly 속성 : http로만 접근해야함

실제 쿠키는 브라우저와 웹사이트의 상호 작용을 기록할 필요는 없음 아이디, 접속날짜 등등만 기록

서드 파티 쿠키 : 사용자 행동을 추적하는 일반 도구
좋아요 누르면 서드 파티 쿠키를 수락하는 것 

쿠키 및 관리 및 제어 : 쿠리를 끄면 웹 사이트에서 일어나는 복잡한 상호 작용의 일부 사용이 불가능

추적 스크립트는 작은 스크립트 : 활동을 기록하는 방문 기록, 광고 추적 대행사가 이용

추적 픽셀은 웹 비컨이라는 일반적인 객체 범주의 예
html <img> 태그를 사용해서 전달
눈에 작은 객체 1x1 gif이미지

추적토큰 url자체의 쿼리 문자열을 통해 접근 추적을 위한 수단을 제공
url 쿼리쪽에 스파이 심어두는 거 

추적 금지 Do Not Track

웹 광고사가 사용하는 추적 알고리즘을 거부할 수 있는 기능을 제공

http 헤더 dnt를 통해 표현

0 : 허용 
1 : 금지
null : 선택하지 않음

20장 이메일

이메일 텍스트를 효율적으로 전송하기 위해 설계
이후에 2진 첨부파일을 포함하도록 확장
다목적 인터넷 우편 확장 MIME(Multipurpose Internet Mail Extension)형식으로 인코딩

이메일 형식
제목 필드

MIME : 이메일을 통해 2진 파일을 보내기 위해 더 일반적이고 범용적인 해결책
첨부파일을 위한 표준 인코딩, 이미지, 사운드가 있는 텍스트를 메시지를 통합하기 위한 조항

이메일 작동 방식

MTA: message transfer agent :smpt -> 보내는 겁니다.
MAA: message access agent : pop3, imap <- 가져오는거 
MTA server -> MTA Client -> Internet -> MTA server -> MAA server 

Mail box : 사용자를 위한 수신 메시지 저장
spool 송신메시지의 저장

mail server 간에 smtp mta로 보냄 최종 목적지에서 서버에서 클라이언트 이때 imap/pop maa

이메일 주소

mx(mail exchanger) (도메인이름이랑 메일서버로 변환) 리소스 레코드를 가진다. 

일부 네트워크는 더 효율적인 전달을 위해 여러 개의 이메일 서버의 계층 구조를 사용

smtp simple mail transfer protocol
서버포트25번 tcp

이메일 요청 눕

서버 응답 코드

헤더(송신자, 수신자 정보)와 바디(데이터 내용) 블랭크라인으로 구분

mime으로 인코딩하고 디코딩한다. 베이스64라는 아스키코드표처럼 존재

메일박스에 최종적으로 송신하기 위해서 smtp를 씀
사용자는 메일박스에 접근해서 메일을 봐야함

메시지 접근 프로토콜 pop : post office protocol : 권한 획득과 다운로드 볼수만 있다.
imap internet mail access protocol : pop 보다 좋은 듯 왜냐 많은 기능이 있다. 구현 복잡, 편지함을 생성 삭제 변경할 수 있다.

이메일 클라이언트 : smtp를 사용해 전송, pop3 imap을 써서 수집, 메일 메시지를 읽기 관리, 작성할 수 있는 ui 제공

이메일클라이언트는 smtp클라이언트와 메일 검색(pop imap) 클라이언트를 모두 수행 할 수 있어야 함

웹 메일

핫 메일, 야후 메일, 구글 지메일이 웹 메일 서비스

smtp -> smtp -> http
http -> smtp -> http

스팸(spam) : spam 메일박스에 혼란을 야기하는 대량 이메일 메시지의 별명 

스팸을 식별하고 제거할 수 있는 옵션
대규모 주소 목록(블랙리스트)를 축적하여 필터링

방화벽 뒤에 smtp 서버를두고 수신 smtp요청을 차단해서 스팸발송자로부터 서버를 보호

허용된 주소 목록 화이트리스트 (보안 높음)

알 수 없는 출처의 메시지를 거부하는 그레이리스트 (스팸은 자동화도구인데 받았을 때 가지고 있으면 재전송을 안하겠지? 안하면 스팸이구나!)

피싱Phishing : 악성 웹 사이트의 링크를 보낸다. 가짜 위장 웹사이트

1번 piconet은 블루투스 pan의 구성요소
무선 랜 기본 구성단위는 bss입니다.

2번 단말이 이동 중에도 지속적으로 통신을 가능하게 하는 프로토콜 -> 모바일 ip 프로토콜

3번 자원레코드의 유형
soa start of authority : 존에 대한 책임 이름 하나의 soa를 가짐
mx : mail exhanger -> 메일 서버 지정
A(Address) -> ipv4 주소 지정
cname - 공식 호스트 이름

4번 호스트 구성 정보가 아닌 것은?
dhcp 서버주소

5번 제로 구성은 인터넷 연결이 안됨 로컬에서 쓰는거임

6번 방화벽에 대한 설명으로 틀린것?
방화벽은 주로 물리주소를 필터링 x <- ip주소랑 포트를 필터링

7번 nat : 공인 <-> 사설 주소 

8번 ipv6 128비트, flow label 자원 예약용, 다음 헤더 필드는 ipv4의 프로토콜 필드에 대응된다. ipv6는 icmp 프로토콜 기능을 포함하지 않는다. icmpV6는 포함

9번 ICMP를 이용한 것 : Traceroute 

10번 최상위 도메인 : kr, net, com, org, edu

11번 로컬 및 원격 파일들을 동일한 인터페이스 내에서 편리하게 접근

NFS LDAP(경량파일접근 연결은 아니다) CIFS/SMB 

12번 다음 중 원격 시스템 로그인이 아닌 것
route : routing 테이블 조회시 사용

13번 클라이언트가 서버에 접속할 때 1번
변경 명령은 연결설정이 아니구나
파일 목록을 서버에 요청 2번
서버에서 다운로드 3번

14번 자신을 제외한 나머지 노드로 브로드캐스트해서 스위칭 테이블을 채워야한다.

15번 목적지 ip 주소로 브로드 캐스트용 ip 주소가 사용되는 거

dhcp 서버 브로드캐스트용 ip, arp나 icmp 물리주소 dns 목적지 ip주소

16번 csma/ca 매커니즘

무선 lan에서 사용할 수 있는 매체접근제어 프로토콜
802.3은 근거리 통신망x ieee802.11 표준이다.
bss를 구성하는 프로토콜이다. 프로토콜이아니라 알고리즘임
rts랑 cts를 이용하여 충돌을 회피하는프 로토콜이다.

17번 ipv6의 주소 자동 구성 절차를 기술하시오.

mac주소를 이용해서 만든 인터페이스 식별자를 이용하여 링크로컬 ip주소를 생성 -> duplicate adreess detection 중복 주소 탐지 -> router solicitation/router advertisement -> global ip 주소가 생성

18번 www.amazone.com의 주소를 학교의 dns 서버로 질의하였다. 학교의 dns가 해당 주소를 캐시로 가지고 있지 않는 경우 반복적인 이름 해석으로 www.amazone.com의 주소를 얻어 오는 과정

local dns server 에서 com server에 질의 전달 amazone.com 주소를 com server이 알려줌 amazone.com 서버는 주소를 알고 있으므로 이를 전달해줌 www.amazon.com을 알려줌




15번 
```
