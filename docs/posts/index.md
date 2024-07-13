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

## My Progress Tracker
<!-- 
{% assign progressPercentage = 20 %}

<div style="background-color: #ECEFF1; border-radius: 20px; overflow: hidden; height: 30px; box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2); position: relative;">
    <div style="width: {{ progressPercentage }}%; height: 100%; border-radius: 20px; background-color: #0077B5; transition: width 0.3s ease;"></div>
    <div style="position: absolute; top: 50%; transform: translateY(-50%); right: 10px; font-weight: bold; color: #000000;">{{ progressPercentage }}%</div>
</div> -->

{% assign progressPercentage = 20 %}

<div class="progress-box">
    <div style="background-color: #ECEFF1; border-radius: 20px; overflow: hidden; height: 30px; box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2); position: relative;">
        <div style="width: {{ progressPercentage }}%; height: 100%; border-radius: 20px; background-color: #0077B5; transition: width 0.3s ease;"></div>
        <div style="position: absolute; top: 50%; transform: translateY(-50%); right: 10px; font-weight: bold; color: #000000;">{{ progressPercentage }}%</div>
    </div>
</div>