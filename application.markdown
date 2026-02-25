---
theme: jekyll-theme-primer
layout: sub-page
title: CLEWs
permalink: /applications/
---

<div class="container-lg p-responsive py-4 py-md-6 ">
<h2 class="alt-h2 text-center mb-3 mt-lg-6" id="more-than-just-code">{% octicon paintbrush height:36 %}
Featured Publications</h2>
{% for reference in site.data.publication %}
 <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto" style="text-align: justify; font-size: 0.875em;">
  {% include reference.html reference=reference %}
  </p>
{% endfor %}
</div>
<!-- <script>
    window.location.href = "/coming-soon/";
</script> -->
