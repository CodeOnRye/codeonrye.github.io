---
title: The Tea App and Verifying Identities
draft: false
date: 2025-07-30
tags:
  - privacy
  - data exposure
  - trust
summary: With the recent Tea App data exposure, I wanted to take a moment to think about the choices on how to verify user identities.
blueskythread: 3lv7ib3axzc2u
---
## The Tea App

Right now there is an ongoing development of the Tea App having multiple data exposures. I don’t think I can give the details justice, so please look to [404media.co](https://www.404media.co?ref=ryanpmeyer.eu) as they have been covering it quite well!

{{% center %}}
[Initial Exposure by 404media](https://www.404media.co/women-dating-safety-app-tea-breached-users-ids-posted-to-4chan/?ref=ryapmeyer.eu) 

[Second Exposure by 404media](https://www.404media.co/a-second-tea-breach-reveals-users-dms-about-abortions-and-cheating/?ref=ryanpmeyer.eu) 
{{% /center %}}

The long and short, this app was purported to be a safe and private space for women to discuss dating. However, because they wanted to ensure it was only women they had a problem, verifying that fact. 

They decided to use a selfie-with-id method, and ended up failing to secure that data both in storage and in deletion. Now, there are other issues with this app, but I want to focus on this particular problem they were trying to solve. How do you verify someone is who they say they are, with minimal compromise to their privacy?

Let’s look at what they ended up doing and where that failed. 

{{< alert >}}
I am going to make some educated guesses on how they may have handled some processes, but the point I want to focus on will be that the method they chose is a difficult one with a lot of nuances. 
{{< /alert >}}

To verify if someone was a woman, Tea would request the user to send them an iID document (License, Passport, etc) with a selfie of user in the photo. This is an effective way to verify someone, I will grant them that. However, it completely breaks any privacy expectations. 

Because they chose to accept Personal Identifiable Information (PII) data the Tea app then needed to consider how they handle the data. How should it be transferred to the verification system? Who or what is verifying the data; is it automated or human based? Are you encrypting the data throughout this process? If so, you will need to decrypt it to verify, will that have any caching, logging or other artifact concerns? If there is a human involved, will they be able to exfiltrate the data by saving it, taking a photo with their phone, or otherwise? Once the data is reviewed how do you ensure it is deleted from the system properly?

As you can see, there are already a lot of questions, which will lead to more questions. In the end there was at least one point where the data was not encrypted and stored on a firebase storage bucket and that bucket was not protected. 

So, in all honesty, it was a bad idea.

Looking back at the original problem, what is another way we could solve this problem that could have avoided these potential problems and resulting outcome?

## A Trust Ring

Rather than having the App take the responsibility of verifying the user’s identity, they could let the users do it amongst themselves.

Setting up a system where the trust is created and developed between the users could allow for a more private and secure system. A hypothetical way this could work is:
1. Make the sign-up invite only from other members
2. Accepting an invite creates a trust between the two users
3. Users can also sign-off on others to create additional trusted links and networks of trust

This is a basic idea, you could add more layers like having to only send the invite over bluetooth (forcing a more localized requirement). Or adding in different levels of trust (invited, in real life confirmation, etc).

The trust ring would be able to rely on its core principles of:
1. Direct trust established between users
2. Transitive Trust: If User A and B trust each other, and B trust’s C, then A is one degree away from trusting that user.
3. Leveraging the Degrees you can weigh how much someone could be trusted to discuss sensitive issues with.
4. Someone that has many direct and reciprocated trusts could help establish them as trusted even at a distance.

### How could this look for the user?

Suppose you hear about the app from a friend, they would give you their invite code and you can sign up. That creates an initial trust between you and that person. From there you might be able to see their first level trusted friends on the app, you could then ask your friend that invited you to verify if they know those users and also trust them, maybe at a lower level of trust, but you trust your friend and they trust these users. Over time this could create a network effect, where you have a strong set of trusted people to talk to. Since this app was designed around dating, and most of that is fairly localized, that can also help determine who is actually in your area or who might not be. Additionally, suppose a new user reaches out, you can see how you might know them through the trusted network you have, or maybe see that they don’t have much of a network at a time and work to confirm things first.

Now this wouldn’t be the final solution, but it would be a good start to keeping the users a lot more safe and private; rather than handing over their ID and everyone needing to trust the Application’s Owners and Moderators.

Additionally, this isn’t a perfect system, this can still be abused through manipulation of the trust network and it doesn’t directly prevent non-welcomed users (men in this case) from signing up and trying to pose as a legitimate user. But fake IDs and AI exist well enough to make a convincing selfie-with-ID - so I’d call it even there. 

You could also extend this using other attribute based methods. As mentioned with using local proximity to verify or send invites, you could also use user general locations to help verify the legitimacy of trusts being created. I am sure there is some math to help determine what the average expected trusts would be between people and if it exceeds that or looks abnormal it could flag a user. I remember during COVID there were apps that would be able to share exposure proximity via BLE, that could potentially be adapted too. Anyway I am digressing a bit here.

## Final Thoughts

The long and short here is, if an App or service states it is privacy focused and asks for very sensitive information to be able to access it, maybe think twice before handing that over. And from the design perspective, sometimes the simplest choice initially, will be the more complicated and riskier process. 
