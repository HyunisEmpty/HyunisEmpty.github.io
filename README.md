## Build 과정
### 1. Repository 생성
Github에서 \<username>.github.io 이름의 Repository 생성

### 2. Local-Remote Repository 연동
1. Remote Repository의 주소를 복사한 후  
2. `git clone <복사한 Remote Repository의 주소> <path>`로 clone  
3. `git commit -m "<commit msg>"`로 커밋 남기기  
4. `git branch -M main`으로 현재 branch의 이름을 main으로 변경  
5. `git status`로 현재 상태 확인 후 `git add .`로 변경파일 추가  
6. `git push origin main`으로 main에 로컬 변경사항 push  

### 3. Jekyll 설치
[Windows용 Jekyll 가이드 참조](https://jekyllrb-ko.github.io/docs/installation/windows/)

[Windows용 Ruby + Devkit](https://rubyinstaller.org/downloads/)  
위의 링크를 통해 Ruby 설치

Jekyll과 Bundler를 설치  
`gem install jekyll bundler`

Jekyll이 올바르게 설치되었는지 확인  
`jekyll -v`

### 4. Jekyll 사이트 생성
현재 디렉토리(.)에 Jekyll을 설치
`jekyll new . --force`

Jekyll 시작하기  
`bundle exec jekyll serve` 을 실행 후,  
localhost:4000 접속

* LoadError 발생 시 webrick 파일 설치
`bundle add webtick`
