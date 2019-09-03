---
layout: post
title:  "Github Page와 Jekyll을 이용해 블로그 작성하기 01"
date: 2018-12-31
description: Print Hello World
comments: true
categories: 
- Developments
tags: 
- jekyll
---

## 1. Github Page Repository 생성

깃헙 페이지를 위한 리파지토리를 생성시에는 한가지 규칙이 있다. 프로젝트 네임을 깃헙 사용자의 'username.github.io'로 작성해야 한다. 예를 들어 내 계정명이 woongbinni라고 했을 때, 프로젝트 명은 'woongbinni.github.io'로 해야한다는 것, 이 규칙을 따르지 않을 경우 깃헙 페이지는 동작하지 않는다. 

깃헙의 경우 월 7$의 이용료를 내면 Private 리파지토리를 이용할 수 있지만, 아직까지 내용을 비공개해야할 만한 것도 없기에, 우선 public으로 시작. README.md는 굳이 만들어 줄 필요가 없어서 만들지 않았다.

## 2. Hello World 찍어보기

```bash
# Repository Clone
$ git clone https://github.com/username/username.github.io

# 해당 프로젝트로 이동
$ cd username.github.io

# index.html에 Hello World 작성
$ echo "Hello World" > index.html

# Github에 push
$ git add --all
$ git commit -m "Initial commit"
$ git push -u origin master
```

위의 과정을 거친 후에 브라우저에서 http://username.github.io 를 접근하면 페이지에 'Hello World'가 출력된 것을 확인할 수 있다.

Push 후에 github 내부에서 페이지의 deploy를 위해 나름의 프리컴파일 과정을 거치는 것인지,Hello World 화면을 보는데 어느정도의 시간이 걸리는데, 나중에 포스팅이 많아지면, 페이지가 뜨는데 시간이 더 걸리진 않는건지..
