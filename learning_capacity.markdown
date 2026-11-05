---
layout: sub-page
title: CLEWs
permalink: /learning_capacity/
---
<!-- [jekyll-organization]: https://github.com/jekyll

This is the base Jekyll theme. You can find out more info about customizing your Jekyll theme, as well as basic Jekyll usage documentation at [jekyllrb.com](https://jekyllrb.com/)

You can find the source code for Minima at GitHub:
[jekyll][jekyll-organization] /
[minima](https://github.com/jekyll/minima)

You can find the source code for Jekyll at GitHub:
[jekyll][jekyll-organization] /
[jekyll](https://github.com/jekyll/jekyll) -->

<!-- <div class="container-lg p-responsive py-4 py-lg-6 my-xl-4 text-center">
    <h1 class="alt-h1 mb-2 text-white">About CLEWs</h1>
</div> -->
<!-- <h3 class="alt-h3 text-float-left mb-3 mt-lg-6" id="more-than-just-code">Growing of CLEWs</h2> -->
<section class="bg-gray-light container-lg p-responsive py-4 py-md-6 my-lg-6">

  <div class="container-lg p-responsive py-4 py-md-6 ">
      <h3 class="alt-h3 text-float-left mb-3 mt-lg-6" id="more-than-just-code">
            <a href="https://www.open.edu/openlearncreate/course/index.php?categoryid=528">Introduction to CLEWs</a>
      </h3>
      <div class="col-md-12 animate-out mb-2">
          <!-- CMS:section id=learning_capacity_growing_of_clews_introduction_to -->
          <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
            For those starting their journey with CLEWs or seeking foundational knowledge, an open-access course is available online. This course comprises 11 comprehensive lectures that introduce the key concepts of the CLEWs approach, its methodologies, and practical applications. The self-paced format ensures accessibility for individuals worldwide, allowing learners to engage with the material at their convenience.
            </p>
          <!-- /CMS:section --> 
      </div>
      <h3 class="alt-h3 text-float-left mb-3 mt-lg-6" id="more-than-just-code">
        <a href="https://climatecompatiblegrowth.com/energy-modelling-platform/  ">Practical Training under the EMP</a>
      </h3>
        <div class="col-md-12 animate-out mb-2">
            <!-- CMS:section id=learning_capacity_practical_training_under_the_emp -->
            <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
            To deepen understanding and provide hands-on experience, the Climate Compatible Growth (CCG) programme co-hosts 3 week-long capacity-building events under the Energy Modelling Platform (EMP). These intensive workshops bring together experts, policymakers, and aspiring modelers to collaborate and learn in a dynamic environment. Over the course of three structured weeks, participants gain practical skills in applying the CLEWs framework to real-world challenges, engage in peer-to-peer learning, and explore the latest innovations in integrated system modeling. 
          </p>
            <!-- /CMS:section --> 
        </div>
          <div class="my-4 my-lg-6 clearfix gutter-spacious">
            <h3 class="alt-h3 text-center mb-3">Explore EMP Events</h3>
            {% for event in site.data.learning_events.events %}
            <div class="col-md-4 float-left animate-out mb-4">
              <h3 class="alt-h3 mb-3">{{ event.title }}</h3>
              <p><img src="{{ event.image }}" class="img-border" alt="{{ event.alt }}"/></p>
              <p class="text-gray">{{ event.description }}</p>
              {% if event.outputs and event.outputs.size > 0 %}
              <details>
                <summary class="btn btn-sm btn-outline">Show Outputs</summary>
                <ul class="mt-2">
                  {% for output in event.outputs %}
                  <li>{{ output.flag }} <strong>{{ output.country }}</strong>:
                    <a href="{{ output.url }}" target="_blank">{{ output.title }}</a>
                  </li>
                  {% endfor %}
                </ul>
              </details>
              {% endif %}
            </div>
            {% endfor %}
          </div>
          {% if site.data.learning_events.adjacent_events and site.data.learning_events.adjacent_events.size > 0 %}
          <div class="clearfix gutter-spacious mt-5">
            <div class="col-md-12 animate-out mb-4">
              <h3 class="alt-h3 mb-3">EMP-Adjacent Events</h3>
              <ul>
                {% for adjacent in site.data.learning_events.adjacent_events %}
                <li>{{ adjacent.flag }}
                  <a href="{{ adjacent.url }}" target="_blank">{{ adjacent.title }}</a>
                </li>
                {% endfor %}
              </ul>
            </div>
          </div>
          {% endif %}
    </div>
  <h3 class="alt-h3 text-float-left mb-3 mt-lg-6" id="more-than-just-code">
    <a href="https://climatecompatiblegrowth.com">On-demand Training by CCG</a>
  </h3>
  <div class="col-md-12 animate-out mb-2">
      <!-- CMS:section id=learning_capacity_on_demand_training_by_ccg -->
      <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
        For those with specific needs or unique project requirements, CCG also offers on-demand training tailored to your objectives. This flexible option allows organizations, teams, or individuals to receive customized guidance on applying the CLEWs framework to their specific context. 
      </p>
      <!-- /CMS:section -->
  </div>
  <div class="col-md-12 animate-out mb-2">
      <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
        <a href="mailto:ccg@lboro.ac.uk?subject=Inquiry%20about%20CLEWs%20Training&body=Hello,%20I%20would%20like%20to%20know%20more%20about..." class="btn btn-outline">Contact CCG</a>  
      </p>
  </div>
  <div class="col-md-12 animate-out mb-2">
      <!-- CMS:section id=learning_capacity_on_demand_training_by_ccg_2 -->
      <p class="alt-lead text-gray text-justify-between col-md-15 mx-auto">
      Whether through online learning or immersive workshops, the CLEWs community’s goal is to empower participants with the knowledge and tools to address complex resource challenges holistically. By fostering a growing community of CLEWs practitioners, let’s aim to enhance global capacity for sustainable and integrated systems planning.
      </p>
      <!-- /CMS:section -->
      <p class="alt-lead text-gray text-center col-md-10 mx-auto">
        <a href="{{ '/' | relative_url }}" class="btn btn-outline">For more information, visit the CLEWs website</a>
      </p>
  </div>
</section>