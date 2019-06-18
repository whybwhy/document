## 읽어볼 것
* [git 원리](https://sjh836.tistory.com/37?category=695128)
* [add, commit, push 취소](https://gmlwjd9405.github.io/2018/05/25/git-add-cancle.html)
* [핸드북](https://rogerdudler.github.io/git-guide/index.ko.html)
* [guide](https://git-scm.com/book/ko/v2)
* [git howto](https://githowto.com/setup)
* [git 용어정리](https://tech.10000lab.xyz/git/important-git-terms.html)
* [git 유용한 팁](https://tech.10000lab.xyz/git/git-tips-you-need.html)
* [git 커밋 메세지 가이드](https://meetup.toast.com/posts/106)

## 사용했던 명령어
<pre>
    git init
    git add .
    git commit -m ''
    git push origin
    
    git push -u origin +master // 강제 push
    
</pre>

<pre>
    git rm -r --cached .

    git reset
    git checkout
    git fetch
</pre>

<pre>
    //git add . 후 아래와 같은 경고 발생
    warning: LF will be replaced by CRLF in 파일명
    The file will have its original line endings in your working directory.

    git config --global core.autocrlf input // 다양한 os 플랫폼에서 협업할 경우
    출처: http://handam.tistory.com/127
</pre>

## 물음표
> 가독성이 좋은 diff (기본 diff는 개인적으로 가독성이 안좋음. winmerge 만한게 있을까.)
  * webstrom 활용!
  * [git config](https://blog.outsider.ne.kr/1011)
  * [vimdiff](http://bobcomputer.tistory.com/3)

> fetch vs pull
  * 공통점 : remote repository의 리소스를 local repository로 가져온다
  * 차이점 : fetch 는 현재 작업중인 리소스들을 변경하는 merge 작업은 하지 않는다
        pull은 현재 작업중인 리소스의 merge 하여 통합한다

> 충돌을 해결하는 방법

> 어느 시기에 상태변화를 해야 협업이 편리한가

> branch 생성 및 활용

> 한 버전의 속한 특정 파일만 revert 가능여부

## git
나는 git을 사용해왔지만 부끄럽게도 아직 자신이 없다.

지금까지 실무에서 scm으로 기업형 형상관리솔루션, subversion, perforce, git 총 4가지를 경험해왔다. 이 중에 svn을 가장 자유자재로 사용했고 perforce도 branch 만 추가로 이해하고 바로 사용했는데 git 만큼은 진입장벽이 컸다.

현재 생활코딩 강좌를 통해 git을 다시 시도하고 있고 터미널을 통해 실습하고 있으며 이 과정중에 내 왜 git이 어려웠는 알게되었다.

* 다양하고 확장된 기능
* 이전에 너무나도 잘 사용했던 scm과 비슷하거나 동일한 커맨드로 인한 개념 혼동
* 파일단위가 아닌 버전단위의 관리라는 점을 인지하지 못함
* 다양한 접근을 지원하는 tools과 나와 맞지 않는 tool을 사용했던 것
* 경험으로 인한 해결 못한 너무 많은 궁금증
* 파일의 변경인지 파일 상태의 변경인지 헷갈리는 경우가 많다. 직접 해보기전엔 알수가 없다.
* 어느 리젼에서 해야하는지 헷갈리는 경우가 많다.

생활코딩 git 동영상 수업을 통해 개념을 알게되니 나도 잘 할수있겠다는 생각이 들었고 나와 같은 상태를 가진 분이라면 보길 권한다.

기본적으로 [생활코딩 git 수업](https://opentutorials.org/module/3762)을 통해 진행

## 2019.06.18 

 - stage (commit 대상파일) 
  add .
 
 - 특정 버전으로 checkout == HEAD는 포인트.
 - HEAD를 다시 master로 바꿔줘야함.
 - ? 이걸 master 에 올리는 방법은? -> reset!
 - 삭제하고 싶은 버전의 이전 버전에서 reset. (soft, mixed, hard)
 - 공유하기 전까지 reset 할 수 있다.
 - git reflog
 
 
 
 
 - git은 [commit] 이 되어 있다면 어떤 것도 삭제하지 않음!
 - reset commit id/ version id
 
 3가지 space
 - .git 폴더 (repository)
 - resources  (working directory)
 - stage area -> 수정할 것중 버전관리 대상. commit해서 repository로 이동할 논리적 area
 
  
 
  
  ? 
   * branch - 생성, 관리, 병합
   * 팀 협업
   * add -> revert
     commit -> revert (non version, stage)
     github -> revert (non version, stage)
     
   * complict -> merge
   
   
 ## 2019.06.19
 - branch : master
 - remote 
  
  
 


