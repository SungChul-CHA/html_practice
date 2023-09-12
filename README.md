# html

##### 1. 웹표준

- 시멘틱마크업: 요소의 의미에 맞는 html사용

- 주요브라우저: 크롬(크로미언 렌더링 엔진), edge(크로미언), 삼성인터넷(크로미언), 오페라(크로미언), 사파리(웹킷), 파이어폭스(겟코)
- 브라우저시장 점유율: 크로미언계열 브라우저가 압도적이므로 크롬, 엣지, 모바일크롬, 모바일사파리 위주로 화면테스트</br>https://gs.statcounter.com/browser-market-share/all/south-korea/#monthly-202206-202306
- 크로스브라우징: 주요브라우저에 동일한 화면구현을 위해 css 벤더프리픽스 사용

- 익스플로러는 ie10, ie9, ie8, ie7이 있으며 os별로 다른버전이 설치되며 모두 다른 스펙을 가진 비표준 브라우저
- 2022년 6월 익스플로러 공식 지원 중단으로 익스호환의 시대가 막을 내림(네이버 데스크탑은 익스호환 유지중)

- 결론: 익스플로러 공식 지원 중단으로 크롬, 엣지, 모바일사파리, 삼성인터넷등 주요브라우저에서 지원하는 html5, css3 최신스펙을 대부분 사용가능하며 일부 css는 벤더프리픽스 이용하여 화면 구현
  </br>

#### 2. 웹접근성

- 최소한의 접근성(장애인도 웹사이트의 정보를 인지할 수 있도록)을 지켜 마크업
- 관공서는 접근성인증마크를 취득해야함(장애인 차별 금지법)

#### 3. Entity Code Links

- [W3cub entity code](https://tools.w3cub.com/html-entities)
- [entitycode](https://entitycode.com/)
- [toptal](https://www.toptal.com/designers/htmlarrows/)

#### 4. 파일 연결 경로

- 상대경로: 현재파일을 기준으로 연결할 파일의 위치를 나타내는방식

  - ../(상위폴더) ./(현재폴더,생략), 하위폴더명/파일명.확장자</br>
    `<img src="images/파일명.확장자" alt="">`
    </br>

  - css background:url(../images/파일명.확장자)</br>
    `<a href="ceo.html">ceo</a>`
    </br>

  - 서버경로: 서버 최상위(root)를 기준으로 연결할 파일의 위치를 나타내는 방식
    로컬에서 확인불가
    서버에 올려서 확인하거나 서버환경구축후 확인가능
    주로 백엔드에서 필요에 따라 서버경로로 바꿔서 사용
    /는 서버최상위폴더를 의미함</br>
    `<img src="/images/common/logo.png" alt="tft">`
    </br>

  - 절대경로: 외부서버의 도메인주소를 모두 입력하는 방식 </br>
    `<img src="http://ossamuiux.com/images/logo.png" alt="">`

## 유용한 크롬 익스텐션

- user agent switcher: userAgent변경하여 모바일사이트 접속
- awesome screenshot: 스크롤캡쳐
- svg export: svg 이미지 가져오기
- image downloader: 이미지 가져오기
- openwax: 접근성 테스트
- SVG Viewer Extension for Windows: 윈도우탐색기에서 svg이미지 미리보기, 윈도우 응용프로그램
- React developer Tool: React 프로젝트 확인
- vue devtools: vue 프로젝트 확인
