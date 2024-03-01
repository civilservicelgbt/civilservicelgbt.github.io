---
layout: publication
title: "Register for the Civil Service LGBT+ mentoring programme"
excerpt: "Use this form to register as a mentee or mentor on the Civil Service LGBT+ mentoring programme."
author: "Civil Service LGBT+ Network"
category: ["mentoring"]
image: "/assets/images/uploads/mentoring-scheme/twitter-timeline--mentoring-for-lgbt-civil-servants.png"
permalink: "/mentoring/register"
redirect_from:
- /publication/register-as-a-mentor
- /publication/register-as-a-mentee
- /register-as-a-mentor
- /register-as-a-mentee
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
{% if now >= registration-open and now <= registration-close %}
  {% assign registration = "open" %}
{% else %}
  {% assign registration = "closed" %}
{% endif %}

<!-- Include the following to generate a Table of Contents -->
* Table of contents will generate here
{:toc}

{% if registration == "open" %}
Use this form to register to take part in the Civil Service LGBT+ mentoring programme.

## Before you register

Before you register, you should read [our guidance documents](https://www.civilservice.lgbt/publication/about-our-mentoring-programme) so you know what to expect on the programme. We've also created a series of short [induction videos](/publication/mentoring-induction) to explain how the programme works.

If the guidance doesn't answer your question, you can also email us at [mentoring@civilservice.lgbt](mailto:mentoring@civilservice.lgbt).

## Registration deadline

**Registrations for this round of the programme close on {{ registration-close | date: "%-d %B %Y" }}.** We will not be able to accept your registration after this point. You will need to wait until the next round.


<a href="{{ registration-url }}" title="Visit the mentee registration page" class="button button--action">Register for the programme</a>

> **This form might not work on your departmental IT system.** To complete this survey, you need to complete a Google Form. These forms are blocked on some departmental IT systems.
>
> If you cannot open the form on your departmental system, try again on your personal device.

{% else %}

## Registrations are currently closed

Thank you for your interest in the Civil Service LGBT+ mentoring programme.

The window to register for this round of the programme is now closed. We can no longer accept registrations for either mentors or mentees as the matching process has started. The programme is intended to run annually; please come back next year for another chance to take part.

If you registered before the deadline, then we will contact you by email soon with your mentor or mentee matches.

## Further information

For more information about the Civil Service LGBT+ mentoring programme, please read [our guidance documents](https://www.civilservice.lgbt/mentoring).

If the guidance doesn't answer your question, you can also email us at [mentoring@civilservice.lgbt](mailto:mentoring@civilservice.lgbt).

{% endif %}
