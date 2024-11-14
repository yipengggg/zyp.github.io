<h2 id="Research_Projects" style="margin: 2px 0px -15px;">Research Projects</h2>

<div class="Research_Projects">
<ol class="bibliography">

{% for link in site.data.Research_Projects.main %}

<li>
<div class="pub-row">
  <!-- 图片部分 -->
  <div class="col-sm-3 abbr" style="position: relative;padding-right: 15px;padding-left: 15px;">
    {% if link.image %} 
    <img src="{{ link.image }}" class="teaser img-fluid z-depth-1" style="width=100;height=40%">
    {% endif %}
  </div>

  <!-- 内容部分 -->
  <div class="col-sm-9" style="position: relative;padding-right: 15px;padding-left: 20px;">
      <!-- 项目标题 -->
      <div class="title">{{ link.title }}</div>
      <div class="periodical"><em>{{ link.conference }}</em></div>
      {% if link.mains_content %}
      <div class="content">{{ link.mains_content }}</div>
      {% endif %}    
      {% if link.notes %}
      <strong><i style="color:#e74d3c">{{ link.notes }}</i></strong>
      {% endif %}
  </div>
</div>
</li>
<br>

{% endfor %}

</ol>
</div>
