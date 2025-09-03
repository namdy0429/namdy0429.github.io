---
layout: page
permalink: /teaching/
title: Teaching
---

<style>
.teaching-table {
  width: 100%;
  border-collapse: collapse;
  margin-bottom: 2rem;
}

.teaching-table td {
  padding: 0.5rem 1rem 0.5rem 0;
  vertical-align: top;
  border: none;
}

.teaching-table .year-col {
  width: 15%;
  font-weight: normal;
}

.teaching-table .role-col {
  width: 30%;
  color: #6b6b6b;
}

.teaching-table .course-col {
  width: 55%;
}

.teaching-table .course-col h3 {
  margin: 0;
  font-size: 1.1rem;
  font-weight: normal;
}
</style>

<table class="teaching-table">
  {% for item in site.data.teaching %}
  <tr>
    <td class="year-col">{{ item.year }}</td>
    <td class="role-col">{{ item.role }}</td>
    <td class="course-col">
      <h3>
        {% if item.link %}
          <a href="{{ item.link }}">{{ item.title }}</a>
        {% else %}
          {{ item.title }}
        {% endif %}
      </h3>
      <div style="color: #6b6b6b; font-size: 0.9rem;">{{ item.location }}</div>
    </td>
  </tr>
  {% endfor %}
</table>