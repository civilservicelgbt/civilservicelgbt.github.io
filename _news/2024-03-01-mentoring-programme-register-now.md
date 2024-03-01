---
layout: news
title: "Register now for the 2024 LGBT+ mentoring programme."
excerpt: "Registrations will close on 31 March 2024. Miss it, and miss out until next year."
date: 2024-03-01
author: John Peart
image: /assets/images/uploads/mentoring-scheme/give-a-boost-get-a-boost.png
image-alt: "Give them a boost. Become an LGBT+ mentor. Get a boost back. Become an LGBT+ mentee."
category:
  - mentoring
published: true
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

**You can now register to join the 2024 Civil Service LGBT+ mentoring programme.** You can register as a mentee, a mentor or both. Registrations will close on {{ registration-close | date: "%-d %B %Y" }}, and matching will happen shortly after that.

## How the programme works

### Taking part as a mentee

**Give your career a boost and sign up as a mentee.** The right mentor can help you to refine your career goals, identify opportunities for development and build your networks.

As a mentee, you'll be asked to:

1. **Set up 'speed mentoring' sessions with each mentor we match you with.** It is your responsibility to arrange a suitable time and date. You should meet each mentor for an initial 30 minute session.
2. **Decide if you want to keep a mentor.** If you feel you can learn something from one of the mentors you meet, ask them if they can be your mentor long-term.
2. **Lead your relationship with your mentor.** If you are successful in securing a long-term mentor, it's your responsibility to organise meetings and lead your relationship with them.

As a mentee, you can expect to:

1. receive up to 90 minutes of speed mentoring
2. work with a long-term mentor after your speed mentoring for up to a year
3. receive guidance on how to maximise your role as a mentee

### Taking part as a mentor

**Give something back and become an LGBT+ mentor.** Acting as a mentor can help other, less experienced staff get on with their career. It can be a rewarding experience for you too; you can learn new skills and it makes a great corporate contribution.

As a mentor, you'll be asked to:

1. **Meet with up to 3 mentees for 'speed mentoring'.** You will be asked to meet for one, 30 minute session with each mentee. They will contact you to arrange a suitable time and date.
2. **Agree to mentor at least one longer-term mentee.** Once you have met all your mentees, we'd ask that you agree to keep meeting at least one of them to provide them with a mentoring relationship on an ongoing basis.

As a mentor, you can expect to:

1. be matched with someone one or two grades more junior to you
2. receive guidance on how to maximise your role as a mentor
3. have the chance to join a network of other mentors who you can speak to for advice too

### Check you're eligible to take part

In order to join the programme – either as a mentee or mentor – you must:

1. **be a LGBT+**: you must have a minority sexual orientation, gender identity or expression, or variation in sex characteristics
2. **be a civil servant**: you must be an employee of the UK Civil Service, Civil Service in Northern Ireland, Scotland or Wales – contractors and interim staff **cannot** take part in this programme

### Need more information?

We've published detailed information about what's involved in our ['about the programme' guide](/mentoring/about-the-programme), and in our guides for [mentors](/publication/resources-for-mentors) and [mentees](/publication/resources-for-mentees).

We've also created some [short videos to induct you to the programme](/publication/mentoring-induction/).

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
