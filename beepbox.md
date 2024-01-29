---
layout: page
title: "Beepbox"
permalink: /beepbox/
main_nav: true
---

<ul class="posts-list">
{% for post in site.beepbox %}
  <li>
    <strong>
      <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </strong>
    <span class="post-date">- {{ post.date | date_to_long_string }}</span>
    <br>
    <span class="post-date">{{ post.background }}</span>
  </li>

{% endfor %}
</ul>