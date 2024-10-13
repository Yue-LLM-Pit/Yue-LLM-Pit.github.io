---
permalink: /
title: "Yue Zhou (周 岳) "
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

## PhD student at UIC | NLP for Social Good | LLMs

I'm a fourth-year PhD student at UIC, advised by [Barbara Di Eugenio](https://cs.uic.edu/profiles/barbara-di-eugenio/). My research focuses on Natural Language Processing (NLP), with particular interests in reasoning, safety, and fairness in large language models. My research goal is to build robust, fair, and explainable systems for social good. Previously, I was a visiting researcher at MIT CSAIL and completed my research internship at MIT-IBM Watson AI Lab, where I was advised by [Yada Zhu](https://mitibmwatsonailab.mit.edu/people/yada-zhu/), [Yang Zhang](https://mitibmwatsonailab.mit.edu/people/yang-zhang/), and [Yoon Kim](https://people.csail.mit.edu/yoonkim/).

Prior to my PhD, I obtained my Master's degree in Information Systems from [Albert-Ludwigs-Universität Freiburg](https://uni-freiburg.de/en/), Germany.


## News

{% capture include_content %}
{% include_relative news.md %}
{% endcapture %}
{{ include_content | split: '---' | last }}

## Recent Publications


<style>
.pub-item {
  margin-bottom: 20px;
}
.conference-badge {
  display: inline-block;
  padding: 3px 6px;
  font-size: 0.8em;
  font-weight: bold;
  color: white;
  background-color: #4a4a4a;
  border-radius: 3px;
  margin-right: 10px;
}
.pub-title {
  font-weight: bold;
}
.pub-authors {
  font-style: italic;
  margin-bottom: 5px;
}
.pub-links a {
  margin-right: 10px;
  text-decoration: none;
  color: #0366d6;
}
</style>

{% capture publications_content %}
{% include_relative selected-publications.md %}
{% endcapture %}

{% assign pub_items = publications_content | split: '<div class="pub-item"' %}
{% assign filtered_pubs = "" | split: ',' %}
{% for item in pub_items %}
  {% if item contains 'data-homepage="true"' %}
    {% assign filtered_pubs = filtered_pubs | push: item %}
  {% endif %}
{% endfor %}

{% for pub in filtered_pubs limit:5 %}
<div class="pub-item"{{ pub }}
{% endfor %}


## Miscellaneous

My first name is pronounced /y̯œ/ ("yoo-eh").

I speak Mandarin, English, and German, and I enjoy learning languages.

I am an amateur foil fencer. 
