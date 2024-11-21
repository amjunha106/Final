<h1>Project Planner</h1>
<img src="/images/image1.png" alt="Image">
<br>
<h1>소개 및 개요</h1>
프로젝트 기간 : 2024-07-22 ~ 2024-08-26<br>
인원 : 3인<br>
주제 : PMS(프로젝트 관리)사이트 만들기<br>
사용언어 : JAVA, JAVASCRIPT
<br>

<details>
  <summary>프로젝트 구조</summary>

  <pre>
    C:.
├─java
│  └─com
│      └─web
│          └─projectplanner
│              ├─a00_configure
│              │  └─WebConfig.java (메일언어변경)
│              ├─a01_controller
│              │  └─CalendarController.java (캘린더)
│              │  └─FreeBoardController.java (자유게시판)
│              │  └─MailController.java (메일전송)
│              │  └─ReplyController.java (게시판-댓글)
│              ├─a02_service
│              │  └─CalendarService.java
│              │  └─FileUploadService.java (파일업로드)
│              │  └─FreeBoardService.java
│              │  └─MailService.java
│              │  └─ReplyService.java
│              ├─a03_dao
│              │  └─CalendarDao.java
│              │  └─FreeBoardDao.java
│              │  └─MailDao.java
│              │  └─ReplyDao.java
│              ├─a04_vo
│              │  └─Calendar.java
│              │  └─FreeBoard.java
│              │  └─FreeBoardFile.java
│              │  └─FreeBoardSch.java
│              │  └─Mail.java
│              │  └─Reply.java
│              ├─a05_util
│              └─aspect
├─resource
├─resources
│  ├─messages
│  │    └─messages_en.properties
│  │    └─messages_ko.properties
│  │    └─messages.properties
│  └─static
│      └─z06_emailList.html (사원메일조회)
└─webapp
    ├─a00_com
    ├─img
    ├─WEB-INF
    │  └─views
    │      └─z01_FreeBoardList.jsp
    │      └─z02_FreeBoaredInsert.jsp
    │      └─z03_FreeBoardDetail.jsp
    │      └─z04_MailFrm.jsp
    │      └─z05_Calender.jsp
    ├─z01_upload
    └─z05_bootTmp
  </pre>
</details>

<br>
<h1>팀원소개 및 역할분담</h1>
<img src="/images/image2.png" alt="Image">

<h1>프로젝트 기술스택</h1>
<h2>프론트엔드 (Front-end)</h2>
<ul>
  <li>Jsp : Spring Mvc패턴의 view단으로 사용하기위해 템플릿 역할로 사용하였습니다.</li>
  <li>Javascript(vue.js, ajax) : 사원메일조회, 게시판(게시글, 댓글)/캘린더CRUD의 비동기처리를 하기위해 사용하였습니다.</li>
  <li>CSS : 웹 페이지의 스타일과 레이아웃을 정하기 위해 사용하였습니다.</li>
</ul>

<h2>백엔드 (Back-end)</h2>
<ul>
  <li>java(SpringBoot사용) : Restful Api를 구축하기 위해 사용하였습니다.</li>
</ul>

<h2>데이터베이스 (Database)</h2>
<ul>
  <li>Oracle : 사원정보/일정/게시판의 데이터를 저장하고 조회하기위해 사용하였습니다.</li>
</ul>

<h1>1. Calendar</h1>
<h3>개인/팀/간트차트 별 일정조회, 체크박스 여부에 따라 여러일정을 한번에 조회</h3>
<img src="/gifs/gif1.gif" width="950px" alt="Image">
<h3>일정등록</h3>
<img src="/gifs/gif2.gif" width="950px" alt="Image">
<h3>일정수정/삭제</h3>
<img src="/gifs/gif3.gif" width="950px" alt="Image">

<h1>2. 자유게시판</h1>
<h3>전체게시글 조회, 게시글10개마다 페이징처리</h3>
<img src="/gifs/gif4.gif" width="950px" alt="Image">
<h3>제목or작성자로 게시글검색</h3>
<img src="/gifs/gif9.gif" width="950px" alt="Image">

<h1>2-1) 자유게시판 - 게시글 등록</h1>
<h3>제목과 내용을 입력 후 게시글등록, 파일업로드 가능</h3>
<img src="/gifs/gif5.gif" width="950px" alt="Image">

<h1>2-2) 자유게시판 - 게시글상세</h1>
<h3>게시글상세 확인가능, 업로드된 첨부파일 다운로드</h3>
<img src="/gifs/gif6.gif" width="950px" alt="Image">
<h3>게시글 수정/삭제</h3>
<img src="/gifs/gif6.gif" width="950px" alt="Image">

<h1>2-3) 자유게시판 - 댓글등록/삭제</h1>
<h3>해당 게시글에 댓글등록/삭제 가능</h3>
<img src="/gifs/gif8.gif" width="950px" alt="Image">

<h1> 3. 메일전송(언어변경)</h1>
<h3>상대방에게 메일전송</h3>
<img src="/gifs/gif10.gif" width="950px" alt="Image">
<h3>사원정보 조회(vue.js)</h3>
<img src="/gifs/gif11.gif" width="950px" alt="Image">
<h3>언어변경</h3>
<img src="/gifs/gif12.gif" width="950px" alt="Image">
