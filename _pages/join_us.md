---
layout: page
title: Join us
permalink: /joinus/
nav: true
nav_order: 8
social: false # includes social icons at the bottom of the page
---

<hr>
<b>Unlock the Secrets of Coevolution with Diverse Perspectives!</b> Our team, at the intersection of plant pathology, ecology, evolution, theoretical and computational biology, and genomics, is expanding!

We encourage applications from bright minds in biology, mathematics, computer science, physics, genomics, and other quantitative or biological disciplines who are excited to explore the coevolutionary dance in wild plant pathosystems. Opportunities are available for Research Technicians, Undergraduate Researchers, Graduate Researchers, and Postdoctoral Fellows.

<a href='https://gradschool.utk.edu/future-students/office-of-graduate-admissions/applying-to-graduate-school/' target="_blank">Applying to the Graduate School.</a>

<a href="https://bredesencenter.utk.edu/genome-science/" target="_blank">Genome Science and Technology Program of University of Tennessee - Oak Ridge Innovation Institute.</a>

{% comment %}
SLIDESHOW - commented out until image sizing is resolved
<style>
  .joinus-layout { display: flex; gap: 2rem; align-items: flex-start; }
  .joinus-text { flex: 0 0 40%; }
  .joinus-slider { flex: 0 0 58%; }
  .landscape-swiper { height: 420px; }
  .landscape-swiper swiper-slide,
  .landscape-swiper swiper-slide figure,
  .landscape-swiper swiper-slide picture { display: block; width: 100%; height: 420px; margin: 0; padding: 0; }
  .landscape-swiper swiper-slide img { width: 100%; height: 420px; object-fit: cover; object-position: center; display: block; }
</style>
<div class="joinus-layout">
  <div class="joinus-text">
    ...text content...
  </div>
  <div class="joinus-slider">
    {% assign landscape_images = site.static_files | where_exp: "file", "file.path contains 'assets/img/landscape'" | where_exp: "file", "file.extname != '.webp'" | sample: 100 %}
    <swiper-container class="landscape-swiper" keyboard="true" navigation="true" pagination="true" pagination-clickable="true" space-between="30" pagination-dynamic-bullets="true" rewind="true" centered-slides="true" autoplay-delay="2500" autoplay-disable-on-interaction="false">
      {% for image in landscape_images %}
        {% assign img_path = image.path | remove_first: '/' %}
        <swiper-slide>{% include figure.liquid loading="eager" path=img_path class="img-fluid rounded z-depth-1" %}</swiper-slide>
      {% endfor %}
    </swiper-container>
  </div>
</div>
{% endcomment %}
