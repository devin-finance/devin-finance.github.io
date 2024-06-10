---
layout: page
title: "The Working Capital Channel of Investment under Uncertainty"
permalink: /research/bwe
collection: Working Papers
excerpt: '_Abstract_: This study documents a novel working capital channel of investment under uncertainty, wherein uncertainty affects investment not through adjustment costs or irreversibility but through working capital and cash flows. The uncertainty comes from a prevalent supply chain phenomenon known as the bullwhip effect, where demand volatility is amplified upstream along the supply chain from retailers to raw materials suppliers.'
paperurl: null
---

## Research

{% for paper in site.data.papers %}
<div class="paper">
  <h3>{{ paper.title }}</h3>
  <p>{{ paper.authors }}</p>
  <p>{{ paper.journal }}</p>
  
  <!-- Abstract Button -->
  <button class="btn btn-primary" type="button" data-toggle="collapse" data-target="#abstract-{{ forloop.index }}" aria-expanded="false" aria-controls="abstract-{{ forloop.index }}">
    Show Abstract
  </button>
  
  <!-- Collapsible Abstract -->
  <div class="collapse" id="abstract-{{ forloop.index }}">
    <div class="card card-body">
      {{ paper.abstract }}
    </div>
  </div>
</div>
{% endfor %}
