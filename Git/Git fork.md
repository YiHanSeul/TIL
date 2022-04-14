# Git Workflow

#### 1. 원격저장소가 있는경우 (Shared repository model)

- 원격저장소가 자신도 소유권이 있는 경우

- master에서 개발하는게 아니라 기능별로branch를  만들어서 

  branch에서 push를 하고 pull request를 사용하여 master로 넘어와 merge를 할수 있도록함.

- 병합이 완료가 되면 branch는 삭제함.
- 병합이 완료가 되면 master로 브랜치 전환 
  - git switch master

- 새롭게 merge된 것을 pull해야함
  - git pull origin master
- 다시 repository를 새롭게 다시 다운로드 확인
- 기능 구현 완료하고 merge된 브랜치 삭제
  - git branch -d 브랜치명



#### 2.원격 저장소 권한이 없는 경우 (Fork& Pull model)

- git hub 홈페이지에 들어가서 fork를 해서 내 원격 저장소로 복제한다.

- fork한 자신의 원격저장소의 링크를 clone 한다.

  - git clone http 클론주소

- clone이 되었으면 원본 원격 저장소와 동기화를 한다

  - git remote add upstream http 링크 

  // 원본 원격 저장소에 대한 이름은 upstream을 붙이는게 관례임

- 원격저장소와 동기화가 되었으면 내가 작업할 branch를 생성
  - git branch 브랜치명
- 기능 구현 후 push를 함 master권한이 없기때문에 브랜치명으로 push함
  - git push origin 브랜치명
- git hub 홈페이지로 돌아와 원본 원격저장소로 들어와 Compare&Pull Request를 요청한다. 
  - reviewer : 현재 PR에 대해 코드 리뷰를 진행해 줄 담당자
  - assigness: 현재 PR에 대한 작업을 맡고 있는 담당자