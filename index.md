---
layout: default
title: Home
---

An increasing number of researchers are sharing their grant proposals
openly. They do this to open up science so that all stages of the process can
benefit from better interaction and communication and to provide examples for
younger scientists writing grants. This is a list of some of these proposals to
help you find them.

<table>
  <tr>
	<th>Year</th>
	<th>Funder</th>
	<th>Title</th>
	<th>Author</th>
  </tr>
{% for grant in site.grants %}
  <tr>
    <td>{{ grant.year }}</td>
	<td>{{ grant.funder }}</td>
	<td><a href="{{ grant.link }}">{{ grant.title }}</a></td>
    <td>{{ grant.author }}</td>
  </tr>
{% endfor %}
