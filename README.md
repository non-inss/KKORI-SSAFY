# 🐶 하이퍼 로컬 기반 강아지 산책대행 프로젝트 KKORI 🐶
<div align="center">
  <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/7076d691-7933-4389-a06e-5de73416dcfd" width="200" hight="200">
</div>

# 프로젝트 소개

* 프로젝트명: 너와 나의 연결 KKORI
* 주요 기능
  - BLE,UWB 기기를 통한 반려견 관리
  - 반려견 위치 추적 및 산책현황
  - 게시판, 로그인, 지도
  - real time 채팅
  - QR 인증을 통한 산책대행 관리
* 주요 기술
  - EC2, S3, firebase

  - ReactNative.js, Node.js, Expo, android

  - Springboot, Spring Security, JPA, QueryDSL, JWT Authentication, OAuth, REST API

* 참조 리소스
  * 구글맵
  * 카카오 주소 api : 주소를 지번으로 변환후 지번을 추출하여 위도경도로 변환
  * gifted-chat : 디자인 전반적 사용
  * firebase : realtime DB에 채팅 저장, 산책현황좌표 기록 후 산책 루트 드로잉
  * lottiefiles: 메인 페이지 진입 애니메이션에 활용
* 배포 환경
  -https://drive.google.com/file/d/1o74JpKF7mp-bgxnmIbbMmZ_E3pIn_8e4/view?usp=sharing



# KKORI 기획 :satellite:

SNS와 유튜브 등에서 밈과 성대모사가 활발하게 퍼져나가고 있습니다.<br>
이러한 트렌드를 반영하여, **사용자들이 연기를 손쉽게 연습하고, 공유하고 즐길 수 있는 플랫폼**의 필요성을 인지하게 되었습니다.

# KKORI 소개📄
* REON은 다양한 작품의 명장면을 따라하며 즐겁게 연기하는 서비스입니다.:astonished:
* 홀로 **연기 연습**, 다른 유저와 **연기 베틀**이 가능합니다.:film_frames:
* 사용자의 연기를 **AI가 평가**한 후 연기 점수를 제공합니다.:100:
* 자신의 연기 영상을 공유하며 다른 사용자들과 소통할 수 있습니다.	:clap:

# 기능 소개💡
* KKORI 주요 기능은 다음과 같습니다!
<table>
  <tr>
    <th style="text-align: center;">앱로딩-메인</th>
    <th style="text-align: center;">게시판</th>
  </tr>
  <tr>
    <td style="text-align: center;">
      <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/fe8923f2-395a-4c69-9ec3-820558f541dd" alt="시작" width="300" height="300"/>
      <p>앱 시작 화면입니다!</p>
    </td>
    <td style="text-align: center;">
      <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/6626018b-0f9b-40ad-9638-82ca37818ebf" alt="게시판" width="300" height="300"/>
      <p>게시판 화면입니다!</p>
    </td>
  </tr>
  <tr>
    <td colspan="2">
      <ul>
        <li>1:1 화상 연기 배틀을 진행합니다.</li>
        <li>표정과 음성을 이용하여 연기를 채점합니다.</li>
        <li>AI 모델로 원본 영상과의 감정을 비교하여 채점합니다.</li>
        <li>사용자의 음성을 STT로 변환하여 원본 영상의 대본과 비교하여 채점합니다.</li>
      </ul>
    </td>
  </tr>
  <tr>
    <th style="text-align: center;">채팅</th>
    <th style="text-align: center;">지도 및 클러스팅</th>
  </tr>
  <tr>
    <td style="text-align: center;">
      <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/d1f6e234-17e7-422e-815a-462d4f0f1d31" alt="채팅" width="300" height="300"/>
      <p>게시판에서 견주에게 채팅을 보낼 수 있습니다!</p>
    </td>
    <td style="text-align: center;">
      <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/c7e97ca3-c14b-44fa-af7d-8c265898874a" alt="지도 및 클러스터링" width="300" height="300"/>
      <p>내 위치 기반 게시글을 볼 수 있습니다!</p>
    </td>
  </tr>
  <tr>
    <th style="text-align: center;">반려견 관리</th>
    <th style="text-align: center;">산책현황</th>
  </tr>
  <tr>
    <td style="text-align: center;">
      <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/79ab14af-9a46-4cde-a296-16a78a5d666e" alt="분실견 및 관리" width="300" height="300"/>
      <p>유저들이 업로드한 연기 영상을 볼 수 있습니다!</p>
    </td>
    <td style="text-align: center;">
      <img src="https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/11fce1e6-b512-4adb-bfe3-c1d96d2c0cce" alt="산책" width="300" height="300"/>
      <p>댓글과 좋아요로 소통할 수 있습니다!</p>
    </td>
  </tr>
</table>

## 메인 및 게시판 :movie_camera:

|앱로딩-메인|게시판|
|:---:|:---:|
| ![시작](https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/fe8923f2-395a-4c69-9ec3-820558f541dd) | ![게시판](https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/6626018b-0f9b-40ad-9638-82ca37818ebf)) |
|앱 시작 화면입니다!|게시판 화면입니다!|
- 1:1 화상 연기 배틀을 진행합니다.
- 표정과 음성을 이용하여 연기를 채점합니다.
- AI 모델로 원본 영상과의 감정을 비교하여 채점합니다.
- 사용자의 음성을 STT로 변환하여 원본 영상의 대본과 비교하여 채점합니다.

## 채팅 및 지도 :clipboard:
|채팅|지도 및 클러스팅|
|:---:|:---:|
| ![채팅](https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/d1f6e234-17e7-422e-815a-462d4f0f1d31)|![지도](https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/c7e97ca3-c14b-44fa-af7d-8c265898874a) |
|게시판에서 견주에게 채팅을 보낼수있습니다!|내 위치기반 게시글을 볼수있습니다!|

