---
layout: post
title:  Build Process
date:   2021-12-14 20:11:33 +0900
categories: jekyll update
comments: true
tags: [blog, jekyll, GA, tags]
---
<br/><br/><br/><br/>
<h2>Google Analytics(방문자 통계 추적) 기능 추가</h2>

1. Google Analytics 가입 

2. gtags.js 를 복사하여 _include 의 google-analytics.html 에 적용 

3. _configs.yml 설정 변경

end. Google Analytic에서 실시간 방문자 통계를 확인 할 수 있다.
![1](https://user-images.githubusercontent.com/90315907/145928821-adb216f2-3edd-4385-8239-c19dd7171b44.png)  <br/><br/><br/><br/><br/><br/><br/><br/>
    
    
    
     



<h2>태그 기능 추가</h2>

1.포스트 md문서의 머릿말에 tags 변수를 추가  


2.post.html 파일 수정
  {{contents}} 부분에 아래 코드 추가

<pre>
<code>
{% raw %}
{% if page.tags %}   
  {% for tag in page.tags %}   
    <span class="tag">{{ tag }}</span>   
  {% endfor %}   
{% endif %}   
{% endraw %}
</code>
</pre>


[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
