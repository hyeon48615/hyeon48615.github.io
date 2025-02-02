# 입력 양식
- form 태그 사용
- 데이터를 전송하기 위한 목적으로 사용
- `<form name=폼이름 action=이동대상URL method=전송방식>`
- name : 폼이름
- method : GET(default) / POST
  - GET 방식
    - 256 ~ 4096 byte 까지 전송 가능 (안정적으로 처리 시 2MB 까지 전송 가능)
    - 주소 표시줄에 사용자가 입력한 내용이 그대로 노출
  - POST 방식
    - 전송 데이터의 길이 제한이 없음 (시스템이 받아주는 한)
    - url 입력창 혹은 전송 스트링 상에 노출하지 않음
- action : 서버쪽 URL 지정
- target : action 에서 지정한 파일을 현재창 혹은 다른 위치에서 동작하도록 지정

## 폼 작성하기
- autocomplete
  - 예전에 입력한 내용을 자동으로 표시해주는 자동 완성 기능
  - on(default) / off
- fieldset
  - 폼의 요소를 묶는 용도로 사용하는 태그
  - `<fieldset [속성=속성값]></fieldset>`
- legend
  - 그룹으로 묶는 구역에 제목을 붙이는 태그
  - `<legend>그룹이름</legend>`
- label
  - input 태그와 같은 폼 요소에 레이블을 붙일 때 사용
  - 이름(설명) 구문을 출력할 떄 많이 사용
  - 암묵적인 방법 : label 태그에 상호작용 요소를 포함
  - 명시적인 방법 : label 태그에 for 속성과 대상 태그의 id 속성을 이용하여 설정
  - 두 가지 방법을 함께 사용하기도 함
  
## input 태그
### input 태그의 type 속성
  - text : 한 줄짜리 텍스트를 입력<br>
    password : 비밀번호를 입력하는 용도(입력된 값이 * 로 표시)
    - size : 입력창의 크기. 글자 수
    - value : 입력창에 보여지는 값
    - maxlength : 입력창에 입력할 수 있는 최대 글자 수
  - search : 검색할 때 입력하는 용도
  - url : URL 주소를 입력하는 필드
  - email : 이베일 주소를 입력하는 필드
  - tel : 전화번호를 입력하는 필드
  - checkbox : 주어진 여러 항목을 1개 이상 선택할 수 있는 체크박스<br>
    radio : 주어진 여러 항목 중에서 1개만 선택할 수 있는 체크박스
    - value : 서버에 넘겨줄 값. 영문 또는 숫자. 필수값
    - checked : 기본적으로 선택되어 보여줄 항목
    - name : 같은 그룹에 같은 속성값(이름)을 사용
  - number : 숫자를 입력, 조절할 수 있는 UI 출력
  - range : 숫자를 조절할 수 있는 슬라이드 막대 UI 출력
    - min, max, value
    - step : 숫자 간격. 기본값 1
  - date : 사용자 지역 기준 날짜(년, 워, 일) UI 출력<br>
    month : 사용자 지역 기준 날짜(년, 월) 입력할 수 있는 UI<br>
    week : 사용자 지역 기준 날짜(년, 주) 입력할 수 있는 UI<br>
    time : 사용자 지역 기준 시간(시, 분, 초, 분할 초)를 입력할 수 있는 UI<br>
    datetime : 국제 표준시(UTC)로 설정된 날짜, 시간(년, 월, 일, 시, 분, 초, 분할 초)를 입력할 수 있는 UI<br>
    datetime-local : 사용자 지역 기준으로 datetime 출력<br>
    - min, max, step, value
  - submit : 전송 버튼을 출력, 클릭 시 폼 전송 발생
  - reset : 리셋 버튼을 출력, 클릭 시 폼 항목 초기화
  - image : submit 대신에 이미지를 출력, 클릭 시 폼 전송 발생
  - button : 일반 버튼을 출력
  - file : 파일을 첨부할 수 있는 버튼 출력, 커스터마이징 할 수 없다
  - hidden : 사용자에게 보이지 않지만, 입력된 데이터를 서버로 전달하는 역할

### input 태그의 주요 속성
  - autofocus : 입력 커서를 자동으로 이동
  - placeholder : 입력 힌트를 표시
  - readonly : 읽기 전용 필드 지정
  - required : 필수 입력 필드 지정

## 폼에서 사용하는 태그들
- textarea
  - 여러 줄 입력하는 영역을 만들 때 사용
  - cols : 텍스트 영역의 가로 너비. 문자 단위
  - rows : 텍스트 영역의 세로 너비. 줄 단위
- select, option
  - 드롭다운 목록을 만들 때 사용
  - select
    - size : 화면에 표시할 드롭다운의 항목 개수 지정
    - multiple : 둘 이상의 항목을 선택할 때 사용
  - option
    - value : 서버로 넘겨줄 값
    - selected : 기본적으로 선택되어 보여줄 항목
  - multiple 옵션에서 selected가 여러 개 지정되어 있다면,
    제일 마지막에 지정된 것이 선택되어 보여짐
- button
  - type 속성: submit, reset, button
