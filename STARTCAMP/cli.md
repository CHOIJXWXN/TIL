# CLI



## GUI vs CLI

1. GUI (그래픽 유저 인터페이스)
   1. 그래픽을 통해서 사용자와 컴퓨터가 상호 작용하는 방식
2. CLI (커맨드 라인 인터페이스)
   1. 터미널을 통해 사용자와 컴퓨터가 상호 작용하는 방식



## CLI 사용 이유

New 라는 폴더를 만들고자 한다면,

1. GUI에서는 : 우클릭 -> 새로 만들기 -> 폴더 -> New

2. CLI에서는 : mkdir New (New라는 폴더 만들기)

   ​				   mv markdown.md New/ (New라는 폴더에 markdown.md 파일 옮기기)



## 작업 위치 (경로)

### 루트 디렉토리(/)

* Windows의 경우 C 드라이브

### 홈 디렉토리 (~)

* Windows의 경우 C/Users/Account_name

#### 상대경로

* `./` : 현재 작업하고 있는 폴더
* `../` : 현재 작업하고 있는 폴더의 상위 폴더

TIP : `cmd + l` : 화면 정리



## 명령어

`cd 폴더명` 

* 현재 작업 중인 디렉토리를 변경하는 명령어
* change directory

```bash
$ cd
-> 홈 디렉토리로 이동

$ cd folder # tab으로 자동완성

$ cd ..
-> 상위 폴더로 이동
```



`ls`

* list segments
* 현재 작업 중인 디렉토리의 폴더/파일명을 보여주는 명령어

```bash
#	기본 사용
$ ls

# 숨김 파일까지 모두
$ ls -a

# 상세정보까지
$ ls -l

# 동시 사용
$ ls -a -l
```



`mkdir`

* make directory
* 폴더를 생성하는 명령어

```bash
# folder, folder1 동시 생성
$ mkdir folder folder1
```

* 폴더 이름 사이에 공백을 넣고 싶다면 따옴표로 묶어서 입력

```bash
$ mkdir "This is a folder name"
```



`touch`

* 파일을 생성하는 명령어
* 폴더 생성과 생성 방법 동일
* 숨김 파일 : `.`을 파일명 앞에 추가

```bash
$ touch test.txt
```



`start` or `open` (Windows / Mac)

* 폴더 / 파일을 여는 명령어

```bash
$ open test.txt
```



`rm`

* remove
* GUI는 휴지통으로 보내지만 CLI는 영구삭제
* `-r` : recursive (폴더 삭제 시 필요)

```bash
$ rm test.txt

$ rm -r folder/
```



`mv`

* move

```bash
$ mv test.txt folder/
-> test.txt파일을 folder 폴더로 이동
-> folder 폴더가 없다면 test.txt의 이름이 folder로 변경
```

