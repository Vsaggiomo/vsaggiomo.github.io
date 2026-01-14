---
layout: page
title: project 2
description: Sensing From the Lab to the Field
img: assets/img/sens2.jpg
importance: 2
category: work
related_publications: true
giscus_comments: false
---

My interest in sensing focuses on moving sophisticated analytical capabilities out of the laboratory and into the hands of the people who need them. We develop decentralized, low-cost diagnostic tools that prioritize ease of use, sustainability, and field-readiness. By combining clever material science with open-source electronics, I aim to create sensing platforms that are as effective in a remote field site or a home kitchen as they are in a high-end research facility.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sens3.jpg" title="arduino" class="img-fluid rounded z-depth-1" %}
    </div>
     <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sens4.jpg" title="paper" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sens7.jpg" title="tcup" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

###Molecular Diagnostics and DNA Detection


I am particularly interested in isothermal nucleic acid amplification (LAMP) as a robust alternative to PCR for rapid pathogen detection. To bridge the gap between "bench and bedside," we have developed various non-instrumental and low-cost hardware solutions:

The T-Cup{% cite velders2022t %}: A "non-instrument" device for SARS-CoV-2 detection that repurposes aluminum coffee capsules and phase-change materials (PCM) to maintain a steady 65 °C. It is scalable, sustainable, and requires only boiling water to run.

Arduino LAMP Shields{% cite velders2018loop %}: For more automated needs, I designed battery-operated Arduino shields that offer one-button DNA detection with naked-eye results, making molecular diagnostics accessible for field research.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sens1.jpg" title="scope" class="img-fluid rounded z-depth-1" %}
    </div>
     <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sens5.jpg" title="scope2" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sens6.jpg" title="scope3" class="img-fluid rounded z-depth-1" %}
    </div>
</div>

###Physical and Visual Sensing


Beyond molecular markers, I am interested in developing tools to detect and identify micro-entities—from parasite eggs to microplastics—using accessible hardware and innovative fabrication:

ESPressoscope{% cite li2024espressoscope %}: A modular, ESP32-based digital microscopy platform. Designed for in-situ monitoring, this low-cost "design pattern" allows researchers to build mission-specific microscopes, such as the Anglerfish for underwater ecological observation or time-lapse systems for incubator cell cultures.

Staircase Microfluidics{% cite staircase2023 %}: To simplify the detection of microparticles, I pioneered a "Z-axis" approach to microfluidics. By using the layer resolution of consumer 3D printers to create staircase structures, we can size-sort particles (parasites, zooplankton, microplastics) down to 25 µm without the need for high-resolution lithography.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/sens8.jpg" title="simba" class="img-fluid rounded z-depth-1" %}
    </div>
</div>