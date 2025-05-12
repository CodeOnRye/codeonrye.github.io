---
title: Passing on Passwords
date: 2025-05-12
tags:
  - Tag
  - Tag
summary: Passwords need to be secure, until they don't.
draft: false
blueskythread:
---
{{< lead >}}
Passwords need to be secure, until they don't.
{{< /lead >}}

I recently saw a YouTube channel, [Sun Knudsen](https://www.youtube.com/@sunknudsen), pop back up on feed after a bit of a hiatus.  I'd found Sun's channel way back when I was looking for best practices for hardening Firefox or other browsers and applications. I'd not really followed the channel and him coming back up made me curious to see what he has been up to.

Turns out he was working on a, then paid - now free, tool called [Superbacked](https://superbacked.com). In very simple terms, the tool will take a secret, passphrase, or some other text. It will then encrypt it with a password of your choosing. And then outputs multiple QR codes. To reconstruct the original passphrase, you need to have the encrypting password as well as a subset of the QR codes generate; for example 2 of the 3 generated.

The idea is you can use this for a lot of purposes where there is a need to share the passphrase between multiple people but they need some kind of quorum to reconstruct it. Think of it like in the movies where you need two keys to be turned at the same time to unlock the launch codes for a ballistic missile. 

This can be a great way for companies to share "[break glass](https://en.wikipedia.org/wiki/Computer_access_control#Break-Glass_Access_Control_Models)" account information where you want to ensure not one single person can access it without another. As mentioned by Sun himself, it follows [Shamir's Sharing Secret](https://en.wikipedia.org/wiki/Shamir%27s_secret_sharing) . 

Now for most people, this can still be useful in some narrow use-cases. The one that Sun proposes is as a way to share your master passwords, presumably to your password manager, to loved ones incase of your death. Which makes sense, you will probably want your loved one or family to be able to access things like emails and accounts to take care of your affairs. 

So this made me think, what is my plan? I hope it won't be needed anytime soon, but I should think about how my accounts might be set up to ensure that there isn't more frustrations than needed at that time. Most accounts do let you set up trusted persons, emergency access, or beneficiaries; this is the best place to start for most. 

I guess the takeaway here is to take a look at what you need to access your accounts from square one. If any of your accounts can set up a trusted person, like [Apple](https://support.apple.com/en-ie/102608), [Bitwarden](https://bitwarden.com/help/emergency-access/), [Google](https://support.google.com/accounts/answer/3036546?hl=en), 1Password (they don't seem to have a similar feature, but a similar [blog](https://blog.1password.com/digital-estate-planning-guide/) post to this that goes into more details), etc., set those up!  But keep in mind that you will be giving that person power to do just that, so make sure their security is up to snuff too. If any of those need a password, or you prefer that method, then you need find out a secure way to share the password that meets your needs, maybe using this or a similar tool. 