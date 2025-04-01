<div align="center">

<!-- logo -->
<img src="https://github.com/user-attachments/assets/ce94c520-c5a1-4128-99d1-91c02e46efeb" width="800"/>
<br/>

[<img src="https://img.shields.io/badge/-readme.md-important?style=flat&logo=google-chrome&logoColor=white" />]() [<img src="https://img.shields.io/badge/release-v0.0.0-yellow?style=flat&logo=google-chrome&logoColor=white" />]() 
<br/> [<img src="https://img.shields.io/badge/프로젝트 기간-2025.02.24~2025.04.01-green?style=flat&logo=&logoColor=white" />]()
</div> 

<br/>

# 서비스 소개
얼굴 인식 기술을 활용해 입퇴장을 원활히 할 수 있도록 하고 입장한 방문객들을 관리할 수 있도록 서비스
비접촉식 얼굴 인식 기술을 통해 신속한 출입 인증과 효율적인 방문객 관리를 지원하여 기존 출입 절차의 번거로움과 긴 대기 시간 문제를 해결합니다. 또한, 외부인 출입 통제와 운영 부담을 줄여 행사 관리의 효율성을 높입니다

<br/>
<br/>

# 2. Team Members (팀원 및 팀 소개)
<table>
  <tr>
    <td align="center">
      <a href="https://github.com/lxxjune">
        <img src="https://github.com/lxxjune.png?size=100" width="100px;" alt="이지윤"/>
        <br />
        <sub><b>이지윤</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/s01d0ut">
        <img src="https://github.com/s01d0ut.png?size=100" width="100px;" alt="김혜진"/>
        <br />
        <sub><b>김혜진</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/kkyung99">
        <img src="https://github.com/kkyung99.png?size=100" width="100px;" alt="김현경"/>
        <br />
        <sub><b>김현경</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/funcsom">
        <img src="https://github.com/funcsom.png?size=100" width="100px;" alt="성소민"/>
        <br />
        <sub><b>성소민</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/AhnRian">
        <img src="https://github.com/AhnRian.png?size=100" width="100px;" alt="안리안"/>
        <br />
        <sub><b>안리안</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/sukangpunch">
        <img src="https://github.com/sukangpunch.png?size=100" width="100px;" alt="강형준"/>
        <br />
        <sub><b>강형준</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/Do-oya">
        <img src="https://github.com/Do-oya.png?size=100" width="100px;" alt="박정현"/>
        <br />
        <sub><b>박정현</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/jinhosoon">
        <img src="https://github.com/jinhosoon.png?size=100" width="100px;" alt="순진호"/>
        <br />
        <sub><b>순진호</b></sub>
      </a>
    </td>
    <td align="center">
      <a href="https://github.com/hen715">
        <img src="https://github.com/hen715.png?size=100" width="100px;" alt="이혜성"/>
        <br />
        <sub><b>이혜성</b></sub>
      </a>
    </td>
  </tr>
  <tr>
    <td align="center">PD</td>
    <td align="center">PD</td>
    <td align="center">FE</td>
    <td align="center">FE</td>
    <td align="center">FE</td>
    <td align="center">BE</td>
    <td align="center">BE</td>
    <td align="center">BE</td>
    <td align="center">BE</td>
  </tr>
</table>

<br/>

# 3. Key Features (주요 기능)
- **회원가입**:
  - 회원가입 시 MySQL에 유저정보가 등록됩니다.

- **로그인**:
  - 사용자의 인증 정보를 검증하여 로그인합니다.
  - 인증이 완료되면 Access Token과 Refresh Token이 발급됩니다.
  - Access Token은 클라이언트가 서버에 요청할 때 인증에 사용됩니다.
  - Refresh Token은 Redis에 저장되며, Access Token이 만료될 경우 새로운 Access Token을 발급받는 데 사용됩니다.
 
- **로그아웃**:
  - 사용자 인증을 해제하고, 세션을 종료합니다.
  - Redis에서 저장된 RefreshToken이 삭제되어 더 이상 액세스 토큰을 갱신할 수 없습니다.

