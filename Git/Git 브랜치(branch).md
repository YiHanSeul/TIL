# Git Branch

#### 1. branch

![branch](Git 브랜치(branch).assets/화면 캡처 2022-04-14 141708.png)



- branch를 사용하여 버전관리를 할수 있음.
  - branch는 다른 branch의 영향을 미치지 않기 때문에 여러작업을 동시에 진행 할수 있음.



#### 2. branch 목록확인

1. git branch 
   - *master만 기존에 있음



#### 3. branch 생성

1. git branch 브랜치명
2. git branch  명령어 입력후 브랜치 목록 확인



#### 4. 새로만든 브랜치로 이동

1. git switch 브랜치명 

2. git switch -c 브랜치명 (브랜치명 생성과 동시에 이동)

*스위치가 안될경우는 commit을 했는지 반드시 확인해야함. 

commit을 안하고 switch명령어를 사용하게 될경우 switch가 안됨.

![branch switch](Git 브랜치(branch).assets/화면 캡처 2022-04-14 142909.png)





#### 5. 병합

1. git merge 브랜치명 (master브랜치와 브랜치명이랑 합쳐짐)

* merge 할때는 git switch master로 브랜치를 변경후 병합진행



#### 6. 로그확인

1. git log --online -all-graph



#### 7. 브랜치 삭제

- git branch -d  브랜치명 (삭제 병합이 된 브랜치를 삭제함)
- git branch -D 브랜치명 (강제삭제 커밋찍지 않은 브랜치도 강제로 삭제하는 옵션)



#### 8. 이전 버전으로 되돌리기

1. git log 입력하여 원하는 해시값 확인
2. git checkout  해시값