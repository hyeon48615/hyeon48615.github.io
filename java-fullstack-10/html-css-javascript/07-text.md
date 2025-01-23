<h2>글꼴 스타일</h2>
<ul>
    <li>font-family
        <ul>
            <li>글꼴을 지정하는 속성</li>
            <li>기본형 : <code>font-family: 글꼴1, 2, 3,,,</code></li>
            <li>가장 마지막에는 모든 시스템이 보유하고 있는 글꼴 지정</li>
            <li>body 태그에 정의하면 모든 자식 요소에 같은 글꼴이 반영</li>
            <li>serif, sans-serif, monospace 는 모든 OS 시스템에 존재</li>
        </ul>
    </li>
    <li>font-size
        <ul>
            <li>글자 크기를 지정하는 속성</li>
            <li>기본형 : <code>font-size: 절대크기 | 상대크기 | 크기 | 백분율</code></li>
            <li>절대크기 : 브라우저에서 지정한 크기, px</li>
            <li>상대크기 : 부모요소 글자 크기 기준</li>
            <li>브라우저와 상관없이 글자 크기를 직접 지정</li>
            <li>부모요소의 글자 크기 기준으로 백분율(%)로 표시</li>
            <li>px, pt, %, vw, vh</li>
        </ul>
    </li>
    <li>font-style 
        <ul>
            <li>글자를 이탤릭체로 표현하는 속성</li>
            <li>기본형 : <code>font-style: normal | italic | oblique</code></li>
            <li>normal : 기본형</li>
            <li>italic : 이탤릭체</li>
            <li>oblique : 기울임꼴로 표시</li>
        </ul>
    </li>
    <li>font-wieght
        <ul>
            <li>글자 굵기를 조절</li>
            <li>키워드표기법
                <ul>
                    <li>글자의 굵기를 키워드로 표기</li>
                    <li>lighter, normal, bold, bolder 로 표기</li>
                </ul>
            </li>
            <li>숫자표기법
                <ul>
                    <li>100 단위 굵기로 표시</li>
                    <li>100 ~ 900 사이의 굵기 표현</li>
                        <li>100: 가장 가는 굵기, 900 : 가장 굵은 굵기</li>
                </ul>
            </li>
            <li>기본형 : <code>font-weight: normal | bold | bolder | lighter | 100 ~ 900</code></li>
        </ul>
    </li>
</ul>

<h2>텍스트 스타일</h2>
<ul>
    <li>color
        <ul>
            <li>글자 색 지정</li>
            <li>키워드 표기법(색상명)</li>
            <li>RGB 표기법
                <ul>
                    <li>Red, Green, Balue, alpha 값을 0~255</li>
                    <li><code>color: rgb(255,0,0)</code></li>
                    <li>투명도는 마지막에 알파값 추가 -> <code>color: rgba(255,255,255, 0.3)</code></li>
                    <li><code>color: rgb(red, green, blue, alpha)</code></li>
                </ul>
            </li>
            <li>HEX 표기법
                <ul>
                    <li>R/G/B 값을 16진수로 표기 00~ff</li>
                    <li>#RRGGBB</li>
                    <li>#RGB -> #ff0000 -> #f00</li>
                    <li><code>color: #ffff00</code></li>
                </ul>
            </li>
            <li>HSL
                <ul>
                    <li><code>color: hsl(240,100%,50%)</code></li>
                    <li>색상(hue), 채도(saturation), 밝기(light)</li>
                    <li>투명도 조정시 마지막에 알파값 추가 -> <code>color: hsla(240,100%,50%, 0.3)</code></li>
                    <li>알파값 : 0 ~ 1 값(1:불투명, 0:투명)</li>
                </ul>
            </li>
        </ul>
    </li>
    <li>text-align
        <ul>
            <li>텍스트 정렬 방법 지정</li>
            <li>기본형 : <code>text-align: left | right | center | justify | start | end | match-parent</code></li>
            <li>left : 왼쪽 정렬</li>
            <li>right : 오늘쪽 정렬</li>
            <li>center : 중앙 정렬</li>
            <li>justify : 양쪽 정렬</li>
            <li>start : 현재 테스트 줄의 시작 위치에 맞추어 문단을 정렬</li>
            <li>end : 현재 텍스트 줄의 끝 위이에 맞추어 문단을 정렬</li>
            <li>match-parent : 부모 요소에 따라서 문단을 정렬</li>
        </ul>
    </li>
    <li>line-height
        <ul>
            <li>문단의 행간 크기 조정</li>
            <li>normal : 웹브라우저 기본값</li>
            <li>숫자 : 현재 font-size 값에 입력한 숫자를 곱한 값 적용</li>
            <li>퍼센트 : 현재 font-size 값에 입력한 비율을 곱한 값 적용</li>
            <li>크기 : 사용자가 입력한 크기 적용</li>
        </ul>
    </li>
    <li>text-decoration
        <ul>
            <li>텍스트에 밑줄, 취소선 표시</li>
            <li>링크의 텍스트에 밑줄 제거시에도 사용</li>
            <li>기본형 : <code>text-decoration: none | underline | overline | line-through</code></li>
            <li>none : 밑줄을 표시하지 않음</li>
            <li>underline : 밑줄 표시</li>
            <li>overline : 영역위에 선 표시</li>
            <li>line-through : 취소선 표시</li>
        </ul>
    </li>
    <li>text-shadow
        <ul>
            <li>테스트에 그림자 효과 추가하는 속성</li>
            <li>기본형 : <code>text-shadow : none | 가로거리 세로거리 번짐정도 색상</code> </li>
            <li><code>text-shadow:1px 1px 3px #f00</code></li>
        </ul>
    </li>
    <li>text-transform
        <ul>
            <li>영문 텍스트의 대문자나 소문자를 바꾸는 속성</li>
            <li>기본형 : <code>text-transform : none | capitalize | uppercase | lowercase | full-width</code></li>
            <li>none : 변황 없음</li>
            <li>capitalize : 시작하는 첫 글자를 대문자로 변환</li>
            <li>uppercase : 모든 글자 대문자로 변환</li>
            <li>lowercase : 모든 글자 소문자로 변환</li>
            <li>full-width : 가능한 모든 문자를 전각문자로 변환</li>
        </ul>
    </li>
    <li>letter-spacing, word-spacing
        <ul>
            <li>기본형 : <code>letter-spacing: normal | 크기</code></li>
            <li>기본형 : <code>word-spacing: normal | 크기</code></li>
        </ul>
    </li>
