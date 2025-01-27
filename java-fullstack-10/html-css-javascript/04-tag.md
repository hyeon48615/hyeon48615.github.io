<h1>HTML 입력 태그</h1>
<h2>텍스트 태그</h2>
<ul>
    <li>&lt;hn&gt; 태그
        <ul>
            <li>n의 자리 : 1~6의 숫자</li>
            <li>1 -> 6 일수록 글자의 크기가 작아짐</li>
            <li>h1은 문서에서 한 번만 쓰이며, h1 -> h2 -> h3... 순차적으로 사용</li>
        </ul>
    </li>
    <li>&lt;p&gt; 태그 : 텍스트를 단락으로 묶어서 표시할 때</li>
    <li>&lt;br&gt; 태그 : 줄을 바꿔서 표시할 때</li>
    <li>&lt;hr&gt; 태그 : horizontal. 가로줄을 그어 분위기를 전환할 때</li>
    <li>&lt;blockquote&gt; 태그 : 인용 구문을 사용할 때</li>
    <li>&lt;strong&gt;, &lt;b&gt; 태그 :  텍스트를 강조하거나 굵게 표시할 때</li>
    <li>&lt;em&gt;, &lt;i&gt;, &lt;cite&gt; 태그 : 기울인 텍스트를 표시할 때</li>
    <li>그 외
        <ul>
            <li>&lt;abbr&gt; 태그
                <ul>
                    <li>줄임말을 표시할 때(마우스 오버 시, 텍스트 상자 표시)</li>
                    <li><code>&lt;abbr title="Artificail Intelligence"&gt;AI&lt;/abbr&gt;</code></li>
                    <li><abbr title="Artificail Intelligence">AI</abbr></li>
                </ul>
            </li>
            <li>&lt;code&gt; 태그 : 소스 코드를 표시할 때</li>
            <li>&lt;del&gt; 태그 : 문서에서 삭제된 텍스트를 나타낼 때</li>
            <li>&lt;ins&gt; 태그 : 문서에 추가된 텍스트를 나타낼 때</li>
            <li>&lt;mark&gt; 태그
                <ul>
                    <li>태그를 적용한 부분에 하이라이트를 표시할 때</li>
                    <li><code>&lt;p&gt;껍질에 붉은빛이 돌아 &lt;mark&gt;레드향&lt;/mark&gt;이라 불린다.&lt;/p&gt;</code></li>
                    <li><p>껍질에 붉은빛이 돌아 <mark>레드향</mark>이라 불린다.</p></li>
                </ul>
            </li>
            <li>&lt;small&gt; 태그
                <ul>
                    <li>덧붙이는 글이나 저작권 등 부가 정보를 작게 표시할 때</li>
                    <li><code>&lt;p&gt;가격: 13,000원&lt;small&gt;(부가세 별도)&lt;/small&gt;&lt;/p&gt;</code></li>
                    <li><p>가격: 13,000원<small>(부가세 별도)</small></p></li>
                </ul>
            </li>
            <li>&lt;sub&gt; 태그 : 아래첨자를 표시할 때</li>
            <li>&lt;sup&gt; 태그 : 위첨자를 표시할 때</li>
        </ul>
    </li>
</ul>
<h2>목록 태그</h2>
<ul>
    <li>OL(Ordered List)
        <ul>
            <li>각 항목 앞에 숫자가 붙어서 정렬</li>
            <li>type 속성 : 순서 목록의 숫자 지정
                <ul>
                    <li>1: 숫자(default)</li>
                    <li>a: 소문자</li>
                    <li>A: 대문자</li>
                    <li>i: 로마소문자</li>
                    <li>I: 로마대문자</li>
                </ul>
            </li>
            <li>start 속성 : 목록의 시작 번호 수정</li>
        </ul>
    </li>
    <li>UL(Unordered List)
        <ul>
            <li>순서가 없는 목록을 작성</li>
        </ul>
    </li>
    <li>dl, dt, dd
        <ul>
            <li>이름(제목), 값(설명) 형태로 구성되어 있는 목록</li>
            <li>&lt;dt&gt; 태그 - 이름(제목) 지정</li>
            <li>&lt;dd&gt; 태그 - 값(설명) 지정</li>
            <li>하나의 &lt;dt&gt;에 여러 개의 &lt;dd&gt; 값을 가질 수 있음</li>
            <li>
                <dl>
                    <dt>이름(제목) 1</dt>
                    <dd>값(설명) 1</dd>
                    <dd>값(설명) 1-1</dd>
                    <dt>이름(제목) 2</dt>
                    <dd>값(설명) 2</dd>
                    <dd>값(설명) 2-1</dd>
                </dl>
            </li>
        </ul>
    </li>
