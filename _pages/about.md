---
permalink: /
title: "Emanuel Tewolde"
excerpt: "Academic Website"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

<!-- Welcome to my academic website! It is work in progress, especially starting from the section "Working Papers". -->

I am a fourth-year PhD student in the Computer Science Department of Carnegie Mellon University, where I am fortunate enough to be advised by <a href=" https://www.cs.cmu.edu/~conitzer/ " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">Vincent Conitzer</a>. My work is supported in part by the Cooperative AI PhD Fellowship.
<!-- and to be part of the <a href=" https://www.cs.cmu.edu/~focal/ " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">Foundations of Cooperative AI Lab (FOCAL)</a>. -->

I strive to understand how to enable artificial intelligence and humans to effectively achieve better social outcomes in strategic interactions. More specifically, my current research interests lie in algorithmic game theory, LLM agents, and reinforcement learning, with an emphasis on the safety, coordination, cooperation, and alignment of AI systems. Further research topics I enjoy are mathematical optimization, learning in games, social choice theory, and computational complexity.

Currently, I am working at Meta's research unit FAIR (within Meta Superintelligence Labs) on LLM coding agents for AI research. Prior to CMU, I completed a Master's and Bachelor's degree in Mathematics at Imperial College London and the Technical University of Darmstadt respectively. In addition to that, I have previously researched ML methods for smarter renewable energy systems.
<!-- <a href=" https://www.iee.fraunhofer.de/en.html " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">Fraunhofer-Gesellschaft (IEE)</a> -->

Feel free to reach out to me under emanueltewolde (at) cmu (dot) edu.
<br>
<a href=" ../files/CV.pdf " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">CV</a>,  <a href=" https://scholar.google.com/citations?user=LpZkIogAAAAJ&hl=en " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">Google Scholar</a>, <a href=" https://dblp.org/pid/305/4404.html " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">DBLP</a> 

<!--| <a href=" https://scholar.google.com/citations?user=LpZkIogAAAAJ&hl=en " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">DBLP</a> -->

<!-- {% if author.googlescholar %}
  You can find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %} -->

<div class="news-section">
  <h2>News</h2>
  <div class="news-container" style="height: 280px; overflow-y: scroll; background: white; border: 1px solid #ddd; border-radius: 5px; padding: 15px; box-shadow: inset 0 1px 3px rgba(0,0,0,0.1);">
    <ul class="news-list" style="margin: 0; padding: 0; list-style: none;">
      {% for news_item in site.data.news %}
        <li class="news-item" style="display: flex; justify-content: space-between; align-items: center; margin-bottom: 0.6em; padding-left: 1.2em; position: relative;">
          <span style="color: #ff9500; font-size: 1em; position: absolute; left: 0; top: 50%; transform: translateY(-50%);">•</span>
          <span class="news-content" style="color: #495057; font-size: 0.9em; line-height: 1.4; flex: 1; margin-right: 1.5em;">{{ news_item.content }}</span>
          <span class="news-date" style="font-size: 0.8em; color: #6c757d; font-weight: 500; white-space: nowrap; flex-shrink: 0; text-align: right;">{{ news_item.date | date: "%b %Y" }}</span>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>

## Papers


In below, ' - &alpha;&beta; - &#124;' stands for alphabetical author ordering, and '==' superscripts stand for equal contribution.

{% if site.workingpapers.size != 0 %}
### Working Papers

{% for post in site.workingpapers reversed %}
  {% include archive-single.html %}
{% endfor %}

{% endif %}

### Publications

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Teaching

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}

