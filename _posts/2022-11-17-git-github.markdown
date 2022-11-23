---
layout: post
title:  "Git and Github!"
date:   2022-11-17 12:43:00 +0900
categories: jekyll update
comments: true
---

## Git

### Git 로컬 저장소 생성
- git init

### Git 저장단위
- git status : 현재 Git 상태 확인
- git add example.py : example.py를 생성하고, 이를 Commit에 반영하고 싶은 경우
- git commit -m "add example.py" : 변경사항이 반영된 new commit 생성
- git log : commit 기록 확인하기

### Git의 Branch
- 코드의 흐름을 분산시켜 더욱 효율적인 개발 가능!
- git branch <branch_name> : git branch <branch 이름>을 통해 branch 생성
- git checjout <branch_name> : 현재 작업중인 branch를 전화
- git merge <branch_name> : 현재 작업중인 branch를 원하는 branch에 병합
- git branch -d <branch_name> : 다음을 통해 <branch 이름>을 통해 branch 삭제

### Github
- 지금까지 우리는 Git의 로컬 저장소에서 할 수 있는 일들을 다뤘습니다. (이제는 다른 사람과 협업을!)
- Local 저장소를 넘어 Remote 저장소로! 원격 저장소 중 대표적인 Github

<div id="disqus_thread"></div>
<script>
    /**
    *  RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
    *  LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables    */
    /*
    var disqus_config = function () {
    this.page.url = PAGE_URL;  // Replace PAGE_URL with your page's canonical URL variable
    this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
    };
    */
    (function() { // DON'T EDIT BELOW THIS LINE
    var d = document, s = d.createElement('script');
    s.src = 'https://HyunisEmpty.disqus.com/embed.js';
    s.setAttribute('data-timestamp', +new Date());
    (d.head || d.body).appendChild(s);
    })();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript">comments powered by Disqus.</a></noscript>
