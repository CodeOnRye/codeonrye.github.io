---
title: Thoughts on Reeder.app so far
date: 2025-03-16
tags:
  - rss
  - Thoughts
  - pkm
summary: My thoughts so far on Reeder.app as my RSS Reader.
draft: false
blueskythread: 3lkirnk5wds24
---
{{< lead >}}
My thoughts so far on Reeder.app as my RSS Reader.
{{< /lead >}}

About two months ago [I mentioned](https://ryanpmeyer.eu/posts/revisiting-rss/) that I was updating my RSS workflow and decided to test out the new [Reeder.app](https://reederapp.com/). I wanted to provide some updates on my thoughts and RSS process
### Design Decisions
The application itself is a bit of an opinionated look at how RSS, and other feeds in general, should be consumed. Rather than trying to capture everything and let you know what you have read, what you haven't - it focuses on what is new now and consuming that content. This does help with having a high volume of content from your feeds where you just want to see what is happening - but if you want to keep up with a certain feed, this does not support that. 
#### A more ephemeral RSS
At its core, this application will feed you a chronological list of your feeds. It will only update them when you open the application, and doesn't sync between devices (by design). This means, if you don't use the app all the time, or maybe don't open it often on one device, you will notice a desync between your apps. This is even noted in the [FAQ](https://reeder.app/help/#:~:text=Why%20are%20items%20sometimes%20missing%20or%20appear%20in%20a%20different%20order%20on%20my%20devices?).

Supposing you have it installed on an iPad and your phone, and you read an article maybe a few weeks ago that you wanted to find. If you try to find it on the iPad you won't see it in the feed. On the phone you would be able to find it, so long as you have your retention set long enough on your feed. Now, yes, you can save the article into one of the tags, like the "liked" tag, and that will sync - but I often will read items and then days later think about them and want to find them. 

In my case, I can look at my phone and see about 32k total items, on the mac I see 22k and on an iPad I see 15k items. Note that in all I have set an unlimited retention. As you can see, if I want to find something I read, my best bet would be to use my phone to find it, then save it and then it will sync.

#### FOMO Overload Management
This does help with one thing I do struggle with a lot when it comes to RSS feeds, FOMO. When unread counters climb and I have thousands of posts just sitting there, I just want to close the app and ignore it. But by not showing unread counters and focusing on the now, I feel like I can keep up with my feeds, even if they post dozens of articles a day.

However, it doesn't solve all my FOMO - there are the feeds that I do want to both see everything and know what I might have read and what I have not. Usually these are low volume, smaller blogs or sites - which usually only post a handful of articles that might have built up. This app does not help with that. 

You can create filters and folders to help consolidate those feeds of interest, but because of the lack of "full" syncing and no automated way to indicated if you have read something - I find myself wanting to better track these feeds. 

In short; I no longer feel overwhelmed by the number of articles, but now feel like I am missing the ones I really want to see.
### Social Media Syncing (Bluesky, Mastodon, etc)
Taking a step back, I also want to touch on the types of feeds you can add.

For social media, like Bluesky and Mastodon, it does a nice job of rendering the posts. However, if you want to do more than just read them and either interact with them, view by author, or filter them - you have to do this all in the native app.

You cannot:
- Reply
- Block/Filter
- Select the author to see all posts synced
- Search based on the meta data

So unless you have a really curated home feed, you may not want to connect your account, and instead manually subscribe to posters that you really want to see in your feed. Otherwise you might get inundated with content you just don't want to mentally sort through.

At that point, I would rather just open the social media app, or use something like [OpenVibe](https://openvibe.social) if I want to consolidate my socials a bit more.

### Youtube Feeds
With YouTube, when you log in it auto defaults to the "for you" page. There is a recent push against this and using the subscription feed instead, per [Technology Connections - YouTube.com](https://www.youtube.com/watch?v=QEJpZjg8GuA). Reeder.app can help with seeing the content chronologically and without needing to remember to select your subscriptions feed. Just like any other feed, you can add the channels and see them when they are posted.

The biggest complaint I have with the YouTube integration, is that I cannot log in and sync down my subscription feed. Ideally, I would be able to log in, select the subscriptions I want to sync, and an option to add new subscriptions automatically, so that when I am on YouTube proper I can subscribe there and it will automatically be synced (or I have the option to check it off). 

Right now, I need to manually search for the channel and add it to Reeder.app in addition to possibly subscribing in YouTube.

Additionally, the way videos (regardless of source) are handled in the app could be improved;
- Videos should float to the the bottom and keep playing when you scroll, like how the podcasts work.
- When playing a video the only way to get to a scrub bar is by selecting the fullscreen button, and then you can scrub the video. But then exiting fullscreen pauses the video and you have to tap it again to continue to play it.
- Play position isn't saved when you leave and come back. This is most likely a limitation on how the videos are handled, but it would be nice to have it remember your position.
### Podcast Feeds
Similar to YouTube, you can manually subscribe to podcasts and have them in your feed. This is helpful for podcasts that might be only relevant to the current time, like News podcasts. But, if it is a series or something you want track what you have listened to - this isn't the app to put them in. 

I do like that when you are playing a podcast it adds the player to the bottom. I would like to see a way to queue up some podcasts. I often will be scrolling and see something that would be interesting and will want to listen to it next but I have to either wait for the current one to end or just stop it and move to the next one.

### Filtered Feeds
This is a new feature, so I do hope it improves. But it is very limiting I feel.

- It only supports `include all terms` `include any terms` or `include exact term`. For example I cannot create a filter like: Must include: "Some Phrase" OR "Term"
- I cannot filter specific feeds. For example: `include any terms AND include "FeedA OR FeedB"`
### General Nitpicks
These I just couldn't find a spot for, so let me just run through them here:

- You cannot tap on the content's source to then quickly jump to that feed's view. You need to find it in your side bar and then select it. Worse still is if you connect your social media then those sources aren't really searchable (e.g. you cannot search `source:"someone@some.social"`)
- When adding feeds, you have to add them one at a time, you cannot queue up multiple to be added. I.e. I can search for a YouTube Channel, select the `+` next to them, but have to then click `Add` otherwise if I go back to search for another it forgets that pending subscription
- Additionally, the Add menu just feels very clunky. You seem to have to make more clicks than necessary to do something. I.e. Search for feed, tap `>`, tap `+` next to the feed, finally tap `Add` and then it closes! No way to "Add more" or anything.
- When searching for feeds to add you cannot tap the name of the feed to get more information. This is a bit annoying when you aren't sure which feed is correct if multiple appear.
- It would be nice to auto-tag or label certain feeds.
### Overall Thoughts
After trying out this app, do I like it? Yes. I do, but it doesn't work 100% how I want it to work. Which is okay, I can leverage it for its strengths while compensating them with another tool I might have.

For me, Reeder.app is great for "fire hose" sources that I don't need to, or want to, retain a copy of for later reference. The best example here is News, which comes in fast. If it is worth saving the article, I need to make the conscious effort to send it to something like Readwise.

However, for feeds that I want to stay ontop of, then I think either Readwise Reader or Reeder Classic might be best. Where I can keep track of my read/unread and also have the articles automatically sync.

## What now?
I've already started re-testing Readwise reader, but have already found that the discoverability is very difficult. It seems searching doesn't include searching articles from your feeds, which isn't great. And I also plan to re-test Reeder Classic.

What this has shown me is that I need the following core processes:
- "Stream Feed" - Feeds that I just want to see what is happening, where I don't care too much about retention or revisiting.
- "Priority Feed" - Feeds that I want to review what is posted and most likely will want to retain a copy incase I want to go back. These often should be sent to my highlighter of choice. These also need to be searchable and discoverable.
- Discoverability - In general, I want to be able to find something if I had looked at it. Ideally I do like to know if I read something, or started reading it - and this should be fairly automatic.
- Highlighting - I do like to highlight, so either I have to remember to send something to Readwise or have it there in the first place.

Anyway this is mostly a ramble post, I do want to set some more time aside to work on going over my PKM processes as a whole too, that way as I work on them and maybe discuss them, there is a reference point.