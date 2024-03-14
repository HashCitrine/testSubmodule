# testSubmodule
다른 프로젝트와 공통으로 사용하는 부분을 별도의 Git Repository에 저장하고 해당 Repository를 공용으로 이용할 수 있도록 하는 Git 도구(기능)
 
## Submodule 설정
1. Submodule 적용 : `git submodule add <submodule-git-url>`
- `.gitmodules` 파일이 생성되며 submodule에 대한 정보가 저장됨 ([.gitmodule](.gitmodules))
2. submodule 적용된 Repository를 Clone 한 경우
- git clone 시 `--recurse-submodules` 옵션 추가 : `git clone --recurse-submodules <git-url>`
- git clone 이후 : `git submodule init` & `git submodule update`
3. submodule commit pull : `git submodule update --remote <submodule-name>`


## 참조
- [Git 도구 - 서브모듈](https://git-scm.com/book/ko/v2/Git-%EB%8F%84%EA%B5%AC-%EC%84%9C%EB%B8%8C%EB%AA%A8%EB%93%88)