- **모임 생성**:
  - 카카오 맵을 통해 사용자가 지정한 위치에 해당하는 애견 동반 장소를 보여줍니다.
  - 애견 동반 장소를 클릭하여 장소 상세 정보를 확인하고 모임 생성 버튼을 통해 모임을 생성합니다.
  - 모임 생성시에 최대 인원수, 모임 설명, 모임 날짜 등의 내용을 기입하여 모임을 생성합니다.

- **모임 참가**:
  - 사용자가 지도 혹은 즐겨찾기 알림을 통해 생성된 모임을 확인합니다.
  - 모임 소개글에 적힌 장소, 시간등을 확인 합니다.
  - 참가를 원할 경우 참가 신청을 누릅니다.
 
- **실시간 채팅 기능**:
  - 실시간으로 여러 사람들과 채팅방에서 모임 관련 대화를 할 수 있습니다.
 
- **참여자 평가**:
  - 모임이 종료되면 해댱 모임 참여차들 평가를 선택적으로 할 수 있습니다.

- **즐겨찾기**:
  - 모임을 희망하는 장소를 즐겨찾기 등록합니다.
  - 즐겨찾기 등록한 장소에 모임이 생성되면 알림을 전송합니다.

- **핫플 추천 알림**:
  - 장소에 생성된 모임의 확정된 참가자들 수 기반으로 일정 수치 이상의 참가자수가 발생하면 접속 유저들에게 핫플 장소 알림(SSE)를 전송합니다.

<br/>
<br/>

# 4. Tasks & Responsibilities (작업 및 역할 분담)
<table>
  <tr>
    <th align="center">작업 유형</th>
    <th align="center">담당자</th>
    <th align="center">내용</th>
  </tr>
  <tr>
    <td rowspan="3" align="center" colspan="2"><b>공통 작업</b></td>
    <td>- 테스트 코드</td>
  </tr>
  <tr>
    <td>- ERD 설계</td>
  </tr>
  <tr>
    <td>- 요구사항 정리 및 사용자 시나리오 작성</td>
  </tr>
  <tr>
    <td rowspan="5" align="center"><b>개별 작업</b></td>
    <td align="center">
      <a href="https://github.com/ijnim1121">
        <img src="https://github.com/ijnim1121.png?size=50" width="50px"><br/>
        <b></b>
      </a>
    </td>
    <td>
      <b>유저 도메인</b><br/>
      - 회원가입/로그인<br/>
      - 보안, 인가, 인증 적용 (JWT)
    </td>
  </tr>
  <tr>
    <td align="center">
      <a href="https://github.com/Jung-Taemin">
        <img src="https://github.com/Jung-Taemin.png?size=50" width="50px"><br/>
        <b>정태민</b>
      </a>
    </td>
    <td>
      <b>유저 평가 도메인</b><br/>
      - 평점<br/>
      - 평가 내용
    </td>
  </tr>
  <tr>
    <td align="center">
      <a href="https://github.com/sukangpunch">
        <img src="https://github.com/sukangpunch.png?size=50" width="50px"><br/>
        <b>강형준</b>
      </a>
    </td>
    <td>
      <b>장소 도메인</b><br/>
      <b>알림 도메인</b><br/>
      - 실시간 인기 정보 알림 시스템 적용 (SSE)<br/>
      - 배포 및 CI/CD 구축<br/>
      - 모니터링 서버 구축
    </td>
  </tr>
  <tr>
    <td align="center">
      <a href="https://github.com/leedidu">
        <img src="https://github.com/leedidu.png?size=50" width="50px"><br/>
        <b>이지수</b>
      </a>
    </td>
    <td>
      <b>모임 도메인</b><br/>
      - 모임 상세페이지<br/>
      - 개인 모임 조회<br/>
      - 프로토타입 제작
    </td>
  </tr>
  <tr>
    <td align="center">
      <a href="https://github.com/youngkwanglim">
        <img src="https://github.com/youngkwanglim.png?size=50" width="50px"><br/>
        <b>임영광</b>
      </a>
    </td>
    <td>
      <b>채팅 도메인</b><br/>
      - 장소 별 채팅 기능 적용 (WebSocket)<br/>
      - 프로토타입 제작
    </td>
  </tr>
