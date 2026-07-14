---
title: About
layout: page
---
<div class="page-header">
    <h1 class="page-title">About</h1>
    <p class="page-subtitle">Senior Geospatial Software Engineer specializing in QGIS, Python, PostGIS and enterprise WebGIS — open-source contributor, consultant and technical trainer.</p>
</div>

<div class="about-grid">
    <div class="about-image">
        <img src="{{ site.url }}/{{ site.picture }}" alt="{{ site.name }}" />
    </div>
    <div class="about-content">
        <p>
            I'm <strong>Francisco José Raga López</strong>, a Senior Geospatial Software Engineer with a
            background in Cartography and Geodesy and a career dedicated to bridging geospatial engineering
            and software development.
        </p>
        <p>
            I hold a degree from the Universitat Politècnica de València and have spent my professional
            life designing and delivering GIS solutions — from desktop workflows and QGIS plugin development
            to large-scale WebGIS platforms and spatial data infrastructure. I work on national and
            international projects, building reliable data pipelines, custom tooling and production-ready
            mapping applications for organizations across the public and private sectors.
        </p>
        <p>
            Under <a href="https://github.com/{{ site.github }}" target="_blank" rel="noopener">All4Gis</a>,
            I maintain an active open-source portfolio of QGIS plugins, Python libraries and WebGIS
            components. I also provide freelance development, GIS consulting and hands-on technical training
            for teams looking to adopt or advance their open-source geospatial capabilities.
        </p>
        <p>
            I remain closely connected to the geospatial community, with a long-standing commitment to
            open tools and to building software that delivers measurable value in real-world workflows.
        </p>
    </div>
</div>

<h2>Skills</h2>
<ul class="skill-list">
    {% for category in site.data.skills.categories %}
        {% for skill in category.items %}
        <li>{{ skill }}</li>
        {% endfor %}
    {% endfor %}
</ul>
