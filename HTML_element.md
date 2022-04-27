# HTML 콘텐츠 구분

## header

로고, 제목, 검색, 로그인

## footer

주소, 작성자

## h1~h6

- h1은 한번만 사용
- 크기를 초기화하여 사용

## main

주요 콘텐츠

## article

독립적 콘텐츠

## section

제목을 갖는 구분자

## aside

별도의 콘텐츠, 광고

## nav

다른 페이지 링크를 제공

## address

1개 이상의 연락처 정보

## div

본질적으로 아무것도 나타내지 않는 콘텐츠

# 문자 콘텐츠

## ol, ul, li

- li : 목록을 만드는 콘텐츠
- ol : 정렬된 목록, 순서가 있음
- ul : 정렬되지 않은 목록 , 순서가 필요 없음

1. ol 과 ul은 자식으로 li만 포함 가능
2. li는 단독으로 사용할 수 없음
3. ol의 항목 순서는 중요도를 의미할 수 있음

## dl, dt, dd

용어:dt> 설명:dd> 쌍들의 영역: dl>

- definition term
- definition details
- definition list

* dl은 dd, t을 포함해야 한다.

# 인라인 텍스트, 수정

## a

다른 url로 연결할 수 있는 하이퍼링크
속성

- href : 링크 url
- rel : 현재 문서와 링크 url의 관계 (license, prev, next)
- target : 링크 url의 표시 위치 (\_self, \_blank) 현재 창, 새로운 탭

## span

- 인라인 요소, 의미가 없음
- cf) div> 블록 요소

# 멀티미디어,내장콘텐츠,스크립트

## img

- src
- alt
- srcset : 경로 (띄어쓰기) 원본크기
- sizes : 미디어 조건, 그에 따라 출력될 이미지 크기

### src

- 이미지들과 그 이미지들의 원본 크기를 지정
- 경로, 원본
- px이 아닌, w 단위 혹은 x 단위를 입력
- 작은 크기 이미지부터 순서대로 입력

### W unit

원본 크기의 가로 너비를 의미
400\*300(px)의 크기 이미지의 w 값은 400px이다.

- width 를 지정하면 이미지가 바뀌어도 고정된 사이즈로 출력된다.
- 바뀐 이미지의 크기가 달라진다.

### X unit

이미지의 비율 의도를 의미

### sizes

미디어조건과 그 조건에 해당하는 이미지 출력

min-width : 1000px 이상일 때, 700px

최적화된 출력크기를 출력

## audio 태그

- autoplay: 준비되면 바로 재생
- controls: 제어 메뉴를 표시
- loop: 재생이 끝나면 다시 처음부터 재생
- preload: 페이지가 로드될 때 파일을 로드할지의 지정 (none, metadata, auto)
- scr: 콘텐츠 url
- muted: 음소거 여부

## video 태그

- autoplay
- controls
- crossorigin: 동일 출처 정책
- loop
- muted
- poster: 동영상 썸네일 이미지 url
- preload : 페이지가 로드될 때 파일을 로드할지의 지정(none, metadata, auto)
- src
- width
- height

## iframe

다른 html페이지를 현제 페이지에 삽입

- name: 프레임의 이름
- src: 포함한 문서의 url
- width
- heigth
- allowfullscreen: 전체 화면 모드 사용 여부
- frameborder: 프레임 테두리 사용 여부
- sandbox: 보안을 위한 읽기 전용으로 삽입 (allow-form, allow-scrips, allow-same-origin)

# 표 콘텐츠

## table

- tr> : table row, 행
- th> : table header, 열
- td> : table data, 열

### th

- abbr: 열에 대한 간단한 설명
- headers: 관련된 하나 이상의 다른 머리글 칸 id 속성 값
- colspan: 확장하려는 열의 수
- rowspan: 확장하려는 행의 수
- scope: 자신이 누구의 '머리글칸'인지 명시

### td

- headers : th> id 값 연결
- colspan
- rowspan

## caption

표의 제목을 설정

- 열리는 table> 태그 바로 다음에 작성
- table> 당 하나의 caption>을 가짐

# 양식

## form

웹 서버에 정보를 제출하기 위한 양식의 범위

- action
