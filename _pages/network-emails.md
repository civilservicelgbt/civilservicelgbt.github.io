---
layout: page
title: Network emails
excerpt: "All email addresses for all departmental networks."
permalink: /networks/network-emails
---
<div hidden markdown=1>
{% assign networks = site.data.networks | where_exp: 'network', 'network.type == "Departmental" and network.email != ""'%}
{% for network in networks %}
- {{ network.email }}
{% endfor %}
</div>