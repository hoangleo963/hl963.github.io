---
permalink: /index.html
layout: default
---

## About Me

Hi, I am **Hoang Nguyen-Tien** (in Vietnamese: *Nguyễn Tiến Hoàng*), a 4th year PhD student in Mathematics at the University of Wisconsin-Madison, advised by Professor [Yingkun Li](https://lykpi.github.io). I am interested in automorphic forms.


## Research

{% assign preprints = site.data.publications | where: "section", "preprints" | sort: "sort_date" | reverse %}
{% assign publications = site.data.publications | where: "section", "publications" | sort: "sort_date" | reverse %}
{% assign preprint_count = preprints | size %}
{% assign publication_count = publications | size %}
{% assign total_count = preprint_count | plus: publication_count %}

{% if preprint_count > 0 %}
### Preprints

<ol class="publications" reversed="reversed" start="{{ total_count }}">
{% for publication in preprints %}
  <li>{{ publication.text | markdownify }}</li>
{% endfor %}
</ol>
{% endif %}

{% if publication_count > 0 %}
### Publications

<ol class="publications" reversed="reversed" start="{{ publication_count }}">
{% for publication in publications %}
  <li>{{ publication.text | markdownify }}</li>
{% endfor %}
</ol>
{% endif %}
