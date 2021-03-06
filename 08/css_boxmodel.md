# 08) CSS 박스 모델

## 01. CSS와 박스 모델

- CSS 박스 모델 : 웹 문서의 내용을 박스 형태로 정의하는 방법

- 블록 레벨 요소 & 인라인 레벨 요소
	- 블록 레벨 요소 : 
	태그를 사용애 요소를 삽입했을 때 혼자 한 줄을 차지하는 요소
	혼자 한 줄을 차지하는 요소로 다른 요소가 올 수 없음
	- 인라인 레벨 요소 : 
	줄을 차지하지 않는 요소
	한 줄에 여러 개의 인라인 레벨 요소 표시 가능
	
- 박스 모델 : 텍스트 단락 앞 뒤에 빈 줄이 생기면서 텍스트 단락이 하나의 박스 형태를 가지는 것
	- 콘텐츠 영역 : 내용이 입력되는 곳
	- 패딩 : 박스와 콘텐스 영역 사이의 여백
	- 테두리 : 박스의 테두리
	- 마진 : 여러 박스 모델 사이의 여백
	
- width, height 속성 : 콘텐츠 영역의 크기
	- 실제 콘첸츠 크기 계산하기
		- 모던브라우저에서 박스 모델의 전체 너비 = width 값 + 좌우 패딩 + 좌우 테두리
		- 인터넷 익스플로러 6에서 박스 모델의 width 값 = 콘텐츠 너비 + 좌우 패딩 + 좌우 테두리
		
- display 속성 : 화면 배치 방법 결정
	- block : 해당 요소를 블록 레벨로 지정
	- inline : 블록 레벨 요소를 인라인 레벨로 변경
	- inline-block : 요소를 인라인 레벨로 배치하면서 내용에는 블록 레벨 속성을 지정한 것
	블록 레벨과 인라인 레벨의 특성 보임
	- none : 해당 요소를 화면에 아예 표시하지 않음
	
## 02. 테두리 관련 속성들
	
- border-style 속성 : 테두리 스타일 지정
	- none : 테두리가 나타나지 않음
	- hidden : 테두리가 나타나지 않음
	- dashed : 직선으로 된 점선으로 표시
	- dotted : 테두리를 점선으로 표시
	- double : 이중선으로 표시
	- groove : 테두리를 창에 조각한 것 처럼 표시
	- ridge : 테두리를 창에서 튀어나온 것처럼 표시
	- solid : 테두리를 실선으로 표시
	- inset
	- outset

- border-width 속성 : 테두리 두께 지정

- border-color 속성 : 테두리 색상 지정

- border 속성 : 테두리의 여러 속성들을 묶어서 스타일 지정

- border-radius 속성 : 박스 모서리 둥글게 지정
	- 타원 형태로 둥글게 만드는 법 : 가로 반지름과 세로 반지름의 크기를 함께 지정

- border-shadow 속성 : 그림자 효과. 수평거리와 수직거리 반드시 지정

## 03. 여백을 조절하는 속성

- margin 속성 : 요소 주변 여백 설정
	- 마진 중첩 현상 :
	요소를 세로로 배치할 경우 마진과 마진이 만날 때 마진 값이 큰 쪽으로 겹쳐지는 것
	오른쪽 마진과 왼쪽 마진이 만날 경우엔 중첩되지 않음

- padding 속성 : 콘텐츠 영역과 테두리 사이 여백 설정

