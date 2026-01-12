---
layout: page
title: 32-bit RISC-V (RV32I) Multicycle Processor
description: 
img: assets/img/gtkwave.png
importance: 5
category: 
---

<strong>Github Source Files</strong>: [https://github.com/Ahan-Trivedi2/RISC-V-Processor](https://github.com/Ahan-Trivedi2/RISC-V-Processor)

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/gtkwave.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    <em>Image of GTKWave waveform</em>
</div>

For my computer architecture course, I worked on a team to design and implement a 32-bit RV32I RISC-V processor using an unpipelined, multicycle architecture. The processor follows a Von Neumann model with a finite state machine controlling instruction execution across multiple stages, including instruction fetch, execution, memory access, and writeback. Our design supports the core RV32I instruction set and was verified using a comprehensive testbench that ran compiled RISC-V machine code, along with waveform analysis in GTKWave to validate correct control flow and datapath behavior.

<strong>Check out my full report below: </strong>

<div style="position: relative;">
  <a
    href="{{ '/assets/pdf/RV32I.pdf' | relative_url }}"
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
      src="{{ '/assets/pdf/RV32I.pdf' | relative_url }}"
      width="100%"
      height="100%"
      style="border: 0;"
    ></iframe>
  </div>
</div>


