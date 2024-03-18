---
title: 'Building My Site'
date: 2024-03-18T13:23:47+01:00
tags: ["blog", "hugo", "website", "guide"]

---
{{< lead >}}
A scalable site.  
{{< /lead >}}

## Introduction

For those curious this guide is how I got this site up and running using a combination of Github, as the deployment automation and hosting of the site, and Hugo, a static website generator tool, using the Congo theme. This is all better documented on all the referenced sites, but this might help with bridging any gaps, or maybe provide a more concentrated interpretation of the above guides.

The assumptions are that you know your way around the terminal and know how to use tools like `git`, `brew` (for macs) and modify your domain's DNS. 

All references can be found at the following sites:

https://gohugo.io/getting-started/quick-start/ - Hugo quickstart guide. I would start here if you have no idea what is going on.
https://jpanther.github.io/congo/docs/installation/ - An end to end guide from the theme's creator. Really this should cover most everything.
https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages - Important information using GitHub Pages (which is what we will be doing)
https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site - Important information on DNS for your domain to point it to GitHub Pages.
https://github.com/CodeOnRye/codeonrye.github.io - Lastly, here is all the code running this site, so you could always start from there!

### Schema 

First let's lay out all the pieces to best understand how this will work.

{{< mermaid >}}
graph TD
A[Repository Markdown Files] -->|Git Commit| B(GitHub)
B --> C{GitHub Actions}
C -->|Watches Main Branch| B
C --> F(Runs Hugo)
F -->|Processes MD to HTML| G(Pushed to gh_pages Branch)
D[Domain Registrar] -->|A Record| E(github.io)
G --> B
E --> G
subgraph Local
A
end
subgraph GitHub
B
C
F
G
end
subgraph DNS
D
E
end
{{< /mermaid >}}


## Hugo

First things first. You need to get Hugo up and running and become familiar enough with it. Use the linked guide [above](https://gohugo.io/getting-started/quick-start/) to just try setting up a quick one locally. Once you get a feel you can start by 

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