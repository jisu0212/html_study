# Visual Studio Code(VScode)
* vs code 실행 시 가장 먼저 확인해야 할 것!
* 왼쪽 탐색기가 당일 작업폴더로 연결되어 있는지 확인하기!
* (위) 안되어있다면 -> 파일 -> 작업폴더 닫기 후 -> 폴더열기 다시 진행!
# html 시작
* git, gitHub 개념공부
* '<태그'> 웹 페이지에서 의미적인 정보를 가지는 대상
## HTML5 버전선언
* `<!doctype html>`
## HTML 구조태그
* html : 웹의 시작과 끝. 문서 자체 의미.
* head : 웹 문서의 정보, 제목 포함
* meta : 웹 문서의 정보 기록
* title : 웹 문서의 제목(브라우저 상단 표시)
* body : 웹 문서 내용 (실제 대부분의 서비스가 들어가는 본문)
## 구조 태그 속성
* `lang="ko"` html 문서 언어 설정
* `charset="utf=8"` 다국어 문자열 설정
* `description` 사이트 요약 설명
* `keywords` 사이트 검색 키워드 설정
## 속성 문법
* `<태그 속성="값" 속성="값"></태그>`
* 태그와 속성 사이 공백
* 속성과 속성 사이 공백(속성 개수 제한없음)
* 속성은 시작태그에만 작성하기!
## 구조태그의 `title`작성방법
* 메인페이지 -> 사이트명
* 메인페이지 -> 사이트명 | 광고문구 추가
* 서브페이지 -> 페이지명 | 사이트명
* ex) 책이름-저자명 | 서점명
* ex) 판매아이템명 | 사이트명
## h1~h6 제목태그(block tag)
* h1~h3 태그는 meta keywords와 동일한 검색키워드로 활용된다. (대제목일수록 높음)
* h4~h6 태그는 거의 사용하지 않는다.
* h1은 사이트의 로고 및, 서브 페이지 제목에서 주로 사용한다.
* h 제목의 1~6레벨은 순서대로 작성해야 한다.
## 단락 p(block tag)
* 한 줄 또는 여러 줄 단락 묶을 때 사용하는 태그
* 제목(h)태그 종류와는 형제 태그 관계로 사용해야 한다. 부모-자식(X)
## 인라인태그 br, em, strong, del, s, sup, sub
* `br` : 블록 내 줄바꿈 태그
* `em` : 블록 내 강조 태그
* `strong` : 블록 내 경고용 강조 태그 (위와 특징 동일)
* `del` : 삭제 텍스트, 쇼핑몰의 할인 전 가격 등에 사용
* `s` : 교체 텍스트, 쇼핑몰의 할인 전 가격 등에 사용 (del 자주 사용)
* `sup,sub` : 윗첨자(sup) 아래첨자(sub) 수학, 과학 등의 기호에 사용
## 인용문 처리 blockquote, q
* `blockquote(block)` : 단락 자체가 인용문에 해당할 때 사용, p태그와 부모-자식 관계로 사용해선 안된다!
* `q(inline)` : 단락(p) 내에서 일부가 인용문에 해당할 때 사용
* 공통 속성 `cite="URL"` : `blockquote`, `q` 로 인용문 처리할 경우 출처 표시용도로 주소(URL)을 담아주는 속성.
## 특수문자 태그
* `&` 시작 `;` 종료
* `&lt;` `&gt;` : 좌꺽쇠, 우꺽쇠
* `&copy;` : C모양의 저작권 마크
* `&reg;` : R모양의 마크
## 주소 태그
* `address` : 연락처, 회사소개, 고객센터 등을 담을때 사용
* 다른 블록을 자식 또는 자손으로 배치할 수 없음 (=inline만 넣을 수 있음)
* footer영역에 들어가는 본 사이트 주소
## 수평선 태그
* `hr` : 사이트 각 영역을 구분할 때 사용
* css에서는 숨기는 경우가 대부분
* 주석과 같이 태그 구조 이해에 주 용도로 사용
## 컴퓨터 명령어 태그
* `code` inline 웹강의사이트에서 주로 사용하는 태그
## 링크 태그 a
* block, inline 특징을 모두 가진다.
* 절대경로와 상대경로를 href 속성에 작성한다.
* 상대경로는 a태그 작성중인 파일 위치 기준 연결하고자 하는 목적지 파일이 같은 위치에 있는지, 하위 위치에 있는지, 상위 위치에 있는지에 따라 다르게 작성한다.
* `./` 현재 위치에서 시작
* `../` 상위 폴더로 나가기
* `./doll.jpg` : 현재 위치에서 doll.jpg 파일 찾기
* `../doll.jpg` : 상위 폴더로 한단계 나가서 doll.jpg 파일 찾기
* `../a/doll.jpg` : 상위폴더로 한단계 나가고 a 폴더로 들어가서 doll.jpg 파일 찾기
* `./b/doll.jpg` : 현재위치에서 b폴더로 들어가서 doll.jpg 파일 찾기
## 바로가기링크란?
* 단순 페이지 이동이 아닌 특정 위치로 스크롤 이동하는 바로가기 기능
* `#id` 바로가기 링크 속성
* `<a href="#id">링크1</a>`
* `<p id="pst1">링크1목적지</p>`
* 태그가 가진 아이디명을 href 속성에 작성해 바로가기 링크로 활용할 수 있다.
## 바로가기 링크 제작 순서 및 주의사항
1. 이동 목적지에 가장 가까운 태그에 `id` 적용하기
2. 링크 대상에 `#id` href 속성값에 담기
* 주의사항 : #은 아이디 이동 링크에만 사용하기, 연결될 목적지가 아직 제작 전이라 링크가 없다면 #으로 임시링크를 걸어준다.
## 파비콘 적용 순서
1. 파비콘 크기로 이미지 다운받거나 편집하기
2. html에서 head 안에 link태그로 `favicon` href주소 연결하기
* `<link rel="shortcut icon" href="파비콘.ico 경로" type="image/x-icon">`
* `<link rel="icon" href="파비콘.ico 경로" type="image/x-icon">`
## 이미지태그 `img` (inline)
* `<img src="url"alt="">`
* 의미전달이 필요한 이미지일 경우 alt="" 사이에 의미를 꼭 넣을것
* src 이미지 경로 속성의 값으로는 상대경로 방식으로 작성하는 것을 권장
* inline이기 때문에 block태그인 h나 p와 형제관계에 두려면 블록 안에 묶어야한다.
## figure, figcaption 태그
* 이미지와 글을 하나의 틀로 감쌀때 사용, figcaption은 대상에 대한 정보를 적을 때 사용
* `<figure>`
    `<img src="URL" alt="">`
    `<figcaption>caption</figcaption>`
