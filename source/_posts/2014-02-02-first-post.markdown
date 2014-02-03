---
layout: post
title: "first post"
date: 2014-02-02 15:01:14 -0800
comments: true
categories: 
---

##Installing Octopress and Creating a blog post
  it clone git://github.com/imathis/octopress.git octopress
  cd octopress
  ls
  gem install bundler
  bundle install
  rake install
  rake setup_github_pages
  rake generate
  rake deploy
  git add .
  git commit -m 'first commit'
  git push origin source
  rake new_post["first post]\n"
  rake new_post["first post"]
  ls
  cd source
  ls
  cd _posts
  rake "new_post[first post]"
  cd source
  cd _posts
  ls
  subl 2014-02-02-first-post.markdown
  rake generate
  rake deploy
  git add .
  git commit -m "first draft first post"
  git push origin source