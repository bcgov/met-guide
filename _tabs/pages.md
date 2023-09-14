---
# the default layout is 'page'
title: Pages & Features
icon: fas fa-info-circle
order: 4
---

<div id="post-list" {% unless has_paginator %} class="mb-5" {% endunless %}>
  <div class="row">
{% assign filtered_posts = site.posts | where_exp:"post", "post.categories contains 'pages/features'" | sort: "pages_and_features_sort_order" %}
    {% for post in filtered_posts %}
    <div class="col-md-6 col-lg-4">
      <a href="{{ post.url | relative_url }}" class="card-wrapper">
        <div class="card post-preview flex-md-row-reverse">
          <div class="card-body d-flex flex-column">
            <h1 class="card-title my-2 mt-md-0">{{ post.title }}</h1>

            <div class="card-text post-content mt-0 mb-2">
              <p>
                {% include no-linenos.html content=post.content %} {{ content |
                markdownify | strip_html | truncate: 200 | escape }}
              </p>
            </div>

            <div class="post-meta flex-grow-1 d-flex align-items-end">
              <div class="me-auto">
                <!-- posted date -->
                <i class="far fa-calendar fa-fw me-1"></i>
                {% include datetime.html date=post.date lang=lang %}

                <!-- categories -->
                {% if post.categories.size > 0 %}
                <i class="far fa-folder-open fa-fw me-1"></i>
                <span class="categories">
                  {% for category in post.categories %} {{ category }} {%-
                  unless forloop.last -%},{%- endunless -%} {% endfor %}
                </span>
                {% endif %}
              </div>

              {% if post.pin %}
              <div class="pin ms-1">
                <i class="fas fa-thumbtack fa-fw"></i>
                <span>{{ site.data.locales[lang].post.pin_prompt }}</span>
              </div>
              {% endif %}
            </div>
            <!-- .post-meta -->
          </div>
          <!-- .card-body -->
        </div>
      </a>
    </div>
    {% endfor %}

  </div>
