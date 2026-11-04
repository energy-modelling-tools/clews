---
layout: sub-page
title: CLEWs
permalink: /applications/
---

<section class="bg-gray-light container-lg p-responsive py-4 py-md-6 my-lg-6">
  <div class="text-center">
    <h2 class="alt-h2 mb-4">CLEWs Applications</h2>
  </div>
  <!-- CMS:section id=application_clews_applications -->
  <p class="lead mb-4">
    CLEWs has been applied in research and policy analysis across climate, land, energy and water systems. Featured publications are listed below.
  </p>
  <!-- /CMS:section -->

  <h2 class="alt-h2 text-center mb-3 mt-lg-6" id="more-than-just-code">{% octicon paintbrush height:36 %} Featured Publications</h2>
  {% for reference in site.data.publications %}
   <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
    {% include reference.html reference=reference %}
    </p>
  {% endfor %}
</section>
