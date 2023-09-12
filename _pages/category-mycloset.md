---
title: "MYCLOSET"
layout: archive
permalink: /mycloset
author_profile: true
sidebar_main: true
sidebar:
    nav: sidebar-category
---

{% assign posts = site.categories.mycloset %}
{% for post in posts %} {% include archive-single.html type=page.entries_layout %} {% endfor %}
