---
layout: homepage
---

## About Me

I am a 3rd year Ph.D. student at the University of Virginia advised by Prof. [Zezhou Cheng](https://sites.google.com/site/zezhoucheng/). I do research in 3D Computer Vision.

Before joining UVA, I have completed master of Computer Science and Engineering at the [University of Michigan](https://umich.edu/). I was a member of [SLED lab](https://sled.eecs.umich.edu/). I obtained my bachelor's degree in [Applied and Computational Mathematics Science](https://acms.washington.edu/) at the [University of Washington](https://www.washington.edu/) where I worked with [Prof. Yunhe feng](https://yunhefeng.me/) on Responsible AI.

## Research Interests

Much of what we know about the physical world is never written down. We learn it by watching things move, seeing how they fit together, and discovering what happens when we act on them. I want to build machines that learn this way: through observation and interaction, with language as a guide and the world as a test.

My research focuses on visual perception and grounded reasoning: recovering 3D structure and motion from video, and connecting language to visual evidence so that a model's conclusions can be checked against what it observes. I believe in scale: these models should learn from the world itself, with as little human labelling as possible.

I am now extending this work toward action and scientific understanding. On real robots, this means using what they perceive to act alongside people and learn from the consequences. For science, it means turning learned patterns into explicit physical models that make testable predictions.

My long-term goal is to build machines that use observations to form hypotheses, use actions to test them, and revise their understanding when the world surprises them. I want these machines to help us discover things we do not yet know.

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
