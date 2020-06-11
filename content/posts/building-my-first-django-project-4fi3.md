---
title: Building my first Django project
date: '2020-06-01T12:00:26.409Z'
excerpt: >-
  I'm working through Django for Beginners by William S. Vincent. The second
  chapter gets us into devel...
thumb_img_path: null
comments_count: 0
positive_reactions_count: 2
tags:
  - python
  - django
canonical_url: 'https://dev.to/daveparr/building-my-first-django-project-4fi3'
layout: post
---
I'm working through [Django for Beginners by William S. Vincent](https://djangoforbeginners.com/). The second chapter gets us into developing our first app. It simply displays a single page with an unformatted Hello World on it, but I really appreciated how the project is so fully fleshed out end to end. You start a project with a clean 
`pipenv`
, and make the files and folders through the CLI. The django framework provides some really nice methods to 'boilerplate' the multiple files needed in each project, and having this introduced at the start and then fill in the details later when you are hands on is definitely the best way to go.

Introducing migrations and the url-view-model[-template] core concepts was pretty simple in practice, though a little confusing initially. "I've just made a bunch of files with this single 
`startapp`
 command, what do they all do?" was admittedly my first reaction. 

The best part of the way this book is set up is the definition of done used in the core workflow. A project isn't done unless it has a commit history, is hosted on GitHub and deployed on Heroku. I'm really a fan of approaching deployment in Chapter 2, just like version control and dev environments in Chapter 1. These concepts are your friends, not your monsters :)

Incidentally, having only been aware of Heroku in passing, I really like the PAAS set up. Very usable, the cli tools make the whole thing a doddle and the end satisfaction of being able to point at something that's actually on the web and say 'I did that!' is always a little more satisfying than 'It works on my machine?'.

*[This post is also available on DEV.](https://dev.to/daveparr/building-my-first-django-project-4fi3)*


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
