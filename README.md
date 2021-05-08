## git init 
```
get init
```
일단 ＂-2“  폴더를 생성하고 git init 명령어를 통하여 git
디렉토리로 만들었다.
git init은 .git 디렉토리를 생성하여 해당 디렉토리를 git  repository로 인식시켜 git 명령어를 활용할 수 있게 해준다

## git config
```
git config user.name minwook

git config user.email nike9900@naver.com

git config --list
```
이후 git config user.name 과 git config user.email을 통해 커밋시 git  log에 기록될 이름과 이메일을 기록하였다. 이후 git config –list를  이용하여 적용이 제대로 되었는지 확인한다.

이후 "-2"폴더에 "markdown.md" 파일을 추가한다.

## git status
```
git status
```
git status 명령어를 사용하여 현재 repository의 변화를 확인한다.
Markdown 파일이 untracked상태임을 알려준다.

## git add
```
git add markdown.md

git status
```
Markdown 파일의 수정했다.
해당 파일이 modified 상태로 되고 다시 git add를 통해 staged 상태로 만들어주었다


## git commit
```
git commit
```
git commit을 통해 staged 상태의 모든 파일들을 commit 시켰다.
commit 메세지는 생략하였다.

## git log
```
git log
```
git log 명령어를 통해 제대로 commit이 되었는가 확인해 보았다.

## git remote && git push
```
git remote add origin https://github.com/kminwook/-2.git

git branch -M main

git push -u origin main
```
git remote 명령어를 통해 원격 레포지토리의 주소를 설정한다.  이후 push명령어를 통해 커밋 데이터가 해당 주소지로 넘어갈  것이다.
git push를 통해 커밋된 데이터를 원격 주소지로 넘겨준다.

## git clone
```
git clone https://github.com/kminwook/-2.git
```
서버에 접속해 해당 레포지토리를 복제하자

## git branch && git checkout
```
git branch name_edit

git checkout name_edit

mv markdown.md markdown_homework.md

git commit -a -m "change markdown_homework.md"
```
Markdown 이라는 제목을
Markdown_homework2로 고쳐보자.

master에 바로 해당 변경을 적용하였다가 오류가 발생할 수도  있으므로 name_edit이라는 새로운 branch를 만들어 이름을 먼저  바꿔보자

git branch 명령어는 새로운 branch를 생성하여 master와는 별개의  변경사항을 저장할 수 있도록 해준다.
git checkout을 branch를 변경해준다.

## git reset --hard
```
git reset --hard 8c1d92f
```
실수로 Marksdown_homework.md로 커밋하였으므로 커밋이전 사항으로  돌아가자
변경한 로그도 삭제시키므로 reset –hard는 되도록 이용하지  말도록 하자

이후 브랜치 다시커밋
```
rm markdown.md

mv markdown_homework.md markdown.homework2.md
```
## git merge
```
git checkout main

git merge name_edit
```
git checkout master를 이용해 master branch로 옮겨가 변경사항을
master branch에 합병시켜주도록 하자.

## info branch(git reset) 
``` 
git branch info

git checkout info

 markdown_homework2.md

 git add markdown_homework2.md
```
Markdown_homework2의 내용을 수정 후 staged상태로 올렸다.

## info2 branch
```
git reset

markdown_homework2.md

git add markdown_homework2.md

git branch info2

git checkout info2

markdown_homework2.md
```
처음에 정보를 잘못 수정해서 해당 파일을 git reset을  이용하여 파일을 초기화하기로 하였다.

내용을 다시 변경하였다.

## git rebase
```
git rebase info
```

이후 info 로부터 다시 패치될 것이므로 main branch의 base
정보를 info branch로 하기로 하였다.

git rebase 명령어를 통하여 main branch의 base 정보를  변경하였다.

## git tag
```
git tag init 8c1d92

git tag b0.0 b0a37b

git tag b0.1 62oad

git tag b0.2 4552957
```
init 이후 버젼을 쉽게 관리하기 위해 git tag 명령어를 활용하여 커밋 해쉬코드에 별명을 붙여주기로 하였다

## git push && pull
```
git push
```
git push을 이용하여 원격서버에 올리고 git pull을 이용하여  원격서버에서 받을 수 있다

## git pull
``` 
git pill
```

|git 명령어|
|------|
|[init](#git-init)
|[config](#git-config)
|[status](#git-status)
|[add](#git-add)
|[commit](#git-commit)
|[log](#git-log)
|[remote](#git-remote--git-push)
|[push](#git-remote--git-push)
|[clone](#git-clone)
|[branch](#git-branch--git-checkout)
|[checkout](#git-branch--git-checkout)|
|[reset --hard](#git-reset---hard)
|[merge](#git-merge)
|[branch](#info-branchgit-reset)
|[rebase](#git-rebase)
|[tag](#git-tag)
|[pull](#git-pull)