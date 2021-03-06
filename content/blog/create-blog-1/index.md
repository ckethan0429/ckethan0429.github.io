---
title: 개발자 블로그 만들기(1) - Gatsby quick start
date: 2019-12-31
tags:
  - Develop
  - Blog
---



개발자들의 블로그를 만드는 방법에는 여러가지가 있다.

1. 포털에서 제공해주는 블로그
2. Express 같은 CMS 이용
3. 정적 웹사이트 생성기



나는 요새 대세라고 불리는 정적 사이트 생성기를 이용하여 블로그를 개설하기로 하였다.

사실 제일 유명한 생성기는 jekyll이다. 왜냐하면 Github Page에서 jekyll을 제공해주고 있기 때문이다. 그래서 많은 개발자들이 jekyll을 사용하고 있지만, jekyll은 Ruby 언어로 작성이 되어있다. 나는 따로 Ruby를 배우지 않았고, 요즘 react를 공부하고 있기 때문에 gatsby를 이용하기로 한다. github이 페이지를 배포함에 있어서 익숙하지만 나는 netlify를 이용하여 배포를 해볼 생각이다.



> 정리 1. 자바스크립트, reactr 기반의 정적사이트 생성기를 이용하여 블로그 개설
>
> 정리 2. netlify를 이용하여 블로그 배포
>
> 정리 3. [Node](https://nodejs.org/ko/)가 설치되어 있어야함. 설치확인은 터미널에서 `$ node -v`, `$ npm -v` 으로 확인!



[Gatsby 공식문서 - quick start](https://www.gatsbyjs.org/docs/quick-start) 를 이용하면 빠르게 설치할 수 있다. 간단하게 페이지 생성을 어떻게 하는지 맛만 보고, 바로 테마를 적용해보는 것을 추천한다. 이번 포스틍에서는 간단하게 quick start를 이용하여 빠르게 페이지 생성에 대해 알아본다.



1. Gatsby CLI 설치

   `$ npm install -g gatsby-cli`

   

2.  새 사이트 생성

    ` $ npx gatsby new gatsby-site` 

    > - `npx` 를 사용하면 최신 gatsby로 유지하여 사용할 수 있다. 
    > - `npx` 붙이지 않아도 무관.

    

3.  폴더로 진입하여 개발모드로 시작

    `$ cd gatsby-site`

    `$ npm run develop` 혹은 `$ gatsby develop`

    http://localhost:8000 에서 페이지 만든 것을 확인 할 수 있다.

    

4.  배포모드로 시작

    `$ npm run build` 혹은 `$ gatsby build`

    http://localhost:9000 에서 페이지 만든 것을 확인 할 수 있다.

