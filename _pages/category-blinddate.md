---
title: "소개팅"
layout: archive
permalink: /blinddate
author_profile: true
sidebar_main: true
sidebar:
    nav: sidebar-category
---

{% assign posts = site.categories.blinddate %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