`</figure>`
## video 태그
* `<video src="동영상경로" autoplay muted loop controls>` 자동재생, 음소거, 반복, 컨트롤러 생성
* 유튜브에서 영상을 가져올 때
1. 유튜브에서 음악 선택 후 우클릭해서 소스코드복사 누른다.
2. 비쥬얼스튜디오에 붙여넣기 하고 링크 뒤에 물음표(?)를 붙인다.
3. 그 뒤에 autoplay=1&mute=1&loop=1을 붙이면 자동재생, 음소거, 반복재생 되는 영상 넣기 끝.
# class, id 많이 사용하는 키워드
* wrapper, wrap, area 전체 묶는 영역
* contents, container 중~소 묶는 영역
* group, g 간단한 소그룹 영역
* top, btm, left, right 레이아웃 방향을 의미하는 키워드
* 예) 의미있는 단어_영역명
* 예) product_wrap, item_area, price_g, main_contents, top_btn
## div, span 그룹태그
### div
* 인라인과 블록이 2개 이상 형제일 경우 묶어주는 그룹태그
* 레이아웃 기준 1행에 2열 이상 배치일 경우
* 특정 의미를 가진 행에 같은 디자인 요소가 배치된 경우
### span
* 인라인이 2개 이상 형제일 경우 묶는 그룹태그
* 의미없는 디자인 요소 인라인 처리 필요 시 사용
## html5 semantic tag
### semantic tag란?
* HTML5에서 생성된 의미있는(semantic) 태그
### header
* `<header>`,`</header>`
* 로고 및 내비게이션을 묶어주는 웹 사이트 레이아웃 태그
* 제목, 로고, 검색 폼, 작성자 이름 등의 요소도 포함 가능
### nav
* `<nav>``</nav>`
* 로고 및 웹사이트 주요 내비게이션을 묶어주는 웹 사이트 레이아웃 태그
### gnb, lnb, snb
* 글로벌네비게이션바, 로컬네비게이션바, 사이드네비게이션바
### section
* `<section>`,`</section>`
* 문서의 독립적인 구획을 나타내며 제목(H)을 포함하는 경우가 많다. (필수는 아님)
### aside
* `<aside>`,`</aside>`
* 문서의 주요 내용과 간접적으로만 연관된 부분
* 주로 사이드바 혹은 콜아웃 박스로 표현
### article
* `<article>`,`</article>`
* 사이트 안에서 독립적으로 구분해 배포하거나 재사용할 수 있는 구획
* 게시판과 블로그 글, 매거진이나 뉴스 기사 등이 있음
## ul, ol, li
* `<ul><li></li></ul>`
* `<ol><li></li></ol>`
* ul은 순서가 없는 목록을 나열할 때 사용함
* ol은 순서가 있는 목록을 나열할 때 사용함
* li는 ul과 ol 목록 안에서 나열되는 행으로써 사용함
## details, summary
* `<details><summary>요약</summary>내용</details>`
* 설명을 접었다 펼 수 있는 요약 위젯을 만들 수 있음
## footer, maek, main, time
* `footer`: 웹페이지 가장 하단에 위치하며 address태그를 사용함
* `mark` : 내용이 중요해서 하이라이트 한 부분을 나타냄(형광펜 표시)
* `main` : 문서 `<body>`의 주요 콘텐츠를 나타냄
* `time` : 시간의 특정 지점 또는 구간을 나타냄, ex) `<time datetime="2024-04-11"></time>`
## dl, dt, dd 정의형 목록태그
* `<dl></dl>`:정의형 제목과 내용을 묶는 그룹
* `<dt></dt>`:dl 안 자식으로 배치되며 제목을 의미
* `<dd></dd>`:dl 안 자식으로 배치되며 dt의 다음 형제 요소로 배치되거나 기존 dd의 형제로도 배치될 수 있음, 정의형 목록의 내용을 의미