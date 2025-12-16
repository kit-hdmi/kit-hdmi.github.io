---
title: "HDMI Lab - Team"
layout: gridlay
excerpt: "HDMI Lab -- Team members"
sitemap: false
permalink: /team/
---

# Group Members

 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/vacancies) **!**


Jump to [staff](#staff), [master and bachelor students](#master-and-bachelor-students), [alumni](#alumni), [administrative support](#administrative-support), [lab visitors](#lab-visitors).

## Staff
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <i>{{ member.info }}<br></i>
  <i>email: <{{ member.email }}></i>

  {% if member.number_educ == 1 %}
  {{ member.education1 }}
  {% endif %}

  {% if member.number_educ == 2 %}
  {{ member.education1 | markdownify}}<br>
  {{ member.education2 | markdownify}}
  {% endif %}

  {% if member.number_educ == 3 %}
  {{ member.education1 | markdownify}}<br>
  {{ member.education2 | markdownify}}<br>
  {{ member.education3 | markdownify}}
  {% endif %}
<br>
{% if member.research_interests %}
  <h5>research interests:
    {% for interest in member.research_interests %}
    {{ interest }}
    {% endfor %}
  {% endif %}<h5>
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
- 장지원, Undergraduate Researcher (2024.03 - 2025.12), Current Position: TBD
- 김상민, Undergraduate Researcher (2024.03 - 2025.06), Current Position: Trainee of CISCO Security Academy - Cybersecurity Track
- 최재준, Undergraduate Researcher (2024.03 - 2025.02), Current Position: Graduate Student at Kyung Hee University