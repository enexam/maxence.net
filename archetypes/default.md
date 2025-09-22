---
date: '{{ .Date }}'
draft: true
title: '{{ replace .File.ContentBaseName "-" " " | title }}'
tags:
    - tag1
    - tag2
categories:
    - category1
featured: false
rtwt:
    sidePane: true
    sidePaneSticky: true
---