</ul>

<h2>표(table) 태그</h2>
<ul>
    <li>table, tr, td 태그로 구성</li>
    <li>rowspan : 줄단위 합치기</li>
    <li>colspan : 컬럼단위 합치기</li>
    <li>col과, colgroup 태그 : 열을 그룹화할 떄 사용</li>
    <li>scope : 제목을 나타내는 셀의 범위(row 단위, column 단위로 구분) 표시</li>
    <li>표의 구조를 제목, 본문, 요약 부분으로 구성</li>
    <li>thead, tbody, tfoot 태그를 사용</li>
    <li>(시맨틱 태그 사용 시) 시각 장애인 디바이스에서도 쉽게 이해 가능</li>
    <li>자바스크립트로 본문 부분만 스크롤 가능하게 구현 가능</li>
</ul>

<style>
    #ex-table {
        padding: 10px;
        border: 1px solid black;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        column-gap: 20px;

    }

    table, tr, th, td {
        border-collapse: collapse;
        border: 1px solid black;
    }

    th, td {
        white-space: nowrap;
    }
</style>
<div id="ex-table">
    <table>
        <caption>테이블 태그</caption>
        <tr>
            <td>컬럼1</td>
            <td>컬럼2</td>
            <td>컬럼3</td>
            <td>컬럼4</td>
            <td>컬럼5</td>
        </tr>
        <tr>
            <td>컬럼1</td>
            <td>컬럼2</td>
            <td>컬럼3</td>
            <td colspan="2">컬럼4</td>
        </tr>
        <tr>
            <td rowspan="2">컬럼1</td>
            <td>컬럼2</td>
            <td>컬럼3</td>
            <td>컬럼4</td>
            <td>컬럼5</td>
        </tr>
        <tr>
            <td>컬럼2</td>
            <td>컬럼3</td>
            <td>컬럼4</td>
            <td>컬럼5</td>
        </tr>
    </table>
    <table>
        <caption>시맨틱 태그의 테이블</caption>
        <thead>
            <tr>
                <th>글번호</th>
                <th>제목</th>
                <th>등록일</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1</td>
                <td>제목1</td>
                <td>2024-12-31</td>
            </tr>
            <tr>
                <td>2</td>
                <td>제목2</td>
                <td>2024-12-31</td>
            </tr>
            <tr>
                <td>3</td>
                <td>제목3</td>
                <td>2024-01-01</td>
            </tr>
        </tbody>
    </table>
    <table>
        <caption>col 과 colgroup 테이블 구성</caption>
        <colgroup>
            <col style="background-color: aqua;">
            <col style="background-color: blueviolet;">
            <col style="background-color: chartreuse; width: 150px;">
        </colgroup>
        <thead>
            <tr>
                <th>글번호</th>
                <th>제목</th>
                <th>등록일</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1</td>
                <td>제목1</td>
                <td>2024-12-31</td>
            </tr>
            <tr>
                <td>2</td>
                <td>제목2</td>
                <td>2024-12-31</td>
            </tr>
            <tr>
                <td>3</td>
                <td>제목3</td>
                <td>2024-01-01</td>
            </tr>
        </tbody>
    </table>
</div>

