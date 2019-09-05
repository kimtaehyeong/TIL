# Git

> Git은 분산버전관리시스템(DVCS)이다.
>
> * 참고자료
>   * [GIt 입문자](https://backlog.com/git-tutorial/kr)
>   * [Pro Git](https://git-scm.com/book/ko/v2)

## 설정

### 1. author 설정

```bash
$ git config --global user.name {사용자이름}
$ git config --global user.email {사용자이메일}
```

* `commit` 시 이력을 남기는 작성자(author) 정보를 설정한다.

* 설정 정보를 확인하려면, 아래의 명령어를 입력한다.

  ```bash
  $git config --global --list
  ```

  

## 기초 명령어(로컬 저장소 활용)

1. 로컬 저장소 초기화

   ```bash
   $ git init
   Initialized empty Git repository in C:/Users/multicampus/Desktop/새 폴더/.git/
   multicampus@M16034 MINGW64 ~/Desktop/새 폴더 (master)
   ```

   * `.git/` 폴더가 생성되며, git에 대한 모든 정보가 해당 폴더에 기록된다.
   * `bash`에 `(master)` 라는 표기를 통해 현재 저장소로 활용되고 있음을 알 수 있다.

2.  `add`

   ```bash
   $ git add a.txt b.txt
   $ git add .
   $ git add my_folder/
   $ git status
   ```

   * `working tree(directory)`: 현재 작업 공간
   * `INDEX(staging area)`: 커밋 대상 파일 공간
   * `add`명령어를 통해서 `working tree`에서 `staging area` 로 해당 파일 상태를 이동시킨다.

3.  `commit`

   ```bash
   $ git commit -m {커밋메시지}
   ```

   * `commit`을 통해서 현재 시점의 시냅샷을 찍는다.(이력을 남긴다)
   * 현재까지 `commit`이력을 확인하기 위해서는 아래의 명령어를 입력한다.

   ```bash
   $ git log
   ```

4.  `status` **중요!**

   ```bash
   $ git status
   ```

   * `CLI` 에서 항상 지금 상태를 확인하기 위해서 `status`명령어를 입력해보자!!

## 원격 저장소(remote repository) 활용

1. 원격 저장소 설정

   ```bash
   $ git remote add origin {원격저장소url}
   ```

   - `origin` 이라는 이름으로 `url` 을 설정한다.

2. 원격 저장소 확인

   ```bash
   $ git remote -v
   origin https://github.com/kimtaehyeong/TIL.git (fetch)
   origin https://github.com/kimtaehyeong/TIL.git (push)
   ```

3. 원격 저장소 push

   ```bash
   $ git push origin master
   ```

4.  원격 저장소 pull

   ```bash
   $ git pull origin master 
   ```



### 멀캠-집 개인 활용 시나리오

1. 멀캠 도착 햇을 때,

   ```bash
   $ git pull origin master
   ```

2.  멀캠에서 작업 다하고,

   ```bash
   $ git add .
   $ git commit -m {}
   $ git push origin master
   ```

3.  집에 도착해서,

   ```bash
   $ git pull origin master
   ```

4.  집에서 작업 다하고, `push`

   ```bash
   $ git add
   $ git commit -m {}
   $ git push origin master
   ```

   







# 예시

```bash
1. 집에 도착해서 받아오고(pull)
2. 집에서 작업하고 (add-> commit)
3. 집에서 업로드(push)
4. 멀캠에서 받아오고..(push)
5. 멀캠에서 작업하고(add -> commit)
6. 5시 50분에 업로드 (push)
```

## 1. pull을 하지 않고 집에서(다른)

pull을 다시 받고

merge commit 발생하고

push

## 2. pull을 하지 않고 집에서(같은 파일을) 작업 후 push

pull을 다시 받고

merge conflict 발생하고

직접 충돌 해결한 이후 commit 진행 후 push