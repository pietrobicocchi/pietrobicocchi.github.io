---
layout: page
permalink: /publications/
title: publications
nav: true
nav_order: 1
---

<!-- _pages/publications.md -->

{% capture bib_count %}{% bibliography_count %}{% endcapture %}

{% if bib_count == '0' %}

<p>Coming soon.</p>

{% else %}

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>

{% endif %}
