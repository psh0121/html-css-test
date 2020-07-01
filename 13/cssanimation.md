# 13) CSS와 애니메이션

## 01. 변형

- 2차원 변형과 3차원 변형
	- 2차원 변형(2D transform) :
	웹 요소를 변형시킬 때 단순히 수평이나 수직으로 이동하고 회전하는 것
	- 3차원 변형(3D transform) :
	기존 2차원 변형에서 z값을 추가해 원근감까지 표현할 수 있는 것

- transform과 변형함수 : 웹 요소를 변형할 때 사용하는 속성으로 transform: 다음에 변형함수를 함께 입력
	- 2차원 변형 함수
	<table>
	<tr><th>변형 함수</th><th>설명</th></tr>
	<tr><td>translate(tx, ty)</td><td>지정한 크기만큼 x축과 y축으로 이동</td></tr><tr><td>translateX(tx)</td><td>지정한 크기만큼 x축으로 이동한다.</td></tr><tr><td>translateY(ty)</td><td>지정한 크기만큼 y축으로 이동</td></tr><tr><td>scale(sx, sy)</td><td>지정한 크기만큼 x축과 y축으로 확대/축소</td></tr><tr><td>scaleX(sx)</td><td>지정한 크기만큼 x축으로 확대/축소</td></tr><tr><td>scaleY(sy)</td><td>지정한 크기만큼 y축으로 확대/축소</td></tr><tr><td>rotate(각도)</td><td>지정한 각도만큼 회전</td></tr><tr><td>skew(ax, ay)</td><td>지정한 각도만큼 x축과 y축으로 왜곡</td></tr><tr><td>skewX(ax)</td><td>지정한 각도만큼 x축으로 왜곡</td></tr><tr><td>skewY(ay)</td><td>지정한 각도만큼 y축으로 왜곡</td></tr></table>
	- 3차원 변형 함수
	<table>
	<tr><th>변형 함수</th><th>설명</th></tr><tr><td>matrix3d(n [, n])</td><td>4*4 행렬을 이용해 이동과 확대/축소, 회전 등의 변환을 지정</td></tr><tr><td>translate3d(tx, ty, tz)</td><td>지정한 크기만큼 x축과 y축, z축으로 이동</td></tr><tr><td>translateZ(tz)</td><td>지정한 크기만큼 z축으로 이동</td></tr><tr><td>scale3d(sx, sy, sz)</td><td>지정한 크기만큼 x축과 y축, z축으로 확대/축소</td></tr><tr><td>scaleZ(sz)</td><td>지정한 크기만큼 z축으로 확대/축소</td></tr><tr><td>rotate3d(rx, ry, rz, 각도)</td><td>지정한 각도만큼 회전</td></tr><tr><td>rotateX(각도)</td><td>지정한 각도만큼 x축으로 회전</td></tr><tr><td>rotateY(각도)</td><td>지정한 각도만큼 y축으로 회전</td></tr><tr><td>rotateZ(각도)</td><td>지정한 각도만큼 Z축으로 회전</td></tr><tr><td>perspective(길이)</td><td>입체적으로 보일 수 있는 깊이 값을 지정</td></tr></table>

## 02. 변형과 관련된 속성들

- transform-origin 속성 : 변형 기준점 설정

- perspective, perspective-origin 속성 : 원근감 표현
	- perspective 속성 : 
	원래 위치에서 사용자가 있는 방향이나 반대 방향으로 잡아당기거나 밀어내 원근감 표현
	- perspective-origin 속성 : 
	입체적으로 표현할 요소의 아랫부분의 위치 지정 가능. 더욱 깊은 입체적 표현

- transform-style 속성 : 3D 변형 적용

- backface-visibility 속성 : 요소의 뒷면 표시

## 03. 트랜지션

- 트랜지션 (transition) : 시간에 따라서 웹 요소의 스타일 속성이 조금씩 바뀌는 것
<table><tr><th>속성</th><th>설명</th></tr><tr><td>transition-property</td><td>트랜지션 대상 설정</td></tr><tr><td>transition-duration</td><td>트랜지션 진행 시간 설정</td></tr><tr><td>transition-timing-function</td><td>트랜지션 속도 곡선 설정</td></tr><tr><td>transition-delay</td><td>트랜지션 지연 시간 설정</td></tr><tr><td>transition</td><td>트랜지션의 속성들을 한꺼번에 설정</td></tr></table>

## 04. 애니메이션

- CSS와 애니메이션
애니메이션은 시작 스타일과 끝 스타일을 지정하면 CSS에서 중간 스타일을 자동으로 추가해 전체적으로 부드럽게 변하는 애니메이션 효과를 만들어 낸다는 트랜지션과 비슷한 성격을 가지고 있긴 하지만, CSS 애니메이션은 시작해 끝나는 동안 원하는 곳 어디서든 스타일을 바꾸면 애니메이션을 정의할 수 있다는 차이점이 있음.
	- 키프레임 : 애니메이션 중간에 스타일이 바뀌는 지점
- CSS 애니메이션에서 사용하는 속성
<table><tr><th>속성</th><th>설명</th></tr><tr><td>@keyframes</td><td>애니메이션이 바뀌는 지점을 설정</td></tr><tr><td>animation-delay</td><td>애니메이션 지연 시간 지정</td></tr><tr><td>animation-direction</td><td>애니메이션 종료 후 처음부터 시작할지, 역방향으로 진행할지 지정</td></tr><tr><td>animation-duration</td><td>애니메이션 실행 시간 설정</td></tr><tr><td>animation-fill-mode</td><td>애니메이션이 종료되었거나 지연되어 애니메이션이 실행되지 않는 상태일 때 요소의 스타일 지정</td></tr><tr><td>animation-iteration-count</td><td>애니메이션 반복 횟수를 지정</td></tr><tr><td>animation-name</td><td>@keyframes 로 설정해 놓은 중간 상태의 이름을 지정</td></tr><tr><td>animation-play-state</td><td>애니메이션을 멈추거나 다시 시작</td></tr><tr><td>animation-timing-function</td><td>애니메이션의 속도 곡선을 지정</td></tr><tr><td>animation</td><td>animation 하위 속성들을 한꺼번에 묶어 지정</td></tr></table>