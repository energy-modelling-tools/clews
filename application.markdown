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
</section>

<section class="container-lg p-responsive py-4 py-md-6 my-lg-6">
  <div class="recommended-reading">
    <h2 class="alt-h2 text-center mb-4">Featured Publications</h2>
    <!-- CMS:section id=application_featured_publications -->
    <p class="text-center mb-5">Peer-reviewed papers that use or develop the CLEWs framework.</p>
    <!-- /CMS:section -->

    <div class="publications-list">
      {% for publication in site.data.publications %}
      <div class="publication-item mb-4 p-4 border border-gray-200 rounded">
        <h4 class="publication-title mb-2">
          <a href="{{ publication.url }}" target="_blank" class="text-decoration-none">
            {{ publication.title }}
          </a>
        </h4>
        <p class="publication-authors text-muted mb-2">
          {{ publication.authors }} ({{ publication.year }})
        </p>
        <p class="publication-journal mb-2">
          <em>{{ publication.journal }}</em>
        </p>
        <p class="publication-abstract text-justify">
          {{ publication.abstract }}
        </p>
      </div>
      {% endfor %}
    </div>
  </div>
</section>

<style>
.recommended-reading {
  max-width: 1000px;
  margin: 0 auto;
}
.publications-list {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}
.publication-item {
  background: white;
  padding: 2rem;
  border-radius: 12px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
  border-left: 4px solid #0366d6;
}
.publication-title {
  font-size: 1.2rem;
  font-weight: 600;
  line-height: 1.4;
}
.publication-authors {
  color: #586069;
}
.publication-abstract {
  color: #586069;
  line-height: 1.6;
}
</style>
