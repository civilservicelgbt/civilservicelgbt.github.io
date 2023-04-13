---
layout: publication
title: "Election 2023: Organisations that are eligible to vote"
excerpt: A list of departments that have recognised and confirmed LGBT+ networks, and the agencies they should coordinate a vote with.
author: Civil Service LGBT+ Network
category:
  - election-2023
permalink: /election/2023/networks
---

{:toc}
- toc

## About this document

This document lists the networks that are eligible to vote in the 2023 Chair's election. It also lists organisations that we do not currently have complete details for, and so are ineligible to vote.

It is up to individual networks to determine how they conduct their internal process that determines the candidate they vote for in this election. If your network is listed below and you are a member of an LGBT+ network please contact your departmental network leads for information about how you can participate.

{% assign networks = site.data.networks %}
{% assign eligiblenetworks = networks | where_exp: "network", "network.email" %}
{% assign noteligiblenetworks = networks | where_exp: "network", "network.email == null" %}

{% assign eligiblecount = 0 %}
{% assign noteligiblecount = 0 %}

{% for network in networks %}
  {% unless network.email %}
  {% assign noteligiblecount = noteligiblecount | plus: 1 %}
  {% endunless %}
  {% if network.email %}
  {% assign eligiblecount = eligiblecount | plus: 1 %}
  {% endif %}
{% endfor %}

## {{ eligiblecount }} eligible networks

This is the list of LGBT+ networks we believe are eligible to vote and that we have a current email address for. 

If you believe the contact details for your network are incorrect, please email us at <election@civilservice.lgbt> as soon as possible, and no later that 19 May 2023 at 09:00.

<ul class="list--no-styles networks--network-list">

{% for network in eligiblenetworks %}
  
  {% unless network.email == null %}
  <li class="networks--network-list--item">
    <h3 class="networks--network-list--item--network">{{ network.department }}</h3>
    <p>{{ network.network }}</p>
    <p>The email address we currently hold for this network is:<br> <code>{{ network.email }}</code></p>
  </li>
  {% endunless %}
  
{% endfor %}
</ul>

## {{ noteligiblecount }} not eligible networks

These networks are known to us, but are not currently eligible to vote because we do not have an up-to-date shared mailbox for their network, or do not have current details for the network chairs.

If you run one of these network, please email us at <election@civilservice.lgbt> before 19 May 2023 at 09:00 to confirm your details and eligibility to vote in this election.

<ul class="list--no-styles networks--network-list">

{% for network in noteligiblenetworks %}
  
  <li class="networks--network-list--item">
    <h3 class="networks--network-list--item--network">{{ network.department }}</h3>
    <p>{{ network.network }}</p>
  </li>
  
{% endfor %}
</ul>