---
title: 'Oliver Pattison'
layout: micro
date: 2016-07-18 12:34
updated: 2016-08-15 14:54
unique_id: hire
permalink: /hire/
custom_style: custom-hire.css
description: 'Why you should hire or work with me, Oliver Pattison, a web designer.'
opportunities:
  - title: Full-time role
    description: |+
      I am looking for a design role that requires both design and development expertise. This might be called “web designer” or “front-end developer”, but I am happy to work outside and in between those boundaries.
  - title: Part-time or contract role
    description: |+
      I am available to provide design and light development work for small projects (or as a small part of a larger team).
  - title: Side projects and collaboration
    description: |+
      I am interested in providing design, prototyping, or other assistance for open source projects that solve interesting problems, communicate provocative ideas, or promote social justice.
details:
  - title: HTML and CSS
    expanded: 'I have a passion for well-written, thoughtful HTML and CSS. Although it is sometimes dismissed as a simple markup language, getting HTML right is challenging, both when dealing with visual design and with accessibility and usability.'
    icon: html5
  - title: Jekyll
    expanded: '[Jekyll](http://jekyllrb.com/) is my favorite tool for designing and publishing content on the web. Most of the sites that I build currently are static sites (using Jekyll) with minimal but flexible configuration and high performance.'
    icon: jekyll
  - title: Git
    expanded: 'Version control is essential for designing dynamically, maintaining code, and collaborating quickly and remotely. I use [Git](https://git-scm.com/) as a safety net for all of my work, whether on my own or with a team.'
    icon: git
  - title: JavaScript
    expanded: 'I have been learning JavaScript for the past few years, developing interactive user interfaces with tools like [Velocity.js](http://velocityjs.org/), [Vue.js](http://vuejs.org/) and [Mapbox](https://www.mapbox.com). I believe strongly in [progressive enhancement](https://sixtwothree.org/posts/designing-experience-layers) when designing experience layers.'
    icon: javascript
  - title: Sass/SCSS
    expanded: 'I use [SCSS](http://sass-lang.com/) to help me write effective CSS. I find it invaluable as a creative tool and as a way to organize and develop styles in short and composable parts.'
    icon: sass
  - title: Web publishing systems
    expanded: 'I have designed and developed sites with Shopify, Statamic, WordPress, and other content management systems. My focus has been on integrating front-end design with content editing systems, and creating clear and usable content structures for editors.'
    icon: shopify
recently:
  - Learning the Mapbox GL API to [make interactive maps with JavaScript and WebGL](/2016/10/mapbox-maps-olivermakes/).
  - Redesigned [Jean Flanagan’s website](/2016/10/jean-flanagan-2016/).
  - Presented [a talk at JekyllConf](/2016/05/jekyllconf-responsive-images/) on responsive images with Jekyll and imgix.
  - Learning [Vue.js](http://vuejs.org) to make user interfaces with JavaScript.
  - Attending local meetups like [the IndieWebCamp Homebrew Website Club](https://indieweb.org/Homebrew_Website_Club) and [the CodeNewbie DC community coding group](http://www.meetup.com/CodeNewbie-DC/) to collaborate with like-minded people and those who are new to web development.
  - Developing client websites, such as [Acorn Landscape Supply](http://acornlandscapesupply.ca).
  - Contributing to online communities such as [Spec’s design and development Slack network](http://spec.fm/) and [Jekyll Talk, the official resource for Jekyll](https://talk.jekyllrb.com/).
---

# Available for hire

I’m [Oliver Pattison](/about/), a designer who makes responsive, forward-thinking websites.
{:.focus}

## Seeking

{% assign opportunities = page.opportunities %}

<section class="opportunities">
  {% for opportunity in opportunities %}
    {% if forloop.first %}
      <div class="opportunities-item--featured">
        <h3>{{ opportunity.title }}</h3>
        {{ opportunity.description | markdownify }}
      </div>
    {% else %}
      <div class="opportunities-item">
        <h3>{{ opportunity.title }}</h3>
        {{ opportunity.description | markdownify }}
      </div>
    {% endif %}
  {% endfor %}
</section>

{% include block/outreach.html %}

{% include block/elsewhere.html %}

## What I work with

{% include block/details--hire.html %}

<aside class="ancillary--endnotes">
  <h2>What I’m up to recently</h2>

  {% assign recently = page.recently %}
  <ul>
    {% for item in recently %}
      <li>{{ item | markdownify | p_escape }}</li>
    {% endfor %}
  </ul>
</aside>

{% include block/project--satellite.html id="2016-10-14:mapbox-maps-olivermakes" %}

{% include block/project--satellite.html id="2016-10-08:preserving-jekyll-sites" %}

{% include block/outreach.html %}
