---
title: "Home"
layout: textlay
excerpt: "Carter Lab at UC San Diego."
sitemap: false
permalink: /allnews.html
---

# News

{% for article in site.data.news %}
<p>{{ article.date }} <br>
<em>{{ article.headline }}</em></p>
{% endfor %}
<br><br>
