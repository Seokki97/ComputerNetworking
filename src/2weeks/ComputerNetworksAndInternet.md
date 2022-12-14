데이터 통신과 네트워크
====================

Osi 7 layer이란 ?
--------------
네트워크에서 통신이 일어나는 과정을 7단계로 나눈 것.

나눈 이유는?
-----------------
- 계층을 나눈 이유는 통신이 일어나는 과정을 단계별로 파악하기 위해서.
- 흐름을 한눈에 알아보기 쉽고, 사람들이 이해하기 쉽다.
- 또한 특정한 곳에 이상이 생기면 이상이 상긴 단계만 수정하면 되기 때문이다.


각 계층을 알아보기 
---------------

###1계층 - 물리 계층
- 이 계층에서는 주로 전기적, 기계적, 기능적인 틍성을 이용해서 통신 케이블로 데이터를 전송한다. 
- 통신 단위는 bit이고, 전기신호로 오고간다 생각하면 됨.
- 이 계층에서는 단지 데이터를 전달할 뿐 데이터가 무엇인지, 어떤 에러가 있는지 등에는 전혀 신경쓰지 않는다.
- 대표적인 것: 통신 케이블, 리피터, 허브
- 즉 케이블 리피터 허브를 통한 데이터 전송

### 2계층 - 데이터 링크 계층
- 물리 계층을 통해 송수신되는 정보의 오류와 흐름을 관리하여 안전하게 정보의 전달을 수행할 수 있도록 하는 역할을 한다.
- 이 계층에서는 맥 주소를 가지고 통신하게 된다
- 전송되는 단위는 프레임이고, 장비는 브리지, 스위치 등이 있다.
- 데이터 링크 계층은  point to point간 신뢰성 있는 전송을 보장하기 위해 CRC기반의 오류 제어와 흐름 제어가 필요하다.
- 주소 값은 물리적으로 할당 받는데, 카드가 만드러질 떄부터 맥 주소가 정해져 있다는 뜻이다.
- EX) 이더넷, HDLC ADDCP 프로토콜, 패킷 스위칭 네트워크 , LCC,ALOHA같은 근거리 네트워크용 프로토콜
- 즉 프레임에 주소부여(MAC 물리적 주소), 에러검출/재정송/흐름제어
### 3계층 - 네트워크 계층
- 가장  중요한 기능은 데이터를 목적지까지 가장 안전하고 빠르게 전당하는 기능(라우팅)
- 대표적인 장비 - 라우터
- 네트워크 계층은 여러개의 노드를 거칠 떄마다 경로를 찾아주는 역할을 함, 다양한 길이의 데이터를 전달하고, 전송 계층이 요구하는
- 서비스 품질을 제공하기 위한 기능적, 절차적 수단을 제공함
- 즉 주소부여(IP), 경로설정
### 4계층 - 전송계층
