---
layout: post
title: "Get element size and position"
date: 2015-04-07 12:08:54 -0300
comments: true
share: true
image:
  feature: http://www.jsenv.com/post_images/7fe434088e8c.jpeg
  content: "/post_images_content/get-element-size-and-position"
categories: [tips, web api]
---

Hello everyone.

Today I'm going to talk about an interesting method of the  [Web API  Interface](https://developer.mozilla.org/en-US/docs/Web/API), this method is called [getBoundingClientRect](https://developer.mozilla.org/en-US/docs/Web/API/Element/getBoundingClientRect).
<!--more-->
This method helps us when we want to get the DOM Element's coordinates and rectangular area like top, bottom, left, right, width and height.


```javascript
var el    = document.getElementById('element');
var rect  = el.getBoundingClientRect();
```
See my example:

![exemplo de uso]({{ page.image.content }}/exemplo-de-uso.gif)

The  [getBoundingClientRect](https://developer.mozilla.org/en-US/docs/Web/API/Element/getBoundingClientRect) returns a live object containing bottom, height, left, right, top, width relative to the viewport.

About browser compatibility, I have good news, this method works on most browsers, include IE8+. 
