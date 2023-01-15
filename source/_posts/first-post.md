---
title: Set up My Hexo Blog
date: 2022-11-23 15:54:06
tags:
cover: false
---

## Install Hexo and setting

Here are command for creating my hexo blog:
``` bash
npm install -g hexo-cli
hexo -v # just check hexo's version
hexo init robincpc.github.io    # initialize hexo blog's folder
cd robincpc.github.io
npm install
hexo server
vim _config.yml
```

## Update config file
Some parts I changed in "\_config.yml"
``` yaml
# Site
title: robincpc's note
subtitle: ''
description: 'robincpc"s personal blog'
keywords:
author: Robin Chen
language: en
timezone: 'Asia/Taipei'

# URL
## Set your site url here. For example, if you use GitHub Page, set url as 'https://username.github.io/project'
url: http://robincpc.github.io/


# Deployment
## Docs: https://hexo.io/docs/one-command-deployment
deploy:
  type: 'git'
  repo: https://github.com/RobinCPC/robincpc.github.io.git
  branch: main
```

Clean up
``` bash
hexo generate --watch
hexo new first-post
vim source/_posts/first-post.md # edit your first post
rm source/_posts/hello-world.md # delete demo post
hexo clean
```

## Create a repo on you github for your Hexo blog

``` bash
npm install hexo-deployer-git --save
hexo deploy
```
