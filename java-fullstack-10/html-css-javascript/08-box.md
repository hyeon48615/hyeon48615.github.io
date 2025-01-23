<h2>CSS 박스 모델</h2>
<ul>
    <li>블록 레벨 요소
        <ul>
            <li>요소를 삽입했을 때 한 줄을 차지하는 요소</li>
            <li>요소의 너비가 100%</li>
            <li>div, table, hn, p, form, ul, ol, li, 
                dl, dt, dd, blockquote 등</li>
        </ul>
    </li>
    <li>인라인(non-block) 레벨 요소
        <ul>
            <li>줄을 차지하지 않는 요소</li>
            <li>컨텐츠의 길이만큼 화면 여역을 차지하고,
                나머지 공간에 다른 요소가 올 수 있음</li>
            <li>img, span, label, a, input 등</li>
        </ul>
    </li>
    <li>블록 레벨 요소 VS 인라인 레벨 요소
        <ul>
            <li>width, height : 인라인 요소는 컨텐츠 크기에 따라 자동으로 결정. 블록 요소만 지정 가능</li>
            <li>margin, padding : 인라인 요소는 수평방향(margin-left, margin-right)만 적용. 블록 요소는 모두 적용 가능</li>
        </ul>
    </li>
    <li>width, height 속성
        <ul>
            <li>width : 실제 컨텐츠 영역의 너비 크기를 지정</li>
            <li>height : 실제 컨텐츠 영역의 높이 크기를 지정</li>
            <li>auto : 컨텐츠의 크기에 따라 자동으로 결정 (기본값)</li>
        </ul>
    </li>
    <li>box-sizing 속성
        <ul>
            <li>실제 박스 모델의 너비 계산시 포함하는 영역을 결정</li>
            <li>border-box : 테두리까지 포함하여 너비 값 계산</li>
            <li>content-box : 컨텐츠 영역만 너비 값으로 계산 (기본값)</li>
        </ul>
    </li>
    <li>box-shadow 속성
        <ul>
            <li>선택한 요소에 그림자 효과를 냄</li>
            <li>기본형 : <code>box-shadow: 수평거리 수직거리 흐림정도 번짐정도 색상 inset</code></li>
            <li>수평거리 : 그림자가 가로로 얼마나 떨어져 있는가. 양수-오른쪽, 음수-왼쪽</li>
            <li>수직거리 : 그림자가 세로로 얼마나 떨어져 있는가. 양수-아래쪽, 음수-위쪽</li>
            <li>흐림정도 : 그림자의 진한 정도. 0이 기본값. 음수 사용 불가</li>
            <li>번짐정도 : 양수-모든 방향으로 퍼져서 표시. 음수-모든 방향으로 그림자가 축소되어 표시</li>
            <li>색상 : 한가지 색상/여러가지 색상 지정 가능. 기본값:검정색</li>
            <li>inset : 안쪽 그림자로 표시</li>
        </ul>
    </li>
</ul>
<h2>테두리 스타일</h2>
<ul>
    <li>box 모델의 값 설정
        <ul>
            <li>margin, padding 값의 지정 방향 존재</li>
            <li>전체 방향 지정시에는 방향성 없이 하나의 값으로 설정</li>
            <li>top -> right -> bottom -> left</li>
            <li>margin: 10px</li>
            <li>margin-top: 10px</li>
            <li>margin-right: 10px</li>
            <li>margin-bottom: 10px</li>
            <li>margin-left: 10px</li>
            <li>maring: 10px 10px 10px 10px</li>
            <li>maring: 10px 20px</li>
        </ul>
    </li>
    <li>border-style 속성
        <ul>
            <li>기본값 : none -> 테두리 표시 안됨</li>
            <li>즉, 테두리를 그리기 위해서는 테두리 스타일을 지정해야 함</li>
            <li>기본형 : <code>border-style: none | hidden | dashed | dotted | solid | double | groove | inset | outset | ridge</code></li>
            <li>none : 테두리 없음</li>
            <li>hidden : 테두리를 표시하지 않음. collapse 일 경우에도 표시하지 않음</li>
            <li>dashed : 파선(짧은 직선)</li>
            <li>dotted : 점선</li>
            <li>solid : 실선</li>
            <li>double : 이중선</li>
            <li>groove : 테두리를 창에 조각한 것처럼 표시</li>
            <li>ridge : 테두리가 창틀에서 튀어나온 것처럼 표시</li>
            <li>inset : 표에서 border-collapse: separate 일 경우, 전체 테두리를 창문처럼 표시.
                collapse 일 경우, groove와 동일
            </li>
            <li>outset : 표에서 border-collapse: separate 일 경우, 전체 테두리가 튀어나온 것처럼 표시.
                collapse 일 경우, ridge와 동일
            </li>
        </ul>
    </li>
    <li>border-width 속성
        <ul>
            <li>테두리의 두께 지정</li>
            <li>기본형 : <code>border-width: 크기 | thin | medium | thick</code></li>
            <li>border-width: top right bottom left</li>
            <li>border-width: 값/li>
        </ul>
    </li>
    <li>border-color 속성
        <ul>
            <li>테두리의 색상 지정</li>
            <li>border-color: 값 -> 4방향 모두</li>
            <li>border-top-color, -right-color, -bottom-color, -left-color -> 각각 해당 방향의 테두리 색상 지정</li>
        </ul>
    </li>
    <li>border 속성
        <ul>
            <li>테두리 스타일과 두께, 색상을 한 번에 지정</li>
            <li><code>border: 3px dotted blue</code></li>
        </ul>
    </li>
