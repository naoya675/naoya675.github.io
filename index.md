---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home
---

## About

- [About Me](/about/)

## Account

- [GitHub](https://github.com/naoya675)
- [Twitter](https://twitter.com/naoya675)
- [AtCoder](https://atcoder.jp/users/naoya675)
- [AtCoder Problems](https://kenkoooo.com/atcoder/#/user/naoya675)
- [Codeforces](https://codeforces.com/profile/naoya675)
- [Codeforces Problems](https://cf.kira924age.com/#/user/naoya675)

## Contents

<!--
<ul>
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small>{{ post.date | date: "%b %-d, %Y" }}</small>
  </li>
{% endfor %}
</ul>
-->

<ul>
{% for post in site.posts %}
  {% if post.categories contains "post" %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endif %}
{% endfor %}
</ul>

<ul>
{% for post in site.posts %}
  {% if post.categories contains "yugioh" %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%Y-%m-%d" }}</small>
    </li>
  {% endif %}
{% endfor %}
</ul>
