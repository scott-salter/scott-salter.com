---
layout: page
title: Home
id: home
permalink: /
---

# Hi - I'm Scott! 👋

I'm an SEO based in the South West of England, currently working as SEO & Content Manager at Gymshark.

<img src="https://media.licdn.com/dms/image/D4E03AQGkrVoHxjVz-Q/profile-displayphoto-shrink_800_800/0/1678379575775?e=1720051200&v=beta&t=opclBqkIcYlcr_v_79LuTbvgEqGCy1vZHy5DoLOXJ-w" alt="headshot of Scott Salter" style="width:200px;height:300px;"/>

Welcome to my website. You'll find a mix of my work, some thoughts, but also some in-progress ideas as I learn in public. 

These ideas and notes are written for myself and not necessarily for a third-party reader. So some notes may not make total sense, but that's okay. Some notes or ideas may be innacurate - and that's okay too. 
〰️

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Not sure where to start? I'd recommend my list of <span style="font-weight: bold">[[Topics]]</span> to get started on your exploration. You'll find a list of my most recently updated notes below, too.
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
