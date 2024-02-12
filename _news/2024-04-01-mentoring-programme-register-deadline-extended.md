---
layout: news
title: "2024 LGBT+ mentoring programme: deadline extended"
excerpt: "Registrations will close on 5 April 2024. Don't miss out."
date: 2024-03-01
author: John Peart
image: /assets/images/uploads/mentoring-scheme/give-a-boost-get-a-boost.png
image-alt: "Give them a boost. Become an LGBT+ mentor. Get a boost back. Become an LGBT+ mentee."
category:
  - mentoring
published: false
breadcrumbs-override: true
breadcrumbs:
- title: "Topics"
  url: /topics
- title: "Mentoring"
  url: /mentoring
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

**We have extended the registration deadline for the 2024 Civil Service LGBT+ mentoring programme for one more week.** This is your last chance to register, or you will not be able to take part in this year's programme. Registrations will close on {{ registration-close | date: "%-d %B %Y" }}, and matching will happen shortly after that.

### Need more information?

We've published detailed information about what's involved in our ['about the programme' guide](/mentoring/about-the-programme), and in our guides for [mentors](/publication/resources-for-mentors) and [mentees](/publication/resources-for-mentees).

## Register to take part

{% if registration == "open" %}
Registrations are open from {{ registration-open | date: "%-d %B %Y" }} until {{ registration-close | date: "%-d %B %Y" }}. If you miss the registration deadline, you won't be able to take part and you'll have to wait until the next round of the programme in 2025.

This year we've made registration more simple than ever before, with a new, single registration form that you can access using the button below.

<a href="/mentoring/register" title="Visit the mentee registration page" class="button button--action">Register for the programme</a>
{% else %}
> ### You can't register to take part right now
>
> Registrations for 2024 mentoring programme are currently closed. Our [mentoring topic page](/mentoring) contains the lastest information about the programme and when it will next be available.
{% endif %}
