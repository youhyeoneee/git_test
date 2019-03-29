# git_test

+ how to git pull request ? 

## 1. Fork

+ 타겟 프로젝트의 저장소를 자신의 저장소로 Fork

## 2. clone, remote 설정

+ Fork한 저장소를 로컬에 clone한다.
```
$ git clone 'https://github.com/youhyeoneee/git_test.git'
```

+ 로컬 저장소에 원격 저장소를 추가한다. 

	- 원본 프로젝트 저장소 (직접 추가 필요)
	- fork한 로컬 프로젝트 (clone을 하면 기본적으로 origin이라는 별명으로 추가되어있다.)

```
#원본 프로젝트 저장소를 원격 저장소로 추가
$ git remote add hyeong(별명) https://github.com/DevHyung/git_test

#원격 저장소 설정 현황 확인 
$ git remote -v

hyeong  https://github.com/DevHyung/git_test (fetch)
hyeong  https://github.com/DevHyung/git_test (push)
origin  https://github.com/youhyeoneee/git_test.git (fetch)
origin  https://github.com/youhyeoneee/git_test.git (push)

```

## 3. branch 생성 

+ 자신의 로컬 컴퓨터에서 코드를 추가하는 작업은 branch를 만들어서 진행한다ㅣ 

```
# youhyeon 이라는 이름의 branch를 생성한다.
$ git checkout -b youhyeon
Switched to a new branch 'youhyeon'

# 이제 2개의 브랜치가 존재한다. 
$ git branch
  master
* youhyeon

```