---
permalink: /
title: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a researcher working on compression and acceleration of various deep learning architectures, including 2-D and 3-D Convolutional Neural Networks, Transformers, Large Language/Vision-Language Models, etc. My focus is on making the compression "hardware-friendly"--converting the theoretical reduction in model size into actual acceleration for real-time applications on resource-constrained devices (such as mobile phones, and reconfigurable devices--FPGA).

Education
======
- Ph.D in Computer Engineering
    - Northeastern University (Boston, USA), Sep 2017 -- Aug 2022
- M.S. in Electrical Engineering
    - University of Southern California (Los Angeles, USA), Aug 2014 -- May 2016
- B.S. in Electronics Information Science and Technology
    - Harbin Institute of Technology, Sep 2010 -- Jun 2014

Work Experience
======
- Assistant Professor
    - Beijing University of Technology, Nov 2022 -- Present
- Research Intern
    - Tencent America, LLC (Palo Alto, USA), May 2021 -- Aug 2021

Publications
======
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>

Teaching
======
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
