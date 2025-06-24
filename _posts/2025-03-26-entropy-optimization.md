---
layout: post
title: Creating a distribution with a specific entropy using PyTorch
date: 2025-03-26 12:00:00
description: Using an optimizer to play with the statistical properties of a distribution.
tags: information-theory pytorch
categories: work
giscus_comments: false
related_posts: true
---

<a href="https://github.com/ddegenaro/ddegenaro.github.io/blob/main/assets/jupyter/entropy_opt.ipynb?raw=1" download>Download this Jupyter notebook</a>

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/entropy_opt.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/entropy_opt.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
{% jupyter_notebook jupyter_path %}
{% else %}

<p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
