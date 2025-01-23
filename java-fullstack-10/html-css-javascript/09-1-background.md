<h2>배경색/범위 지정</h2>
<ul>
    <li>background-color 속성
        <ul>
            <li>웹 문서의 요소에 배경색 지정</li>
            <li>16진수, rgb, rgba, 색상이름 사용 가능</li>
            <li>배경색을 상속되지 않는다</li>
            <li>기본형 : <code>background-color: 색상값</code></li>
        </ul>
    </li>
    <li>background-clip 속성
        <ul>
            <li>배경 적용 영역을 결정</li>
            <li>기본형 : <code>background-clip: border-box | padding-box | content-box</code></li>
        </ul>
    </li>
</ul>
<h2>배경 이미지 지정</h2>
<ul>
    <li>background-image 속성
        <ul>
            <li>배경 이미지 파일 경로 지정</li>
            <li>기본형 : <code>background-image: url(파일경로)</code></li>
        </ul>
    </li>
    <li>background-repeat 속성
        <ul>
            <li>배경 이미지의 반복 여부와 방향 설정</li>
            <li>기본형 : <code>background-repeat: repeat | repeat-x | repeat-y | no-repeat</code></li>
            <li>repeat : 브라우저 화면에 가득찰때까지 가로, 세로 반복 (기본값)</li>
            <li>repeat-x : 브라우저 창 너비와 같아질때까지 배경을 가로로 반복</li>
            <li>repeat-y : 브라우저 창 너비와 같아질때까지 배경을 세로로 반복</li>
            <li>no-repeat : 한번만 표시하고 반복하지 않음</li>
            <li>round : 배경 이미지를 지정된 요소의 크기에 맞게 반복 및 크기 조정</li>
            <li>space : 배경 이미지를 지정된 요소의 크기에 맞게 반복하되, 이미지 간 여백을 추가하여 균등하게 배치</li>
        </ul>
    </li>
    <li>background-position 속성
        <ul>
            <li>배경 이미지를 반복하지 않을 경우 이미지를 표시할 위치 지정</li>
            <li>기본형 : <code>background-position: 수평위치 수직위치</code></li>
            <li>수평위치 : left | center | right | 백분율 | 길이</li>
            <li>수직위치 : top | center | bottom | 백분율 | 길이</li>
            <li>px, rem, em, % : 위치를 직접 지정</li>
        </ul>
    </li>
    <li>background-origin 속성
        <ul>
            <li>배경 이미지 배치를 위한 기준 설정</li>
            <li>기본형 : <code>background-origin: border-box | padding-box | content-box</code></li>
            <li>border-box : 박스 모델의 가장 테두리가 기준</li>
            <li>padding-box : 박스 모델의 테두리를 뺀 패딩이 기준</li>
            <li>content-box : 박스 모델의 내용 부분이 기준</li>
        </ul>
    </li>
    <li>background-attatchment 속성
        <ul>
            <li>배경 이미지를 고정하는 속성</li>
            <li>기본형 : <code>background-attatchment: scroll | fixed | local</code></li>
            <li>scroll : 화면 스크롤과 함께 배경 이미지도 스크롤 됨 (기본값)</li>
            <li>fixed : 화면이 스크롤되더라도 배경 이미지는 고정</li>
            <li>local : 삽입된 이미지가 요소와 웹 브라우저에서 모두 스크롤</li>
        </ul>
    </li>
    <li>background 속성
        <ul>
            <li>배경 관련 속성을 한 번에 표시</li>
            <li>순서는 상관 없음</li>
            <li>기본형 : <code>background: url() no-repeat center bottom fixed;</code></li>
        </ul>
    </li>
    <li>background-size 속성
        <ul>
            <li>배경 이미지 크기를 조절</li>
            <li>기본형 : <codee>background-size: auto | contain | cover | 크기 | 백분율</codee></li>
            <li>auto : 이미지 크기만큼 표시 (기본값)</li>
            <li>contain : 요소 안에 배경 이미지가 다 들어오도록 확대/축소</li>
            <li>cover : 배경 이미지로 요소를 모두 덮도록 확대/축소</li>
            <li>크기 : 이미지의 너비/높이 지정. 하나만 설정하였을 경우, 비율에 맞춰 출력</li>
            <li>백분율 : 배경 이미지가 들어갈 요소의 크기를 기준으로,
                그 크기에 맞도록 이미지를 확대/축소
            </li>
        </ul>
    </li>
</ul>