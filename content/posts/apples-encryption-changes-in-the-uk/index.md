---
title: Apple's Encryption Changes in the UK
date: 2025-02-23
tags:
  - Apple
  - Encryption
  - Thoughts
summary: My thoughts on the recent Apple news regarding their changes with encryption in the UK.
draft: false
blueskythread: 3lismngrte22b
---
{{< lead >}}
My thoughts on the recent Apple news regarding their changes with encryption in the UK.
{{< /lead >}}

Recently there was news that the UK has forced Apple to remove encryption from their iCloud service, as seen on the [BBC](https://www.bbc.com/news/articles/cgj54eq4vejo). However there is a bit more nuance to this.

Firstly, I think that the following video does a good job covering what exactly is meant by "Apple removing encryption."

{{< youtube id="f66tYU-k4sQ" >}}

## TLDW
What appears to be happening is the following; 

The UK has demanded a backdoor access to Apple's iCloud data so that they can decrypt it at will. This demand also is behind closed doors and with apparent orders not to share any information about it, so we are learning through various leaks and policy changes.

Apple had three major choices:
1. Deny the request - This would force them to either enter into a long legal battle or leave the market.
2. Accept the request - This would entail creating a backdoor that would allow the UK to be able to decrypt any data at-will, but also creating a major threat surface for bad actors to target - and eventually exploit.
3. Remove features that prevented Apple from decrypting the data upon request from the UK.

It seems, they went with option three. This has been an ability of apple, and really any provider that holds the encryption keys to your data, to do. However, they released a feature back in 2023 called [Apple Advanced Data Protection](https://support.apple.com/en-us/108756). 

This feature, in short, allowed iCloud users to move the decrypting private key from Apple's Servers to their local devices. Thus Apple could no longer decrypt the data unless you provided your trusted device in the request. For reference, Apple has information [here](https://support.apple.com/en-us/102651) - note the services that support "Trusted Devices". 

As you might be able to see, this wouldn't work for the third option to be viable. 

Ergo Apple is rolling back this feature for all UK users - most likely this is based on your iCloud user location, and not where your device was bought or is currently located.
### TLDR
What does this all mean then? Is Apple removing encryption? 

No. 

Apple is just disallowing full control over your encryption, and they will retain a copy of the key to decryption so that they can hand it over on requests.
### What to do now?
If you are in a region that isn't affect, you should enable the Apple Advanced Data Protection. It is still a great tool to use. But keep an eye on any changes, this can be a very slippery slope; and more countries may follow the UK's stance. 

If you are affected, then you should consider either moving your more sensitive information to another service provider that will not be accessible so easily. Or look into running local backups to avoid another policy change at the next provider. 