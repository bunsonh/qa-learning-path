---
layout: default
title: Blog Posts
nav_order: 3
has_children: true
---

### Content

# Liquid Test

{% assign message = "Hello, Liquid!" %}

{{ message }}

## Progress

{% assign progress = page.progress %}
{% assign bar_length = 20 %}
{% assign completed_length = progress | times: bar_length | divided_by: 100 %}
{% assign remaining_length = bar_length | minus: completed_length %}

[{{ '▓' | times: completed_length }}{{ '░' | times: remaining_length }}] {{ progress }}%
