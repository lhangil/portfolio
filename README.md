# portfolio

* 음식점 웹사이트 (개인)
* 2024.06.23 ~ 2024.07.10

* java, jsp,html,css, oracle, sql

* 담당역할 : 프로젝트 전반(기획, 디자인, 백엔드, 프론트엔드)

* GitHub Repository :(https://github.com/lhangil/restaurant)

* 시연영상 : https://drive.google.com/file/d/1qXHIiDydWtNpKVxWAzWZ_SMguZDzs7OY/view?usp=sharing

* 목표: 사용자가 편리하게 음식점 예약을 할 수 있도록 돕고,음식점의 위치를 확인
        관리자는 페이지를 통해서 예약, 회원들의 리뷰, 평점을 확인

  
세부기능
* 로그인한 사용자만 예약을 진행할 수 있도록 구현, 로그인 정보는 Session을 통해 관리. 사용자가 로그인하면, 세션에 저장된 사용자 정보를 기반으로 예약을 진행
* HTML 폼을 통해 날짜와 인원수를 입력받고, request.getParameter를 사용하여 데이터를 서버로 전달
* 서버에서는 DAO 패턴을 사용하여 예약 정보를 데이터베이스에 저장하며, 예약할 때 같은 날짜에 예약이 이미 5개 이상 존재하면, SQL 쿼리로 날짜별 예약 수를 확인하여 조건을 만족할 경우 "그 날짜는 예약이 초과되었습니다"라는 메시지를 표시

　
* 로그인한 사용자가 자신의 예약 정보를 확인하고 관리. 세션에 저장된 사용자 정보를 이용하여, 해당 사용자의 예약 정보만을 데이터베이스에서 조회. DAO 패턴을 사용하여 SQL 쿼리로 사용자의 예약 정보를 필터링하여 조회
* JSP 페이지에서 예약 정보는 HTML 테이블로 출력
* 사용자는 자신의 예약을 취소가능. 예약 취소 버튼을 누르면 해당 예약 ID를 기반으로 DAO에서 SQL 쿼리를 실행해 예약 데이터를 삭제.


* 사용자가 로그인하면 세션을 통해 로그인 정보를 관리. 로그인된 사용자만 리뷰 작성 페이지에 접근
* HTML 폼과 JavaScript를 사용해 1~5개의 별점을 선택
* 로그인 정보는 세션을 통해 관리. manager 권한을 가진 사용자만 리뷰 삭제


![스크린샷 2024-09-15 154401](https://github.com/user-attachments/assets/ad468cbd-a31b-4c78-9e71-c70025e71940)




***

* 실시간 눈 추적을 통한 졸음 감지  (개인)
* 2024.04 ~ 진행중

*Python, Dlib, OpenCV

*GitHub Repository : (https://github.com/lhangil/eye_detect.git)

*목표: 실시간 웹캠 화면에서 얼굴을 인식, 눈 감음 여부를 분석

세부기능

1. 얼굴 인식 및 랜드마크 검출
-Dlib 라이브러리를 사용하여 실시간으로 얼굴을 검출, 얼굴의 랜드마크(특징점)를 추출  
-얼굴 검출 후 68개의 랜드마크 점을 표시하여 시각적으로 확인  

2. 눈 감음 감지
-랜드마크에서 눈 좌표를 계산하여 눈 영역에 박스를 표시합니다  
-눈이 감겼을 때와 떴을 때를 감지하고, 이를 0.0(눈 감음)과 1.0(눈 뜸)으로 표시  
-예측 결과를 기반으로 눈 감음 상태가 지속되면 "SLEEPING.... z" 메시지  

4. 실시간 웹캠 화면 처리
-OpenCV를 사용하여 웹캠에서 실시간 화면을 받아 얼굴 인식과 랜드마크 검출 작업을 수행  
-BGR에서 RGB로 변환 후 저장  

<img src="https://github.com/user-attachments/assets/2b523b85-a46c-4377-bc95-439405d9fecd" width="44%" />  
<img src="https://github.com/user-attachments/assets/a903ff2f-bf4f-4365-a007-9733f41a9831" width="44%" />  
<img src="https://github.com/user-attachments/assets/25e00ed9-b171-48d9-ad64-647532a7adc5" width="44%" />  

***




* 수어 탐지 (개인)
* 2024.07.15 ~ 2024.07.26

* Python, YOLO, OpenCV

* *GitHub Repository (https://github.com/lhangil/hand-detect)

* 목표: 실시간 웹캠에서 손을 인식, 탐지된 수어를 표시

* 세부기능

1. 실시간 웹캠 화면 처리  
-OpenCV를 사용하여 실시간으로 웹캠 화면을 가져오고, YOLO 모델을 통해 수어를 인식  

2. 손 인식 및 수어 탐지  
-손이 없는 경우 별도의 메시지 없이 화면만 출력    


3. 수어 탐지 결과 출력  
-YOLO 모델이 탐지한 수어 제스처에 대해  수어 제스처의 종류 및 신뢰도 출력  

<img src="https://github.com/user-attachments/assets/e32d5851-f844-474d-a90a-b33661b3599b" width="44%" />  
<img src="https://github.com/user-attachments/assets/ef628eb2-9f28-422d-8ab1-b58a40b8e7df" width="44%" />  
<img src="https://github.com/user-attachments/assets/b19a6996-d1db-4b67-93d3-89c596ed26ae" width="44%" />  








***
* 메일 프로그램

* 2024.06.09 ~ 2024.06.14

* java, jsp, css, sql
>
* 담당역할 : 프로젝트 전반(기획, 디자인, 백엔드, 프론트엔드)

* GitHub Repository :https://github.com/lhangil/email-project

* 시연영상 : https://drive.google.com/file/d/1XjiiSj0MGBkJOIZeI9b7cW8vVLPShRRn/view?usp=sharing

* 목표 : 사용자가 로그인한 아이디로 메일을 보내고 받을 수 있음

세부기능
1) 메일보내기
- 사용자는 로그인 후 , 받은 메일함 화면에서 바로 메일쓰기가 가능  
- 상단에서 ‘메일 보내기’를 눌러 새로운 메일쓰기가 가능하다.  

2) 메일함
- 제목과 받는 사람의 아이디를 입력후 내용을 입력하면 받는 아이디로 로그인 시 메일 수신  

3) 로그인 및 회원가입
- 회원가입 후 로그인을 하면 맨 오른쪽 위 상단에 [‘아이디’님으로 로그인중…] 이라고 표시  




![스크린샷 2024-09-15 162248](https://github.com/user-attachments/assets/bcac73b2-033d-43f3-9dad-a531259b8992)




***



