# Git 다운로드

### 업로드 후 Clone

---

#### 1. 초기 프로젝트 다운로드

- clone은 초기에 처음 프로젝트를 다운로드 할때 clone명령어를 사용한다.

git clone http:// 프로젝트 주소



#### 2. 업데이트 (pull, merge)

- pull은 기존에 clone해서 받은 프로젝트를 업데이트 해서 변경점을 merge한다.

git pull origin master

- fetch는 업데이트된 소스를 가져올뿐 merge를 하지않는다.

git fetch origin master