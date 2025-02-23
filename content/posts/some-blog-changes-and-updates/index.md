---
title: Some blog changes and updates
date: 2025-02-23
tags:
  - website
  - blog
summary: A quick update on site changes.
draft: false
blueskythread:
---
{{< lead >}}
A quick update on site changes.
{{< /lead >}}

I've been working a little on the backend of the site to see how I can improve things. My goals are to:

1. Make the site more robust.
2. Have a little better insight into the usage of the site.
3. Adding interactivity.
4. Make it easier for me to post to the site.

## Making the site more robust
Previously I was hosting my DNS with my registrar, but I have been working to split the two and migrate to different services. This should allow for a few things, one; I can use Cloudflare for DNS, which is a well known service and has a lot of additional tooling to boot. Two, I can move my Registrar a bit easier since I would just have to make Nameserver updates upon moving (Though I am still on Squarespace at the time of writing, I am looking at others, like [Porkbun.com](https://porkbun.com/)).

Additionally, I am moving from Github Pages to Cloudflare Pages. Though this goes against the idea of the above where I wanted to unconsolidated; here there are some added benefits from an analytics point of view. Also I can easily move back if I decide there isn't much benefit. 
## Site Insight
I also want to try to get a better idea on if the site is getting any traffic. I would like to reiterate that this blog is more for me to work on my own skills, and have control over my content. But, it is still helpful to know if people do access the site. 

I weighed some options and came to two possible tools; one was to use [Fathom Analytics](https://usefathom.com/), which is a privacy focused analytics service. The other was to, as you can possibly guess, use Cloudflare. I am going to most likely opt for the Cloudflare option as it is free, and I really can't justify (yet) on adding more to my monthly subscriptions. Now, if this site gets to a point where it can generate enough money to support itself then that will change. Though, I don't see that as a current goal for the site.
## Adding Interactivity
Next thing I wanted to setup were comments for those interested to interact with posts. Unfortunately it looked like a lot of the plug and play systems were either not free or needed to have more than just static pages.

Luckily, I found out that [Matt Dyson](https://mattdyson.org/blog/2024/11/bluesky-posts-as-hugo-blog-comments/) made a way to [integrate to Bluesky comments with my same Hugo and Congo setup](https://github.com/mattdy/bluesky-hugo/). This works out well since Bluesky is my current primary sharing media. (Though maybe I can also add Mastodon next?) So, now there are comments available! I will need to update some of my older articles where I also posted on Bluesky.

Side note to all of this; I had also looked at migrating to a platform like [Ghost](https://ghost.org/) or [Beehiiv](https://www.beehiiv.com/). Both would offer a lot of these tools, but again my issue would be justifying the cost to maintain them. Also their entry tiers seem to leave a lot of customization features out. Anyway, I am going to keep this as a static site for now.

## Writing ease
Lastly, I think this will continue to be a struggle for me as I work out how to best write articles for the site. I would like to be able to do so both on my computer, which is the easier one; and on my iOS devices like iPad. 

Right now, I am using Obsidian as it has strong markdown support - but there is still a gap on getting the files uploaded to Github easily, especially from iOS. And it isn't the most seamless process. This will most likely be my next big focus on site improvements.