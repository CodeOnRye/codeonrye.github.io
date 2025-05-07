---
title: Thoughts on Vibe Coding
date: 2025-05-07
tags:
  - Thoughts
  - AI
  - Vibe
  - Coding
summary: Some thoughts on the vibe coding concept.
draft: false
---
{{< lead >}}
Some thoughts on the vibe coding concept.
{{< /lead >}}

I've been thinking of the concept (idea? methodology?) of vibe coding. It was only a recently coined term from February 2025, based on [Wikipedia](https://en.wikipedia.org/wiki/Vibe_coding) .  Roughly, it is the use of AI tools to generate functional code without fully understanding or questioning it. You, as a "Vibe Coder", would, in its simplest form, act as a Project Manager of sorts and speak to what you want. The tools would generate implementation guides, implementation plans and the various code iterations until you have a functional program. One of the key elements of this process, and it seems like the degree of this is up for debate, is that you do as minimal code understanding or reviewing as possible - basically if the code works it ships.

Now, as it is a new concept I do expect it to continue to evolve, and the processes around it to become a bit more concrete. But I have some thoughts on some aspects and the overall concept of how it might play out.

## vibe coding vs googling

Let's start with the obvious, what this is replacing. Before vibe coding started taking off, one of the most common ways to "generate" code was to use google.  You'd often end up in places like StackOverflow where you might find a snippet close to what you were trying to do. You'd then copy and paste this -- and it doesn't work! Because you still haven't updated it to work with your actual code. You still have to do a bit of critical thinking with how the code actually works and how you need to update it to make it work for you.

In most cases, this isn't seen negatively. You simply need a function and get a boilerplate that is 90% of the way there. You update it. And it works. 

Now sometimes copied code "works" out of the box and you can straight up paste it and run it without thinking. This is what I think early vibe coding was without the AI wrapper we are seeing now. And that is usually when people start running into trouble, because they didn't really analyze how the code works and down the line it could end up being the thorn in the lion's paw.

What the function is doing, if it is inefficient, or could even created vulnerabilities -- this wasn't considered by the developer. But, hey, it works, so all is good! "That's a problem for future me" is what many would say to justify this.
## vibe coding vs no code solutions
Where I can see a strong use case of vibe coding is as a no-code solution. There are already many tools out there that  position themselves as low-code, visual-coding or no-code - and now we can add vibe code to that mix. In all intents and purposes you may not even need to see the code when you are "truly" vibe coding, so services like https://lovable.dev/ already are pushing for this "no need to view the code" mentality. Compared to https://www.cursor.com which is more adjacent to helping you with the code, but you can still just have it make something and run  with it.

My opinion here is that a blind box solution can work but only in highly scoped solutions, but the real winner will be the more open-box solutions.  There still will be a need to understand some concepts of programming - but that need is getting smaller all the time. 
## dabbling in vibe coding at a ctf
I would be a bit amiss to not including how I've dabbled in the idea of vibe coding. 

There was a CTF I was at recently where, as with most hacking or red-teaming, anything goes. To that effect, I wanted to focus on what commercial AI models could do when it came to some of the challenges. 

If you've not participated in CTFs (this was my first real life event) before, they are usually a mixed game of knowledge challenges, riddles and puzzles. Usually there are clues in the name or description of the challenge on what might be the way to complete it or where the flag might be. From there it is up to you think about the approach and what exploits or vulnerabilities exist that could get you there.

Vibe coding these exercises worked extremely well with one major caveat, you still need some baseline knowledge to guide the AI to the right place or be able to discern when the AI might be going off track. Now, I'll admit that I am still a novice with CTFs, but by shifting to include AI in a way where I directed it what I needed, tested and reworked the code with it, I was able to successfully complete quite a few challenges.

At this point, I am fairly convinced that the tooling is at a point where this tooling is able to heavily accelerate the skills of threat actors to a point that adoption is required for those on the defense. I like to think of this as part of the evolution from one threat actor with one machine, to the many threat actors each with fleets of machines, to each threat actor to now a fleet of agents on a fleet of machines. 

This has brought out a new layer of resources available to threat actors that need to be considered.
## dabbling in general
Additionally to trying a bit of vibe coding with the CTF, I have also found AI helpful when I need a quick script made in a language I am comfortable with, like python. I generally know what I need, how to phrase and and can review the code (yes, I am not the best vibe coder in that sense) if needed.

I have also managed to generate an, albeit janky, app built on JavaScript and html. It wasn't anything mind blowing, but it really does show that the generalist models, like Gemini 2.5 Pro, can handle complex functions and files. However, I want to reiterate that it still required a lot of coaching and realigning the AI to get it to stay on track.

Occasionally, once it got [stuck on a loop of a problem it couldn't fix](https://news.ycombinator.com/item?id=43688933), the best option was to have it generate a new handoff prompt and spin up a "new" chat and get that instance up to the same speed. I would bet that the dedicated tooling is much better, but I have not tested them just yet.
## vibe coding and security
One of the largest concerns about vibe coding is the quality of the security of the code. This is where I think a lot of the ethos misses the mark. Sure, you could just "vibe out" a cool new app, but if you aren't considering security in either a secure-by-design (which I guess that would mean to make sure the AI agent is prompted to consider it?) nor in code reviews (which is against the core idea of vibe coding), nor implementing any security testing -- then this is just a disaster waiting to happen.

There are already [instances](https://nmn.gl/blog/vibe-coding-fantasy) of this already happening. So, yeah, this isn't ready for primetime at its current state. It reminds me of when someone might spin up a VPS with LAMP and maybe Wordpress and then not put in any security controls around access to the server, and then within a few days it becomes compromised. It's not that it isn't a secure option - it's just that it wasn't considered correctly.
## pre-requirements to be a good vibe coder
So what makes someone a good vibe coder? Or better yet, what makes good vibe coding? I think there is still a heavy need to actually understand what you are making - even if it is just handed to you and "works." Beyond security concerns, there is just the ability to know what the code is doing and how it could be improved and what limitations it might have at that moment. 

Will we get to a point that we don't need to look at the code? Probably, or at least close to it. But for now we should recognize the limitations, but understand the fact that this can help someone really accelerate their coding proficiency.