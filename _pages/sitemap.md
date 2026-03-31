---
layout: archive
title: ""
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

<div class="section-card section-card--compact">
<h2>🗺️ Sitemap</h2>

<p>A list of all the posts and pages found on the site. For you robots out there is an <a href="{{ base_path }}/sitemap.xml">XML version</a> available for digesting as well.</p>
</div>

<div class="section-card">
<h3>Pages</h3>
{% for post in site.pages %}
  {% include archive-single.html %}
{% endfor %}
</div>

<div class="section-card">
<h3>Posts</h3>
{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}
</div>

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
{% unless collection.output == false or collection.label == "posts" %}
  {% capture label %}{{ collection.label }}{% endcapture %}
  {% if label != written_label %}
<div class="section-card">
<h3>{{ label | capitalize }}</h3>
  {% capture written_label %}{{ label }}{% endcapture %}
  {% endif %}
{% endunless %}
{% for post in collection.docs %}
  {% unless collection.output == false or collection.label == "posts" %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
{% unless collection.output == false or collection.label == "posts" %}
</div>
{% endunless %}
{% endfor %}
