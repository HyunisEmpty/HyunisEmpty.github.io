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

### 5. lanyon 테마 적용하기
테마를 적용하는 과정에서 CSS가 깨지는 현상을 발견

_config.yml의 6번 라인 baseurl을 주석 처리

_config.yml의 5번 라인 http를 https로 변경   

### 6. 댓글 기능 추가
[Disqus 사이트](https://jekyllrb-ko.github.io/docs/installation/windows/)
#### Disqus 가입 & 세팅
2. 회원 가입
3. "I want to install Disqus on my site" 선택
4. 사이트 정보 입력 - Website Name 기억해두기
5. Platform중 Jekyll 선택
6. install Instruction을 읽어본 후 Configure를 눌러 다음을 진행
7. Website URL에 사이트 주소 입력 후 Next로 이동
8. Comment 정책 체크 후 Complete Setup을 눌러 설정 마무리

### 6. favicon 추가
1. favicon을 할 이미지를 준비
2. 아래 사이트를 이용 이미지를 favicon으로 바꿈
[favicon generator](https://www.favicon-generator.org/)
3. ' Download the generated favicon ' 을 클릭해서 zip 파일을 다운받고 what's next? 밑의 코드를 다 복사해줍니다.
4. public 폴더에 다운로드 받은 파일을 복사하여 넣는다.
5. _includes에 새로운 파일의 head.html에 복사한 코드를 삽입
