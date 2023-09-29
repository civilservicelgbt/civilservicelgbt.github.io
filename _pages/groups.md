---
title: "Groups"
excerpt: "Register for personalised updates from our regional and national teams, and our inclusion programmes."

layout: page
permalink: /groups/
---

Civil Service LGBT+ Network 'Groups' are email distribution lists run by people in our local organiser team and programme teams. They are separate from [our email alerts which you can sign up to on our website](/join-us). Unlike our email alerts, Groups are a bit less formal and a bit more personal.

This page lists the groups that are available, and explains how to subscribe and unsubscribe to each.

## Available groups

{% assign regions-groups = site.data.groups | where: "type", "Region" %}
{% assign projects-groups = site.data.groups | where: "type", "Project" %}

{% for group in regions-groups %}
{% if forloop.first == true %}
### Regions and nations
{% endif %}
<details>
  <summary>{{ group.name }}</summary>
  {{ group.description | markdownify }}
  
  <h4>Subscribe to the {{ group.name }} group</h4>
  <p>You can subscribe to this group by <a href="{{ group.url }}" title="Open the Group for the {{ group.name }} (Opens in a new window)" target="_blank">visiting the Group page</a> or by sending an email to:
  <br><code>{{ group.email | replace: "@", "+subscribe@" }}</code></p>
  
  <a href="mailto:{{ group.email | replace: "@", "+subscribe@" }}?subject=SUBSCRIBE&body=Send%20this%20email%20to%20subscribe%20to%20the%20{{ group.name}}%20group.%0D%0A%0D%0AYou%20will%20receive%20a%20reply%20asking%20you%20to%20confirm%20your%20subscription.%0D%0A%0D%0AReply%20with%20a%20blank%20email%20to%20confirm%20your%20subscription.%0D%0A%0D%0AIf%20you%20change%20your%20mind%2C%20you%20can%20unsubscribe%20at%20any%20time%20by%20emailing%20{{ group.email | replace: "@", "+unsubscribe@"}}" class="button" title="Subscribe to the {{ group.name }} Group (Opens a new email in a new window)" target="_blank">Subscribe to the {{ group.name }} group</a>


  You should receive an email asking you to confirm your subscription. Please click 'Reply' and send a blank email back. You should then get confirmation that you have subscribed to this Google Group. There are complete generic instructions at the bottom of this page.

  
  <h4>Unsubscribe from the {{ group.name }} group</h4>
  <p>If you want to stop receiving emails from this group send an email from the same email as you registered with to:
  <br><code>{{ group.email | replace: "@", "+unsubscribe@" }}</code>.</p>
  
  <a href="mailto:{{ group.email | replace: "@", "+unsubscribe@" }}?subject=UNSUBSCRIBE&body=Send%20this%20email%20to%20unsubscribe%20from%20the%20{{ group.name}}%20group.%0D%0A%0D%0AYou%20must%20send%20the%20email%20from%20the%20same%20email%20address%20you%20signed%20up%20with%20in%20order%20for%20this%20to%20work." class="button" title="Unsubscribe from the {{ group.name }} Group (Opens a new email in a new window)" target="_blank">Unsubscribe from the {{ group.name }} group</a>

  
</details>
{% endfor %}

{% for group in projects-groups %}
{% if forloop.first == true %}
### Projects
{% endif %}
<details>
  <summary>{{ group.name }}</summary>
  {{ group.description | markdownify }}
  
  <h4>Subscribe to the {{ group.name }} group</h4>
  
  <p>You can subscribe to this group by <a href="{{ group.url }}" title="Open the Group for the {{ group.name }} (Opens in a new window)" target="_blank">visiting the Group page</a> or by sending an email to:
  <br><code>{{ group.email | replace: "@", "+subscribe@" }}</code></p>
  
  <a href="mailto:{{ group.email | replace: "@", "+subscribe@" }}?subject=SUBSCRIBE&body=Send%20this%20email%20to%20subscribe%20to%20the%20selected%20group.%0D%0A%0D%0AYou%20will%20receive%20a%20reply%20asking%20you%20to%20confirm%20your%20subscription.%0D%0A%0D%0AReply%20with%20a%20blank%20email%20to%20confirm%20your%20subscription.%0D%0A%0D%0AIf%20you%20change%20your%20mind%2C%20you%20can%20unsubscribe%20at%20any%20time%20by%20emailing%20{{ group.name }}%2Bunsubscribe%40groups.civilservice.lgbt" class="button" title="Subscribe to the {{ group.name }} Group (Opens a new email in a new window)" target="_blank">Subscribe to the {{ group.name }} group</a>


  You should receive an email asking you to confirm your subscription. Please click 'Reply' and send a blank email back. You should then get confirmation that you have subscribed to this Google Group. There are complete generic instructions at the bottom of this page.

  
  <h4>Unsubscribe from the {{ group.name }} group</h4>
  <p>If you want to stop receiving emails from this group send an email from the same email as you registered with to:
  <br><code>{{ group.email | replace: "@", "+unsubscribe@" }}</code>.</p>
  
  <a href="mailto:{{ group.email | replace: "@", "+unsubscribe@" }}?subject=UNSUBSCRIBE&body=Send%20this%20email%20to%20unsubscribe%20from%20the%20selected%20group.%0D%0A%0D%0AYou%20must%20send%20the%20email%20from%20the%20same%20email%20address%20you%20signed%20up%20with%20in%20order%20for%20this%20to%20work." class="button" title="Unsubscribe from the {{ group.name }} Group (Opens a new email in a new window)" target="_blank">Unsubscribe from the {{ group.name }} group</a>

  
</details>
{% endfor %}

## How to join a group

You can sign up to a Group via a web browser or by email. 

### Sign up via a web browser

To sign up to a group via a web browser, use the links in the drop down boxes above. You will be redirected to a Google Group page. On the Group page, click 'Join this group'. You may be asked to sign in with a Google account.

If you cannot access the page via your device, or you don't have a Google account, you can sign up via email.

### Sign up via email

To join a group:

1. Send an email to the email address of the group you want to subscribe to. The email address will be in the format <br>`NAME-OF-GROUP+subscribe@groups.civilservice.lgbt`
2. You will receive an automated reply from our email system within a few minutes. The email will be from an email address in the format <br>`NAME-OF-GROUP+subconfirm@groups.civilservice.lgbt`<br> Check your spam or junk folder if it doesn't arrive.
3. Send a reply to the email you receive. It doesn't matter what the message content is. The reply-to email address will be in the format <br>`NAME-OF-GROUP+subconfirm@groups.civilservice.lgbt`
4. You should now be subscribed to the group. You will receive email updates whenever our teams send one out.

## How to leave a group

To remove yourself from a group:

1. From the same email address as the one you subscribed with, send an email to the dedicated group unsubscribe email address. This is in the format <br>`NAME-OF-GROUP+unsubscribe@groups.civilservice.lgbt`
2. You should be unsubscribed within a few minutes.


