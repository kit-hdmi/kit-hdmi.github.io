---
title: "HDMI Lab - Members"
layout: gridlay
excerpt: "HDMI Lab -- Members"
sitemap: false
permalink: /team/
---

# Current Members

{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" style="float: left; width: 120px; height: 120px; object-fit: cover; object-position: top; margin-right: 16px; border-radius: 10%;" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}</i><br>
  <i>Email: {{ member.email }}</i>{% if member.education1 %}<br>
  <i>{{ member.education1 }}</i><br>
  <i>{{ member.education2 }}</i>{% endif %}
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


## Alumni
- 구보명, Undergraduate Researcher (2025.11 - 2026.06), Current Position: Undergraduate Student at kit
- 장지원, Undergraduate Researcher (2024.03 - 2025.12), Current Position: TBD
- 김상민, Undergraduate Researcher (2024.03 - 2025.06), Current Position: Trainee of CISCO Security Academy - Cybersecurity Track
- 최재준, Undergraduate Researcher (2024.03 - 2025.02), Current Position: Graduate Student at Kyung Hee University
