---
layout: post
title: "Azure Kinect Recording and Playback API"
date: 2019-01-28
categories: projects
---

While working at Microsoft, I was tasked with finding an open-source friendly video format that can record RGB color, 12-bit depth, multi-channel nicrophones, and an IMU sensor. This is a lot to handle, but luckily the [Matroska Media Container](https://www.matroska.org/what_is_matroska.html) is an open standard that can be extended to enable recording any data stream.

The [Azure Kinect SDK Recording API]() exists as part of the larger [Azure Kinect Sensor SDK](https://github.com/microsoft/Azure-Kinect-Sensor-SDK) project.