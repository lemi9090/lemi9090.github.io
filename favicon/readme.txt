만드는 법
1. 파비콘 이미지 정하기.
2. 파비콘 만드는 사이트에서 파비콘 만들기 
  (https://www.favicon-generator.org/)
3. 만들면 zip 파일과 코드가 나옴. 둘 다 저장하기.
4. 깃헙에서 하나 폴더를 만들고 그 안에 또 폴더를 만들어 압축파일을 여기에 해제하기
5. 복사한 코드는 _includes에서 head.html 파일에서 수정해야 함.

6. 어떻게 하나면 복사한 코드는 수 많은 link rel로 이루어져 있는데 
<link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png">
이렇게 저장되어있음. 이걸 압축파일을 해제시킨 폴더 경로로 해야함.
그래서 바꾸면 <link rel="icon" type="image/png" sizes="16x16" href="{{ site.favicon }}/favicon/logo.ico/favicon-16x16.png"> 이렇게 됨.

7. 이걸 <head></head> 사이에 넣어서 마무리하면 됨. 
