---
layout: page
title: 7-Bit DAC Design & Layout
description: 
img: assets/img/DAC.png
importance: 1
category: 
---

<strong>Github Source Files</strong>: [https://github.com/Ahan-Trivedi2/mosfet-dac](https://github.com/Ahan-Trivedi2/mosfet-dac)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/DAC.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <em>Screenshot of final DAC layout</em>
</div>

For my Mixed Analog-Digital VLSI course, I worked on a team of three to design and layout a seven-bit current-output digital-to-analog converter (DAC) implemented using a MOSFET-based R–2R-like ladder network in the SkyWater 130nm CMOS (sky130pdk) process. Operating from a 1.8V single-ended supply, the DAC converts seven digital inputs into an analog output current capable of sourcing or sinking with less than 0.5 %/V variation across at least 80% of the supply range and minimal dependence on VDD. The design achieves differential and integral nonlinearities (DNL/INL) below 2 LSB and 4 LSB under nominal conditions, and within 8 LSB under mismatch as verified through Monte Carlo simulations in Ngspice. A single external resistor provides the bias current, and the design passes all DRC and LVS checks. Layout practices such as symmetry, dummy devices, and selective common-centroiding were used to minimize mismatch, and the architecture incorporates subcircuits including a bootstrap bias generator (BBG), forward-voltage follower (FVF), cascode current mirror (CCM), and a current-steering output stage, inspired by [Hammerschmied and Huang’s untrimmed 10-bit MOSFET DAC](https://ieeexplore.ieee.org/document/705353).

<strong>Check out my full report below: </strong>

<div style="position: relative;">
  <a
    href="{{ '/assets/pdf/MOSDAC_Report.pdf' | relative_url }}"
    target="_blank"
    rel="noopener"
    title="Open PDF"
    style="
      position: absolute;
      right: 0;
      top: -2.5rem;
      font-size: 1.5rem;
    "
  >
    <i class="fas fa-file-pdf"></i>
  </a>

  <div style="width: 100%; height: 85vh;">
    <iframe
      src="{{ '/assets/pdf/MOSDAC_Report.pdf' | relative_url }}"
      width="100%"
      height="100%"
      style="border: 0;"
    ></iframe>
  </div>
</div>


