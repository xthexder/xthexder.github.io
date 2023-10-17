---
layout: post
title: "Controllable CSS/JS Factorio Spidertron"
date: 2020-10-12
categories: projects
---

As a fun side-project, I decided to animate a copy of the Spidertron from [Factorio](https://factorio.com/) for the community-run [Alternative Friday Factorio Fan Facts](https://alt-f4.blog/) blog as an easter egg.
This was achieved using CSS animations and JavaScript, with some careful optimization done to not slow down the page for smartphone users.
A more detailed write up was posted as part of [issue #12](https://alt-f4.blog/ALTF4-12/) of the Alt-F4 blog.

You can control the Spidertron below by clicking / tapping on it, and then selecting a location to move to.  
Click on the Spidertron again to have it return home.

<link href="/assets/spidertron.css" rel="stylesheet">
<script src="/assets/spidertron.js"></script>

<div style="width: 150px; height: 150px;">
    <div style="position: relative; left: 75px; top: 100px;" class="spidertron-home" data-spidertron-scale="0.6" data-spidertron-speed="400"></div>
</div>

The source code is available of github here: <https://github.com/AlternativeFFFF/spidertron>
