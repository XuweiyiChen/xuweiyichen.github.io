<h2 id="publications" style="margin: 2px 0px -15px;">Selected Publications</h2>

<div class="publications">
<ol class="bibliography">

{% for link in site.data.publications.main %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
    {% if link.conference_short %} 
    <abbr class="badge">{{ link.conference_short | replace: "(Highlight)", "<span style='color:#e74d3c'>(Highlight)</span>" }}</abbr>
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      {% capture title_href %}{% if link.pdf %}{{ link.pdf }}{% elsif link.blog and site.show_blog %}{{ link.blog }}{% endif %}{% endcapture %}
      <div class="title"><a{% if title_href != "" %} href="{{ title_href }}"{% endif %}>{{ link.title }}</a></div>
      <div class="author">{{ link.authors | replace: "Xuweiyi Chen", "<span class='me'>Xuweiyi Chen</span>" }}</div>
      <div class="periodical"><em>{{ link.conference }}</em>
      </div>
      <div class="links">
        {% if link.pdf %} 
        <a href="{{ link.pdf }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">PDF</a>
        {% endif %}
        {% if link.pdf_soon %}
        <a class="btn btn-sm z-depth-0" aria-disabled="true" style="font-size:12px; opacity:0.5; pointer-events:none; white-space:nowrap;">PDF (soon)</a>
        {% endif %}
        {% for name in link.soon %}
        <a class="btn btn-sm z-depth-0" aria-disabled="true" style="font-size:12px; opacity:0.5; pointer-events:none; white-space:nowrap;">{{ name }} (soon)</a>
        {% endfor %}
        {% if link.code %} 
        <a href="{{ link.code }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Code</a>
        {% endif %}
        {% if link.page %} 
        <a href="{{ link.page }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Project Page</a>
        {% endif %}
        {% if link.blog and site.show_blog %}
        <a href="{{ link.blog }}" class="btn btn-sm z-depth-0" role="button" style="font-size:12px;">Blog</a>
        {% endif %}
        {% if link.video %} 
        <a href="{{ link.video }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Video</a>
        {% endif %}
        {% if link.livedemo %} 
        <a href="{{ link.livedemo }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Live Demo</a>
        {% endif %}
        {% if link.dataset %} 
        <a href="{{ link.dataset }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">Dataset</a>
        {% endif %}
        {% if link.bibtex %} 
        <a href="{{ link.bibtex }}" class="btn btn-sm z-depth-0" role="button" target="_blank" style="font-size:12px;">BibTex</a>
        {% endif %}
        {% if link.notes %} 
        <strong> <i style="color:#e74d3c">{{ link.notes }}</i></strong>
        {% endif %}
        {% if link.others %} 
        {{ link.others }}
        {% endif %}
      </div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>

