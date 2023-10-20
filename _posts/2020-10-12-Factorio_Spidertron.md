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

<style>
    .warning-border {
        width: 210px;
        height: 210px;
        border: 4px solid #111;
        position: relative;
        background: linear-gradient(45deg, #111 25%, #DD2 25%, #DD2 50%, #111 50%, #111 75%, #DD2 75%);
        background-size: 25% 25%;
    }
    .warning-box {
        background-color: #DD2;
        border: 4px solid #111;
        width: 160px;
        height: 160px;
        margin-left: 23px;
        margin-top: 23px;
    }
</style>

<div class="warning-border">
    <div class="warning-box">
        <div style="position: relative; left: 50%; top: 64%;" class="spidertron-home" data-spidertron-scale="0.6" data-spidertron-speed="400"></div>
    </div>
</div>

The source code is available of github here: <https://github.com/AlternativeFFFF/spidertron>
