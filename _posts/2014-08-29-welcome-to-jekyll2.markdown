---
layout: post
title:  "Ubuntu install"
date:   2016-02-28 14:34:25
categories: jekyll update
tags: featured
image: /assets/article_images/2014-08-29-welcome-to-jekyll/desktop.jpg
---
### vmware workstaion pro 설치
 - workstations 12 pro trial 설치 후에는 serial key를 넣어야 하는데 이건 인터넷에 치면 나온다.
 - 설치할때 바로 iso 이미지로 시작하지 말고 없는 걸로 한다음에 하드웨어 설정에서 cd-rom 에 iso 파일을 넣어 주자. 그래야 설치할 때 한글로 하기 편하다.

### 우분투 언어
 - 우분투를 설치할 때 한글로 해서 나중에 영어로 바꾸는게 키보드 설정에 훨씬 편하다. hangul이 없을 때도 있다.

### vmware tools 설치 방법
 - 언어 설정을 끝내고 나면 vmware tools를 설치해야하는데 이건 https://www.youtube.com/watch?v=0U8mnEg7nEw 동영상 참고 

### 우분투 설치 직후 설치할 것(zsh git-core vim ruby rbenv)

 - 우분투를 설치한 직후에는 sudo apt-get install git-core vim zsh 부터 하자
 - 우분투에 oh my zsh 설치하는 방법은 https://gist.github.com/tsabat/1498393 참고
 - ruby를 까는 것은 조심해서 해야한다. .zshrc 파일로 경로 바꾸는 것 잊지말고 다음 사이트를 참고할 것 https://cbednarski.com/articles/installing-ruby/
 - 이건 확실하진 않지만 그 외 하드웨어적인 세팅을 하면 성능이 향상된다고 한다. http://programmingsummaries.tistory.com/301 참고할 것
 - 

### jekyll
 - ~/.gemrc 에다가는 위에 페이지에서 하라는 대로 하기
 - gem install bundle 을 한다. bundle 은 gem 패키지 관리자이다.
 - ~/Gemfile 을 만든다.
 - source 'https://rubygems.org' gem 'jekyll' gem 'github-pages'
### Git global config and time caching

 - https://help.github.com/articles/which-remote-url-should-i-use/ 참고할 것.
 -

### 최초의 git init  후에 풀하기
 - 첫번째 방법은 아예 깨끗한 데에 디렉터리 통쨰로 받아오는 방법 이떈 upstream 이 자동으로 설정된다.
 - 두번째 방법은 git fetch 를 한 후에 git merge origin/master를 하고 git branch --set-upstream-to=origin/master master 이라고 하면 된다.
 - master branch 가 없다는 에러는 아마 init을 하고 나면 master branch 조차 없다고 인식해서 인듯 함. 
 - git clone 으로 받은 후에도 로컬 디렉터리 이름은 변경 가능


