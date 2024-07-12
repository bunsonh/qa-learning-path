---
layout: default
title: Category 1 - Hello World 1
nav_order: 2
---

This is it! I might have gotten this straightened out!

## Heading 2

This is where a paragraph might be.  

This would be the second line.  
And the third.  

### Heading 3

- list item 1
- list item 2

## My Progress Tracker

{% assign progressPercentage = 20 %}

<div style="background-color: #ECEFF1; border-radius: 20px; overflow: hidden; height: 30px; box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2); position: relative;">
    <div style="width: {{ progressPercentage }}%; height: 100%; border-radius: 20px; background-color: #0077B5; transition: width 0.3s ease;"></div>
    <div style="position: absolute; top: 50%; transform: translateY(-50%); right: 10px; font-weight: bold; color: #000000;">{{ progressPercentage }}%</div>
</div>