</ul>
<li>border-radius 속성
    <ul>
        <li>박스 모델의 테두리의 꼭지점 부분을 둥글게 처리</li>
        <li>기본형 <code>border-radius: 크기 | 백분율</code></li>
        <li>크기 : ps, em 을 사용하여 반지름의 크기를 수치로 표시</li>
        <li>백분율 : 현재 요소의 크기 기준으로 비율(%)를 지정</li>
        <li>border-top-left-radius, -top-right-radius, 
            -bottom-right-radius, -bottom-left-radius</li>
    </ul>
</li>
<h2>웹 문서의 레이아웃</h2>
<ul>
    <li>display 속성
        <ul>
            <li>요소의 배치 방법을 결정</li>
            <li>HTML 태그가 기본적으로 가지고 있는 박스 모델의 성격을 변경</li>
            <li>박스 모델의 성격
                <ul>
                    <li>블록 성격 : 요소의 너비가 컨텐츠의 유무와 상관없이 항상 가로 한 줄을 차지</li>
                    <li>인라인 성격 : 요소의 너비를 컨텐츠 크기만큼 차지</li>
                    <li>인라인 블록 : 요소의 너비가 컨텐츠의 크기만큼 차지하지만 그 외 성격은 블록 성격을 가지는 것</li>
                    <li>block : 인라인 레벨 요소를 블록 레벨 요소로 만듦</li>
                    <li>inline : 블록 레벨 요소를 인라인 레벨 요소로 만듦</li>
                    <li>inline-block : 인라인 레벨 요소와 블록 레벨 요소의 속성을 모두 각지고 있으며,
                        마진과 패딩 등을 지정할 수 있음
                    </li>
                    <li>none : 해당 요소를 화면에 표시하지 않음</li>
                </ul>
            </li>
        </ul>
    </li>
    <li>float 속성
        <ul>
            <li>요소를 왼쪽, 오른쪽 등으로 위치</li>
            <li>적용대상의 원래 위치를 보장하지 않음</li>
            <li>기본형 : <code>float: left | right | none</code></li>
            <li>left : 해당 요소를 문서의 왼쪽으로 배치</li>
        </ul>
    </li>
    <li>clear 속성
        <ul>
            <li>float 속성을 무효화 시키는 속성</li>
            <li>기본형 : <code>clear: none | left | right | both</code></li>
            <li>left: <code>float: left</code> 해제</li>
            <li>right: <code>float: right</code> 해제</li>
            <li>both: left, right 해제</li>
        </ul>
    </li>
</ul>
<h2>웹 요소의 위치 지정</h2>
<ul>
    <li>left: 기준 위치와 요소 사이의 왼쪽의 공백</li>
    <li>right : 기준 위치와 요소 사이의 오른쪽 공백</li>
    <li>top : 기준 위치와 요소 사이의 위쪽 공백</li>
    <li>bottom : 기준 위치와 요소 사이의 아랫쪽 공백</li>
    <br>
    <li>position 속성
        <ul>
            <li>웹 문서에 요소를 배치하기 위한 속성</li>
            <li>기본형 : <code>position: static | relative | absolute | fixed</code></li>
            <li>static : 요소를 기본 흐름에 따라서 배치</li>
            <li>relative : 요소를 기본 흐름에 따라서 배치. 좌표 속성 사용</li>
            <li>absolute : relative 값을 사용한 상위 요소를 기준으로 위치 지정</li>
            <li>fixed : 지정한 위치에 고정하여 배치. 화면에서 잘리거나, 보이지 않을 수 있음</li>
        </ul>
    </li>
    <li>z-index 속성
        <ul>
            <li>position 속성으로 배치한 요소의 z축 위치를 결정</li>
            <li>기본형 : <code>z-index: 정수값</code></li>
            <li>1~1000</li>
        </ul>
    </li>
</ul>