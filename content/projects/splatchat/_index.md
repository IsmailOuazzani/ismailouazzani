---
title: Splatchat
toc: false
cascade: 
    type: blog
---

### Introduction
I got inspired after using Niantic's Scaniverse, an app that captures 3D scenes by filming around using gaussian splatting, a cutting-edge 3D reconstruction technique. My main observation was that if people truly enjoyed these "splats," they’d prefer sharing them with friends and family rather than broadcasting on public profiles or feeds. In essence, I wanted to create the WhatsApp of 3D pictures, with Scaniverse as the Instagram counterpart.

With that idea in mind, I took a "build it first" approach. I hacked together a prototype in just three weeks and then invited my friends to test it. Typically, I focus on back-end, so this was my first time building a front-end for iOS and Android, as well as deploying my own API in the cloud.

### Tech Stack
- React Native: Used for building the mobile app for both iOS and Android.
- FastAPI: Handles the API and authentication.
- Google Cloud Compute: Hosts the API.
- Nginx: Manages routing and domain names.
- Docker: Packages the environment with all the Gaussian splatting dependencies.
- Runpod: Provides serverless GPU support to run Gaussian splatting.
- Gsplat: The tool that performs Gaussian splatting.

### Demo
{{< video src="splatchatdemo.mp4"  width="300px" muted="true" autoplay="true" loop="true">}}

### Why it didn't work
I struggled to pinpoint a compelling use case. Even my own friends weren't motivated to use it. Capturing videos of scenes that are inherently static proved inconvenient, and ultimately, the concept didn't generate enough interest.