# git

## git의 장점
<p>
1. 빠른속도

2.단순한 디자인

3.비선형적 개발지원 
<br><font color = "skyblue">-- 수천개의 브랜치를 병행할 수 있음</font>

4.완전 분산형 시스템

5.리눅스와 같은 거대한 프로젝트도 속도 저하의 문제없이 관리할 수 있는 시스템
</p>

```
@git 명령어

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest (master)
$ mkdir MathTool

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest (master)
$ ls
MathTool/  README.md

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest (master)
$ cd MathTool/

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ git init
Initialized empty Git repository in C:/gitTest/MathTool/.git/

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ ls -al
total 4
drwxr-xr-x 1 1004_ 197609 0 Jan 30 18:28 ./
drwxr-xr-x 1 1004_ 197609 0 Jan 30 18:27 ../
drwxr-xr-x 1 1004_ 197609 0 Jan 30 18:28 .git/

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ cd .git

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool/.git (GIT_DIR!)
$ ls - al
ls: cannot access '-': No such file or directory
ls: cannot access 'al': No such file or directory

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool/.git (GIT_DIR!)
$ ls -al
total 11
drwxr-xr-x 1 1004_ 197609   0 Jan 30 18:28 ./
drwxr-xr-x 1 1004_ 197609   0 Jan 30 18:28 ../
-rw-r--r-- 1 1004_ 197609  23 Jan 30 18:28 HEAD
-rw-r--r-- 1 1004_ 197609 130 Jan 30 18:28 config
-rw-r--r-- 1 1004_ 197609  73 Jan 30 18:28 description
drwxr-xr-x 1 1004_ 197609   0 Jan 30 18:28 hooks/
drwxr-xr-x 1 1004_ 197609   0 Jan 30 18:28 info/
drwxr-xr-x 1 1004_ 197609   0 Jan 30 18:28 objects/
drwxr-xr-x 1 1004_ 197609   0 Jan 30 18:28 refs/

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool/.git (GIT_DIR!)
$ cd ..

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ ls -al
total 5
drwxr-xr-x 1 1004_ 197609  0 Jan 30 18:39 ./
drwxr-xr-x 1 1004_ 197609  0 Jan 30 18:27 ../
drwxr-xr-x 1 1004_ 197609  0 Jan 30 18:28 .git/
-rw-r--r-- 1 1004_ 197609 68 Jan 30 18:39 calculator.py

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ git config user.name "gitTest"

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ git config user.email "1004_sunah@naver.com"

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ git commit -m "gitTest_day_1_1"
On branch master

Initial commit

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        calculator.py

nothing added to commit but untracked files present (use "git add" to track)

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ git add calculator.py

1004_@DESKTOP-UIK0UTK MINGW64 /c/gitTest/MathTool (master)
$ git commit -m "gitTest_day_1_1"
[master (root-commit) 469b235] gitTest_day_1_1
 1 file changed, 4 insertions(+)
 create mode 100644 calculator.py
```
* mkdir : 디렉토리 생성
* ls : 디렉토리 및 파일 출력
* cd : 작업위치 변경 (디렉토리로 이동)
* git init : 저장소(repository) 생성
<br>
<font color = "orangered"> 프로젝트 디렉토리의 각 버전이 담기는 저장소</font>
* ls -al : 디렉토리의 내용을 알고싶을때 사용
```
@ commit시 작성자 알리기
1. 처음으로 커밋을 하기 전 사용자의 이름과 이메일 주소를 설정
2. 커밋 메세지 남기기(옵션-m)
3. 커밋할 파일 git add로 남기기

* git config user.name "커밋시 작성자 이름"
* git config user.email "커밋시 작성자 이메일"
* git add 파일이름 : 커밋할 파일 이름 
* git commit -m "커밋메세지" : 옵션-m 변경사항 메세지 
```