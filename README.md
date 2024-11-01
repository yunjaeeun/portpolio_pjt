# 🙌🏻 주제 : 반응형 Portfolio 웹사이트 구현

#### 공통 요구사항
- 예시를 참고해 본인만의 반응형 웹 포트폴리오 사이트 만들기.
    - 예시 화면은 참고일 뿐, 그대로 구현하지 마세요!
- UI 설계부터 구현까지 스스로 도전해 봅니다.
- Bootstrap & CSS를 적절하게 사용하여 구현합니다.
- [참고] 구글 검색 : 개발자 포트폴리오 참고 사이트
    - 다양한 포트폴리오 웹사이트 모음 등을 참고합니다
- 반응형 웹 포트폴리오
    - 다양한 개발자 포트폴리오를 참고합니다.
    - 본인만의 개성있는 포트폴리오 페이지를 구현합니다
    - 설계 및 구현 시 생성형 AI를 활용합니다
      - 예시 1) 자주 활용되는 개발자 포트폴리오 사이트 구조 알려줘
      - 예시 2) 시멘틱 태그에 대해 알려줘
      - 예시 3) 자기소개 페이지에 이미지 넣는 방법 알려줘. Bootstrap 활용할꺼야
<br/>

# 🖼 결과
<h3><em><ins><strong>[Desktop]</strong></ins></em><br></h3>
![port_desk](/uploads/77f6e4cff3e21e9f20b248009122d5ec/port_desk.gif)

<h3><em><ins><strong>[app]</strong></ins></em><br></h3>
![port_app](/uploads/f0fb1ca7bbbc1920fa03dbee38c1c68b/port_app.gif)


<details>
<summary><h4>코드</h4></summary>

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="styles.css">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link rel="preconnect" href="https://cdn.jsdelivr.net" crossorigin="anonymous" />
    <link rel="preload" as="style" crossorigin href="https://cdn.jsdelivr.net/gh/wanteddev/wanted-sans@v1.0.3/packages/wanted-sans/fonts/webfonts/variable/split/WantedSansVariable.min.css" />
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/wanteddev/wanted-sans@v1.0.3/packages/wanted-sans/fonts/webfonts/variable/split/WantedSansVariable.min.css" />
    <link rel="stylesheet" href="styles.css">
