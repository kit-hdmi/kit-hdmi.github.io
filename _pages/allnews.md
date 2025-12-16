---
title: "HDMI Lab - News"
layout: textlay
excerpt: "HDMI Lab -- News"
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ **article.date** }} <br> 
{{ article.headline}} <br>
{{ article.details}}</p>
{% endfor %}
