---
title: "Publications"
layout: gridlay
sitemap: false
permalink: /publications/
---

<style>
.jumbotron{
    padding:3%;
    padding-bottom:10px;
    padding-top:10px;
    margin-top:10px;
    margin-bottom:30px;
}
</style>

## Publications
##### (Citations: {{ site.data.scholar.citations }} | h-index: {{ site.data.scholar.h_index }} | i10-index: {{ site.data.scholar.i10_index }} by [Google Schalor](https://scholar.google.com/citations?user={{site.data.scholar.id}}))



<div class="jumbotron">
### Refereed journal articles
{% bibliography --query @article %}
</div>

<div class="jumbotron">
### Refereed conference proceedings
{% bibliography --query @inproceedings %}
</div>

<div class="jumbotron">
### Other publications
{% bibliography --query @thesis,@report %}
</div>

