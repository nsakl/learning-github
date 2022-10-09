# 6 Week
## 버전 방식 Changes vs snapshots(Git)
## 협업방식 Local, Centralized, Distributed(Git)
### working Directory에서 수정 후 Staging Area에서 점검 후 Commit함(스냅샷 생김)
### Git config: First-time setup
1.  System level: —system option. 모든 사용자,repositories에 영향(administrative)
2.  Global (user)level: —global option. 모든 현재 유저의 repositories 
3.  Local level: —local option. 현재 repository에 대해서만
### 문법
- ex) git config —global user.name “Hong JiMIn”
- 
- **git init** : initialized empty git repository in / .git/ 

- **git status** : 현재 repository가 어떤 status인지 확인

- **git add file_name** : file 추가 , Staging Area에 올라와있기에 Untracked files가 아닌 Changes to be committed에 추가됨

- **git add** 로 인해 추가된 경우 tracked 되기에 파일이 수정된 경우 경고 문구가 나오며 다시 git add를 통해 Staging Area로 올려주어 갱신해야지 수정된 파일로 commit됨

- **git add .** 현재 폴더의 모든 파일을 Staging Area에 올림

- **git rm —cached file_name** : git의 Staging Area에서 제거하여 Untracked filed로 분류됨

- **.gitignore** 라는 파일을 만든 후 포함하고 싶지 않은 파일명을 적을 시 그 파일은 Staging Area로 올라가지 않는다(Untracked에 조차 표시되지 않는다)

- **git commit -m “commit message”

- **git branch** : 현재 브랜치 이름

- **git branch -m 현재 브랜치 바꿀 브랜치  →브랜치 이름 변경
