---
layout: page
title: 4-Bit Shift Register Design & Layout
description: 
img: assets/img/fbsr.png
importance: 4
category: 
---
<strong>Github Source Files</strong>: [https://github.com/Ahan-Trivedi2/Mixed-Analog-Digital-VLSI/tree/main/Miniproject2](https://github.com/Ahan-Trivedi2/Mixed-Analog-Digital-VLSI/tree/main/Miniproject2)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fbsr.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <em>Screenshot of final CSRL 4-bit shift register layout</em>
</div>

For my Mixed Analog-Digital VLSI course, I designed and verified a rising-edge-triggered CSRL D flip-flop and composed it into a 4-bit shift register using the Sky130 CMOS PDK. I completed the full transistor-level design flow, including schematic capture and transient simulation across multiple process corners to validate robust operation under variation. I then implemented a compact, abuttable standard-cell layout in Magic optimized for minimal width, tiled the cells to form the complete shift register, and verified the design through DRC and layout-versus-schematic (LVS) checks using the OSS CAD Suite. This project was inspired from Massimo Sivilotti's PHD thesis at Caltech on CMOS Single Phase Registers.

<strong>Check out my full report below: </strong>

<div style="position: relative;">
  <a
    href="{{ '/assets/pdf/Miniproject2.pdf' | relative_url }}"
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
      src="{{ '/assets/pdf/Miniproject2.pdf' | relative_url }}"
      width="100%"
      height="100%"
      style="border: 0;"
    ></iframe>
  </div>
</div>
