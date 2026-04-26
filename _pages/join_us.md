---
layout: page
title: Join us
permalink: /joinus/
nav: true
nav_order: 8
social: false # includes social icons at the bottom of the page
images:
  slider: true
---

<style>
  .joinus-layout { display: flex; gap: 2rem; align-items: flex-start; }
  .joinus-text { flex: 0 0 40%; }
  .joinus-slider { flex: 0 0 60%; }
  .landscape-swiper { height: 480px; }
  .landscape-swiper swiper-slide img { width: 100%; height: 480px; object-fit: cover; object-position: center; }
</style>

<div class="joinus-layout">
  <div class="joinus-text">
    <hr>
    <b>Unlock the Secrets of Coevolution with Diverse Perspectives!</b> Our team, at the intersection of plant pathology, ecology, evolution, theoretical and computational biology, and genomics, is expanding!
    <br><br>
    We encourage applications from bright minds in biology, mathematics, computer science, physics, genomics, and other quantitative or biological disciplines who are excited to explore the coevolutionary dance in wild plant pathosystems. Opportunities are available for Research Technicians, Undergraduate Researchers, Graduate Researchers, and Postdoctoral Fellows.
    <br><br>
    <a href='https://gradschool.utk.edu/future-students/office-of-graduate-admissions/applying-to-graduate-school/' target="_blank">Applying to the Graduate School.</a>
    <br><br>
    <a href="https://bredesencenter.utk.edu/genome-science/" target="_blank">Genome Science and Technology Program of University of Tennessee - Oak Ridge Innovation Institute.</a>
  </div>
  <div class="joinus-slider">
    {% assign landscape_images = site.static_files | where_exp: "file", "file.path contains 'assets/img/landscape'" | where_exp: "file", "file.extname != '.webp'" | sample: 100 %}
    <swiper-container class="landscape-swiper" keyboard="true" navigation="true" pagination="true" pagination-clickable="true" space-between="30" pagination-dynamic-bullets="true" rewind="true" centered-slides="true" autoplay-delay="2500" autoplay-disable-on-interaction="false">
      {% for image in landscape_images %}
        <swiper-slide>{% include figure.liquid loading="eager" path=image.path class="img-fluid rounded z-depth-1" %}</swiper-slide>
      {% endfor %}
    </swiper-container>
  </div>
</div>
