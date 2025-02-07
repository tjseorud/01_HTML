# HTML Tag

## 글자
 TAG | 내용 | -
 ---:|---|---
 `<!DOCTYPE html>` |현재 문서는 html 형식으로 정의
 `<html>` |시작 / 종료 | `</head>`
 `<head>` |html을 정의하는 내용 작성 | `</head>`
 `<meta>` |보이지 않는 작은 설정(검색 엔진 노출 설정)
 `<title>` |문서의 제목을 작성 | `</title>`
 `<body>` |브라우저에 보여질 내용 작성 | `</body>`
 `<hr>`|horizon : 수평선
 markup 언어 |태그(mark)형태대로 브라우저에 모양이 떠오르는 언어
 -|제목 : Highlight 
 `<h1>...<h6>`|<h1>h1 <h2>h2 <h3>h3 <h4>h4 <h5>h5 <h6>h6|`</h1>...</h6>`
 `<br>`|엔터 : `br`(line BReak)
 `&nbsp;`|띄어쓰기
 `<pre>`|PREformatted<br> `pre` 내부에 작성된 형태 그대로 화면에 출력|`</pre>`
 `<p>`|글을 작성하는 용도|`</p>`
 -|글자의 적용 되는 태그
 `<b>`|<b>`b`(bold) : 단순 글자를 굵게 표시</b>|`</b>`
 `<i>`|<i>`i`(italic) : 단순글자를 기울여 표시</i>|`</i>`
 `<strong>`|<strong>`strong` : 글자(단어)를 강조</strong>|`</strong>`
 `<em>`|<em>`em` : 문장의 맥락을 변화시키는 강조</em>|`</em>`
 `<mark>`|<mark>`mark` : 형광펜 효과주는</mark>|`</mark>`
 `<u>`|<u>`u`(under) : 밑줄 긋는</u>|`</u>`
 `<s>`|<s>`s` : 글자 가운데 선을 긋는 (취소, 오타)</s>|`</s>`
 `<del>`|<del>`del` : 삭제선을 긋는 (있다 없어짐)</del>|`</del>`
 `<sup>`|`sup`(윗첨자) : x<sup>3</sup>|`</sup>`
 `<sub>`|`sub`(아랫첨자) : log<sub>2</sub>|`</sub>`
 `<abbr>`|`abbr`(abbreviation, 약어) : 마우스 오버시 툴팁 제공|`</abbr>` 
  
## 목록
TAG | 내용 | -
 ---:|---|---
 `<table>`|행, 열을 작성하기 위한 영역(판)을 지정하는|`</table>`
`<tr>`|`tr`(Table Row) :  `table`의 한행을 나타내는|`</tr>`
`<th>`|`th`(Table Header) :  열의 제목을 나타내는<br>  `td`와 같은 레벨로 작성<br>  굵은 글씨+가운데 정렬|`</th>`
`<td>`|`td`(Table Data) : `table`에 출력될 data를 작성하는<br> 각 행의 열(col) 역할|`</td>`
`<thead>`|`table` 상단 영역(값 작성 영역)|`</thead>`
`<tbody>`|`table` 중단 영역(값 작성 영역)|`</tbody>`
`<tfoot>`|`table` 하단 영역(합계 작성 영역)|`</tfoot>`
`colspan`|열로 나열 된 방향(가로, 옆) 병합
`rowspan`|행으로 나열 된 방향(세로, 위/아래) 병합
`caption`|표 또는 이미지의 설명을 작성하는
`<ul>`|`ul`(Unordered List) : 순서가 없는 목록|`</ul>`
`<li>`|`li`(List Item) : 목록의 한 줄|`</li>`
`<ol>`|`ol`(Ordered List) : 순서가 있는 목록|`</ol>`
`type`|표시되는 숫자 형식 지정
`type="a"`|영어 소문자(a,b,c)
`type="A"`|영어 대문자(A,B,C)
`type="i"`|로마 소문자(i,ii,iii)
`type="I"`|로마 대문자(I,II,III)
`type="1"`|숫자(1,2,3)(기본값)
`start`|목록 시작 번호
`reversed`|역순

## 이미지
TAG | 내용 | -
 ---:|---|---