<h2>이미지 태그</h2>
<ul>
    <li>img 태그
        <ul>
            <li>웹 문서에 이미지를 삽입할 때 사용</li>
            <li>이미지, 버튼 등의 용도로 사용</li>
            <li>파일형식 : gif, jpg, png, 웹이미지 형태 지원</li>
            <li>src : 이미지의 경로</li>
            <li>alt : 이미지 설명글, '' 빈공백으로 채우기도 한다</li>
            <li>width : 가로. 기본값, px, % 지정 가능</li>
            <li>height : 높이. 기본값, px, % 지정 가능</li>
            <li>border : 테두리</li>
            <li>&lt;figure&gt;, &lt;figcaption&gt; 태그
<pre>
    &lt;figure&gt;
        &lt;img src="images/spring.png" alt="제주의 봄"&gt;
        &lt;figcaption&gt;가장 먼저 봄을 맞이하는 제주도&lt;/figcaption&gt;
    &lt;/figure&gt;
</pre>
            </li>
            <li>srcset : 한꺼번에 이미지 정보로 여러개 지정하고, 화면 너비나 해상도에 따라 이미지를 적절하게 표시하는 속성<br>
<pre>
    &lt;img src="baloon.png" srcset="small.png 700w, large.png 1000w" alt="하늘 위로 올라가는 풍선"&gt;
    &lt;!-- w: 화면 너비 / 화면 너비가 640px 이라면 small.png를 표시하고, 1400px이라면 large.png를 표시 --&gt;<br>
    &lt;img src="sky.png" srcset="sky-1.png 1x, sky-2.png 2x" alt="파란 하늘 사진"&gt;
    &lt;!-- x: 픽셀 비율 / 일반 화면에서는 sky-1.png를 표시하고, 고해상도 화면에서는 sky-2.png를 표시 --&gt;
</pre>
            </li>
        </ul>
    </li>
    <li>object 태그
        <ul>
            <li>음악, 동영상, 자바 애플릿, pdf 등 객체 삽입</li>
            <li>오디오 : mp3, mp4, m4a</li>
            <li>도영상 : mp4, webm(브라우저마다 다름)</li>
            <li>width : 너비</li>
            <li>height : 높이</li>
            <li>data : 파일 정보</li>
            <li>&lt;object data="img/01.pdf" width="500px"&gt;&lt;/object&gt;</li>
        </ul>
    </li>
</ul>

<h2>오디오/비디오 태그</h2>
<ul>
    <li>audio 태그 : <code>&lt;audio src="audio/" controls&gt;&lt;/audio&gt;</code></li>
    <li>video 태그 : <code>&lt;video src="video/" controls&gt;&lt;/video&gt;</code></li>
    <li>속성
        <ul>
            <li>controls : UI 기능 노출</li>
            <li>autoplay : 자동 플레이 기능</li>
            <li>loop : 반복 재생 기능</li>
            <li>muted : 소리 제거 기능</li>
            <li>preload
                <ul>
                    <li>파일을 어떻게 로딩할 것인지 지정</li>
                    <li>auto(default), metadata, none</li>
                </ul>
            </li>
            <li>width, height : 플레이어의 너비와 높이 지정</li>
            <li>poster="파일 이름" : &lt;video&gt; 태그에서 사용. 썸네일 이미지 지정</li>
        </ul>
    </li>
</ul>

<h2>하이퍼링크 태그</h2>
<ul>
    <li>사이트 내의 문서, 문서 내의 특정 부분, 다른 사이트로 바로 연결해주는 기능</li>
    <li>기본형 <code>&lt;a href="링크주소"&gt;텍스트 또는 이미지&lt;/a&gt;</code></li>
    <li>href 속성 : 필수 속성</li>
    <li>추가 속성 : id, target</li>
    <li>target : _blank, _parent, _top, _self, 창이름</li>
</ul>

<style>
    #ex-a {
        display: flex;
        justify-content: center;
        column-gap: 20px;
    }

    #ex-a a {
        color: blue;
    }

    #ex-a a:hover {
        color: red;
    }
</style>

<div id="ex-a">
    <a href="https://www.naver.com" target="_blank">네이버</a>
    <a href="https://www.daum.net" target="_parent">다음</a>
    <a href="https://www.google.com" target="_top">구글</a>
    <a href="https://www.cnn.com" target="_self">CNN</a>
    <a href="https://www.nate.com" target="NEW">NATE</a>
</div>