## 1. <u>스타일</u>을 사용하는 이유?
- HTML 은 웹 사이트의 내용 + CSS 는 디자인을 담당
-> 내용과 디자인을 수정해도 서로 영향을 미치지 않음
- 다양한 기기에 맞는 **반응형 웹 디자인** 구현

## 2. 스타일 형식
기본형 : `선택자 { 속성1: 속성값1; 속성2: 속성값2; }`

- 중괄호 { } 사이에 규칙 나열
- 세미콜론(;)으로 구분
- /* 와 */ 사이에 주석

## 3. 스타일 시트
### 브라우저 기본 스타일
- 브라우저에서 적용하는 스타일
- 사용자가 스타일을 지정하지 않아도 브라우저에 따라 적용되는 스타일

### 사용자 스타일
- 인라인 스타일
    - 스타일 시트를 사용하지 않고 적용할 대상에 직접 표시
    - 적용할 태그에 `style="속성: 속성값;"`을 사용
- 내부 스타일 시트
    - 스타일을 문서 안에 정리한 것
    - 작성법
        ```
        <head>
            <style>
                스타일
            </style>
        </head>
        ```
- 외부 스타일 시트
    - 스타일을 별도의 파일로 저장해 놓고 필요할 때 파일에서 가져와 사용
    - `<link rel="stylesheet" href="">`

## 4. 선택자
### 전체 선택자 
- 모든 요소를 대상으로 스타일을 적용
- `* { } `
### 타입 선택자
- 문서의 특정 태그에 스타일을 적용
- `태그 { }`
### class 선택자
- 특정 클래스에 스타일을 적용
- 문서 안에서 여러 번 반복할 스타일일 경우 사용
- `.클래스명 { }`
### id 선택자
- 특정 아이디에 스타일을 적용
- 문서 안에서 한번만 사용하는 경우 사용
- `#아이디명 { }`
### 그룹 선택자
- 같은 스타일을 사용하는 선택자를 모두 정의
- `선택자1, 선택자2 { }`

## 5. 캐스케이딩
### 캐스케이딩이란
- 스타일 시트에서 우선순위가 <u>위에서 아래로</u> 계단식으로 적용된다는 의미
- 스타일 충돌을 막기 위해 우선순위에 따라 적용할 스타일을 결정
- 원칙
    1. 스타일 우선순위 : 스타일의 규칙의 중요성과 적용 범위에 따라 우선순위가 결정되고, 그 우선순위에 따라 <u>위에서 아래로</u> 스타일을 적용
    2. 스타일 상속 : 태그들의 포함 관계에 따라 부모 요소의 스타일을 자식 요소로, <u>위에서 아래로</u> 전달

### 스타일 우선순위
<style>
    .container {
        display: flex;
        justify-content: space-between;
    }
    @media (max-width: 980px) {
        .container {
            display: block;
            width: 100%;
            height: 100%;
        }

    }
</style>
<div class="container">
    <div>
        <b>중요도</b>
        <ol>
            <li>사용자 스타일</li>
            <li>제작자 스타일</li>
            <li>브라우저 스타일</li>
        </ol>
    </div>
    <div>
        <b>적용 범위</b>
        <ol>
            <li>!important</li>
            <li>인라인 스타일</li>
            <li>id 스타일</li>
            <li>class 스타일</li>
            <li>타입 스타일</li>
        </ol>
    </div>
    <div>
        <b>소스 순서</b>
        <ul>
            <li>중요도와 적용 범위가 모두 같은 경우</li>
            <li>소스에서 더 나중에 온 스타일이 적용</li>
        </ul>
    </div>
</div>

### 스타일 상속
- 부모 요소에 있는 스타일 속성들이 자식 요소로 저달됨
- 단, 모든 요소가 상속되지는 않음. 예) `background-color`