</head>
<body class="bg-light">
    <!-- 네비게이션 바 -->
    <header>
      <nav class="navbar navbar-expand-lg bg-secondary-subtle my-header">
        <div class="container-fluid">
          <a class="navbar-brand" href="#">&#128218; Jaeeun's Portfolio</a>
          <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
            <span class="navbar-toggler-icon"></span>
          </button>
          <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
            <div class="navbar-nav ms-auto">
              <a class="nav-link active" aria-current="page" href="#about">&#128270; About Me</a>
              <a class="nav-link" href="#skills">&#128296; Skills</a>
              <a class="nav-link" href="#experience">🧬 Experience</a>
              <a class="nav-link" href="#projects">&#128193; Projects</a>
              <a class="nav-link" href="#contact">&#128241; Contact</a>
            </div>
          </div>
        </div>
      </nav>
    </header>
    <main>
    <!-- 소개 섹션 -->
    <section id="about" class="container mb-5 mt-5">
      <h1 class="ms-4">&#128270; About Me</h1>
      <div class="row">
        <div class="col-md-4 text-center">
            <img src="img/white.jpg" alt="" class="profile-img img-fluid rounded shadow-sm">
        </div>
        <div class="col-md-8">
          <h4 class="mt-4 mt-md-5 mb-3">😊 안녕하세요 저는 윤재은 입니다 😊</h4>
          <h6>
            열정적인 Backend 개발자로 SpringBoot를 활용해 문제를 해결하고,<br> 
            혁신적인 솔루션을 개발하는 데 관심이 많습니다. <br><br>
            부트캠프에서 웹개발 풀스택을 공부하며 여러 웹 프로젝트를 통해 실무 경험을 쌓았습니다.<br>
            SpringBoot와 SQL에 대한 깊은 이해를 바탕으로 여러 문제들을 해결하며<br>
            다양한 프로젝트를 성공적으로 이끌었습니다.<br><br>
            제 포트폴리오에서는 제가 참여했던 프로젝트와 기여한 바를 확인하실 수 있으며<br>
            제 기술과 경험이 어떻게 실제 문제를 해결하는 데 도움이 되었는지 보여드립니다.<br>
            함께 일할 기회를 기대하며, 항상 새로운 도전에 열려있는 개발자입니다.
          </h6>
        </div>
      </div>
    </section>

    <!-- 기술 스택 섹션 -->
    <section id="skills" class="container skill-container">
      <h2 class="ms-4">&#128296; Skills</h2>

      <div id="customCarousel" class="carousel slide my-skills col-12 col-md-10 offset-md-1" data-bs-ride="carousel">
        <div class="carousel-inner">
            <div class="carousel-item active">
                <div class="d-flex align-items-center justify-content-center my-stack" style="height: 300px">
                    <div class="text-center">
                        <h2 class="mb-4">Backend</h2>
                        <img src="img/java.png" alt="Java" class="img-fluid me-2">
                        <img src="img/python.png" alt="Python" class="img-fluid me-2">
                        <img src="img/spring.png" alt="Spring" class="img-fluid">
                    </div>
                </div>
            </div>
            <div class="carousel-item">
                <div class="d-flex align-items-center justify-content-center my-stack" style="height: 300px;">
                    <div class="text-center">
                        <h2 class="mb-4">Frontend</h2>
                        <img src="img/html.png" alt="HTML" class="img-fluid me-2">
                        <img src="img/css.png" alt="CSS" class="img-fluid me-2">
                        <img src="img/javascript.png" alt="Javascript" class="img-fluid me-2">
                        <img src="img/vue.png" alt="Vue" class="img-fluid">
                    </div>
                </div>
            </div>
            <div class="carousel-item">
                <div class="d-flex align-items-center justify-content-center my-stack" style="height: 300px;">
                    <div class="text-center">
                        <h2 class="mb-4">Others</h2>
                        <img src="img/mariadb.png" alt="MariaDB" class="img-fluid me-2">
                        <img src="img/aws.png" alt="AWS" class="img-fluid">
                    </div>
                </div>
            </div>
        </div>      
        <button class="carousel-control-prev" type="button" data-bs-target="#customCarousel" data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#customCarousel" data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
      </div>
    </section>

    <!-- 경력 섹션 -->
    <section id="experience" class="container mt-5 mb-5">
        <h2 class="ms-4">🧬 Experience</h2>
        <div class="row justify-content-center">
            <div class="card mb-3 me-md-3 col-12 col-md-5 d-flex flex-column">
                <img src="img/beyondpng.png" class="card-img-top" alt="Beyond SWcamp">
                <div class="card-body d-flex flex-column flex-grow-1">
                    <h5 class="card-title">한화시스템 Beyond SWcamp</h5>
                    <h6 class="card-title">2023.12 ~ 2024.06 (수료)</h6>
                    <p class="card-text">웹 개발 풀스택 과정 수강<br>
                      SQL, Java, SpringBoot, HTML, CSS, JS, Vue3
                    </p>
                </div>
            </div>
            <div class="card mb-3 col-12 col-md-5 d-flex flex-column">
                <img src="img/ssafy.jpg" class="card-img-top" alt="SSAFY">
                <div class="card-body d-flex flex-column flex-grow-1">
                    <h5 class="card-title">삼성청년SW아카데미(SSAFY)</h5>
                    <h6 class="card-title">2024.07 ~  (수강중)</h6>
                    <p class="card-text">웹 개발 풀스택 과정 수강<br>
                    Python, HTML, CSS, Javascript, Django, Vue, SQL
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- 프로젝트 섹션 -->
    <section id="projects" class="container">
        <h2 class="ms-4">&#128193; Projects</h2>
        <div class="row justify-content-center">
            <div class="card mb-3 me-md-3 col-12 col-md-5 d-flex flex-column">
                <img src="img/erpc.png" class="card-img-top" alt="ERPC">
                <div class="card-body d-flex flex-column flex-grow-1">
                    <h5 class="card-title">ERPC</h5>
                    <h6 class="card-title">2024.04 ~ 2024.06</h6>
                    <p class="card-text">ERPC는 최적의 영업을 위한 영업관리 ERP 솔루션으로 사용자의 문서화 시간을 줄여줄 수 있는 서비스입니다.</p>
                    <a href="https://github.com/beyond-sw-camp/be04-final-team06-ERPC" class="mt-auto card-text"><small class="text-body-secondary">Github로 이동</small></a>
                </div>
            </div>
            <div class="card mb-3 col-12 col-md-5 d-flex flex-column">
                <img src="img/cineverse.png" class="card-img-top" alt="CINE-VERSE">
                <div class="card-body d-flex flex-column flex-grow-1">
                    <h5 class="card-title">CINE-VERSE</h5>
                    <h6 class="card-title">2024.04 ~ 2024.04</h6>
                    <p class="card-text">CINE-VERSE는 영화 마니아들을 위한 전문 커뮤니티 사이트로 서로의 취향을 공유하고 소통할 수 있는 서비스 입니다.</p>
                    <a href="https://github.com/beyond-sw-camp/be04-4th-6team-CINE-VERSE" class="mt-auto card-text"><small class="text-body-secondary">Github로 이동</small></a>
                </div>
            </div>
        </div>
    </section>

    <!-- 연락처 섹션 -->
    <section id="contact" class="container mt-5">
        <h2 class="ms-4">&#128241; Contact</h2>
        <div class="row align-items-center justify-content-center">
            <div class="col-12 col-md-5">
                <h5>연락처: 010-5629-7169</h5>
                <h5>이메일: yunjaeeun12@naver.com</h5>
            </div>
            <div class="col-12 col-md-6 text-md-end">
              <a href="https://github.com/yunjaeeun">
                <img src="img/github.png" alt="Github" class="img-fluid me-2">
              </a>
              <a href="https://www.notion.so/HOME-d94dfeed6198448da1e04908329dc961?pvs=4">
                <img src="img/notion.png" alt="Notion" class="img-fluid">
              </a>
            </div>
        </div>
    </section>
  </main>

    <!-- 푸터 -->
    <footer class="text-center mt-5">
        <p>&copy; 2024 YoonJaeEun. All rights reserved.</p>
    </footer>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