`<img>`|웹 문서에서 이미지를 삽입하는 용도
-|시작 태그에 작성하는 내용
`src`|삽입할 이미지의 경로를 작성하는 속성(파일 위치(경로), `url`)
`width` `height`|너비 높이를 지정하는 속성(단위 : `px` `%` `em` `rem` 등)
`alt`|이미지 설명을 작성하는 속성
`px`|화면의 크기가 변해도 항상 고정된 크기를 지님
`%` `em` `rem` `...`|브라우저 크기 또는 지정된 영역의 크기에 대한 상대적인 크기 단위

## 영역
TAG | 내용 | -
 ---:|---|---
`block`|화면(공간, 영역)을 (세로 공간을 잘라서 층을 나눔)<br> `width` `heigth` 크기 지정 속성 적용ok<br> `h1-h6`(제목)<br> `p` `pre`(문단)<br> `hr`(수평선)<br> `div`(영역 분할)<br> 시맨틱 태그(div의 이름 변경된 태그)|항상 직사각형의 형태로 영역을 지정
`inline`|화면 수평 분할(가로 화면/영역을 잘라서 열로 분할)<br> `width` `heigth` 크기 지정 속성 적용 X<br> 작성된 내용 만큼 크기만 차지함<br> `b` `i` `strong` `em` `mark` `span`(영역 분할)|작성된 내용(content) 단위로 영역을 지정
`inline-block`|`inline` : 특징 중 열 나눔<br>`block` : 특징 중 크기 지정<br>두 특징만을 가져와 섞은 형식|`iframe` `img`
`iframe`|웹 문서(html) 내부에 또 다른 웹 문서(html)를 추가하는|`/iframe`

## 링크
TAG | 내용 | -
 ---:|---|---
Hyper Link|현재 문서를 넘어 다른 문서와 연결
Hyper Text|클릭시 연결된 다른 문서로 넘어가는 글자(문자열)
`a`|`a`(Anchor, 연결)<br>현재 문서`html`와 다른 문서`html`를 연결시켜 클릭 시 이동하게 만드는
`href`|`href`(Hyper Text REFerence) : 연결할 주소를 작성하는 속성
`target`|`a` 클릭시 현재 탭, 새 탭 중 어떻게 열것인지 지정
`id`|`id`(Identifier, 식별자)<br>한 페이지 내에서 지정된 `id `속성 값을 가진 요소로 이동<br>요소를 구분하는 용도의 속성<br>하나의 `html` 파일 내에 같은 `id` 값을 지닌 요소가 있어서는 안됨

## 입력
TAG | 내용 | -
 ---:|---|---
`input`|웹 문서에서 사용자(클라이언트)가 입력할 수 있는 양식을 제공하는<br>다수의 `type`이 존재하고, `input`이 변형된 태그도 존재<br>`input`에는 `name`이라는 속성을 작성 할 수 있다<br>(작성된 값에 이름을 부여 -> 서버/다른 페이지 제출 시 사용)
-|`text` 관련 `input`
`type="text"`|한 줄 텍스트 입력 상자 (기본값)
` type="password"`|비밀번호 입력 상자(모자이크 처리)
`type="url"`|모양은
`type="search"`|`text`와 동일
`type="tel"`|용도 구분용
`type="email"`|(+유효성 검사)
-|숫자 관련 `input`
`type="number"`|숫자만 입력 가능한 입력 상자
`type="range"`|슬라이드바를 이용해서 숫자를 지정<br>(단독 사용 X, JS와 혼용)
`max` `min`|최대값 최소값
`step`|숫자가 증가/감소하는 간격(단계)
`value`|초기 값(기본 값) 지정
-|날짜/시간 관련
`type="date"`
`type="month"`
`type="week"`
`type="time"`
`type="datetime-local"`
`radio` `checkbox`|여러 연관된 값을 묶어서 선택하는 경우에 사용하는
`type="radio"`|여러 값 중 하나만 선택
`type="checkbox"`|여러 값 중 원하는 값 모두 선택

## 폼
TAG | 내용 | -
 ---:|---|---
``||``
``||``
``||``
``||``
``||``
