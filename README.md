# Qualcomm Institute Health-Related IoT Tracking Platform

기간: 2019년 7월 4일 → 2019년 8월 14일
태그: IoT, Qualcomm Institute, 개발, 백엔드

## 🧐Overview


- 초미세 먼지 센서, 공기 질 센서, 심박수 센서를 활용한 사용자 산책 경로의 AQI(Air Quality Index) 제공 서비스 개발

<details>
<summary>서비스 화면 </summary>
<div markdown="1">


* 메인화면

![메인화면](https://user-images.githubusercontent.com/43032391/212911956-8a9d798b-93f6-4309-90d4-f274cdebe69e.png)

* 메인화면2

![메인화면2](https://user-images.githubusercontent.com/43032391/212912055-3e26e545-8cb2-43ce-b848-4b92f558f68a.png)

* 로그인 후 화면, 지도에서 Real-time Air Quality Data(최근 1분동안 측정된 값) 값을 확인 할 수 있다. 값은 CO,NO2,O3,SO2,PM2.5이며 AQI 색 값을 지도에 나타낸다

![로그인 후 화면, 지도에서 Real-time Air Quality Data(최근 1분동안 측정된 값) 값을 확인 할 수 있다. 값은 CO,NO2,O3,SO2,PM2.5이며 AQI 색 값을 지도에 나타낸다](https://user-images.githubusercontent.com/43032391/212912163-b5d962fa-22de-4d9e-85d7-2fe8d27d1892.png)


</div>
</details>


## 🙄Goal



1. 센서 파트, 웹클라이언트와 DB파트, 안드로이드 파트로 나누어 외국인 Instructor로부터 강의 수강
2. Heath-care IoT Tracking Platform 아이디어 주제 선정
3. 교육과정 최소 요구조건 만족하도록 개발(Reference Model, System Architecture, ER Model 등)



## 😤stack


- PHP, JavaScript, MySQL
- git, Vagrant,Postman

## 👓Role


## 설계 참여(팀)

<details>
<summary>1. Referene Model 작성</summary>
<div markdown="1">


* ReferenceModel - Node 간 관계를 나타내고 Protocol 이름을 정의

![ReferenceModel - Node 간 관계를 나타내고 Protocol 이름을 정의](https://user-images.githubusercontent.com/43032391/212912299-244b7212-ff71-4bba-a7ab-d95d92a3225a.png)


</div>
</details>

<details>
<summary>2. System Architecutre 작성</summary>
<div markdown="1">

* System Architecutre - 각 Node 별 기능 작성

![System Architecutre - 각 Node 별 기능 작성](https://user-images.githubusercontent.com/43032391/212912337-d5772603-aeb5-4c70-bf0b-37baccf405e8.png)


</div>
</details>



<details>
<summary>3. Database 의 ER Model 작성</summary>
<div markdown="1">

* ER Model - 회원가입 인증 전 정보를 저장하는 Temp_user, 인증된 회원을 관리하는 User, Polar Sensor 데이터값을 저장하는 Heart_rate_sensor, 공기질 센서 데이터값을 저장하는 Airquality_sensor, 센서 등록 데이터 값을 저장하는 Sensor_info 테이블로 구분

![ER Model - 회원가입 인증 전 정보를 저장하는 Temp_user, 인증된 회원을 관리하는 User, Polar Sensor 데이터값을 저장하는 Heart_rate_sensor, 공기질 센서 데이터값을 저장하는 Airquality_sensor, 센서 등록 데이터 값을 저장하는 Sensor_info 테이블로 구분](https://user-images.githubusercontent.com/43032391/212912373-1c4d80bc-ebf5-4347-8e92-8c667f033c7d.png)


</div>
</details>



<details>
<summary>4. Message 정의</summary>
<div markdown="1">

* 각 Procedure의 Request, Response, Query Name과 Parameter를 excel로 관리

![각 Procedure의 Request, Response, Query Name과 Parameter를 excel로 관리](https://user-images.githubusercontent.com/43032391/212912407-12af283e-f45d-4cef-a3e3-32e74b4ce75b.png)


</div>
</details>



<details>
<summary>기능 Procedure 작성</summary>
<div markdown="1">

* 회원가입 Procedure

![회원가입 Procedure](https://user-images.githubusercontent.com/43032391/212912428-e85df981-adbe-447d-8820-cb32951bac41.png)


* 로그인 Procedure
![로그인 Procedure](https://user-images.githubusercontent.com/43032391/212912445-ebb6fc36-ed49-4c20-9b85-f4a57ecd40bb.png)


* 로그아웃 Procedure
![로그아웃 Procedure](https://user-images.githubusercontent.com/43032391/212912497-c1b745e2-c1a8-4489-9963-19d06f993809.png)


* 비밀번호 찾기 Procedure

![비밀번호 찾기 Procedure](https://user-images.githubusercontent.com/43032391/212912515-0aa4fa0d-c5f5-42c8-a6a7-d3eabe309157.png)


* 비밀번호 변경 Procedure

![비밀번호 변경 Procedure](https://user-images.githubusercontent.com/43032391/212912537-3a4f6ca1-c15c-4640-8481-05c586adf097.png)


* 아이디 삭제 Procedure

![아이디 삭제 Procedure](https://user-images.githubusercontent.com/43032391/212912544-7afd4dc6-5848-4309-bc47-cf045f7777d3.png)


* 센서 등록 Procedure

![센서 등록 Procedure](https://user-images.githubusercontent.com/43032391/212913475-422fd33b-e13a-4c0b-ba3e-72f704b791ad.png)


* 센서 해제 Procedure

![센서 해제 Procedure](https://user-images.githubusercontent.com/43032391/212914085-dedca518-4a13-4313-889f-5b193b600b3b.png)


* 실시간 AQI 데이터 모니터링 Procedure

![실시간 AQI 데이터 모니터링 Procedure](https://user-images.githubusercontent.com/43032391/212914138-86a3755d-8780-4771-b5e7-f985ed42bf1c.png)



* 시간별 AQI 데이터 모니터링 Procedure

![시간별 AQI 데이터 모니터링 Procedure](https://user-images.githubusercontent.com/43032391/212915684-40a36e70-bafb-4c12-b2e6-163ab794832c.png)


* 실시간 심박수 데이터 모니터링 Procedure

![실시간 심박수 데이터 모니터링 Procedure](https://user-images.githubusercontent.com/43032391/212916394-a484301d-6fe9-4345-b1dc-c4fd2faacc85.png)


* 시간별 심박수 데이터 모니터링 Procedure

![시간별 심박수 데이터 모니터링 Procedure](https://user-images.githubusercontent.com/43032391/212916421-fc8b75db-e84f-4d4b-9fca-eb6df25a20cd.png)


</div>
</details>






## 백엔드 기능 개발(2인 1조)


1.MySQL 을 사용하여 데이터 베이스 구축

2.PHP Slim Framework를 이용한 서버 구축

<details>
<summary>3.유저 회원가입 및 메일인증 기능 구현</summary>
<div markdown="1">


* 회원가입 홈페이지

![회원가입 홈페이지](https://user-images.githubusercontent.com/43032391/212912820-352fb72f-8290-4752-9bed-14006d9ede20.png)


* 회원 가입 시 메일 인증

![회원 가입 시 메일 인증](https://user-images.githubusercontent.com/43032391/212912837-a2d847bf-c2ea-4e5e-ba74-9a9b862f24ee.png)


</div>
</details>



<details>
<summary>4.센서 연동 및 해제 기능 구현</summary>
<div markdown="1">


* 센서 등록 페이지
![센서 등록 페이지](https://user-images.githubusercontent.com/43032391/212913049-8d489ba7-5549-42a5-aa20-4b62ab467a95.png)



</div>
</details>

<details>
<summary>5.Javascript 을 사용하여 회원가입 및 센서 데이터 모니터링을 위한 프론트 앤드 개발</summary>
<div markdown="1">

* Google Direction API를 사용하여 시작 주소와 도착 주소를 입력하면 지도위에 경로를 나타냄

![Google Direction API를 사용하여 시작 주소와 도착 주소를 입력하면 지도위에 경로를 나타냄](https://user-images.githubusercontent.com/43032391/212913009-cd0391df-0553-4d0d-9cee-5d3acc5b8c55.png)

* Smoothie Charts API를 사용하여 실시간 심박수를 나타냄

![Smoothie Charts API를 사용하여 실시간 심박수를 나타냄](https://user-images.githubusercontent.com/43032391/212912964-cdff3bea-5ff1-41c1-a659-85c3fb9e97ac.png)


* Google Chart API를 사용하여 각 공기질 센서 데이터 값을 나타냄

![Google Chart API를 사용하여 각 공기질 센서 데이터 값을 나타냄](https://user-images.githubusercontent.com/43032391/212912977-4a451e8d-34e8-4959-b5f5-08beb2aae81d.png)
</div>
</details>



## 느낀 점
낯선 미국 땅에서 처음 보는 사람들과 약 한 달 동안 프로젝트를 진행하면서 팀워크의 중요성이 무엇보다 중요하다는 것을 느끼게 되었습니다.

교육 과정의 처음 1, 2주차에는 팀의 영어 발표가 미숙하여 가장 순위가 낮았지만, 팀원 모두 부족한 점을 알고 모두 열심히 참여하여 최종 발표 전엔 1등, 최종 발표 후엔 3등으로 순위가 오르는 성과가 있었습니다.

설계부터 개발까지 수 많은 피드백을 받았지만  5명의 팀원 모두 합심하여 한명도 포기하지 않고 무사히 프로젝트를 완료할 수 있었습니다. 다양한 사람과 새로운 환경에서 몰입하여 개발하였기 때문에 인상 깊은 프로젝트였습니다.

