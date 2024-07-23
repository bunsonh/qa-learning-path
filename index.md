---
layout: home
title: Welcome to My Project Portfolio
nav_order: 1
---

# Welcome to My Project Portfolio

Hello and welcome to my project portfolio! Here, I document my journey through various projects, courses, and learning activities. Explore my progress, insights, and accomplishments as I advance my skills and knowledge.

## Featured Projects

### [LinkedIn Learning Courses](projects/linkedin-learning/)
I am currently refreshing skills using LinkedIn Learning courses. 

[**Getting Started With Software Testing**](https://www.linkedin.com/learning/paths/getting-started-with-software-testing)

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


- [Course 1: Lesson 1](/2024/07/11/course-1-lesson-1)
- [Course 1: Lesson 2](/2024/07/12/course-1-lesson-2)
- More courses and lessons coming soon!

### [Awesome Sites to Test On](projects/awesome-sites/)
I am testing various websites to broaden my understanding of web development and QA practices. Check out my findings and reports:

- [Site 1](/2024/07/11/site-1)
- [Site 2](/2024/07/12/site-2)
- More sites and tests coming soon!

<!-- ## Recent Blog Posts

{% assign posts = site.posts | sort: 'date' | reverse %}
{% for post in posts limit: 5 %}
- [{{ post.title }}]({{ post.url }})
{% endfor %} -->

## About Me

I am passionate about technology, learning, and sharing my knowledge. This portfolio serves as a way to document my journey and connect with like-minded individuals. Feel free to reach out to me on [LinkedIn](https://www.linkedin.com/).

Thank you for visiting my portfolio. I hope you find my projects and insights valuable and inspiring!

---