|반려견 관리|산책현황|
|:---:|:---:|
| ![분실견 및 관리](https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/79ab14af-9a46-4cde-a296-16a78a5d666e) | ![산책](https://github.com/non-inss/KKORI-SSAFY--/assets/122503960/11fce1e6-b512-4adb-bfe3-c1d96d2c0cce) |
|유저들이 업로드한 연기영상을 볼 수 있습니다!|댓글과 좋아요로 소통할 수 있습니다!|

- 연기 배틀을 종료하고, 여러분의 연기를 저장할 수 있습니다.
- 저장한 연기 영상을 공유하여 다른 사용자들과 소통하고 평가할 수 있습니다.
- 많은 사랑을 받은 연기는 REON 인기 영상으로 진입합니다.


# 서비스 이용 시나리오

|메인페이지|메인페이지|
|:---:|:---:|
| ![메인페이지1](./assets/images/메인페이지.png) | ![메인페이지2](./assets/images/메인페이지2.png) |
|상단 메뉴바를 이용하여 원하는 서비스를 이용할 수 있습니다.|사용자 메뉴를 선택하여 로그인, 로그아웃, 마이페이지 이동이 가능합니다.|

|같이하기-백스테이지|같이하기-튜토리얼|
|:---:|:---:|
| ![같이하기-백스테이지](./assets/images/같이하기-벡스테이지.png) | ![같이하기-튜토리얼](./assets/images/같이하기-튜토리얼.png) |
|상단 메뉴 같이하기 선택 시 입장하게 되는 페이지입니다.<br> 개인의 배틀 정보와 현재 top랭킹을 확인 할 수 있습니다.|게임을 시작하기에 앞서 튜토리얼을 통해 게임 방법을 확인 할 수 있습니다.|

|같이하기- 베틀페이지(1)|같이하기- 베틀페이지(2)|
|:---:|:---:|
| ![같이하기-베틀페이지1](./assets/images/같이하기-베틀페이지1.png) | ![같이하기-베틀페이지2](./assets/images/같이하기-베틀페이지2.png) |
|매칭된 유저의 화면이 보이고 가운데에 연기할 연기 영상 및 대본이 보입니다.|연기 영상이 보여진 후 차례대로 연기를 진행합니다.|

|같이하기-베틀페이지(3)|같이하기-베틀페이지(4)|
|:---:|:---:|
| ![같이하기-베틀페이지3](./assets/images/같이하기-베틀페이지3.png) | ![같이하기-베틀페이지4](./assets/images/같이하기-베틀페이지4.png) |
|자신의 차례가 아니라면 음소거 처리됩니다.|게임이 종료되면 승패 여부가 보여지고 자신의 연기 영상을 저장할 수 있습니다.|

|마이페이지|마이페이지-프로필 수정|
|:---:|:---:|
| ![마이페이지](./assets/images/마이페이지.png) | ![마이페이지-프로필수정](./assets/images/마이페이지-프로필수정.png) |
|유저 정보와 공개 연기영상, 비공개 연기영상, 좋아요를 누른 연기영상을 볼 수 있습니다.<br>다른 유저의 페이지라면 해당 유저가 공개한 연기 영상만 확인이 가능합니다.|프로필 이미지 수정이 가능합니다.|

|마이페이지-프로필 수정|마이페이지-비공개 영상 상세보기|
|:---:|:---:|
| ![마이페이지-프로필수정2](./assets/images/마이페이지-프로필수정2.png) | ![마이페이지-비공개영상상세보기](./assets/images/마이페이지-비공개영상상세보기.png) |
|자신의 닉네임, 자기소개 수정이 가능합니다.|저장된 연기영상을 볼 수 있고 투표해줘 게시판에 작성이 가능합니다.|

|마이페이지-게시글|마이페이지-좋아요|
|:---:|:---:|
| ![마이페이지-게시글](./assets/images/마이페이지-게시글.png) | ![마이페이지-좋아요](./assets/images/마이페이지-좋아요.png) |
|투표해줘 게시판에 올린 연기영상을 의미합니다.<br> 좋아요와 댓글로 소통이 가능합니다.|내가 좋아요를 누른 다른 사람의 연기영상을 볼 수 있습니다.|

|투표해줘 게시판|투표해줘-인기영상|
|:---:|:---:|
| ![투표해줘-게시판](./assets/images/투표해줘-게시판.png) | ![투표해줘-인기영상](./assets/images/투표해줘-인기영상.png) |
|소통과 평가를 위해 공개한 연기 영상들을 볼 수 있습니다.|한달동안 가장 좋아요를 많이 받은 영상들을 보여줍니다.|

|혼자하기|혼자하기|
|:---:|:---:|
| ![혼자하기](./assets/images/혼자하기.png) | ![혼자하기2](./assets/images/혼자하기2.png) |
|혼자 연기 연습을 할 수 있는 페이지입니다.|연기를 진행한 뒤 베틀과 동일하게 AI로 채점을 진행합니다.|


# 사용Tool
![kkori_tool](https://github.com/non-inss/KKORI-SSAFY/assets/122503960/a8189352-66af-4b74-868e-78ce06912d0c)

# API 연동 규격서 

[API 연동규격서 2975d5ee4025451b86d5de19703ef893.pdf](https://github.com/non-inss/KKORI-SSAFY/files/13446920/API.2975d5ee4025451b86d5de19703ef893.pdf)

# 시스템 구조도🏗️

![아키텍처](https://github.com/non-inss/KKORI-SSAFY/assets/122503960/bd179587-75fb-415e-9d14-6191188051d7)




