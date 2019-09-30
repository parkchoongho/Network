# Network

## 1. Ip와 도메인

### IP 주소 (Internet Protocol Address)

Protocol은 약속을 의미한다. 인터넷과 같은 거대한 체계가 움직이기 위해서는 약속된 체계가 필요한데 그것이 바로 **Internet Protocol**이다. 인터넷에 연결되어 있는 컴퓨터들이 서로 정보를 주고 받기 위해서는 고유한 식별 주소를 가지고 있어야 한다. 그 주소를 바로 **IP 주소** 라고 한다.

이러한 **IP 주소**는 큰 단점을 가지고 있는데 바로 기억하기 힘들다는 점이다. 우리가 전화할 때, 전화번호를 다 기억해서 전화하지 않고 이름을 검색해서 전화하듯이 인터넷에서도 같은 방식의 통신 방법이 존재한다. 인터넷은 **도메인 네임**을 통해 통신한다. 도메인 네임을 입력하면 그 도메인 네임에 해당되는 IP 주소로 접속하게 되는 것이다. 

ex) naver.com => 202.131.30.12, google.com => 216.58.220.174

컴퓨터는 도메인을 통해서 서버에 접속할 수 없다. (도메인은 사람들이 보기 쉽게 만들어 놓은 것.) 서버에 접속하기 위해서는 반드시 IP주소를 통해서만 가능하다. 

**그런데 어떻게 도메인 네임을 브라우저에 입력했는데 해당 서버에 접속이 가능한걸까?**

그건 바로 **Domain Name System**(이하 DNS)이 이를 가능하게 해주기 때문이다.

### DNS (Domain Name System)

**Domain Name System**이 동작하는 방식은 다음과 같다. 클라이언트 상에서 도메인 네임을 입력하면 Domain Name Server에 접속한다. 클라이언트 컴퓨터는 **Domain Name Server**의 IP 주소를 알고 있기 때문에 Name Server에 접속해서 클라이언트가 모르는 해당 도메인 네임의 IP 주소를 물어본다. Name Server에는 도메인 네임과 연결되는 IP 주소를 담고 있기 때문에 해당 IP 주소를 클라이언트에게 알려준다. 그러면 이제 클라이언트는 IP 주소를 알고 있기 때문에 도메인 네임에 연결되는 서버에 접속할 수 있게 된다.

**Tip**: 도메인을 사용하고 싶으면 도메인을 구입해서 Name Server에 등록해야 한다.