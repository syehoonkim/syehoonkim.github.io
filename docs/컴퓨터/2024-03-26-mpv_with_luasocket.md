---
title: Luasocket을 mpv.io에서 사용하기
date: 2024-03-26 +09:00
categories: [mpv]
tags:
  [mpv, luasocket]
---
Luasocket을 mpv 내에서 활용하고 싶었다. subprocess로 FFmpeg을 실행하고, 그 progress를 udp로 받아보기 위함이었다.  
그런데 아무리 해도 Luasocket을 mpv에 적용시킬 수가 없어서 각종 시도를 다하던 중, 다음 글을 발견했다.  
[https://github.com/mpv-player/mpv/issues/2009](https://github.com/mpv-player/mpv/issues/2009)  
즉 mpv를 직접 빌드하고 Luasocket을 적용하면 된다는 것이었다. 그래서 직접 빌드해봤더니 정말 되었다.