---
title: "Mentoring"
date: 2022-05-17T00:00:00.00Z # YYYY-MM-DD
excerpt: "Give yourself a boost, or give something back."
layout: topic
category: mentoring
background: yellow
redirect_from:
- /mentoring
- /mentoring-scheme

image: "/assets/images/uploads/mentoring-scheme/mentoring-scheme-csa-banner.png"

# Social Media
# Set to 'true' to turn on the social links
social-links: false

# Archived posts
# Add 'show-archive: false' to disable old posts from the _archives folder being displayed
show-archive: false
---
{% assign now = site.time | date: "%s" %}
{% assign mentoring = site.data.mentoring %}
{% for registration in mentoring %}
  {% assign registration-open = registration.registration-open | date: "%s" %}
  {% assign registration-close = registration.registration-close | date: "%s" %}
{% endfor %}
{% if now >= registration-open and now <= registration-close %}
  {% assign registration = "open" %}
{% else %}
  {% assign registration = "closed" %}
{% endif %}

{% if registration == "open" %}
The next cohort of the Civil Service LGBT+ mentoring programme is open for registrations from {{ registration-open | date: "%-d %B %Y" }} until {{ registration-close | date: "%-d %B %Y" }}. 

If you miss the registration deadline, you won't be able to take part and you'll have to wait until the next round of the programme in 2025.

**Registration is currently open.**

<a href="/mentoring/register" title="Visit the mentee registration page" class="button button--action">Register for the programme</a>
{% else %}
The next cohort of the Civil Service LGBT+ mentoring programme is open for registrations from {{ registration-open | date: "%-d %B %Y" }} until {{ registration-close | date: "%-d %B %Y" }}. 

If you miss the registration deadline, you won't be able to take part and you'll have to wait until the next round of the programme in 2025.

**Registration is currently closed.**
{% endif %}
