---
layout: post
title:  "Git Branch"
date:   2021-11-30
---

## Git의 Branch
<img src="git branch.png"><img>
코드의 흐름을 분산시켜 더욱 효율적인 개발 가능!

### Branc 생성
#### git branch <branch 이름>을 통해 branch 생성
{%- highlight ruby -%}
user $ git branch <branch_name>
{%- endhighlight -%}

### Branch 전환
#### 현재 작업중인 branch를 전환
{%- highlight ruby -%}
user $ git checkout <branch_name>
{%- endhighlight -%}

### Branch 병합
#### 현재 작업중인 branch를 원하는 branch에 병합
{%- highlight ruby -%}
user $ git merge <branch_name>
{%- endhighlight -%}

### Branch 삭제
#### git branch -d <branch 이름>을 통해 branch 삭제
{%- highlight ruby -%}
user $ git branch -d <branch_name>
{%- endhighlight -%}
