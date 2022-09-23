# TIL Day 02 
 >- github README - profile
 >- .gitignore
 >- clone, pull
 >- Branch - merge
 >- Git Workflow

## 1. github README
---
- 나의 프로파일을 만드는 공간
- 사용자 이름과 같은 repository를 만든다.
- README.md라는 파일에 프로파일 내용을 넣으면 됨.

## 2. .gitignore
---
- 민감한 특정 파일 혹은 폴더에 대해서 Git이 버전관리를 못하도록 지정
- git add 전에 제외하고 싶은 파일을 .gitignore파일에 작성해야함!!
- [gitignore.io](https://www.toptal.com/developers/gitignore/)를 이용하면 운영체계와 같은 다양한 부분에 대해서도 자동으로 작성해준다.
  
## 3. Clone, Pull
---
### Clone
- push가 로컬에 있는 커밋을 github에 올리는 것이라면, Clone은 github에 있는 커밋 내역을 모두 가져와서, 로컬 저장소를 생성한다.
- 통째로 가져온다!!!   
```bash
git clone <원격 저장소 주소>
```

### Pull
- 원격저장소의 변경사항을 가져와서 로컬저장소를 업데이트
- Commit에 대한 정보만 가져온다.   
```bash
git pull <원격 저장소 주소>
```


## 3. Branch
---
### Branch
![branch](https://hphk-edu.notion.site/image/https%3A%2F%2Fs3-us-west-2.amazonaws.com%2Fsecure.notion-static.com%2Fd6378065-5864-4832-8122-0fde3eb4f6ec%2FUntitled.png?table=block&id=c1098d7b-0ae2-4c68-befe-ece29a09f197&spaceId=f7ab64f0-6613-4035-b609-06b6865d9b61&width=1630&userId=&cache=v2)
- 독립적인 작업 공간
- master branch는 상용을 의미
- 개별/기능별로 브랜치를 만들고 검증을 통해 상용에 merge(병합)한다
- Ex) login / logout / signup
```bash
#브랜치 목록 확인
git branch 브랜치 

#remote 브랜치 목록 확인
git branch -r

#브랜치 생성
git branch <이름>

#브랜치 삭제
git branch -d <이름>
git branch -D <이름> #강제삭제


#브랜치 변경(HEAD이동)
git switch <name>


 ```

 ## 4. Branch Merge
 ---
 >각 브랜치에서 작업이 끝나고 `master`에 반영 = merge

### git merge
```bash
#1 메인 브랜치로 switch
git switch master

#2 merge(name을 master에 붙임)
git merge <name>

#세가지 시나리오 추가 공부필요
```

## 5. Git workflow
fork를 통해 가져오는 방법 학습   

Notion으로 돌아가 사진과 함께 학습진행   