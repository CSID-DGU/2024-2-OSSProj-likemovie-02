[![ReelVision](https://github.com/user-attachments/assets/148ddd24-061a-4791-a571-06c624f01f31)](http://54.252.232.89:8000/)

<br/>
<br/>

# 1. Project Overview (프로젝트 개요)

- 프로젝트 이름: ReelVision
- 프로젝트 설명: 연극영화과 졸업작품 홍보/후원 플랫폼

<br/>
<br/>

## 1.1 개발동기 및 기대효과

- 졸업작품을 선보일 플랫폼 부족
  현재 졸업 작품은 영화제 혹은 짧은 시간 영화관을 대여하는 것을 제외하고는 외부에 공개할 수 있는 기회가 제한되어있다. 오랜 시간 공들여 완성한 작품이 조금 더 다양한 곳에서 공개될 수 있다면 영화과 학생들의 창작의지가 더욱 커질 수 있을 것이라고 생각한다.

- 영화과 졸업 학생들을 타겟으로 한 플랫폼의 필요성
  졸업영화는 대부분 사비로 제작비용을 충당하고, 나머지는 크라우드 펀딩 플랫폼으로부터 펀딩을 받아서 제작되고 있다. 하지만 막상 펀딩은 제작비용의 많은 비율을 차지하지 않고 있다. 비용에 대한 갈증이 조금이나마 해소가 된다면 졸업영화의 퀄리티가 높아지고 그것이 곧 졸업영화에 대한 관심으로 이어질 수 있을 것이라고 생각한다.

## <선행사례와의 비교>

![선행사례 비교](https://github.com/user-attachments/assets/e680a2ef-a4c6-4d9e-abfb-159506b7a6e7)

# 2. Team Members (팀원 및 팀 소개)

- **오픈소스소프트웨어프로젝트 2조**:

  - 고윤건: BE
  - 신예성: FE
  - 정가경: BE
  - 허재원: BE
  - 현광수: BE
    <br/>
    <br/>

# 3. Key Features (주요 기능)

- **회원관리**:

  - 회원가입: 사용자 입력 데이터의 유효성 검사, 중복 확인 등의 절차를 포함하고 있음
  - 로그인: 사용자 정보를 입력받아 일치하는 경우 또는 세션 토큰을 발급함
  - 로그아웃: 사용자 세션을 종료함

  ![OSSP_Group_2_LikeMovie_중간_발표_자료 (1)](https://github.com/user-attachments/assets/2cea2e1e-a0b3-44d1-9e71-618d8aa29a28)

- **마이페이지**:

  - 프로필 확인 및 수정: 회원가입에서 등록한 user의 정보 수정, 프로젝트를 등록할 때와 프로젝트에 후원한 금액 환불
  - 영화 목록 확인: user가 구매한 영화, 후원한 영화, user가 등록한 프로젝트 확인

- **결제**:

  - 후원 결제
  - 스트리밍 결제
  - 결제 페이지 리디렉션

- **영화 등록/재생**:

  - 영화를 등록하고 재생할 수 있음

  ![OSSP_Group_2_LikeMovie_중간_발표_자료 (3)](https://github.com/user-attachments/assets/d70db255-fa4e-4ef2-a26b-e18f8150c567)
  ![OSSP_Group_2_LikeMovie_중간_발표_자료 (6)](https://github.com/user-attachments/assets/e966ea32-af49-4aa1-b282-0e6e5218c06a)

- **admin**:

  - 회원 정보 및 프로젝트 정보 수정

- **프로그램 전체 ERD**:

![OSSP_Group_2_LikeMovie_중간_발표_자료](https://github.com/user-attachments/assets/37ec3ea9-cb9e-4b7c-83a1-eba1644a772b)

- **시스템 구성 다이어그램**:

<img width="877" alt="구성다이어그램" src="https://github.com/user-attachments/assets/6bd50ef3-4836-4e85-82c9-1e8d29c7ce55" />

- **Use-case 다이어그램**:

<img width="613" alt="use" src="https://github.com/user-attachments/assets/89c38162-ab93-4cf9-870b-ea34f7e0fc74" />

- **시스템 구조**:

<img width="401" alt="시스템" src="https://github.com/user-attachments/assets/e9760ce4-76ca-4030-9bb3-2bad8636ddc0" />

- **프로젝트 구조**:
```plaintext
├── common
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── authentication.py
│   ├── middleware.py
│   ├── migrations
│   ├── session_backend.py
│   ├── static
│   ├── templates
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── db.sqlite3
├── funding
│   ├── __init__.py
│   ├── forms.py
│   ├── migrations
│   ├── models.py
│   ├── static
│   ├── templates
│   ├── urls.py
│   └── views.py
├── get-pip.py
├── main_page
│   ├── __init__.py
│   ├── __pycache__
│   ├── admin.py
│   ├── apps.py
│   ├── migrations
│   ├── models.py
│   ├── static
│   ├── templates
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── manage.py
├── mongodbconnect
│   ├── __init__.py
│   ├── __pycache__
│   ├── asgi.py
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
├── mypage
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py
│   ├── migrations
│   ├── static
│   ├── templates
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── payments
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py
│   ├── templates
│   ├── tests.py
│   ├── urls.py
│   └── views.py
├── static
│   ├── images
│   └── style.css
└── streaming
    ├── __init__.py
    ├── admin.py
    ├── apps.py
    ├── forms.py
    ├── migrations
    ├── models.py
    ├── serializers.py
    ├── static
    ├── templates
    ├── tests.py
    ├── urls.py
    └── views.py
```


<br/>
<br/>

# 4. 배포(AWS)

### 1. EC2 인스턴스 생성

- **인스턴스 이름**: ReelVision
- **인스턴스 유형**: t2.micro
- **AMI**: Ubuntu
- **네트워킹**: 퍼블릭 IP 활성화 (외부 연결 허용)
- **보안 그룹 설정**:
  - 포트 22: SSH 접속 허용
  - 포트 8000: Django 접속 허용
  - 포트 27017: MongoDB 접근 허용

### 2. EC2 접속 및 환경 설정

1. **SSH를 통해 EC2 인스턴스 접속**
2. **로컬에서 완성한 Django 프로젝트를 EC2 서버로 옮기기**
3. **Docker 및 Docker Compose 설치**
   - Docker와 `docker-compose.yml` 파일을 이용해 환경 구성
4. **프로젝트 및 DB 컨테이너 구성 및 실행**
   - Docker 컨테이너를 사용하여 Django 프로젝트와 DB 실행
5. **Django 애플리케이션 DB와 연결**
   - EC2 서버에서 Django 애플리케이션을 실행하고 DB 연결 확인
6. **퍼블릭 IP를 사용한 외부 접근 허용**
   - AWS EC2의 퍼블릭 IP를 사용하여 어플리케이션에 외부에서 접근 가능하도록 설정
<br/>
<br/>

# 5. Technology Stack (기술 스택)

<div align=center> 
  <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white"> 
  <img src="https://img.shields.io/badge/django-092E20?style=for-the-badge&logo=django&logoColor=white"> 
  <img src="https://img.shields.io/badge/pycharm-000000?style=for-the-badge&logo=pycharm&logoColor=white">
  <br>
  
  <img src="https://img.shields.io/badge/html5-E34F26?style=for-the-badge&logo=html5&logoColor=white"> 
  <img src="https://img.shields.io/badge/css-1572B6?style=for-the-badge&logo=css3&logoColor=white"> 
  <img src="https://img.shields.io/badge/javascript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"> 
    <img src="https://img.shields.io/badge/vue.js-4FC08D?style=for-the-badge&logo=vue.js&logoColor=white"> 
 <img src="https://img.shields.io/badge/figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white">
  <br>
  
  <img src="https://img.shields.io/badge/mongoDB-47A248?style=for-the-badge&logo=MongoDB&logoColor=white">
  <img src="https://img.shields.io/badge/mongoose-880000?style=for-the-badge&logo=mongoose&logoColor=white">
  <img src="https://img.shields.io/badge/amazone s3-569A31?style=for-the-badge&logo=amazone s3&logoColor=white">
  
  <br>
  
  <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white">
  <img src="https://img.shields.io/badge/git-F05032?style=for-the-badge&logo=git&logoColor=white">
  <br>
</div>

<br/>
<br/>

# 6. API 명세서

| **기능**          | **HTTP Method** | **API 경로**                        | **설명**                   |
|------------------|-----------------|-------------------------------------|---------------------------|
| **회원가입/로그인** |                 |                                     |                           |
| 회원가입           | POST            | `/signup/`                          | 신규 사용자 회원가입       |
| 로그인             | POST            | `/signin/`                          | 사용자 로그인             |
| 동국대 인증 메일 발송 요청 | POST    | `/verify-email/<str:token>/`       | 이메일 인증 요청          |
| 메일 인증 확인     | GET             | `/verify-email/<str:token>/`       | 이메일 인증 확인          |
| 로그아웃           | GET             | `/logout/`                          | 사용자 로그아웃           |
| **마이페이지**     |                 |                                     |                           |
| 프로필 조회        | GET             | `/mypage/`                          | 마이페이지 프로필 정보 조회|
| 프로필 수정        | GET             | `/update_profile/`                  | 프로필 정보 수정          |
| 비밀번호 수정      | GET             | `/change_password/`                 | 비밀번호 변경             |
| 등록한 프로젝트 조회| GET           | `/my_projects/`                     | 내가 등록한 프로젝트 목록  |
| 후원한 프로젝트 조회| GET           | `/funded_movie/`                    | 후원한 프로젝트 목록      |
| 구매한 프로젝트 조회| GET           | `/purchased_movie/`                 | 구매한 프로젝트 목록      |
| **펀딩**           |                 |                                     |                           |
| 펀딩 영화 업로드    | POST            | `/funding/upload`                   | 펀딩 영화 업로드          |
| 펀딩 영화 상세 조회 | GET             | `/funding/<str:movie_id>/`          | 특정 펀딩 영화 상세 조회  |
| 펀딩 영화 목록 조회 | GET             | `/funding/movie/list`               | 펀딩 영화 목록 조회       |
| 이미지 조회        | GET             | `/funding/poster/<str:poster_id>/`  | 포스터 이미지 조회        |
| 결제 성공          | GET             | `/funding/payment/success/`         | 결제 성공 리디렉션        |
| 결제 실패          | GET             | `/funding/payment/fail`             | 결제 실패 리디렉션        |
| 결제 여부 확인      | GET             | `/funding/check_payment_status/`    | 결제 상태 확인            |
| **스트리밍**       |                 |                                     |                           |
| 스트리밍 영화 업로드| POST            | `/streaming/upload`                 | 스트리밍 영화 업로드      |
| 스트리밍 영화 상세 조회 | GET        | `/streaming/<str:movie_id>/`       | 특정 스트리밍 영화 상세 조회|
| 스트리밍 영화 목록 조회 | GET        | `/streaming/movie/list`            | 스트리밍 영화 목록 조회   |

<br/>
<br/>

# 7. 관련 자료

- [회의록](https://github.com/CSID-DGU/2024-2-OSSProj-likemovie-02/tree/main/Doc/%ED%9A%8C%EC%9D%98%EB%A1%9D)
- [시연영상](https://github.com/CSID-DGU/2024-2-OSSProj-likemovie-02/tree/main/Doc/%EC%8B%9C%EC%97%B0%EC%98%81%EC%83%81)
- 보고서
  - [수행계획서](https://github.com/CSID-DGU/2024-2-OSSProj-likemovie-02/blob/main/Doc/%5B2%EC%A1%B0%5D%20%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4SW%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%88%98%ED%96%89%EA%B3%84%ED%9A%8D%EC%84%9C.pdf)
  - [중간보고서](https://github.com/CSID-DGU/2024-2-OSSProj-likemovie-02/blob/main/Doc/%5B2%EC%A1%B0%5D%20%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4SW%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8_%EC%A4%91%EA%B0%84%EB%B3%B4%EA%B3%A0%EC%84%9C.pdf)
  - [최종보고서](https://github.com/CSID-DGU/2024-2-OSSProj-likemovie-02/blob/main/Doc/%5B2%EC%A1%B0%5D%20%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4SW%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%B5%9C%EC%A2%85%EB%B3%B4%EA%B3%A0%EC%84%9C.pdf)
- [발표자료](https://github.com/CSID-DGU/2024-2-OSSProj-Running-Machines-04/blob/main/doc/241119_%EC%A4%91%EA%B0%84%EB%B3%B4%EA%B3%A0%EC%84%9C/Running%20Machines_04%20%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4SW%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A4%91%EA%B0%84%EB%B3%B4%EA%B3%A0%EC%84%9C.pdf)

<br/>
<br/>
