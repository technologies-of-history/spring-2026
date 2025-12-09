---
layout: default
title: Syllabus
---

This blog features the research of students in HIST 30693, Technologies of History from Cuneiform to Coding, taught at Texas Christian University in Spring 2026. Throughout the semester, students will be posting their work related to the history of communicatiosn technologies from the ancient world to the present day, using various digital "tools" that they learn over the semester. Through these posts, students will learn the basics of GitHub workflows and Markdown language, taking advantage of the possibilities of digital storytelling and digital analytical methodologies. 

Click the menu in the upper left corner to learn more about the [student contributors]({{ site.baseurl }}/contributors) or to peruse the course [syllabus](https://technologies-of-history.github.io/course).

---
<br>

<div class="posts" id="top">
  {% for post in site.posts %}
    <article class="post">
      <header class="post-header">
      <h2 class="post-title"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
      <h4>By {{ post.author }} on {{ post.date | date: "%B %e, %Y" }}</h4>
      </header>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}

  <div class="breadcrumbs">
    <a href="#top">Return to the top</a>
  </div>
</div>
