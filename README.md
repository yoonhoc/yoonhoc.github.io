# yoonhoc.github.io

이 저장소의 웹사이트는 내려간 상태입니다.

`index.html` 과 이미지 파일을 제거해서 `https://www.yoonhoc.dev` 및
`https://yoonhoc.github.io` 는 더 이상 페이지를 서빙하지 않고 404 를 반환합니다.
404 는 검색엔진이 기존 색인을 지우게 하는 가장 확실한 신호입니다.

## robots.txt 를 두지 않은 이유

`robots.txt` 에 `Disallow: /` 를 넣으면 크롤러가 페이지에 아예 접근하지 못해서
404(또는 noindex)를 **확인하지 못합니다.** 그 결과 이미 색인된 검색 결과가
오히려 오래 남습니다. 내리는 것이 목적이라면 크롤링은 열어두고 404 를
보여주는 편이 빠릅니다.

## CNAME 을 남겨둔 이유

DNS 가 아직 GitHub Pages 를 가리키는 동안 `CNAME` 을 지우면, 다른 GitHub
사용자가 `www.yoonhoc.dev` 를 자기 Pages 사이트에 등록해 이 도메인으로 임의의
페이지를 띄울 수 있습니다(서브도메인 탈취). 도메인 등록처에서 yoonhoc.dev 의
DNS 레코드를 제거한 뒤에 `CNAME` 도 함께 지우는 것이 안전합니다.
