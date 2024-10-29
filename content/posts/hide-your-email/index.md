---
title: 'Hiding Your Email Services'
date: 2024-10-29T21:00:00+01:00
tags: ["blog", "privacy", "security"]

---
{{< lead >}}
Data breaches are a constant, what can you do? 
{{< /lead >}}

## Introduction

Unfortunately, it's highly likely that your information will be exposed at some point. This has become a common enough occurrence that instead of asking, "If it happens, what do I do?" it's more prudent to ask, "When it happens, have I prepared enough to minimize the impact?"

I’ve considered this from various angles, but one method of protection worth discussing is "Hide My Email Services" like Apple's [service](https://support.apple.com/en-us/105078) with iCloud, or Proton's [service](https://proton.me/support/aliases-mail) and how these services can be used to protect your privacy. 

Keep in mind though, that whenever you plan to increase your security or privacy you will, in most cases, lose some convenience or ease of use. 

### What Are Hide My Email Services?

To start, these services create an alias that will relay any emails sent to it directly to your main email address. These aliases are often a randomly generated name with one or several domains. So, if your email is `jdoe@gmail.com` and you use Apple's Service, it will generate an email like `Jade.0a.Kiwi@icloud.com`. You can then use this email for a website, and even generate multiple aliases that point back to `jdoe@gmail.com`

Think of it as having an unlimited number forwarding addresses for your main email. 

```
Website --Sends Email--> Alias Email --Forwards--> Main Email
```

#### Aliases Alternatives

Some email services also offer a similar feature by allowing you to append a `+` to your email address. So `jdoe@gmail.com` can use something like `jdoe+facebook@gmail.com` as an email for Facebook. This would allow them to know that, in theory, only emails from Facebook should be going to that email, and if they get something from somewhere else they may be able to assume that the email was sold, exposed, or otherwise leaked. 

Now, the issue with this from a privacy perspective is that the root email is clearly exposed. Instead, the goal is to make it difficult to guess your main email address and to ensure your provided email is as unlinkable to you as possible.

## When to Use Hide My Email Services

Now that we know, in general, that these services offer an ability to create unique, random emails that can be used to protect your main email, let's discuss when it might be appropriate to use these services, and the drawbacks in each case. I will order these in what I think are the best way to start as a path to more "advanced" usage. 

### Level 1: This is just temporary

If you run into a site or service that needs an email, but you don't ever plan to really manage the account (I will come back to this point though) then this is a perfect service for that. 

Suppose you're at a restaurant and want to place an order through their website, which requires an email address. You can use these services to generate a temporary email, complete your order, and then delete that email to prevent any future spam.

And that's really it! Use the service as a temporary email, you can make just one for all use cases or generate a new one every time. I would suggest making a unique one for each, if possible, because that let's you get used to managing multiple ones at ones and move on to the next level.

### Level 2: Why do I *Have* to Make an Account?!

Okay, so same as before, you're in a situation where you have to not only provide an email, but also make an account. Rather than using your main email, use a Hidden email instead! Additionally, make sure to use your password manager to generate a random password. 

This site will now send spam only to your randomly generated email. And since the site now has associated login credentials, it could potentially be a source for email and password leaks. However, since they are both random, it is basically just junk. Sure you do need to make sure to secure that account the best you can, remove any other information, credit cards, etc. 

But now this data cannot be used to comprise your accounts on other sites.

### Level 3: Change My Email

At this point, I hope you see where we are going. Taking this a step further, we can start changing our non-critical accounts to use Hide My Email services. Randomly generate a new email, log in to your site still using your root email, and then change it. Oh, and update your password while you are there to make sure it is fully randomized while you are there; and set up MFA. 

Remember, this is only protecting you when it comes to linking the email to you directly and cross referencing/attacking to other sites.

I will want to also add a note here that you should take care on which sites you do this with. For social media, video game accounts, shopping accounts, there shouldn't be too much of a risk using these emails. However, financial sites, government accounts, and other "Identity based sites" you may want to use your root email or other softer alias techniques like the `+` appending technique. Why? Well, it could be more frustrating to maintain or get support with a randomly generated email. Also, these sites tend to, but not always, have a stronger security posture. Remember, we are looking at minimizing impact here, not remove it entirely!


## Is it worth the effort?

To summarize what we can do here is:

1. Get a new service, and yet another subscription.
2. Give spammers meaningless, disposable emails.
3. Use throw-away emails for throw-away accounts.
4. Move existing accounts to these new, randomly generated emails.

This helps isolate sites to a single email, lowering the value of your data provided and protecting you from being identified in a data leak. Additionally, in combination with randomly generated passwords, helps to isolate credential stuffing attacks to just that one site.

But, it isn't all perfect. There are some negatives to consider!

### Negatives

#### Communication
There are times when you may need to send an email from that randomly generated address, like when reaching out to support. This can be clunky or even impossible, depending on the service, and it's generally not as simple as using your regular email address.

Also, trying to call support, or provide the email can get you some odd looks. And it is cumbersome to generate one in person, but not a non-stopper.

#### Authenticity
Another thing to be aware of, some sites have protections around temporary email addresses, particularly ones like 10minutemail. This can lead to issues where your generated email may not be accepted if the domain isn't well known. For example, Apple's uses icloud.com as the domain, which is well known and accepted in most cases. However if you use a service that uses less known domains, or you can use your own, that can lead to issues with the email not being accepted. 

#### Service Provider trust

A significant concern with these services is that all emails going to those alias addresses are accessible to the service providers. For example, Apple could, in theory, see what is sent to `Jade.0a.Kiwi@icloud.com`.

#### Data breaches

When a breach happens you can go to places like [Have I been Pwned](https://haveibeenpwned.com) and put in your email to see where you were affected. However, now you don't see all your potential accounts, as most will have a unique email. In these cases, usually the site does send you an email to alert you, so you will want to monitor for those a bit more actively. When you do get one, you can do your normal response like resetting the password, but also reset the email! 

## All in all

Is this worth it? For you, I don't know. But for me, it is worth applying some of these items. 
