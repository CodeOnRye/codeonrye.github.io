---
title: 'Hello World'
date: 2024-01-25T13:23:47+01:00
tags: ["blog", "hugo", "website"]
summary: "Hello World."

---
{{< lead >}}
Hello World. 
{{< /lead >}}

## Introduction

The classic initialization of any project always ends up beginning with those words. I've decided to take another shot at curating a digital space for myself. In the past I have tried to create websites using various frameworks and tools, but they always became more work than I felt they were worth. Looking back, I've always tried to create something more complex than I needed. Hoping to grow into it, rather than grow with it. But I really hadn't hammered out the foundation of what I actually needed, and focused on what I wanted. Taking a step back I wanted to focus on what I needed from this projected. With hopes that the choices will be flexible enough to not require a lot of work to expand later or maintain.

Those needs have boiled down to the following.

### Defining My Goals

In short, answering this was the hardest part. Simply "a website" is too broad of an answer; I needed to really think about what content I wanted, how I wanted to present it, how it should be maintained and what I wanted to get out of my time with the project. So lets start with defining the content.

The content will be my own musings, or ramblings for some. I don't want to lock myself into a certain type of topic or subject matter. So a semi-professional blog and portfolio I think will strike a balance. That means the site must be able to provide an easy way for me to both create that content and present it.

Presentation of the website should be clean and modern. Next I need to be able to customize it once I start having a more fully formed idea of the content. So again, it needs to be a flexible solution that can be changed without much headache.

And headaches is what I have gotten in the past with frameworks like wordpress or other blog focused solutions. They did so much more than I needed at the time, that I would get stuck in the weeds. I'd enable features I didn't need, or maybe even fully understand. This solution needed to be simple, but extendable when I needed it to be. 

Lastly, in the end what I want out of this project is a website I can call my own. A place that is easy for me to keep up to date both on content and patches. It had to work for me, rather than me work for it. Which has lead me to go with this set up.

## The Project

This project is created with as minimal tools as possible; Hugo as the website generator and will be served by GitHub.

* Hugo - This is the website framework tooling solution, a static website generator
* Github/Gitlab Pages Hosted - Since I am setting up a static website, that means no backends - and not servers - needed! So why not use Github or GitLab's pages and actions to handle the hosting and publishing?

### Openness

I am always a big fan of Free and Open Source Software, FOSS for short. So where I can, I try my best to leverage systems and tools for that. Granted there comes a time where, well, time isn't as available. Its the well-known adage of FOSS not being free in the cost of time. However, if the system is simple enough and the data portable enough, then it might very well be worth that time and effort to setup and maintain. 

### The Framework

Needing the site to be maintainable, is key to keeping the project, and thus the site, up and running. So, where I could, I would remove systems that needed my attention to work or stay in good working order. Too many website frameworks required lots of backends, databases and the like, as well as had features I simply didn't care for. I just needed something that was dead simple to set up, run and update with new content when I felt like it. 

### The Platform

In the past I have always set up servers, installed the needed services and then install any applications to get a website up and running. But each of those items introduces complexity and friction. I need to make sure the services are up to date. The database needs to be backed up properly. How do I migrate to a new server if needed, and so on. With the static aspect of Hugo I can avoid this because, in the end, the website is just a bunch of files. And those files are already backed up in Github which is also "publishing them." Overall reducing complexity to make it easier to maintain and use, which is exactly what I want.

## TL;DR

In short, I have set up a Hugo based static website that I can use Github Pages and Actions to host and manage! I will probably also post a guide incase someone wants to try themselves!