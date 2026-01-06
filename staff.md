---
layout: default
title: Staff
---
<div class="section">
  <h1 class="header">Our Staff</h1>

  <div class="row">
    {% for author in site.authors %}
      <div class="col s12 m6 l4">
        <div class="card">
          <div class="card-content">
            <span class="card-title">{{ author.name }}</span>
            <p class="blue-text">{{ author.position }}</p>
            <div class="divider"></div>
            <div class="section">
              {{ author.content | markdownify }}
            </div>
          </div>
          <div class="card-action">
            <a href="{{ author.url }}">View Profile</a>
          </div>
        </div>
      </div>
    {% endfor %}
  </div>
</div>