---
title: Automating Robot Success Classification with Vision-Language Models
toc: false
cascade: 
    type: blog
---

### Introduction

Robots performing real-world tasks often require human annotations to determine whether a task was completed successfully. This slows down development cycles and limits scalability. We explored an AI-driven approach to classify robot demonstration success using only video data and natural language instructions.

### Our Approach
We fine-tuned InternVL2 Vision-Language Models on a subset of the [Droid](https://droid-dataset.github.io/) dataset, which contains 76,000+ robotic demonstrations across 86 tasks and 564 unique environments. Instead of using predefined heuristics, our model learns from video and language context to determine whether a task was completed correctly.

{{< video src="droid.mp4" muted="true" autoplay="true" loop="true">}}

### Results
Our findings show that Vision-Language Models can autonomously evaluate robot performance, reducing reliance on human labels and accelerating robotic learning and deployment. Future work includes temporal localization (pinpointing success/failure moments in video) and adapting models for diverse robotic platforms.

### Code
{{< card link="https://github.com/IsmailOuazzani/RoboSuccessVLM" title="View on Github" icon="github" >}}

### Project Report
{{< pdf "CSC413_project_report.pdf" >}}