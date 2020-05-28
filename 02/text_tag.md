# 01) 텍스트 관련 태그들

## 01. 블록 레벨 태그

텍스트를 덩어리로 묶어주는 태그

- &lt;hn> : 제목 표시
- &lt;p> : 단락
- &lt;br> : 줄 바꿈 (닫는태그가 없음)
- &lt;hr> : 수평 줄 삽입 (닫는태그가 없음)
- &lt;blockquote> : 인용문 삽입. 들여쓰기로 구분
- &lt;pre> : 입력 그대로 화면 표시

## 02. 인라인 레벨 태그

텍스트를 한 줄로 표시하는 태그

- &lt;strong&GT;, &lt;b&GT; : 굵게 표시
    - &lt;strong&GT; : 중요한 내용 강조. 화면 낭독기에 강조 표시
    - &lt;b&GT; : 단순 굵게 표시
- &lt;em&GT;, &lt;i&GT; : 이탤릭체로 표시
    - &lt;em&GT; : 특정 부분 강조
    - &lt;i&GT; : 단순 이탤릭체 표시
- &lt;q&GT; : 인용 내용 표시. 줄 바꿈 없이 따옴표로 구분
- &lt;mark&GT; : 형광펜 효과
- &lt;span&GT; : 줄 바꿈 없이 영역 묶기
- &lt;ruby&GT;, &lt;rt&GT; : 주석 달기

## 03. 목록 태그

- &lt;ul&GT;, &lt;li&GT; : 순서 없는 목록
- &lt;ol&GT;, &lt;li&GT; : 순서 있는 목록
    - type 속성 : 숫자 종류 설정
    - start 속성 : 시작 번호 설정
    - reversed 속성 : 역순 설정
- &lt;dl&GT;, &lt;dt&GT;, &lt;dd&GT; : 설명 목록

## 04. 표를 만드는 태그

- &lt;table&GT;, &lt;tr&GT;, &lt;td&GT;, &lt;th&GT; : 기본적인 표
    - colspan, rowspan 속성 : 열과 행 합치기
    - aria-describedby 속성 : 테이블 밖에 인용문 id와 연결
- &lt;caption&GT;, &lt;figcaption&GT; : 표에 제목 붙이기
    - &lt;caption&GT; : table 태그 안에서 사용. 중앙에 제목 표시
    - &lt;figcaption&GT; : table 태그 밖에서 사용. 중앙에 표시되지 않음
- &lt;thead&GT;, &lt;tbody&GT;, &lt;tfoot&GT; : 표 구조 정의
- &lt;col&GT;, &lt;colgroup&GT; : 여러 열 묶어 스타일 지정
