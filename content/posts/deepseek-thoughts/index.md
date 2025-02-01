---
title: Thoughts on Deepseek's Impact
date: 2025-02-01
tags:
  - AI
  - Thoughts
summary: Exploring the Initial Impact of Deepseek AI
draft: false
---
{{< lead >}}
Exploring the Initial Impact of Deepseek AI
{{< /lead >}}

It has been about a week since the most people became aware of Deepseek AI. Although Deepseek AI's r1 model initially released on the 20th went largely unnoticed, it gained attention after impacting the stock market the following week. During that week a lot has happened; from confusion to dismissals to speculations and concerns. I've been asked by a decent number of people what I thought of this situation, which spurred me to write up my thoughts.

I must preface this by stating I'm not an LLM expert; however, there is a lot of information to unpack. My aim is to highlight which aspects of Deepseek are crucial, worth considering now, and which remain unknown. I'll try to break this down into a couple of topics; how it affects the current AI incumbents, is it safe to use, what information we could accept or should be critical of, and how this can affect things in the future. 

# Deepseek and the Incumbents

This is most likely where most have initially heard of Deepseek, that it is a new Chinese built LLM that is comparable to the most powerful, available, models from places like OpenAI. Benchmarks are available to analyze how different models compare. However, many people simply want to know whether it's good, and in that regard, yes, it is.

A new model being better than an older one isn't really news worthy in of itself, but it is more so the cases of how it was made, where it was made and its availability.

Starting with how it was made; this was a side project from a Chinese investment firm which was able to make this model with around $6 Million dollars worth of investment. It is important to be critical of this number for various reasons, but we should not overly focus on it. Even if it cost $100 Million, it would still be significantly less than what it has cost to create the models it is competing with. 

The next key fact of its creation is that China is under an embargo from getting the latest computer hardware, e.g. chips. Meaning this model was trained on older hardware. Again, it should be noted there is a consideration of "[standing on the shoulders of giants](https://www.404media.co/openai-furious-deepseek-might-have-stolen-all-the-data-openai-stole-from-us/)," in that some research and development has already been done, and they were potentially leveraging other available models to support the training of this model. Regardless, they proved that it was relatively cheap to create this model.

Lastly, the model was made under an open license: meaning (1) the model is free to use and modify; (2) you can use their website or app and run the model on their servers; (3) you can also download the model and run it locally. Essentially, this means that you now have the ability to run a model on par with the best available from OpenAI for a fraction of the cost.

So in short, this was made extremely cheaply, provided freely with the ability for others to modify it for their needs - [showing that maybe the incumbents with their access to powerful hardware may not be as untouchable as initially thought](https://www.404media.co/deepseek-mania-shakes-ai-industry-to-its-core/). Thus confidence fell, causing the stock market to react. 
# Is it safe?

With that being said, is it safe to use? Well, it depends. 

Starting with the hosted version, from their website or app. When it first came out I was wary of it, mostly because it is a new SaaS tool and hasn't really been reviewed or tested. So use at your own risk, and maybe don't ask it (read provide it) anything personal or private. That wariness proved to be warranted as [security researchers have already found a fully accessible database that they were using to chats and logs](https://www.wiz.io/blog/wiz-research-uncovers-exposed-deepseek-database-leak). 

Additionally, Italy has begun pressuring them to review and adhere to various data processing laws. They did something similar with OpenAI's ChatGPT when it first came out, and was later sufficiently reviewed and approved. However, with Deepseek, they have taken the stance that they only seem to fall under Chinese data laws; as that is where their servers and company are located. 

So, is it safe to use the app and website? I would say **no**, not until they start adhering to and proving that they are handling data securely. Now, I do also think that when you use ChatGPT, Google Gemini or any of the other hosted AIs, you should always take care to avoid providing more information than you feel comfortable with being used and stored by them.

Consider using DeepSeek locally instead. Running a [large language model (LLM) locally](https://medium.com/@ahmed.imtiaz2000/how-to-run-deepseek-locally-using-ollama-a-step-by-step-guide-14cd7b3feec5), without an internet connection, should offer more privacy since you control the computer processing the requests and have full control over it. 
# Being Critical

There is a point of contention on the model's training data and censorship. The gist is, this model has censorships on things like the Tiananmen Square and other topics. Now, I think the topic of censorship is beyond this post, but I do want to say that all models are censored in some way; they will all have bias and you should always consider who built the model. 

Furthermore, there are concerns about models being trained to provide seemingly harmless but actually malicious information. [This is theoretically possible](https://arxiv.org/abs/2401.05566). It is important to carefully examine the information provided by any model before taking action. 

I have often taken the stance that you should treat an AI like an Intern, where they have a lot of time to get you answers on things or confirm things, but they can get things wrong. And they are heavily dependent on how you ask them to do something. In short, use them to augment and not replace you processes.
# The future

In summary, DeepSeek has demonstrated that creating a powerful large language model (LLM) doesn't require massive hardware investments like OpenAI and others have made. This opens up the possibility of more players entering the field. However, it also highlights the importance of not blindly trusting new SaaS offerings with sensitive information until they have been thoroughly vetted.

For now, it might be prudent to avoid using the app until it has passed regulatory scrutiny in both the EU and US. Although these regions have their own biases, a consensus of reviews can help establish a baseline level of security.

We will probably see more models come out that are based on Deepseek, or trained in similar ways. This also applies to the big players, who should also benefit from this information to optimize their own training on top of having the most compute power to do even more. 

Time will tell if this pushes to more availability of LLM models, or if the most powerful will still be closed behind big technology players.
