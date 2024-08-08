---
layout: page
title: Home
id: home
permalink: /
---

# Hi - I'm Scott! 👋

I'm an SEO based in the South West of England, currently working as SEO & Content Manager at Gymshark.

With a range of experience - from e-commerce to the third sector - I am passionate about driving organic growth. 

Welcome to my corner of the internet. It's nothing special. In fact, I spent a long time tweaking with fancy looking websites, but ultimately decided that I didn't need that. I didn't need the monthly hosting subscriptions. Instead, I've gone back to basics. 

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Not sure where to start? I'd recommend my <span style="font-weight: bold">[[About]]</span> page, where you can learn more about me. You'll find a list of my most recently updated notes below, too.
</p>



<strong>Recently updated notes</strong>

<ul>
  {% assign recent_notes = site.notes | sort: "last_modified_at_timestamp" | reverse %}
  {% for note in recent_notes limit: 5 %}
    <li>
      {{ note.last_modified_at | date: "%Y-%m-%d" }} — <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>
