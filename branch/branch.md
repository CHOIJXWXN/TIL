# BRANCH



## git branch 명령어

* 브랜치 `생성, 삭제, 조회` 명령어

```bash
# 브랜치 조회
$ git branch

# 원격 저장소의 브랜치 목록 확인
$	git branch -r

# 브랜치 생성
$ git branch {branch_name}

# 브랜치 삭제
# 병합된 후에 삭제 가능
$ git branch -d {branch_name}
# (주의) 병합되지 않은 브랜치 강제 삭제
$ git branch -D {branch_name}
```



## git switch

* 현재 브랜치에서 다른 브랜치로 `HEAD`를 이동시키는 명령어
* `HEAD`는 현재 브랜치를 가리키는 포인터

```bash
# 다른 브랜치로 이동
$ git switch {branch_name}

# 브랜치를 생성하고 동시에 이동
$ git switch -c {branch_name}
```

* 주의 사항

  git switch 하기 전에 commit 하셨나요?