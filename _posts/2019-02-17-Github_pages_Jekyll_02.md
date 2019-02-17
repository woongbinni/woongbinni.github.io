---
layout: post
title:  "Github Page와 Jekyll을 이용해 블로그 작성하기 02"
categories: [Developments]
tags: [jekyll]
---

너무 쉽게 다짐이 깨져버렸다.


매일 조금씩이라도 깃헙에 내 흔적을 남기는 것이 2019년의 목표였는데... 
블로깅을 조금씩 하려고 깃헙 페이지 기반의 블로그를 만드는 작업도 Hello World만 찍고 손 놓은지가 -_-;;

이번엔 깃헙페이지에 jekyll을 적용해보려고 한다.
[Jekyll 공식 홈페이지의 Quick Start](https://jekyllrb.com/docs/)를 참고로... 

### 1. Ruby 개발환경 구축
- MAC 사용자라면 기본적으로 ruby가 MAC에 설치가 되어 있다. 
- Linux나 Windows 사용자라면 [여기](https://www.ruby-lang.org/ko/documentation/installation/)를 참고하자. 
- 추후 시간이 나면 ruby 개발환경 세팅에 대해서도 포스팅해볼 예정

### 2. jekyll, bundler 설치

```bash
$ gem install jekyll bundler 
```

### 3. myblog라는 블로그를 만들 생각이라면..

```bash
$ jekyll new myblog
```

해당 명령어를 통해 블로그 실행에 필요한 jekyll 관련 설정파일과 폴더들이 하위에 생성된다.

### 4. myblog 폴더로 이동해서 블로그 페이지를 띄워본다. 

```bash
$ cd myblog
$ bundle exec jekyll serve
```

브라우저 주소창에 http://localhost:4000를 입력 후, 접근하면 기본적인 블로그가 만들어진 것을 확인할 수 있으며, 
해당 프로젝트를 깃헙에 푸시하면, 깃헙 서비스에서 자동으로 빌드, 블로그를 생성해준다.

포스팅은 '_posts' 폴더 내에 마크다운 포멧으로 작성하면 포스팅한 마크다운 파일들을 깃헙에서 html로 변환해서 보여준다. 

jekyll은 다양한 테마를 제공하고 있으며, 본 블로그는 [basically-basic](https://github.com/mmistakes/jekyll-theme-basically-basic)이라는 테마를 적용하고 있다. 급하게 로고와 메인 이미지 정도만 넣었으며, 짬짬이 기능 수정중이다.