---
layout: about
title: about
permalink: /
subtitle: DPhil student, <a href="https://www.cs.ox.ac.uk/">Department of Computer Science</a>, University of Oxford

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular

selected_papers: true # includes a list of papers marked as "selected={true}"
social: false # icons are rendered at the end of the bio below, with email protection

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a DPhil student in Computer Science at the University of Oxford, supervised by
[Michael Wooldridge](https://www.cs.ox.ac.uk/people/michael.wooldridge/),
[J. Doyne Farmer](https://www.inet.ox.ac.uk/people/j-doyne-farmer) and
[Anisoara Calinescu](https://www.cs.ox.ac.uk/people/ani.calinescu/).
I am a member of the [Large Agent Collider (LAC)](https://largeagentcollider.github.io/) group,
[INET Oxford](https://www.inet.ox.ac.uk/) and the [BOLD Lab](https://bold-lab.ai/). My DPhil is funded by a
Jane Street Graduate Research Fellowship.

{% comment %}
TODO: rewrite the research paragraph below once the research direction settles (first drafted November 2026).
{% endcomment %}

My research is on multi-agent systems, combining differentiable simulation, agent-based modelling and reinforcement learning.

{% capture social_icons %}{% social_links %}{% endcapture %}
<div class="social"><div class="contact-icons">{{ social_icons | al_email_protect_html }}</div></div>
