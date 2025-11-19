---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% include base_path %}

# Spatial Web

Spatial Web -- the overlay of virtual content on top of the physical world, holds promise for dramatically changing many applications from navigation, to engineering, education and more. A broad range of new tools and infrastructure are needed to make the Spatial Web "real" and to make it easy for developers to create and publish Spatial Web content and applications. The goal of this project is to develop a coherent architecture for the Spatial Web. This includes tools and algorithms for each step in the process of generating a Spatial Web view for the user.

The first step in this process is the OpenFLAME (Open Federated Localization and Mapping Engine) project. OpenFLAME is a federated platform for hosting, organizing, and discovering digital maps. The vision of OpenFLAME is to enable world-scale mapping to support the next generation of spatial applications.

<p align="center">
  <a href="https://openflam.github.io/">
    <img src= 
      "{{ "/images/openflame_logo.png" | prepend: base_path }}"
      alt="OpenFLAME Logo" 
      width="200"/>
  </a>
</p>


# Publications

{% for post in site.publications reversed %}
  {% if post.selected %}
    {% include single-publication.html post=post %}
  {% endif %}
{% endfor %}