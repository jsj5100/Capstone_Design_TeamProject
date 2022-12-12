# Capstone_Design_시각장애인을 위한 자판기
   * 이 파일은 캡스톤 디자인 포트폴리오를 위해 작성되었습니다.
   * 팀장 전성진, 팀원 윤준영, 김병현으로 구성된 팀 프로젝트입니다.
   * 과제 개발이 완성 될때까지 갱신되는 포트폴리오 입니다. /22.12.12
   
   ![image](https://user-images.githubusercontent.com/119272401/206913526-dd158bc4-9f01-4fbd-90b9-d0ceffc31b34.png)
   ![image](https://user-images.githubusercontent.com/119272401/206913530-69504620-6ac5-4a21-a274-aff0466e477e.png)


   
# 팀원 명단
  * 남서울대학교 지능정보통신공학과
1. 전성진 18100175
2. 윤준영 18100154
3. 김병현 18100099

# 역할
1. 전성진 - 웹서버 & 자판기 제작 & 설계
2. 윤준영 - 아두이노 & 중간레포트 작성
3. 김병현 - 라즈베리 파이 & 웹 서버

# 프로젝트 기간
  * 2022 년 8 월 29 일 ~ 2022 년 12 월 5 일 (3 개월)

# 과제 수행비
1. 지원금 - 200,000
2. 사용 금액 - 36,000
3. 잔액 - 164,000

# 개요

### 과제 개요 및 필요성
[캡스톤] IT종합설계기초 수업의 과제를 개발하기에 앞서, 우리 조는 ‘시각장애인을 위한 자판기’라는 주제로 선정했다.
우리 사회에서 시각장애인을 위한 배려는 사소한 부분까지 잘 이루어지고 있지 않다. 교차로의 음향 신호등 또한 턱없이 부족하거나, 길거리의 점자블록이 훼손된 상태로 방치 되어 있거나, 여러 부분 중 우리가 편하게 이용하는 자판기도 시각장애인은 대부분 점자조차 제대로 부착되어 있지 않아, 이용하기에 불편함을 느낀다. 심지어 자판기에 부착 되어 있는 음료와 관련된 점자는 '음료', '탄산', ‘맥주’ 세 가지 점자 정도로만 표기하는 경우가 많다.
그래서 시각장애인을 위해 보이지 않아도 소리로 들어 위치를 알 수 있는 자판기가 조금 더 실생활에 필요하다고 생각하여 개발하게 되었다.

![image](https://user-images.githubusercontent.com/119272401/206913569-8d6a3cb1-bf88-49aa-ad1a-ff14af4ff0de.png)
![image](https://user-images.githubusercontent.com/119272401/206913558-fd34ddf1-e122-4114-920e-a029f8340a1b.png)

### 과제의 기술
  * 아두이노 : C++
  * 라즈베리 파이 : Python
  * 웹 서버 : Java Script
  *
  * 시각장애인을 위한 자판기 개발 구성도
  
   ![image](https://user-images.githubusercontent.com/119272401/206912368-769636bd-99ec-4330-8764-14bf5440be7e.png)
   ![image](https://user-images.githubusercontent.com/119272401/206912455-75915cd4-5e8c-4e24-a38a-3f0d2881ba73.png)


# Capstone_Design 과제개발 내용

### 과제 내용
개발 구성안은 하드웨어와, 웹&서버 두 가지로 구성하여 설계하였다.
하드웨어 부분으로는 아두이노를 이용하여 행동(모션)을 인식하여 손을 인식하고. 인식한 감지 데이터를 웹서버를 통해 라즈베리 파이로 전송하여 데이터 가공 후에 스피커로 음성을 송출하는 개념이다.
웹&서버 부분은 라즈베리 파이가 가공된 데이터를 서버로 전송하면, 자판기 및 음료 정보나 판매된 음료 정보, 음료별 판매 통계등 기록하는 역할을 한다.
이 자판기를 만들기 위해서는 먼저 행동(모션) 인식이 제대로 이루어져야, 모든 것을 시작할 수 있다. 저항에 전하는 전류의 값을 보다 넓고, 편하게 전달하기 위하여 알루미늄 호일을 이용하여 저항과 납땜하여 센서를 만들었다.
  * 푸쉬버튼
  
  ![image](https://user-images.githubusercontent.com/119272401/206912523-0e477b98-58d1-4e8c-b130-e9f9079090d4.png)
  
  * 센서
  
  ![image](https://user-images.githubusercontent.com/119272401/206912550-65707a49-19bb-40dc-81cf-3c4695c2b31a.png)
  
  * 음성 출력
  
  ![image](https://user-images.githubusercontent.com/119272401/206912568-9bc6bc69-684c-4322-aece-6f51bc1b77b4.png)
  
  * 자판기 제작 & 센서 연결
  
  ![image](https://user-images.githubusercontent.com/119272401/206912589-7df0b094-84ed-494e-9b9a-8fb8df45963f.png)
  ![image](https://user-images.githubusercontent.com/119272401/206912591-686f2dab-b384-445f-ba82-0d8690ce15a5.png)

# Capstone_Design 과제개발 결과 및 활용방안
1. 작품 구성도 중, 하드웨어를 완성하였고, 웹서버와 클라이언트는 개발 단계에 있다.
이 자판기는 아두이노와 라즈베리 파이 두가지를 이용하여 개발된다. 현재 하드웨어 부분은 각각 완성하였고, 웹과 서버를 구축하여 연결하여 ‘인식’ 하여 ‘음성 송출’하는 시각장애인을 위한 자판기이다.

2. 이 자판기는 음료 자판기 뿐만아니라, 여러 종류의 간식 / 채소나 물건 / 도서 등 음성으로 알려줄 수 있기때문에 여러 방향으로 이용이 가능하다. 또한 언어적으로도 추가만 한다면 여러 나라별 언어로 음성 송출이 가능하다.
특히, 자판기 관련 웹을 개발한다면 전국에 이 자판기가 여러대 있다는 가정하에, 자판기의 위치도 지정이 가능해 자판기의 위치를 본인이 직접찾아 이용할 수 있다.


# 참고한 웹 사이트
한고 - https://youtu.be/D2CXURqW8qs

# 캡스톤디자인 과제개발비 정산보고서
  * (가공비) 자판기 모형
모형원판 (나무판자) 1개 = 11,000
원단보드롱(흰색)2P 1개 = 1,000
전기인두30W 1개 = 5,000
땜납 (전기인두용) 3개 = 3,000
스카치테이프 (18mm) 1개 = 2,000
바이오홈실리콘 1개 = 3,000
매장용 종이봉투(대) 1개 = 200
총 25,200

  * (재료비) 아두이노
중국 DS-JPC40C-MM30 2개 = 1,600
브레드보드SYB-170 흑 10개 = 3,000
TACK S/W (L) 8.5mm 10개 = 1,100
1/4W 1개 = 100
총 5,800

  * (재료비) 라즈베리파이
접지형스위치 콘센트3구 1개 = 5,000
총 5,000

합계 : 36,000
