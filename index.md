---
layout: homepage
---

## About Me

I am a 3rd year Ph.D. student at the University of Virginia advised by Prof. [Zezhou Cheng](https://sites.google.com/site/zezhoucheng/). I do research in 3D Computer Vision.

Before joining UVA, I have completed master of Computer Science and Engineering at the [University of Michigan](https://umich.edu/). I was a member of [SLED lab](https://sled.eecs.umich.edu/). I obtained my bachelor's degree in [Applied and Computational Mathematics Science](https://acms.washington.edu/) at the [University of Washington](https://www.washington.edu/) where I worked with [Prof. Yunhe feng](https://yunhefeng.me/) on Responsible AI.

## Research Interests

Most of what is true about the physical world has never been written down. It is in how things look, move, break and fit together. I am interested in machines that learn it directly from the world.

That takes four things. **Seeing**: recovering the 3D structure and motion of the world from any video. **Reasoning**: tying language to what is really there, and checking every answer against it. **Acting**: robots and personal agents that put this to use next to people. **Explaining**: writing the physics down so that a machine can prove what it predicts. My work so far is on the first two. The other two are where I am going.

I believe in scale, and the world is the largest dataset there is.

A machine that learns from what people wrote can become as good as people. A machine that learns from the world itself can go further, and tell us things we do not know. That is the one I want to build.

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

- **Summer 2026** Internship at Meta.
- **Apr. 2026** WildRayZer has been selected as Highlight at CVPR 2026.
- **Feb. 2026** One first-author paper has been accepted to CVPR 2026.
- **Jan. 2026** One first-author paper has been accepted to ICLR 2026.
- **Nov. 2025** One first-author paper has been accepted to 3DV 2026.
- **Feb. 2025** Two first-author papers have been accepted to CVPR 2025.
- **Nov. 2024** One first-author paper has been accepted to TMLR.
- **Sep. 2024** One first-author paper has been accepted to NeurIPS 2024.
- **Aug. 2024** Join the University of Virginia advised by Zezhou Cheng.
- **Jan. 2024** Our first-author paper has been accepted by ICRA 2024.
- **Aug. 2022** Joined the SLED lab at the University of Michigan.


{% if site.show_blog %}
{% include_relative _includes/blog.md %}
{% endif %}

{% include_relative _includes/publications.md %}

{% include_relative _includes/services.md %}
