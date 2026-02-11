---
layout: default
title: Projects
---

# Projects

Highlighting AI/ML, IoT, and creative tech fusions from my BS at COMSATS.

{% for project in site.data.projects %}  // Jekyll can loop if you add to _config, but for now, hardcode or use JS later
## {{ project.title }}

{{ project.description }}

Tech: {{ project.tech | join: ", " }}

[Demo/Link]({{ project.link }})

![Project Image]({{ project.image }})
{% endfor %}

<!-- Add dynamic JS section below -->
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<canvas id="projectChart"></canvas>
