---
permalink: /
title: "Emanuel Tewolde"
excerpt: "Academic Website"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<!-- Welcome to my academic website! It is work in progress, especially starting from the section "Working Papers". -->

I am a third-year PhD student in the Computer Science Department of Carnegie Mellon University, where I am fortunate enough to be advised by <a href=" https://www.cs.cmu.edu/~conitzer/ " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">Vincent Conitzer</a>. My work is supported in part by the Cooperative AI PhD Fellowship.
<!-- and to be part of the <a href=" https://www.cs.cmu.edu/~focal/ " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">Foundations of Cooperative AI Lab (FOCAL)</a>. -->

I strive to understand how to enable artificial intelligence and humans to effectively achieve better (social) outcomes in strategic interactions with other agents. More specifically, my current research interests lie in algorithmic game theory and reinforcement learning, with an emphasis on the safety, coordination, cooperation, and alignment of AI systems. The tools I enjoy using involve mathematical optimization, learning in games, LLMs, and computational complexity.

Prior to CMU, I completed a master's and bachelor's degree in mathematics at Imperial College London and the Technical University Darmstadt respectively. In addition to that, I have also worked with the Fraunhofer-Gesellschaft (IEE) on machine learning methods for smarter renewable energy systems.
<!-- <a href=" https://www.iee.fraunhofer.de/en.html " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">Fraunhofer-Gesellschaft (IEE)</a> -->

Feel free to reach out to me under emanueltewolde (at) cmu (dot) edu.
<br>
<a href=" ../files/CV.pdf " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">CV</a>,  <a href=" https://scholar.google.com/citations?user=LpZkIogAAAAJ&hl=en " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">Google Scholar</a>, <a href=" https://dblp.org/pid/305/4404.html " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">DBLP</a> 

<!--| <a href=" https://scholar.google.com/citations?user=LpZkIogAAAAJ&hl=en " target="_blank"  rel="noopener noreferrer" style="text-decoration: none">DBLP</a> -->

<!-- {% if author.googlescholar %}
  You can find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %} -->

In below, ' - &alpha;&beta; - &#124;' stands for alphabetical author ordering, and '&#42;' stands for equal contribution.

{% include base_path %}


{% if site.workingpapers.size != 0 %}
## Working Papers

{% for post in site.workingpapers reversed %}
  {% include archive-single.html %}
{% endfor %}

{% endif %}

## Publications

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Teaching

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}

