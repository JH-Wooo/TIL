# Git의 시작 

## git이란?

### VCS(Version Control System)

== SCM (Source Code management)
< SCM (Software Configuration Management:형상관리)

***git by Linus Torbalds*** 

* BitKeeper의 이용약관 위반으로 라이센스 제한에 화가 나 2주만에 만든 분산형 버전관리시스템
* 압도적 업계 1위

***Characteristics of git***
* 빠른속도, 단순한 구조
* 분산형 저장소 지원
* 비선형적 개발(수천개의 브랜치) 가능

## Conventional Commits

ref: [커밋컨벤션](https://www.conventionalcommits.org/ko/v1.0.0/)
	1. commit의 제목은 commit을 설명하는 하나의 구나 절로 완성
	2. importanceofcapitalize Importance of Capitalize
	3. prefix 꼭 달기	
		+ feat: 기능 개발 관련
		+ fix: 오류 개선 혹은 버그 패치	
		+ docs: 문서화 작업
		+ test: test 관련
		+ conf: 환경설정 관련
		+ build: 빌드 관련
		+ ci: Continuous Integration 관련
		+ BREAKING CHANGE: 없어진 기능이 있다면 사용
		+ refactor: 코드 리펙토

## commit 할때 기억할 것

+ commit은 동작 가능한 최소단위로 자주 할 것.
+ 해당 작업단위에 수행된 모든 파일 변화가 해당 commit에 포함되어야 한다.
+ 모두가 이해할 수 있는 log를 작성할 것.
+ Open Source Contribution시 영어가 강제되지만, 그렇지 않을 경우 팀 내 사용 언어를 따라 쓸것.
+ 제목은 축약하여 쓰되(40자 이내), 내용은 문장형으로 작성하여 추가설명 할것.
+ 제목과 내용은 한 줄 띄워 분리할 것.
+ 내용은 이 commit의 구성과 의도를 충실히 작성할 것.

## README.md
+ 프로젝트와 Repository를 설명하는 책의 표지와 같은 문서
+ 나와 동료, 이 repo의 사용자를 위한 문서

## .gitignore

.gitignore는 git이 파일을 추적할 때, 어떤 파일이나 폴더 등을 추적하지 않도록 명시하기 위해 작성하며, 해당 문서에 작성된 리스트는 수정사항이 발생해도 git이 무시하게 됩니다. 특정 파일 확장자를 무시하거나 이름에 패턴이 존재하는 경우, 또는 특정 디렉토리 아래의 모든 파일을 무시할 수 있습니다.


## LICENSE

오픈소스 프로젝트에서 가장 중요한 License는 내가 만들 때에도, 배포할 때에도 가장 신경써야 하는 일 중 하나입니다.
가장 많이 사용하는 License는 다음과 같다.

+ MIT Licence
	* MIT에서 만든 라이센스로, 모든 행동에 제약이 없으며, 저작권자는 소프트웨어와 관련한 책임에서 자유롭습니다.
* Apache License 2.0
	* Apache 재단이 만든 라이센스로, 특허원 관련 내용이 포함되어 있습니다.
* GNU General Public LIcense v3.0
	* 가장 많이 알려져있으며, 의무사항(해당 라이센스가 적용된 소스코드 사용시 GPL을 따라야 함)이 존재



warking directory에서 add를 이용해 staging area로 이동 가능 취소도 가능
commit을 입력해 local history에 저장하고 push로 remote서버에 전달 
pull과 fetch를 입력해 가져올수 있다
