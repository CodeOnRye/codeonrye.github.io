---
title: Supply Chain Attacks for the Average Person
draft: false
date: 2025-07-20
tags:
  - supply-chain
  - security
summary: Supply Chain attacks are more than something just a Company needs to consider.
blueskythread: 
---

I’ve noticed in the news a lot more upticks on supply chain attacks that exploit people’s natural trust instinct. I want to try to help demystify what this all is for the average person, and hopefully that will help someone better understand what is going on and how they could try to protect themselves.

First, what is a supply chain attack? As the name suggests, it is when someone, we will call them the Threat Actor, attacks a part of the process that builds something, rather than attacking the end product. Take Google Chrome for example, the product, Chrome, is maintained by a huge company with a lot of staff involved in making sure it is secure. However, Chrome, like most software, doesn’t have all the parts built in-house, instead they leverage other software - often Free Open Source Software (FOSS) - as an off the shelf part. In the case of a supply chain attack, the Threat Actor would focus on identifying a part that Chrome uses, that might be maintained with minimal resources. If successful, they could get this compromised part into the final product, which would get to their ultimate goal of compromising Chrome.

There is a great recent example of a near miss with the well known XZ Utils Backdoor, it’s worth a deep dive if you don’t know much about it. You can start with the [Wikipedia Article](https://en.wikipedia.org/wiki/XZ_Utils_backdoor)

Okay so this is well and good, but really the average person has no real control about what open source software is used in their favorite programs. Which is true, but there is another supply chain attack that is happening.

# Exploiting your trust

Let’s again consider Chrome, when you download the software you expect it to be well maintained and secure. However, Chrome may not do everything you need it to do, so you install some extensions. And that is where these attacks are happening; based on people’s trust of extension, modification, or utility markets. Honestly though, browser extension compromises are nothing new. 

There was the [Cyberhaven compromise from an external threat actor.](https://www.darktrace.com/blog/cyberhaven-supply-chain-attack-exploiting-browser-extensions)

Or worse still, when [The Great Suspender sold the extension and the new owner/maintainer compromised it.](https://thehackernews.com/2021/02/warning-hugely-popular-great-suspender.html)

In both cases they were trusted extensions due to either a Company behind it or being recognized for a while as a trusted owner.

Further this is breaking out beyond what you think would be a “good” place to exploit.

For developers, more and more Packages are getting attacked, and now with the rise of long-con attacks, where a Threat Actor will work on trying to get trusted by a maintainer to eventually push malicious code.

For Gamers, mods are also a new vector for attack, recently there was one that aimed to [compromise Crypto Wallet information in City Skylines](https://www.paradoxinteractive.com/games/cities-skylines-ii/news/traffic-breach-statement). Which is a case where the Maintainer was compromised and then those credentials were used to maliciously impact the mod.

This list could go on, but what I want to hammer home on is that you may trust the source/product, whether it be Chrome, npm, or a video game, as soon as you start installing third party extensions, packages, mod or otherwise then you should be aware that those could lead to a compromise.

# Where do I see this going?

I expect to see the types of vectors to continue to expand beyond what we might think as “the usual suspects”. Mainly because a lot of software out there is trying to act as a base foundation which you can then build up to your needs. I could see software that leverages and focuses on User-generated templates, functions, etc. to possibly become a new vector path, if it hasn’t already happened 

# With all that being said, what can you do? 

Take a look at your computer or phone and consider the following:

First, take a look at the applications you have installed. Have you used them recently? Are they worth keeping installed or can you uninstall them without much issue? For example, do you really need your Airline app installed when you aren’t traveling anytime soon? What about having both Microsoft Office and Libre Office installed? Do you really need both installed?

Next, once you have cleaned up your applications, which ones offer extensions, mods, or otherwise “third-party” functionality. Review that in a similar way; especially extensions. Reduce down to the ones that really help you with your workflows. I often realize I have extensions or apps installed in a “just in case” scenario that has never actually happened!

Lastly, take this forward. Sometimes it isn’t worth installing the application, especially on phones, when the website works just fine. Create a checklist of apps you might need to install during certain events, like if you are traveling you install you airline app, taxi apps for where you are going, and so on. 

Remember, you can always install the software again at a later date! When in doubt, delete and see if you still need it.