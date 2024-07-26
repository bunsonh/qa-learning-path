---
layout: default
title: Blog Posts
nav_order: 4
has_children: true
---

### Content

# Liquid Test

{% assign message = "Hello, Liquid!" %}

{{ message }}

## My Progress Tracker

{% assign progressPercentage = 84 %}

<div class="progress-box">
    <div style="background-color: #ECEFF1; border-radius: 20px; overflow: hidden; width: 250px; height: 20px; box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2); position: relative;">
        <div style="width: {{ progressPercentage }}%; height: 100%; border-radius: 20px; background-color: #0077B5; transition: width 0.3s ease;"></div>
        <div style="position: absolute; top: 50%; transform: translateY(-50%); right: 10px; font-weight: bold; color: {% if progressPercentage == 100 %}#FFD700{% else %}#000000{% endif %};">{{ progressPercentage }}%</div>
    </div>
</div>

## Time Percentage

{% assign hours_left = 13 %}
{% assign minutes_left = 52 %}
{% assign hours_total = 16 %}
{% assign minutes_total = 30 %}

{% assign total_minutes_left = hours_left | times: 60 | plus: minutes_left %}
{% assign total_minutes_total = hours_total | times: 60 | plus: minutes_total %}

{% assign total_minutes_completed = total_minutes_total | minus: total_minutes_left %}
{% assign progressPercentage = total_minutes_completed | times: 100 | divided_by: total_minutes_total %}

<div class="progress-box">
    <div style="background-color: #ECEFF1; border-radius: 20px; overflow: hidden; width: 250px; height: 20px; box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2); position: relative;">
        <div style="width: {{ progressPercentage }}%; height: 100%; border-radius: 20px; background-color: #0077B5; transition: width 0.3s ease;"></div>
        <div style="position: absolute; top: 50%; transform: translateY(-50%); right: 10px; font-weight: bold; color: {% if progressPercentage == 100 %}#FFD700{% else %}#000000{% endif %};">{{ progressPercentage }}%</div>
    </div>
</div>

## progress box
<div class="highlight-box">
    <p>Your text goes here. Describe the progress or any other details you want to highlight.</p>
    {% assign hours_left = 13 %}
    {% assign minutes_left = 10 %}
    {% assign hours_total = 16 %}
    {% assign minutes_total = 30 %}

    {% assign total_minutes_left = hours_left | times: 60 | plus: minutes_left %}
    {% assign total_minutes_total = hours_total | times: 60 | plus: minutes_total %}

    {% assign total_minutes_completed = total_minutes_total | minus: total_minutes_left %}
    {% assign progressPercentage = total_minutes_completed | times: 100 | divided_by: total_minutes_total %}

    <!-- Debugging output -->
    <p>Total minutes left: {{ total_minutes_left }}</p>
    <p>Total minutes total: {{ total_minutes_total }}</p>
    <p>Progress percentage: {{ progressPercentage }}</p>

    <div class="progress-box">
        <div style="background-color: #ECEFF1; border-radius: 20px; overflow: hidden; width: 250px; height: 20px; box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.2); position: relative;">
            <div style="width: {{ progressPercentage }}%; height: 100%; border-radius: 20px; background-color: #0077B5; transition: width 0.3s ease;"></div>
            <div style="position: absolute; top: 50%; transform: translateY(-50%); right: 10px; font-weight: bold; color: {% if progressPercentage == 100 %}#FFD700{% else %}#000000{% endif %};">{{ progressPercentage }}%</div>
        </div>
    </div>
</div>

# css test

<div class="test-box">
  This is a test box with custom styling.
</div>

<div style="background-color: #FFDDC1; border: 2px solid #FF5733; padding: 20px; margin: 20px 0; text-align: center;">
  This is a test box with inline styling.
</div>