<em><ins><strong>[CSS]</strong></ins></em>

```
* {
  font-family: Wanted Sans Variable;
}
.profile-img {
  width: 100%;
  max-width: 250px;
  height: auto;
  display: block;
  margin: auto;
  border: 2px solid #ccc; /* 테두리 색상 및 두께 설정 */
  border-radius: 8px; /* 테두리 모서리를 둥글게 만듭니다 (선택 사항) */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* 그림자 효과 설정 */
}

.my-stack img {
  max-width: 100px;
  height: 100px;
}

.my-stack {
  border-radius: 10px;
  width: 100%;
  border: 2px solid #ccc; /* 테두리 색상 및 두께 설정 */
  border-radius: 8px; /* 테두리 모서리를 둥글게 만듭니다 (선택 사항) */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* 그림자 효과 설정 */
}

.project img {
  max-width: 100%;
  height: auto;
}

.card img{
  width: 100%;
  height: 50%;
  margin-top: 3px;
  border: 2px solid #ccc; /* 테두리 색상 및 두께 설정 */
  border-radius: 8px; /* 테두리 모서리를 둥글게 만듭니다 (선택 사항) */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* 그림자 효과 설정 */
}

.card {
  border: 2px solid #ccc; /* 테두리 색상 및 두께 설정 */
  border-radius: 8px; /* 테두리 모서리를 둥글게 만듭니다 (선택 사항) */
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2); /* 그림자 효과 설정 */
}

footer {
  text-align: center;
  margin-top: 40px;
  padding: 20px;
  background-color: #f8f9fa;
}

#contact img {
  width: 40%; /* 너비를 40px로 고정 */
    height: auto; /* 높이를 자동으로 조정하여 비율 유지 */
    max-height: 90px;
}


 /* 이전 버튼 아이콘 색상 변경 */
 .carousel-control-prev-icon {
  filter: invert(100%) sepia(0%) saturate(0%) hue-rotate(93deg) brightness(102%) contrast(102%);
}

/* 다음 버튼 아이콘 색상 변경 */
.carousel-control-next-icon {
  filter: invert(100%) sepia(0%) saturate(0%) hue-rotate(93deg) brightness(102%) contrast(102%);
}
```

</details>


# 💬 소감
<em><ins><strong>1. 학습 내용</strong></ins></em>
- HTML
    - HTML의 구조, 각종 태그의 사용처
- CSS
    - CSS의 기본 문법, 상속
    - Flexbox, OOCSS
- Bootstrap
    - Bootstrap 기본 사용법, 응용
- Responsive Web 
    - Grid system


<em><ins><strong>2. 어려웠던 것</strong></ins></em><br>
1. Grid system<br>
`화면의 크기별로 grid를 부여하는 과정이 어려워 추가 학습이 필요할 것 같다.`

2. 이미지 크기<br>
`이미지 요소를 소속한 태그 범위에 알맞게 맞추는 방법이 어려워 추가 학습이 필요할 것 같다.`

<em><ins><strong>3. 느낀점</strong></ins></em><br> 
HTML, CSS, Bootstrap을 이용하여 포트폴리오를 만들며
다양한 컴포넌트들을 적용해보기도 하고 직접 커스텀 하기 위해 공식문서, 기술블로그 등 여러 자료들을 찾아보며 Bootstrap의 다양한 설정들을 학습할 수 있었고, 사용자의 화면 크기를 고려하여 Grid를 세세하게 적용하는 과정이 쉽지 않았지만 수업자료, 생성형 AI를 바탕으로 학습 해 성공적으로 완성할 수 있었다.
<br><br>
더욱 더 많은 기능을 추가하지 못한 점이 아쉬웠지만 추후 프로젝트를 고도화하며 메일발송, 방문자 체크 등 여러 기능을 추가해보고 싶은 생각이 들었고 배포 과정까지 거쳐 이후 포트폴리오로 제출하면 경쟁력이 있을 것 같다는 생각이 들었다.
