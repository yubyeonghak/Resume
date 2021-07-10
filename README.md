# 이력서

한림대학교 컴퓨터공학과 유병학


<img src="https://user-images.githubusercontent.com/73990783/125161374-e5c61f80-e1bc-11eb-9d95-b80980551ce7.jpg" alt="사진" width=30% hight="30%">


> - __E-mail__
>> qudgkr5652@naver.com
> - __전화번호__
>> __010-3309-5652__
> 
> - __학력__
>> __한림대학교 재학__ (2022년 졸업 예정)
> - github 주소
>> https://github.com/yubyeonghak


```
어제보다 더욱 발전하는 것을 모토로 삼고 있습니다.
```

- 군필여부: 육군 복무완료
- 취미: 볼링, 당구, 음악 감상, **카페 코딩**
- 자격증 : **정보처리기사**, 1종 보통 면허
- 수상 이력 : Coding Festival 입상

## 사용 언어
### C언어(강점)
- 멘토의 자격으로 C언어 멘토링 1년
- Socket 통신을 통한 리눅스 환경에서의 다중 채팅방 구현
- Coding Festival 입상

### Python
- IoT기반 반려동물 케어시스템 구현
- 이미지를 활용한 영상처리 프로젝트

### JAVA
- MQTT기반 IoT 통신 시스템 구현
- 위치기반 나눔 거래 어플 제작


### 기타
- C++언어를 사용할 수 있으며 활용하는 능력 보유
- 나눔 거래 어플 및 반려동물 케어시스템으로 창업 동아리 경험
- 학술 동아리 '노네임' 3년 활동 및 총무부장 1년
- 빅데이터 학생회 홍보 국장 1년
- 반려동물 케어 시스템관련 서베이 논문 1매

--- 
## 다중 채팅방 구현
- Kali linux 환경에서 C언어로 구현
- 동시 동작 : 다수의 클라이언트 및 다수의 채팅방을 동시에 서비스 할 수 있어야 함
- 비동기 채팅 : 사용자는 언제든 메시지를 입력할 수 있어야 함
- 다중 채팅 : 하나의 채팅방에 다수의 사용자가 참여할 수 있어야 함
---

<img src="https://user-images.githubusercontent.com/73990783/125162236-b239c400-e1c1-11eb-879e-06352907297c.png" alt="사진" width="45%" hight="45%">   <img src="https://user-images.githubusercontent.com/73990783/125162528-4fe1c300-e1c3-11eb-8e3d-4c8afe380afc.jpg" alt="사진" width="50%" hight="50%">

네트워크에 대한 지식을 토대로 SOCK_STREAM(TCP) 다중 채팅방을 구현하였습니다.

소스 코드는 Server, Client_Display, Client_input으로 구성되어있으며 각 역할은 아래의 표와 같습니다.

|이름|역할|
|-----|-----|
|Server| **AF_INET Server** <br> - Client 접속 시 메뉴 전송　　　　　 - 입력 받은 값에 따른 수행 및 출력　 |
|Client_Display| **AF_INET Client & AF_UNIX Server** <br> - Server에게 받은 메뉴 출력 　　　　 - Client_input 에게 받은 값 전달　 |
|Client_input| **AF_UNIX Client** <br> - 입력하여 Client_Display에게 전달 　| 


- 아래는 각 채팅방에 입장 후, 같은 채팅방에 있는 Client끼리 채팅하는 과정을 보여준다.

- Client_input 창에서 입력을 하면 Client_Display 창에 출력이 되고 서버로 메세지를 전송해준다.  <br>

- 위와 같은 행위를 감지하면 서버는 어떤 행위인지 출력하고 같은 채팅방의 Client에게 메세지를 보내준다. <br>

<img src="https://user-images.githubusercontent.com/73990783/125167288-bcb48780-e1da-11eb-9821-257e4e2a9a82.jpg" alt="사진" width="100%" hight="100%">


