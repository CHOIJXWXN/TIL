# GITHUB



## 회원가입

### 설정 변경

* main 브랜치를 master 브랜치로 기본값 수정



## 원격 저장소와 로컬 저장소 연결

### Repository 생성

* git remote
* git push

### gitignore

* 원격 저장소에도 파일이 있고, 로컬에서 이미 있고, 이미 트래킹 중인 파일을 로컬에서만 더 이상 추적하지 않도록 설정

  ```bash
  $ git update-index --assume-unchanged {file_name}
  ```

* 로컬에 있는 파일 변동 추적 멈춤

* 원격 저장소에 해당 파일이 이미 있다면, 원격 저장소에 push 시 그 파일 삭제

  ```bash
  $ git rm --cached {file_name}
  ```

* 로컬, 원격 저장소 모두 파일 삭제 후 추적 중지

  ```bash
  $ git rm {file_name}
  ```