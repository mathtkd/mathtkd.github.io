---
layout: default
title: ホーム
---
# 授業資料置き場
<div class="grid">
{% for g in "1nen,2nen,3nen" | split: "," %}
  <div>
    <h3>{% if g == "1nen" %}中1{% elsif g=="2nen" %}中2{% else %}</h3>
    <p>
    {% assign subs = site.data.subjects.grades[g] %}
    {% for s in subs %}
      <a href="/{{ g }}/{{ s }}/">{{ site.data.subjects.labels[s] }}</a>
    {% endfor %}
    </p>
  </div>
{% endfor %}
</div>

サイト準備中。
