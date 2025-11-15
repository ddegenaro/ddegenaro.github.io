---
layout: post
title: A brief introduction to Python.
date: 2025-11-15 12:00:00
description: A brief introduction to the Python programming language. This notebook is adapted from I gave to some fellow grad students in Georgetown's linguistics department.
tags: teaching
categories: work
giscus_comments: false
related_posts: true
---

<a href="{{ '/assets/downloads/python_intro.ipynb' | relative_url }}" download="python_intro.ipynb">Download this Jupyter notebook</a>

{::nomarkdown}
{% assign jupyter_path = "assets/jupyter/python_intro.ipynb" | relative_url %}
{% capture notebook_exists %}{% file_exists assets/jupyter/python_intro.ipynb %}{% endcapture %}
{% if notebook_exists == "true" %}
{% jupyter_notebook jupyter_path %}
{% else %}

<p>Sorry, the notebook you are looking for does not exist.</p>
{% endif %}
{:/nomarkdown}
