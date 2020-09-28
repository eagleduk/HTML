참고 사이트: https://heropy.blog/

A. HTML - 블록 레벨(Block Level) 요소와 인라인(Inline) 요소
    - 블록요소
        1. div, h1, p...
        2. 사용가능한 최대 가로 너비를 사용한다. (기본값)
        3. 크기를 지정할 수 있다.
        4. width: 100%, height: 0 으로 시작한다.
        5. 수직으로 쌓인다.
        6. margin, padding 위,아래,좌,우 여백 사용 가능하다.
        7. 레이아웃을 만드는데 주로 사용

    - 인라인 요소
        1. span, img...
        2. 필요한 만큼의 너비, 높이를 사용한다. (기본값)
        3. 크리를 지정할 수 없다.
        4. width: 0, height: 0 으로 시작한다.
        5. 수평으로 쌓인다.
        6. margin, padding 좌, 우 여백만 사용 가능하다.
        7. TEXT, 컨텐츠를 출력하는데 주로 사용

B. HTML 태그
    - DOCTYPE - html 버전 명시
    - html
        1. head - 문서의 정보
            1. HTML 문서의 제목 <title></title>
            2. 기타 정보 <meta>
                - charset : UTF-8, EUC-KR
                - name, content : 메타 정보 이름, 메타 정보 값.
                - http-equiv, content
            3. 링크 <link>
            4. 스타일 <style></style>
            5. 베이스 <base>
                - 상대경로를 미리 저장
                - HTML에 하나만 사용 가능.

        2. body - 문서의 구조
            : 각 태그들은 효과보다 의미에 맞게 사용하는것이 중요

            <블록(display: block) 요소>
                1. header
                    - header에 들어갈 내용이 들어있는 영역 > 주로 로고, 메뉴등
                2. footer
                    - footer 들어갈 내용이 들어있는 영역 > 주로 회사정보 등
                3. h1-h6
                    - 단계별 제목 등을 오름차순으로 표현
                4. main
                    - 주요 콘텐츠가 들어갈 내용이 들어있는 영역
                    - 문서의 주요 콘텐츠를 설정
                    - 한 문서(HTML)에 하나의 요소만 포함 가능
                5. article
                    - 독립성, 재사용
                6. section
                    - 영역을 나누는데 많이 사용 > 섹션
                    - 제목을 포함하는 영역
                7. aside
                    - 사이드의 광고 등이 들어있는 영역
                8. nav
                    - 메뉴의 내용이 들어있는 영역
                9. address
                    - 연락처 정보가 들어있는 영역
                10. div
                    - 영역 구분을 위해 사용
                11. ol, ul, li
                    - Ordered-List, Unordered-List, List-Item
                    - li는 ol, ul의 자식으로만 사용 가능
                    - ol 의 항목순서는 중요도를 의미할 수 있다.
                    - ol은 순서가 있는 리스트, ul은 순서가 없는 리스트
                12. dl, dt, dd
                    - 용어(Description Term - DT)와 정의(Definition Details - DD) 쌍들의 영역(Description List - DL)
                    - dl은 dt와 dd 만 포함
                13. p
                    - 문단을 설정
                14. hr
                    - 문단의 분리
                    - 수평선
                15. pre
                    - html 에디터에서 작성한 대로 화면에 표시. (들여쓰기, 공백, 줄바꿈)
                16. blockquote
                    - 일반적인 인용문을 설정
                17. figure, figcaption
                    - 이미지나 삽화, 도표의 설명을 같이 표시할때 사용. 이미지나 삽화, 도표와 설명(figcaption)을 그룹화(figure)
                    - figure > figcaption

            <인라인(display: inline) 요소>
                1. a
                    - 외부 링크
                    - 같은 페이지 이동(# + id)
                2. abbr
                    - 약어
                3. b
                    - bold 효과
                4. mark
                    - 형광펜 효과
                5. em
                    - 의미 강조
                    - 이탤릭체
                6. strong
                    - 의미의 중요성
                    - bold 효과
                7. i
                    - 아이콘이나 특수기호 구분하기위해 사용
                    - 이탤릭체
                8. dfn
                    - 용어 정의할 때
                9. cite
                    - 창작물에 대한 참조
                10. q
                    - 짧은 인용문
                11. u
                    - 밑줄 효과
                12. code
                    - 컴퓨터 코드 범위 설정
                    - 모노스페이스체(공백및 글씨 너비가 모두 동일-일반적인 IDE 처럼) 효과
                13. KBD
                    - 키보드 입력 명시 설정
                    - 모노스페이스 효과
                14. sup, sub
                    - sup: 위첨자
                    - sub: 아래첨자
                15. time
                    - 날짜나 시간을 나타냄
                16. span
                    - div와 비슷한 inline 요소
                17. br
                    - 줄바꿈
                    - 문단 사이의 간격을 만들어내는 방식으로 사용하면 안됨.
                18. del
                    - 삭제된 텍스트 표시
                    - 가운데 줄긋기 효과
                19. ins
                    - 새로 추가된 텍스트 표시
                    - 밑줄 효과

            <멀티미디어 요소>
                1. img
                    - 이미지 삽입
                    - src, alt 필수
                    - srcset : 반응형 사이즈에 맞는 이미지 후보들. 쉼표로 구분, 이미지가 낮은것부터 기록 width 속성과는 다르게 브라우저의 크기에 이미지가 변경된다. 단위는 w(너비), x(배수)
                        ex) srcset="이미지주소 최소크기(w|x), 이미지주소 최소크기(w|x)..."
                    - sizes : 최적화 출력 크기, 조건에 부합할때, 최적화 크기의 이미지 출력, 쉼표로 구분
                        ex) sizes="(조건) 크기" => 조건에 맞을때 크기에 맞는 srcset의 이미지 출력
                2. audio
                    - autoplay, loop, muted, controls
                3. video
                    - autoplay, loop, muted, controls, poster

            <내장 컨텐츠 요소>
                1. iframe
            
            <스크립트 컨텐츠 요소>
                1. canvas
                    - Canvas API, WebGL API 를 사용하여 그래픽이나 애니메이션을 랜더링.
                2. script
                    - defer : body 내용을 먼저 읽고 js 실행 src 속성 필수
                3. noscript
                    - script가 실행되지 못하는 환경일때 수행

            <표 컨텐츠>
                1. table
                    - display: table
                    - border-collapse: collapse => 테이블 사이사이 공간 없애기
                2. tr
                    - table row
                3. th
                    - table header
                4. td
                    - table data
                5. caption
                    - 테이블(표)의 제목
                6. colgroup, col
                    - col > span : span의 갯수만큼 col 동기화
                7. thead, tbody, tfoot
                    - 화면에는 영향이 없고, html에서 구분하기 위함

            <양식 컨텐츠>
                1. form
                    - 서버에 정보를 제출하기위한 범위
                    - autocomplete, novalidate, target
                2. input
                    - 입력받는 데이터 양식
                    - form
                    - type.file multiple => 여러 파일 가능
                    - type.image => submit 으로도 사용가능
                    - placeholder => hint
                3. label
                    - for 참조할 라벨가능 요소(보통 input) 또는 label에 참조할 태그(보통 input) 포함
                4. button
                    - input.button, input.reset=type.reset, input.submit=type.submit 과 동일
                5. textarea
                6. fieldset, legend
                    - fieldset => 여러개의 양식을 그룹화
                    - legend => 제목 양식
                7. select
                8. datalist
                    - 자동완성 가능한 select
                    - input의 list와 datalist의 id 가 동일하면 입력 가능한 select가 만들어짐
                9. optgroup
                    - option 리스트를 그룹화
                10. option
                    - select, datalist의 list들
                11. progress
                    - 로딩바

            <Html 전역속성>
                1. class
                    - 별명
                2. id
                    - 주민등록번호
                3. style
                    - 외모
                4. title
                    - 툴팁
                5. lang
                    - 요소의 언어
                6. data-*
                    - 사용자 정의 데이터 속성을 지정.
                    - 해당 태그에 저장하는 사용자 임의 데이터
                    - html::data-my-name="###" Javascript::element.dataset.myName
                    - 태그에서는 하이픈(-) 부분은 Javascript 에서는 카멜 표기법으로
                7. draggable
                8. hidden
                9. tabindex
                    - 대화형 컨텐츠 탭키로 포커스 하는 순서
                    - 비대화형 컨텐츠는 '0'으로 포커스 부여 가능
                    - '-1'이면 포커스 순서에서 제외
                10. 주석
                11. 특수기호