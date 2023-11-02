---
layout: post
title: "BBCode Compiler in Golang"
date: 2014-02-08
categories: projects
---

For one of my past projects, I wanted to allow content to be copied from forum posts (using the BBCode formatting style) into my website as a page description. This was an alternative option to Markdown, which was also available, but would require users to manually reformat their content when migrating.

When looking for an existing BBCode compiler, I was disappointed to learn that every implementation I came across simply used a long list of regular expression replacements for each tag type, which is rather inefficient. Instead of following the existing pattern, I endeavored to build a proper parser and transpiler from BBCode to HTML that behaves the same as existing solutions. This has the interesting side-effect of making parse errors an impossible output, as a regular expression would just ignore bad tags and output them as plaintext.

This BBCode compiler is written in the Go programming language, and has a full test suite including both input fuzzing, and many specific hard-coded edge-cases.  
You can find the source code and documentation for this compiler here: <https://github.com/frustra/bbcode>
