---
layout: publication
title: "Register for the Civil Service LGBT+ mentoring programme"
excerpt: "Use this form to register as a mentee or mentor on the Civil Service LGBT+ mentoring programme."
author: "Civil Service LGBT+ Network"
category: ["mentoring"]
image: "/assets/images/uploads/mentoring-scheme/twitter-timeline--mentoring-for-lgbt-civil-servants.png"
permalink: "/mentoring/register-after-2024-deadline"
breadcrumbs-override: true
breadcrumbs:
- title: "Topics"
  url: /topics
- title: "Mentoring programme"
  url: /mentoring
---
{% assign now = site.time | date: "%s" %}
{% assign mentoring = site.data.mentoring %}
{% for registration in mentoring %}
  {% assign registration-open = registration.registration-open | date: "%s" %}
  {% assign registration-close = registration.registration-close | date: "%s" %}
  {% assign registration-url = registration.registration-url %}
{% endfor %}

<a href="{{ registration-url }}" title="Visit the mentee registration page" class="button button--action">Register for the programme</a>

> **This form might not work on your departmental IT system.** To complete this survey, you need to complete a Google Form. These forms are blocked on some departmental IT systems.
>
> If you cannot open the form on your departmental system, try again on your personal device.