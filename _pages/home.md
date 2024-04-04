---
title: "Home"
layout: homelay
sitemap: false
permalink: /
---

<style>
a:hover {
  color: grey;
  background-color: transparent;
  text-decoration: underline;
}
.heading {
    color: grey;
    background-color: transparent;
}
</style>

<h2 class="heading"> About me </h2>

I am currently working as a Project Associate at the [ML Research Lab](https://dr-j-saketha-nath-ml-research-group.github.io/home/) in Indian Institute of Technology Hyderabad(IITH) under [Prof. J. Saketha Nath](https://people.iith.ac.in/saketha/).

Prior to this, I completed my undergraduate (B.Tech) and master's (MS by Research) degrees at International Institute of Information Technology, Hyderabad (IIITH) in Computer Science and Engineering with a specialization in Theory and Algorithms.
I was a part of the [Machine Learning Lab](https://mll.iiit.ac.in/) under the primary supervision of [Prof. Sujit Gujar](https://www.sujitgujar.com/), and co-advised by [Prof. Girish Varma](https://girishvarma.in/).

<!-- During my time at IIITH, I studied Fairness in Machine Learning and worked on performance analysis of personalized pricing strategies under various fairness constraints. This work led to my Master's thesis on ENTER THESIS TITLE. -->

<!-- INSERT AAAI WORK HERE.

I also studied probabilistic graphical models (PGMs) and Markov Chain Monte Carlo (MCMC) sampling for complex structures such as graph colorings and path sampling on planar graphs.  -->

I am looking for Research Associate/Pre-Doctoral roles in Machine Learning. Link to my [CV]({{ site.url }}{{ site.baseurl }}/assets/cv/cv.pdf).

<h3 class="heading"> Interests </h3>
My interests broadly lie at the intersection of Machine Learning, Applied Probability and Causal Inference. 
Particularly, I am interested in developing theory and algorithms to build robust, fair, and explainable machine learning models by applying the pricinples of causality and causal inference.

<h3 class="heading"> News </h3>

<div class="jumbotron">
{% for article in site.data.news %}
<b>[{{ article.date }}]: </b>{{ article.headline }}
{% endfor %}
</div>

<h3 class="heading"> Publications </h3>

<div class="container-fluid">
<div class="row">
<ul>
{% for paper in site.data.publications %}
<li>
<b>{{ paper.title }}</b><br>
<i>with {{ paper.authors }}</i><br>
at {{ paper.forum }} 
{%- if paper.link %}
    <a href="{{ paper.link }}" role="button">[Paper]</a>
{%- endif %}
</li>
{% endfor %}
</ul>
</div>
</div>
