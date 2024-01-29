---
layout: page
title: "Beepbox"
permalink: /beepbox/
main_nav: true
---

{% assign sorted_beepbox_posts = site.beepbox | sort: "ordering" %}
<ul class="posts-list">
{% for post in sorted_beepbox_posts %}
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