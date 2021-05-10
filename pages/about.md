---
layout: page
title: About
description: "maybe"
keywords: Lexi, Bu
comments: true
menu: About
permalink: /about/
---
# Connect
<div class="btn-inline">
{% for website in site.data.social %}
<a href="{{ website.url }}" class="btn btn-outline" type="button">{{ website.sitename }}</a>
{% endfor %}
</div>

# Skill Keywords
{% for category in site.data.skills %}
### {{ category.name }}
<div class="btn-inline">
{% for keyword in category.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
