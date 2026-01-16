---
layout: homepage
---

## About Me

I am a 2nd year Ph.D. student at the University of Virginia advised by Prof. [Zezhou Cheng](https://sites.google.com/site/zezhoucheng/). I do research in 3D Computer Vision.

Before joining UVA, I have completed master of Computer Science and Engineering at the [University of Michigan](https://umich.edu/). I was a member of [SLED lab](https://sled.eecs.umich.edu/). I obtained my bachelor's degree in [Applied and Computational Mathematics Science](https://acms.washington.edu/) at the [University of Washington](https://www.washington.edu/) where I worked with [Prof. Yunhe feng](https://yunhefeng.me/) on Responsible AI.

## Research Interests

My research centers on scalable approaches to 3D Computer Vision, Language, and Robotics. Currently, I am focusing on two key areas:

- Developing Vision-Centric 3D Foundational Models.
- Grounding Language Concepts in 3D Environments and Robotic Actions.

## Internships

<div class="internship-list">
{% for internship in site.data.internships %}
<div class="internship-item">
  <img src="{{ internship.logo }}" alt="{{ internship.company }} logo" class="internship-logo">
  <div class="internship-info">
    <strong>{{ internship.company }}</strong><br>
    <em>{{ internship.duration }}</em>
  </div>
</div>
{% endfor %}
</div>

<style>
  .internship-list {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;
  }
  .internship-item {
    display: flex;
    align-items: center;
    border: 1px solid #ddd;
    padding: 10px;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  }
  .internship-logo {
    width: 50px;
    height: 50px;
    margin-right: 15px;
    border-radius: 50%;
  }
  .internship-info {
    font-size: 0.9rem;
  }
</style>

## News

- **[Nov. 2025]** One first-author paper has been accepted to 3DV 2026.
- **[Feb. 2025]** Two first-author papers have been accepted to CVPR 2025.
- **[Nov. 2024]** One first-author paper has been accepted to TMLR.
- **[Sep. 2024]** One first-author paper has been accepted to NeurIPS 2024.
- **[Aug. 2024]** Join the University of Virginia advised by Zezhou Cheng.
- **[Jan. 2024]** Our first-author paper has been accepted by ICRA 2024.
- **[Aug. 2022]** Joined the SLED lab at the University of Michigan.


{% include_relative _includes/publications.md %}

{% include_relative _includes/services.md %}
