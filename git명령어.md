# Git 명령어

### 업로드전

---

#### 1. 초기설정

1. git config --global user.name "유저명"
2. git config --global user.email "깃허브 메일"



#### 2. 설정확인

1. git config --global --list



#### 3. 파일만들기

1. touch README.md



#### 4. git ADD- COMMIT

1. git add README.md
2. git status (add가 잘되었는지 상태확인)
3. git commit -m "커밋할 메시지" (add를 한게 없으면 commit을 할수 없음)
4. git log --oneline (git 변경사항 내역 확인)



### 업로드 후

---

#### 1.git hub 홈페이지

1.  새로운 repository를 생성한다.
2.  repository가 생성되면 url을 http로 복사한다.



#### 2. git hub와 git 연결하기

1. git remote add origin 복사한 url (연결 명령어)
2. git remote -v (연결 확인)
3. git remote rm origin (remote명령어를 잘못 입력했을때)



#### 3. 깃 최종 커밋

1. git push origin master

처음 연결을 했을 경우 로그인하라는 창이 뜬다. 로그인하면 정상적으로 업로드 완료

