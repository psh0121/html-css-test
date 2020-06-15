# 09) CSS 레이아웃

## 01. CSS 포지셔닝과 주요 속성들

- CSS 포지셔닝 : 브라우저 화면 안에 각 콘텐츠 영역을 어떻게 배치할 지 결정하는 것

- box-sizing 속성 : 박스 너비 기준 정하기
	- content-box : width 속성 값을 콘텐츠 영역 너비 값으로 사용
	- border-box : with 속성 값을 콘텐츠 영역에 테두리까지 포함한 박스 모델 전체 너비 값으로 사용

- float 속성 : 왼쪽이나 오른쪽으로 배치
	- left : 왼쪽으로 배치
	- right : 오른쪽으로 배치
	- none : 어느 쪽으로도 배치하지 않음

- clear 속성 : float 속성 해제

- position 속성 : 배치 방법 지정
	- static : 요소를 문서의 흐름에 맞추어 배치
	- relative : 이전 요소에 자연스럽게 연결해 배치하되 위치지정 가능
	- absolute : 원하는 위치에 지정 배치
	- fixed : 지정한 위치에 고정 배치

- visibility 속성 : 요소 보이게 하거나 보이지 않게 설정
	- visibility : 화면에 요소 표시
	- hidden : 화면에서 요소 감춤. 크기 그대로 유지해 배치에 영향 미침
	- collapse : 겹치도록 조절

- z-index 속성 : 요소 쌓는 순서 설정

## 02. 다단으로 편집하기

- column-width 속성 : 단의 너비 고정 빛 다단 구성
	- 크기 : 단 너비를 직접 지정
	- auto : 다른 속성에 따라 단의 너비 자동 계산

- column-count 속성 : 단의 개수 고정 및 다단 구성
	- 숫자 : 콘텐츠가 들어간 단의 개수 지정. 0보다 큰수 사용
	- auto : 다른 속성에 따라 단의 개수 자동 계산

- column-gap 속성 : 단과 단 사이의 여백
	- 크기 : 단과 단 사이의 여백 숫자로 지정
	- normal : 여백을 자동으로 지정

- column-rule 속성 : 구분선의 색상, 스타일, 너비 지정
	- column-rule-color : 색상
	- column-rule-style : 스타일
	- column-rule-width : 너비

- break-after 속성 : 다단 위치 지정
	- break-before : 특정 요소 앞
	- break-after : 특정 요소 뒤
	- break-inside : 특정 요소 안

- column-span 속성 : 여러 단을 하나로 합치기
	- 1 : 단을 하나만 합치는 것. 합치지 않는 것과 같음
	- all : 전체 단을 하나로 합쳐 표현. 단의 일부만 합치는 것은 불가능

## 03. 표 스타일

- caption-side 속성 : 표 제목 위치 설정
	- top : 캡션을 표의 윗부분에 표시
	- bottom : 캡션을 표의 아랫부분에 표시

- border 속성 : 표 테두리 스타일 결정

- border-collapse 속성 : 테두리 통합, 분리
	- collapse : 테두리를 하나로 합쳐 표시
	- separate : 테두리를 따로 표시

- border-spacing 속성 : 인접한 셀 테두리 사이 거리

- empty-cells 속성 : 빈 셀의 표시 여부 지정
	- show : 빈 셀 주위에 테두리를 그려 빈 셀을 표시
	- hide : 빈 셀 테두리를 그리지 않고 비워 둠

- width, height 속성 : 표 너비와 높이 지정

- table-layout 속성 : 콘텐츠에 맞게 셀 너비 지정
	- fixed : 셀 너비 고정
		- word-break: break-all; : 셀 너비보다 긴 내용도 셀 안에 표시
		- height: auto; : 셀의 줄 바꿈에 따라 높이 값 자동 조절
	- auto : 셀 내용에 따라 셀 너비 조정

- text-align 속성 : 셀 안에서 수평 정렬

- vertical-align 속성 : 셀 안에서 수직 정렬
	- <table><tr><th>속성값</th><th>설명</th></tr><tr><td>baseline</td><td>인라인 요소의 기준선을 부모 요소의 기준선에 맞춤</td></tr><tr><td>sub</td><td>인라인 요소의 기준선을 부모 요소의 아래 첨자 위치에 맞춤</td></tr><tr><td>super</td><td>인라인 요소의 기준선을 부모 요소의 위 첨자 위치에 맞춤</td></tr><tr><td>top</td><td>인라인 요소의 윗 부분을 부모 요소의 윗 부분에 맞춤</td></tr><tr><td>middle</td><td>인라인 요소의 중앙 부분을 부모 요소의 기준선에서 x-높이의 반만큼 올려서 맞춤</td></tr><tr><td>bottom</td><td>인라인 요소의 아랫부분을 부모 요소의 아랫부분에 맞춤</td></tr><tr><td>text-top</td><td>인라인 요소의 윗부분을 부모 요소 글꼴의 윗부분에 맞춤</td></tr><tr><td>text-bottom</td><td>인라인 요소의 아랫부분을 부모 요소 글꼴의 아랫부분에 맞춤</td></tr><tr><td>길이값</td><td>기준선을 0px로 생각하고 길이 값이 양수이면 기준선 위로, 음수이면 기준선 아래로 지정한 크기만금 옮김</td></tr><tr><td>백분율 값</td><td>기준선을 0%로 생각하고 line-height의 몇 %인지에 따라 양수면 위로, 음수면 아래로 옮김</td></tr></table>