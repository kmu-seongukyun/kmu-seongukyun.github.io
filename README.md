## Github Repo를 Webpage로!  

## Git Blog Build 과정  

- Repository 생성    
- Local-Remote Repository 연동
- 예시 문서 작성 후 원격 저장소 반영 시도
- Personal Access Token(PAT) 생성 후 원격 저장소 반영 재시도
- Jekyll 설치
- Theme 적용 (처음부터 다시 시작..)
- 파일 내용 변경
- navigation bar 수정
- 사이트 내 배경이미지 변경 및 favicon 추가
- CSS 수정
- Post 작성
- Google Analytics 기능 추가
- 댓글 기능 추가(Disqus)

### 1. Repository 생성  
Git 설치 이후, Github 계정에 kmu-seongukyun.github.io 이름의 Repository를 생성했습니다.  

### 2. Local-Remote Repository 연동  
Git CMD에서 `git clone <repo_name> <path>` 명령어를 통해 Remote Repository의 주소를 복사하여 Local-Remote Repository를 연동했습니다.

### 3. 예시 문서 작성 후 원격 저장소 반영 시도
VS code를 이용해 예시 파일(index.html) 작성한 후,   
Git CMD에서 git status, git add, git commit, git branch, git push 명령어를 이용해 원격 저장소에 반영하려 했지만 실패했습니다.   

### 4. Personal Access Token(PAT) 생성 후 원격 저장소 반영 재시도
github의 Setting에 들어가 Developer settings, Personal access tokens, Generate new token을 클릭 후 Note(토큰 메모), Expiration(유효기간), Scope(권한 범위) 결정하여 PAT를 생성했습니다.   
이후 Password에 PAT을 입력하여 git push를 해보니 원격 저장소에 반영할 수 있었습니다.  
kmu-seongukyun.github.io 주소로 접속해보니 이전에 입력했던 HTML 문서(index.html)가 잘 보이는 것을 확인 할 수 있었습니다.

### 5. Jekyll 설치  
Window를 이용해 진행했기에, Jekyll을 설치하기 전에 https://rubyinstaller.org/downloads/ 다음과 같은 사이트 접속하여 Ruby와 Devkit을 설치했습니다.  
이후 `gem install jekyll bundler` 명령어를 이용해 Jekyll을 설치했습니다.   
( Jekyll이 정상적으로 설치되어 있는지 확인하기 위해 `jekyll -v` 명령어를 이용했습니다. )  
이후 현재 디렉토리(Git Blog 디렉토리)에 `jekyll new . -- force` 명령어를 통해 Jekyll 설치를 완료했습니다.    
`(bundle exec) jekyll serve`명령어로 Jekyll를 실행하여 기본 테마로 된 Jekyll 사이트가 생성됨을 확인할 수 있었습니다.   

### 6. Theme 적용(처음부터 다시 시작..) 
기본테마가 너무 밋밋했기에 새로운 태마를 아래의 두가지 사이트를 이용해 찾아보았습니다.    
http://jekyllthemes.org/, https://jekyllthemes.io/free    
다양한 테마를 찾아보며 나에게 맞는(?) 테마를 발견하여 테마를 적용하기 위한 방법을 알아보던 도중 ppt의 조금 더 쉽게... 부분을 발견하게 되었습니다.  
결국 기존의 생성했던 repository를 삭제하고, 원하는 테마의 원격 저장소를 나의 원격 저장소로 fork받아 온 후 해당 저장소의 이름을 kmu-seongukyun.github.io로 변경하였습니다. 그리고 나서 git clone을 통해 해당 저장소를 받아왔습니다.  

### 7. 파일 내용 변경 
모든 파일을 하나하나 들어가보며 대부분의 블로그 속성을 관리하는 _config.yml부터 시작해서 index.html, _includes 폴더 내의 header.html 등 다양한 파일의 내용들을 제 블로그의 컨셉에 맞게 수정했습니다.

### 8. navigation bar 수정
Home과 Github 두개의 nav를 생성하여 Home을 누르게 되면 index.html에 연결되어 있어 홈페이지의 초기화면으로 돌아가도록 설정했으며, Github를 누르게 되면 새 창이 띄워지며 실제 제 Github가 띄워지도록 했습니다.

### 9. 사이트 내 배경이미지 변경 및 favicon 추가
제 블로그의 컨셉에 맞게 수정하기 위해 assets/img 폴더 내애 기존에 있었던 이미지들을 삭제하고 새롭게 다운로드한 이미지로 대체하여 사이트의 배경사진을 변경했습니다.    
favicon 또한 원하는 이미지를 찾아 header.html 부분에 코드를 추가해주었습니다.

### 10. CSS 수정
글자색상, 글자를 마우스로 드래그했을때 나타내는 색상, footer부분의 로고 색상까지 제 블로그 컨셉에 맞게 수정했습니다.   

### 11. Post 작성
_posts 폴더에 특강에서 다뤄줬던 내용을 주제로 post를 작성했습니다.YYYY-MM-DD-TITLE.md 형태로 새로운 문서를 생성하였으며 Markdown 형식으로 내용을 작성했습니다.   
( Post 초안 작성은 이때 이루어졌지만, Post에 변경할 사항이 생기면 이후의 Build 과정에서도 중간중간 수정하며 깃에 반영했습니다. )

### 12. Google Analytics 기능 추가
수업시간에 다루어지지 않은 기능인 Google Analytics을 추가하기 위해 구글링을 이용했습니다.    
Githubpage와 Google Analytics 연동하는 과정을 Post로 작성했습니다.  

### 13. 댓글 기능 추가(Disqus) 
댓글 기능을 추가하기 위해 Disqus에 가입 및 세팅을 진행했습니다.   
이후 _config.yml에 key-vale를 추가했으며, disqus 홈페이지에서 Universal Code를 복사한 후, _layouts/post.html에 복사한 코드를 붙여넣고 강의자료를 참고해 일부 코드를 추가했습니다.  
실제 post의 댓글 기능을 추가하기 위해 각 post마다 comments: True 설정을 추가했습니다.  

#### 참고
위에서 설명한 대부분의 Git Blog Build 과정은 VS Code를 이용해 진행했으며,   
VS code 내의 터미널에서 git add, git commit, git push 명령어를 이용해 변화과정을 Github에 지속적으로 연동시켰습니다.