</table>

<br/>

# 5. Technology Stack (기술 스택)
### Back-end
<div>
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Java.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/SpringBoot.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/SpringSecurity.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/SpringDataJPA.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/JWT.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Mysql.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/MongoDB.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Redis.png?raw=true" width="80">

</div>

### Infra
<div>
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/AWSEC2.png?raw=true" width="80">
</div>

### Tools
<div>
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Github.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Notion.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Docker.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Figma.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Postman.png?raw=true" width="80">
<img src="https://github.com/yewon-Noh/readme-template/blob/main/skills/Swagger.png?raw=true" width="80">


</div>

<br />


# 6. Project Structure (프로젝트 구조)
```bash
src
└── main
    ├── java
    │   └── findme.dangdangcrew
    │       ├── chat
    │       ├── evaluation
    │       ├── global
    │       │   ├── config
    │       │   ├── dto
    │       │   ├── entity
    │       │   ├── exception
    │       │   ├── interceptor
    │       │   ├── publisher
    │       │   ├── service
    │       ├── meeting
    │       ├── notification
    │       ├── place
    │       ├── sse
    │       ├── user
    │       │   ├── controller
    │       │   ├── dto
    │       │   ├── entity
    │       │   ├── repository
    │       │   ├── service
    │       └── DangdangcrewApplication
    ├── resources
    │   └── application.yml

```

<br/>
<br/>

# 7. ProtoType (프로토타입)
<table>
  <tr>
    <td align="center"><img src="https://github.com/user-attachments/assets/65ed7461-a6ac-4b98-94d1-355cc42b906d" width="200"/></td>
    <td align="center"><img src="https://github.com/user-attachments/assets/5636ea4c-be1b-4d64-8665-ec62eef152b9" width="200"/></td>
    <td align="center"><img src="https://github.com/user-attachments/assets/2ffb3a21-2db4-4610-a52d-3862c3b1fd16" width="200"/></td>
    <td align="center"><img src="https://github.com/user-attachments/assets/3e333b4a-658f-4d53-9cb9-6212ef92dc43" width="200"/></td>
  </tr>
  <tr>
    <td align="center"><b>로그인</b></td>
    <td align="center"><b>장소선택</b></td>
    <td align="center"><b>장소선택 - 모임목록</b></td>
    <td align="center"><b>알림목록</b></td>
  </tr>
  <tr>
    <td align="center"><img src="https://github.com/user-attachments/assets/5ea740d4-da39-43d1-89f1-350737cbbbae" width="200"/></td>
    <td align="center"><img src="https://github.com/user-attachments/assets/797493d4-ec47-4041-a4d3-c0a5f425e33a" width="200"/></td>
    <td align="center"><img src="https://github.com/user-attachments/assets/30cbe416-7cc2-44b6-b7e3-f032803acced" width="200"/></td>
    <td align="center"><img src="https://github.com/user-attachments/assets/fe8fe120-2c76-410c-ba62-94c4a53590ed" width="200"/></td>
  </tr>
  <tr>
    <td align="center"><b>모임소개</b></td>
    <td align="center"><b>모임관리</b></td>
    <td align="center"><b>채팅방</b></td>
    <td align="center"><b>평가창</b></td>
  </tr>
</table>

# 8. Development Workflow (개발 워크플로우)
## 브랜치 전략 (Branch Strategy)
- dev Branch
  - 배포 가능한 상태의 코드를 유지합니다.
  - 모든 배포는 이 브랜치에서 이루어집니다.
  
- feature Branch
  - 팀원 각자의 개발 브랜치입니다.
  - 모든 기능 개발은 이 브랜치에서 이루어집니다.
  - 브랜치명: 태그-#이슈번호-개발내용
    - ex) feat-#14-user-api

<br/>
