---
layout: page
title: internships
permalink: /internships/
description: I've had the opportunity to work on impactful technology!
nav: true
nav_order: 2
---

<div class="projects">
  {%- assign sorted_internships = site.internships | sort: "importance" -%}

  <div class="container px-0">
    <div class="row row-cols-1 row-cols-md-2 g-4">
      {%- for project in sorted_internships -%}
        <div class="col">
          {% include projects.html %}
        </div>
      {%- endfor -%}
    </div>
  </div>
</div>

