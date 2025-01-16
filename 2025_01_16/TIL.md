# Local

## repository
1. git init을 실행
2. .git 폴더가 숨김 파일로 생성
3. staging에서 commit을 하게되면 local repository에 저장

## work 
내가 작업한 모든건 work 영역이라고 생각한다

## work -> repository
* 내가 work에서 repository로 저장하고 싶은 경우 work, repository를 동기화 하면 비효율적이다.

* work에서 내가 repository에 저장하고 싶은것만 비동기로 올리기 위해서 staging이란 중간 과정을 추가한다.

## staging
* git add를 해주면 지정한 파일이나 폴더를 work -> staging으로 옮긴다.

* 예를 들어 git add .는 현재 위치의 모든 파일을 staging에 올린다.

## repository

* git commit을 할 경우 staging -> repository로 파일을 옮긴다.

# remote repository

## 의미

local repository들이 통신하기 위해서 github 서버에 올리는 원격 repository

## local -> remote repo 연결
git remote add (로컬 이름) (remote repository branch)

## commit

연결된 상태에서 push (로컬 이름) (remote repository branch) 해주면 원격 저장소로 commit 됨

## pull
충돌이 안나야 공동작업이 가능하다. 로컬과 원격 레포를 동기화하기 위해서 원격 레포의 내용을 로컬에 덮어쓰기 하는것

git pull (로컬 이름) (remote repository branch)


## 명령어
* git add . : 현재 위치의 모든 파일을 스테이징으로 옮김
* git commit -m : staging에서 repository로 파일을 옮긴다.
이때 m 뒤에 "~~~"로 메세지를 남길 수 있는데 각 프로젝트의 규칙에 따라 작성할 것
* git add remote: 로컬과 원격을 연결
* git push : 로컬에서 원격으로 커밋
* git commit --amend: 가장 최신의 커밋을 수정
* git pull: 원격에서 로컬로 파일 동기화





