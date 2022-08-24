---
layout: page
title: Archive
---

<html>
<head>
<style>
body {
  background-image: url('{{ site.baseurl }}/images/bg_elly.png');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-position: right;
}
</style>
</head>

</html>

MoJo (unlike BoJo) never forgets! <br>

{% for tag in site.tags %}
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ site.url }}/blog{{ post.url }}">{{ post.date | date: "%B %Y" }} - {{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
