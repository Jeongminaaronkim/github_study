# GIT 초기 설정

커밋 작성자 설정

```bash
# 명령을 시키고자 하는 주체
# git아, 전역 설정중, 유저의 email을 설정할 거야.
$ git config --global user.email jeongminaaronkim@gmail.com
# git아, 전역 설정중, 유저의 name을 설정할 거야.
$ git config --global user.name jeongminaaronkim
```

- 커밋을 작성하는 사람이 누구인지 알아야 하기 때문에



지정된 설정 확인

```bash
# git아 현재 전역에 설정된 설정 목록 보여줘
$ git config --global -l
# $ git config --global -l
```



# Git Basic

## 로컬 저장소 설정

```bash
$ git init
```

- 폴더에 git 저장소를 초기화하면,
  - .git이라는 숨김 폴더가 생기고
  - bash에는 (master)라는 표기가 생성된다.

- 주의사항
  - .git 폴더를 직접적으로 수정하는 일은 없을 것이다.
  - 이미 git으로 관리하고있는 bash창에 master가 표기되어있는 폴더 내에서는 절대 git init 하지 말 것



## status

```bash
# git아 너가 관리중인 폴더의 상태 보여줘
$ git status
```



## add

```bash
$ git add 파일명
$ git add . # 현재 디렉토리 내 모든 파일
$ git add a.txt # 특정 파일 
$ git add directory_name/ # 특정 폴더가 가진 모든 파일
```

- working directory 상태의 파일을 staging area 상태로 변경
- 커밋을 위한 파일 및 폴더들을 추가하는 명령어



## commit

```bash
# git아, commit 할건데 -메세지는 "이걸로 해줘"
$ git commit -m "commit message"
# git commit -m "210624created CLI.md"
```

- 커밋을 통해 하나의 버전으로 기록됨

- 커밋 메세지는 현재 변경사항들을 잘 나타낼 수 있도록 작성하는 것을 권장

- 커밋 목록은 git log를 통해서 확인할 수 있음

  ```bash
  $ git log --oneline
  ```

  

