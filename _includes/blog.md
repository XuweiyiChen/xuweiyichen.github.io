<h2 id="blog" style="margin: 2px 0px -15px;">Blog</h2>

<div class="publications">
<ol class="bibliography">

{% for post in site.data.blog.posts %}

<li>
<div class="pub-row">
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if post.image %}
    <a href="{{ post.link }}"><img src="{{ post.image }}" class="teaser img-fluid z-depth-1" alt="{{ post.title }}"></a>
    {% endif %}
    {% if post.badge %}
    <abbr class="badge">{{ post.badge }}</abbr>
    {% endif %}
  </div>
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <div class="title"><a href="{{ post.link }}">{{ post.title }}</a></div>
      <div class="author">{{ post.subtitle }}</div>
      <div class="periodical"><em>{{ post.date }}</em></div>
      <div class="links">
        <a href="{{ post.link }}" class="btn btn-sm z-depth-0" role="button" style="font-size:12px;">Read</a>
      </div>
  </div>
</div>
</li>

<br>

{% endfor %}

</ol>
</div>
