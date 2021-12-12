---
layout: post
title:  "Git Branch"
date:   2021-11-30
description: Git의 Branch / Branch 생성 / Branch 전환 / Branch 병합 / Branch 삭제
---

## Git의 Branch
<img src="/assets/img/git branch.png"><img>
<br>
Commit을 기준으로 구분된 파일을 분기로 나누어 새로운 commit을 만들 수 있는 가지, 가지들의 모임을 브랜치(Branch)라고 한다.
<br>
코드의 흐름을 분산시켜 더욱 효율적인 개발 가능!
<br>
<br>

### Branch 생성
#### git branch <branch 이름>을 통해 branch 생성
{%- highlight ruby -%}
user $ git branch <branch_name>
{%- endhighlight -%}
<br>
<br>

### Branch 전환
#### 현재 작업중인 branch를 전환
{%- highlight ruby -%}
user $ git checkout <branch_name>
{%- endhighlight -%}
<br>
<br>

### Branch 병합
#### 현재 작업중인 branch를 원하는 branch에 병합
{%- highlight ruby -%}
user $ git merge <branch_name>
{%- endhighlight -%}
<br>
<br>

### Branch 삭제
#### git branch -d <branch 이름>을 통해 branch 삭제
{%- highlight ruby -%}
user $ git branch -d <branch_name>
{%- endhighlight -%}
