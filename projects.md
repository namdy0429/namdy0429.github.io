---
layout: page
permalink: /projects/
title: Projects
class: projects
---

{:.hidden}
# Projects

{:.lead}
Projects I have worked on for school, work, or fun can be found on [GitHub](https://github.com/namdy0429).

<div class="grid">
  {% for project in site.data.projects %}
    {% include project.html project=project %}
  {% endfor %}
</div>
