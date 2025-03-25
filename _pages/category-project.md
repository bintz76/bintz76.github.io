---
title: "PROJECT"
layout: archive
permalink: /project
author_profile: true
sidebar_main: true
sidebar:
    nav: sidebar-category
---

{% assign posts = site.categories.project %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