</ul>

<h2>목록 스타일</h2>

<ul>
    <li>list-style-type
        <ul>
            <li>순서 없는 목록의 불릿이나 순서 목록의 숫자를 바꾸는 속성</li>
            <li>dic : 속이 찬 원모양</li>
            <li>circle : 빈 원모양</li>
            <li>square : 속이 찬 사각형</li>
            <li>decimal : 1부터 시작하는 숫자</li>
            <li>decimal-leading-zero : 앞에 0이 붙는 숫자 : 01, 02</li>
            <li>rower-roman : 로마숫자 소문자</li>
            <li>upper-roman : 로마숫자 대문자</li>
            <li>lower-alpha, lower-latin : 알파벳 소문자</li>
            <li>upper-alpha, upper-roman : 알파벳 대문자</li>
            <li>none : 블릿이나 숫자를 없앨 때 사용</li>
        </ul>
    </li>
    <li>list-style-image
        <ul>
            <li>불릿을 원하는 이미지로 지정</li>
            <li>기본형 : <code>list-style-image: url(이미지 경로) | none</code></li>
        </ul>
    </li>
    <li>list-style-position
        <ul>
            <li>불릿이나 번호의 위치를 들여쓰는 속성</li>
            <li>기본형 : <code>list-style-position: inside | outside(기본값)</code></li>
        </ul>
    </li>
    <li>list-style
        <ul>
            <li>목록 속성을 한 번에 지정할 때 사용</li>
            <li><code>ol { list-style: lower-alpha inside }</code></li>
        </ul>
    </li>
</ul>

<h2>표 스타일</h2>

<ul>
    <li>caption-side
        <ul>
            <li>캡션(설명글)의 위치 표시</li>
            <li>기본형 : <code>caption-side: top | bottom</code></li>
        </ul>
    </li>
    <li>border
        <ul>
            <li>표의 바깥 테두리와 셀 테두리를 지정</li>
            <li>기본형 : <code>border: 선의굵기 선의종류 색상</code></li>
            <li><code>border: 1px solid red;</code></li>
        </ul>
    </li>
    <li>border-spacing
        <ul>
            <li>셀과 셀 사이의 여백 조정</li>
            <li>기본형 : <code>border-spacing: 수평거리 수직거리</code></li>
        </ul>
    </li>
    <li>border-collapse
        <ul>
            <li>표 테두리와 셀의 테두리를 합칠 것인지 지정</li>
            <li>기본형 : <code>border-collapse: collapse | separate</code></li>
            <li>collapse : 테두리를 하나로 합쳐서 표시</li>
            <li>separate : 테두리를 따로 표시(기본값)</li>
        </ul>
    </li>
</ul>