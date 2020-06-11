---
title: Building my first Django project with pages
date: '2020-06-11T08:30:27.897Z'
excerpt: >-
  I'm working through Django for Beginners by William S. Vincent. Chapter 3
  starts using templates and...
thumb_img_path: null
comments_count: 0
positive_reactions_count: 4
tags:
  - python
  - django
  - hugo
  - jekyll
canonical_url: 'https://dev.to/daveparr/building-my-first-django-project-with-pages-kjn'
layout: post
---
I'm working through [Django for Beginners by William S. Vincent](https://djangoforbeginners.com/). Chapter 3 starts using templates and introduces Class-Based Views.

There is a section introducing Class-Based views, and then mentioning older Function-Based views. It was interesting to see this evidence of the framework progressing, though it's not so surprising for something that's a decade or so old!

The templating syntax was really neat. I'd seen very similar in Hugo and Jekyll, and so the idea of having a kind of 'placeholder' with 
`“{% block content %}{% endblock content %}`
 was nice to use. I've admittedly done very little webdev though. I was curious what other approaches might be common alternatives? If you have an example please let me know in the comments!

Something that was curious to me was the inversion of structure in django vs hugo.

In hugo, I've very regularly used partials such as in [the SatRdays theme here](https://github.com/satRdays/hugo-satrdays-theme/blob/cfc0873e03a7f278f8e09227875affbfcc50169f/layouts/index.html). Here, I have a single home page with my headers and footers, and 'inject' a partial into it with 
`{{ partial "nav.html" . }}`
. In django I feel like it kind of works the other way. We create a project, and then the equivalent to a hugo partial would actually be a django app within the project? Then, each app shares top level content through lines like 
`{% extends 'base.html' %}`
 within each apps template?

It seems like it might be more brittle to me, but maybe also more powerful? There's more duplicate lines to get wrong, but also more opportunities to vary what it does?

What do veteran djangians(is that right?) think? Does anyone use both Hugo and Django, but for different projects and for specific reasons?

*[This post is also available on DEV.](https://dev.to/daveparr/building-my-first-django-project-with-pages-kjn)*


<script>
const parent = document.getElementsByTagName('head')[0];
const script = document.createElement('script');
script.type = 'text/javascript';
script.src = 'https://cdnjs.cloudflare.com/ajax/libs/iframe-resizer/4.1.1/iframeResizer.min.js';
script.charset = 'utf-8';
script.onload = function() {
    window.iFrameResize({}, '.liquidTag');
};
parent.appendChild(script);
</script>    
