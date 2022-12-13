# html

## 정보를 의미하는 태그 살펴보기

- meta
    - HTML 문서(웹페이지)의 제작자, 내용, 키워드 같은 여러 정보를 검색엔진이나 브라우저에게 제공
    - 속성
        - `charset`
            
            > Character Set
            > 
            - 문자 인코딩 방식을 지정하는 HTML 속성
        
        <aside>
        💡 문자 인코딩(Encoding)이란 문자나 기호들을 컴퓨터가 이해할 수 있는 신호로 만드는 것을 말하며, 웹에서는 UTF-8을 사용하는 것을 권장하고 있다.
        
        </aside>
        
        - `name` 정보의 종류
        - `content` 정보의 값
    
    ```html
    <meta charset="UTF-8" />
    <meta name="author" content="HEROPY" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    ```
    
    <aside>
    💡 사용자는 스마트폰(테블릿)에서 웹사이트를 오픈할 수도 있다. 즉, 스마트폰(모바일 환경)이 meta에서의 viewport를 의미한다. 모바일에서 웹 페이지의 가로 너비를 모바일 환경의 가로 너비와 일치시키거나, 웹 사이트가 처음 출력될 때의 확대/축소 여부나 정도를 결정하는 등의 정보를 META태그로 명시하는 개념이 name=’viewport’의 내용이다.
    
    </aside>
    
- title
    
    `<title>제목</title>`
    
    - HTML 문서의 제목(title)을 정의
    - 웹 브라우저 탭에 표시됨
- link
    - 외부 문서를 가져와 연결할 때 사용하며, 대부분 CSS 파일을 연결할 때 사용한다.
    - 필수 속성
        - `rel`
            
            > Relationship
            > 
            
            가져올 외부 문서(대표적으로 CSS파일)가 현재의 HTML과 어떤 관계인지를 명시하는 HTML 속성
            
        - `href`
            
            > Hyper Text Reference
            > 
            
            브라우저가 참조할 특정 경로(Path)를 지정하는 HTML 속성
            
    
    ```html
    <link rel=”stylesheet” href=”./main.css” />
    <link rel=”icon” href=”./favicon.png” />
    ```
    
    <aside>
    💡 Favicon(Favorite Icon) : HTML Favicon을 적용할 때는 이름을 favicon으로 지정하는 것을 권장하며, favicon.ico 혹은 favicon.png파일이 주로 사용된다.
    
    </aside>
    
- script
    - 속성
        - `src`
            
            > Source
            > 
            
            사용할 소스 코드(파일)를 지정하는 HTML 속성
            
        
        ```html
        <!-- 자바스크립트(JS)파일을 가져오는 경우 -->
        <script src="./main.js"></script>
        <!-- 자바스크립트(JS)를 HTML 문서 안에서 작성하는 경우 -->
        <script>
        	console.log('Hello world');
        </script>
        ```
        
- style
    - 스타일(CSS)를 HTML 문서 안에서 작성하는 경우에 사용
    
    ```html
    <style>
    	div {
    		color: red;
    	}
    </style>
    ```
