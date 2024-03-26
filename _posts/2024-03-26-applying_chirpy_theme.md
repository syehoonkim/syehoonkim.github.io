---
title: Chirpy 테마 적용 시 *.min.js 문제
date: 2024-03-26 +09:00
categories: []
tags:
  [테마]
---
처음 Jekyll로 블로그를 만들어보았다. 테마는 흔히 쓰이는 Chirpy를 이용했는데, 문제가 생겼다.  
theme mode 등이 작동하지 않고, ```assets/dist/home.min.js``` 등과 같은 파일이 없다고 메시지가 뜨는 것이었다.  
이에 대한 해결책은 [https://velog.io/@lzlko/github-%EB%B8%94%EB%A1%9C%EA%B7%B8](https://velog.io/@lzlko/github-%EB%B8%94%EB%A1%9C%EA%B7%B8) 의 댓글에서 찾았다.  
바로 ```tools/init```을 실행하면 된다는 것이었다.  
문제는 윈도 상에서는 이를 바로 실행할 수 없다는 것이었다. MSYS2를 쓰면 될지도 모르겠는데, 나는 Windows Subsystem for Linux를 이용했다.  
Ubuntu를 설치 후 node를 설치하고 ```bash tools/init```하자 ```assets/dist/*.min.js```파일들이 만들어졌고, theme mode 변경 등이 정상적으로 작동했다.