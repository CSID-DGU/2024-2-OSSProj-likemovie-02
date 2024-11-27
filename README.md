![ReelVision](https://github.com/user-attachments/assets/148ddd24-061a-4791-a571-06c624f01f31)

<br/>
<br/>

# 1. Project Overview (프로젝트 개요)

- 프로젝트 이름: ReelVision
- 프로젝트 설명: 연극영화과 졸업작품 홍보/후원 플랫폼

<br/>
<br/>

# 1.1 개발 동기

- 졸업작품을 선보일 플랫폼 부족
  현재 졸업 작품은 영화제 혹은 짧은 시간 영화관을 대여하는 것을 제외하고는 외부에 공개할 수 있는 기회가 제한되어있다. 오랜 시간 공들여 완성한 작품이 조금 더 다양한 곳에서 공개될 수 있다면 영화과 학생들의 창작의지가 더욱 커질 수 있을 것이라고 생각한다.

- 영화과 졸업 학생들을 타겟으로 한 플랫폼의 필요성
  졸업영화는 대부분 사비로 제작비용을 충당하고, 나머지는 크라우드 펀딩 플랫폼으로부터 펀딩을 받아서 제작되고 있다. 하지만 막상 펀딩은 제작비용의 많은 비율을 차지하지 않고 있다. 비용에 대한 갈증이 조금이나마 해소가 된다면 졸업영화의 퀄리티가 높아지고 그것이 곧 졸업영화에 대한 관심으로 이어질 수 있을 것이라고 생각한다.

## <선행사례와의 비교>
(![선행사례 비교](https://github.com/user-attachments/assets/e680a2ef-a4c6-4d9e-abfb-159506b7a6e7)
)

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
  - 로그인: 사용자 정보를 입력받아 일치하는 경우 또는 JWT 세션 토큰을 발급함
  - 로그아웃: 사용자 세션을 종료하고 JWT 또는 세션 토큰의 만료 시간을 연장하기 위한 기능

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

<br/>
<br/>

# 4. Technology Stack (기술 스택)
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
