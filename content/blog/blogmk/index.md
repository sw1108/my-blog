---
layout: post
title: 블로그 만들기
image: img/gatsby-logo.png
author: CS-W
date: 2020-03-26
tags: 
  - Develope
---

Don't say I did my work very hard, just do well

---

# gatsby를 이용하여 블로그 만드는 법
<br/>

## 템플릿 클론
<br/>

해당 홈페이지에 많은 템플릿들을 확인할 수 있다.  
[https://www.gatsbyjs.org/showcase/?filters[0]=Featured](https://www.gatsbyjs.org/showcase/?filters%5B0%5D=Featured)

원하는 템플릿을 선택하여 다운로드<br/>
[https://github.com/tryghost/gatsby-starter-ghost](https://github.com/tryghost/gatsby-starter-ghost)

```bash
npm install -g Gatsby-cli
git clone https://github.com/tryghost/gatsby-starter-ghost blog
cd blog
npm i
rm -rf .git
git init
git add .
git commit -m "Init project"
``` 
```bash
git remote add origin git@github.com:suites/blog.git
git push -u origin master
npm run start
http://localhost:8000/
http://localhost:8000/___graphql
```
<br/>

## 첫 게시글 작성
content/blogmk.md
```md
---
layout: post
title: 블로그 만들기
image: img/gatsby-logo.png
author: CS-W
date: 2020-03-26
tags: 
  - Develope

### 블로그 만들기
만들면 됩니다.
- 게시글
- 작성하듯이
- 작성하면 됩니다.
```
## netlify에 블로그 배포
이제 드디어 대망의 배포를 진행해볼 차례다. 아래의 주소로 가서 가입을 진행한다.
[https://www.netlify.com/](https://www.netlify.com/)

###### 1번
![](img/blogmk1.PNG)
로그인 후 New site from Git 클릭
###### 2번
![](img/blogmk2.PNG)
GitHub 클릭
###### 3번
![](img/blogmk3.PNG)
블로그를 만들 저장소 클릭
저는 sw1108/blog 입니다.
###### 4번 
![](img/blogmk4.PNG)
Deploy site 클릭
###### 5번
![](img/blogmk5.PNG)
Site deploy in progress 상태이다. <br/>
1분에서 5분정도 기다리면 site에 접속할 수 있다.
###### 6번
![](img/blogmk6.PNG)
사이트 이름 변경을 한다.
![](img/blogmk7.PNG)
site 이름 변경 저는 csworld로 설정하였습니다.
## 🐣 완성 🐣
[https://csworld.netlify.com/](https://csworld.netlify.com/)로 접속하여 확인하기