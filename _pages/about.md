---
permalink: /
title: "Emanuel Tewolde"
excerpt: "Academic Website"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Welcome to my academic website! 

I am a first-year PhD student in the Computer Science Department of Carnegie Mellon University, where I am fortunate enough to be advised by <a href=" http://www.cs.cmu.edu/~conitzer/ " target="_blank"  rel="noopener noreferrer">Vincent Conitzer</a> and to be part of the <a href=" http://www.cs.cmu.edu/~focal/ " target="_blank"  rel="noopener noreferrer">Foundations of Cooperative AI Lab (FOCAL)</a>. 

My current research interests lie in algorithmic game theory and (multi-agent) reinforcement learning. I strive to understand how to enable artificial intelligence and humans to effectively achieve better (social) outcomes in strategic interactions with other agents. The methods I enjoy using include mathematical optimization, complexity theory, learning in games and deep learning.

Prior to CMU, I completed a master's and bachelor's degree in mathematics at Imperial College London and the Technical University Darmstadt respectively. In addition to that, I have also worked with the <a href=" https://www.iee.fraunhofer.de/en.html " target="_blank"  rel="noopener noreferrer">Fraunhofer IEE</a> on machine learning methods for smarter renewable energy systems.

Feel free to reach out to me under emanueltewolde (at) cmu (dot) edu
<br>
<a href=" ../files/CV_Emanuel_Tewolde_26_04_23.pdf " target="_blank"  rel="noopener noreferrer">CV</a>,  <a href=" https://scholar.google.com/citations?user=LpZkIogAAAAJ&hl=en " target="_blank"  rel="noopener noreferrer">Google Scholar</a> 

<!--| <a href=" https://scholar.google.com/citations?user=LpZkIogAAAAJ&hl=en " target="_blank"  rel="noopener noreferrer">DBLP</a> -->

<!-- {% if author.googlescholar %}
  You can find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %} -->

{% include base_path %}

## Working Papers

{% for post in site.workingpapers reversed %}
  {% include archive-single.html %}
{% endfor %}

## Publications

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

## Teaching

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}

