---
layout: event
title: Register for the Civil Service LGBT+ mentoring programme
excerpt: "Registrations are open from 1 March to 31 March 2024. "
date: 2024-01-08T09:00:00Z
event:
  host: Civil Service LGBT+ Network
  start: "2024-03-01T08:00:00.000Z"
  end: "2024-03-31T23:59:00.000Z"
  deadline: "2024-03-31T23:59:00.000Z"
  location: Register online during the registration window
  no-register: Register online during the registration window
category:
  - mentoring
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

Registrations for the third round of the Civil Service LGBT+ Network's [award-winning](/news/2021/12/16/weve-won-a-civil-service-award) mentoring programme will open {{ registration-open | date: "%-d %B %Y" }}. LGBT+ civil servants who want to sign up as a mentor or mentee on this year's programme will be able to register via the Civil Service LGBT+ Network's website.

{% if registration == "open" %}

> ## Registrations are currently open
>
> Registrations are open from {{ registration-open | date: "%-d %B %Y" }} until {{ registration-close | date: "%-d %B %Y" }}. If you miss the registration deadline, you won't be able to take part and you'll have to wait until the next round of the programme in 2025.
>
> <a href="/mentoring/register" title="Visit the mentee registration page" class="button button--action">Register for the programme</a>

{% else %}

> ## Don't miss out on future updates
>
> [Sign up for email alerts](/email-alerts/) from the Civil Service LGBT+ Network so you don't miss the registration window.
>
> We will also publish all our updates on the [mentoring topic page](/mentoring).

{% endif %}

## Mentoring exclusively for and by LGBT+ civil servants

The Civil Service LGBT+ mentoring programme is the largest and only mentoring programme of its kind in the Civil Service. Since 2021, more than 1,800 mentors and mentees have signed up to take part.

We created the programme to give LGBT+ civil servants greater development opportunities, and to give junior staff greater access to more senior LGBT+ role models across government.

Everyone involved in the programme – the mentors, the mentees, and the people running the programme – is LGBT+.

## It's speed mentoring leading to long-term mentoring

When you join the programme, you'll be matched with up to 3 people for speed mentoring. Mentees are matched with mentors that are at least 1 grade more senior than they are; and usually 2 grades.

Mentees can use their speed mentoring sessions for one-off advice or to explore whether the mentor they've been matched with could be a good longer-term mentor that will work with them for the next 12 months.

## Don't miss it!

The registration window will be open for 4 weeks. If you don't register during that window, you'll have to wait until the next round of the programme, which won't be until 2025 at the earliest.

All our matching happens once using a software package. It's fast. So fast, that we'll be able to send out matches a couple of days after the registration window closes.

So there are no second chances or last minute registrations. If you miss it, you miss out!

> ## Find out more about our mentoring programme
>
> We've published everything you need to know about our award-winning mentoring programme on our [mentoring topic page](/mentoring)
