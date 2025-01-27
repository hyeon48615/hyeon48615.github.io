<h1>HTML</h1>
<ul>
    <li>웹 문서를 만드는 언어</li>
    <li>HyperText Markup Language
        <ul>
            <li>HyperText : 문서를 서로 연결해주는 링크</li>
            <li>Markup Language : 태그 등을 이용하여 문서나 데이터의 구조 표현하는 언어</li>
        </ul>
    </li>
    <li>웹 브라우저에 보여 줄 내용에 마크업하고 문서끼리 링크하는 것</li>
    <li>HTML 문서의 구조
        <ul>
            <li>&lt;!DOCTYPE html&gt; : 현재 문서가 HTML 언어로 작성한 웹 문서라는 뜻</li>
            <li>&lt;html&gt;&lt;/html&gt;
                <ul>
                    <li>웹 문서의 시작과 끝을 나타내는 태그</li>
                    <li>lang 속성 : 문서에서 사용할 언어 지정</li>
                    <li><code>&lt;html lang="ko"&gt;&lt;/html&gt;</code></li>
                </ul>
            </li>
            <li>&lt;head&gt;&lt;/head&gt;
                <ul>
                    <li>웹 브라우저가 웹 문서를 해석하는 데 필요한 정보를 입력하는 부분</li>
                    <li>&lt;meta&gt; 태그
                        <ul>
                            <li>웹 문서와 관련된 정보를 지정할 사용</li>
                            <li>
                                화면에 글자를 표현할 때 어떤 인코딩을 사용할지 지정<br>
                                <code>&lt;meta charset="UTF-8"&gt;</code>
                            </li>
                            <li>웹 사이트의 키워드, 간단한 설명, 제작자 등의 정보 지정
                                <pre>
&lt;meta name="keywords" content="html의 구조"&gt;
&lt;meta name="description" content="html의 구조를 알아봅시다."&gt;
&lt;meta name="author" content="Kyunghee Ko"&gt;</pre> 
                            </li>
                        </ul>
                    </li>
                    <li>&lt;title&gt; 태그
                        <ul>
                            <li>웹 문서의 제목 지정</li>
                            <li><code>&lt;title&gt;HTML 문서의 구조&lt;/title&gt;</code></li>
                        </ul>
                    </li>
                </ul>
            </li>
            <li>&lt;body&gt;&lt;/body&gt; : 웹 브라우저 화면에 나타나는 내용</li>
        </ul>
    </li>
    <li>HTML 문서 작성
        <ul>
            <li>태그 작성법
                <ul>
                    <li>태그는 소문자로 작성한다.</li>
                    <li>여는 태그와 닫는 태그를 정확히 입력한다.</li>
                    <li>적당하게 들여쓰기를 한다.</li>
                    <li>일부 태그는 속성과 함께 사용한다.
                        <ul>
                            <li>&lt;태그 속성="속성값' ... &gt;</li>
                        </ul>
                    </li>
                </ul>
            </li>
            <li>시맨틱 태그(Semantic Tag)
                <ul>
                    <li>포함된 콘텐츠의 특정 의미를 정의하고 목적을 갖는 태그</li>
                    <li>태그에 의미를 부여하여 웹사이트의 구조를 파악하기 쉬움</li>
                    <li>
                        <code>
                            &lt;header&gt;, &lt;nav&gt;, &lt;article&gt;, &lt;section&gt;, &lt;footer&gt;, &lt;main&gt;
                        </code>
                    </li>
                </ul>
            </li>
            <li>시맨틱 태그의 이점
                <ul>
                    <li>접근성 향상 : 화면 판독기, 키보드 또는 음성 명령과 같은 보조 기술에 유용한 정보와 단서 제공
                        <ul>
                            <li><code>&lt;nav&gt;</code> : 탐색 링크 포함</li>
                            <li><code>&lt;article&gt;</code> : 독립형 콘텐츠 포함</li>
                        </ul>
                    </li>
                    <li>SEO(검색엔진최적화) 향상</li>
                    <li>가독성 향상</li>
                </ul>
            </li>
            <li>시맨틱 태그의 종류
                <ul>
                    <li>&lt;header&gt; 태그</li>
                    <li>&lt;nav&gt; 태그</li>
                    <li>&lt;main&gt; 태그
                        <ul>
                            <li>웹 문서에서 한 번만 사용 가능</li>
                        </ul>
                    </li>
                    <li>&lt;article&gt; 태그</li>
                    <li>&lt;section&gt; 태그</li>
                    <li>&lt;aside&gt; 태그</li>
                    <li>&lt;footer&gt; 태그</li>
                </ul>
            </li>
            <li>&lt;article&gt; VS &lt;section&gt;
                <ul>
                    <li>&lt;article&gt; : 문서내에서 그룹화해서 분리하는 역할</li>
                    <li>&lt;section&gt; : 섹션들을 그룹화해서 분리하는 역할</li>
                    <li>&lt;article&gt;은 내용이 독립적이다.
                         <ul>
                            <li>&lt;article&gt;은 &lt;section&gt;과 다르게 독립적으로 존재할 수 있고,
                                재사용할 수 있다.</li>
                            <li>&lt;article&gt;이 좀 더 구체적이다.</li>
                            <li>주로 블로그글, 포럼, 뉴스 기사 등에 사용</li>
                         </ul>
                    </li>
                    <li>&lt;section&gt;은 주제별로 구분한 그룹이다.
                        <ul>
                            <li>논리적으로 관계있는 요소 또는 문서를 분리할 때 사용한다.</li>
                            <li>논리적인 관계가 없는 요소들을 그룹화 할 경우에는 주로 &lt;div&gt;를 사용한다.</li>
                        </ul>
                    </li>
                    <li>
                        <pre>
&lt;article&gt;
    &lt;h1&gt;모집공고&lt;/h1&gt;
    &lt;section&gt;
        &lt;h2&gt;지원자격&lt;/h2&gt;
        &lt;p&gt;경력무관&lt;/p&gt;
        &lt;p&gt;학력무관&lt;/p&gt;
    &lt;/section&gt;
    &lt;section&gt;
        &lt;h2&gt;근무조건&lt;/h2&gt;
        &lt;p&gt;계약직&lt;/p&gt;
    &lt;/section&gt;
&lt;/article&gt;</pre>
                    </li>
                </ul>
            </li>
        </ul>
    </li>
</ul>