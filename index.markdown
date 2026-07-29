---
permalink: /index.html
layout: default
---

## About Me

Hi, I am **Hoang Nguyen-Tien** (in Vietnamese: *Nguyễn Tiến Hoàng*, a 4th year PhD student in Mathematics at the University of Wisconsin-Madison, advised by Professor [Yingkun Li](https://lykpi.github.io). I am interested in automorphic forms.


## Publications

{% assign sorted_publications = site.data.publications | sort: "sort_date" | reverse %}
<ol class="publications" reversed="reversed">
{% for publication in sorted_publications %}
  <li>{{ publication.text | markdownify }}</li>
{% endfor %}
</ol>
