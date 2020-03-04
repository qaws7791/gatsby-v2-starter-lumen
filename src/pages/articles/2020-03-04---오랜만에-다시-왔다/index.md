---
title: 오랜만에 다시 왔다
date: "2020-03-04T23:22:37.121Z"
layout: post
draft: false
path: "/posts/오랜만에-다시-왔다/"
category: "잡글"
tags:
  - "Handwriting"
description: "리액트 공부하다가 오랜만에 다시 옴"
---

리액트 공부하다가 오랜만에 다시 옴.
리액트를 공부하니 gastby를 다룰 수 있다.
gastby의 router를 아직 모르겠다.

└── src
    ├── assets
    │   ├── fonts
    │   │   └── fontello-771c82e0
    │   │       ├── css
    │   │       └── font
    │   └── scss
    │       ├── base
    │       ├── mixins
    │       └── pages
    ├── components
    │   ├── CategoryTemplateDetails // ./category/~~ 카테고리 상세보기
    │   ├── Disqus // 댓글
    │   ├── Links // 사이드바 의 메뉴 밑 링크들 
    │   ├── Menu //사이드바의 메뉴들 게시글, 태그, 나에 대해서 등
    │   ├── PageTemplateDetails //about ,contact 등 페이지 상세보기 ./~~
    │   ├── Post //게시글 탭의 포스트 한 개 
    │   ├── PostTemplateDetails // 포스트 상세보기 /posts/~~
    │   ├── Sidebar // menu, links 포함
    │   └── TagTemplateDetails //  ./tags/~~
    ├── layouts
    ├── pages  //글 내용들
    │   ├── articles // posts/~~ 의 게시글
    │   └── pages // ./about, ./contact 등 page
    └── templates


gatsby-config에서 설정을 하고 
gatsby-node에서 data를 gatsby-source-filesystem 플러그인을 이용해 마크다운 파일 폴더를 읽고 마크다운 파일을 gatsby-transformer-remark 플러그인을 이용해 html로 변환하여 data.allMarkdownRemark.edges 데이터를 만들어 createpage액션을 이용해 페이지를 만든다
