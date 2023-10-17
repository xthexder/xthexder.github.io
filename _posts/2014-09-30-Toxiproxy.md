---
layout: post
title: "Toxiproxy"
date: 2014-09-30
categories: projects
---

[Toxiproxy](https://github.com/Shopify/toxiproxy) is a network resiliency testing tool I helped develop for [Shopify](https://www.shopify.com/). It is designed as a TCP proxy that can programmatically configured to tamper with connections via "toxics" in a development / testing environment.

A number of different toxic types are available including:
 - Adding latency / jitter
 - Limiting bandwidth
 - Dropping or refusing connections

Proxies and toxics can be controlled through a web interface, command-line, or from within automated testing via one of the available client libraries.

You can read more about how Shopify uses this for resiliency testing in their [blog post](https://shopify.engineering/building-and-testing-resilient-ruby-on-rails-applications).
