---
layout: post
title: Getting started with PyTorch in Google Colab
date: 2024-09-18 12:00:00
description: A brief introduction to using PyTorch in Colab. This notebook is adapted from some guest lectures I gave for courses for which I served as a TA.
tags: teaching pytorch
categories: work
giscus_comments: false
related_posts: true
---

<a href="{{ '/assets/downloads/get_started.ipynb' | relative_url }}" download="get_started.ipynb">Download this Jupyter notebook</a>

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/get_started.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/get_started.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
{% jupyter_notebook jupyter_path %}
{% else %}

<p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
