---
title: "Anthropic’s $1B to $19B growth run: how Claude became the fastest-growing AI product in history | Amol Avasare"
date: "2026-04-05"
type: "podcast"
guest: "Amol Avasare"
description: "How Claude became the fastest-growing AI product in history, covering growth systems, AI product work, and team leadership."
word_count: 22125
---

**Lenny Rachitsky** (00:00:00):
A lot of companies claim to be the fastest growing companies of all time. Anthropic actually is. You guys were at a billion ARR at the start of 2025. The last number I've seen is 19 billion ARR. That's $1 to $19 billion in 14 months.

**Amol Avasare** (00:00:14):
Historically, we were very much the smallest, least well-funded player in this space. We didn't have the free cash flow or the distribution of a Meta or Google. We didn't have the first-mover advantage of an OpenAI. It's a complete miracle that we've gotten to the stage that we have.

**Lenny Rachitsky** (00:00:29):
Give us just a glimpse of what is like to be leading growth inside of Anthropic.

**Amol Avasare** (00:00:34):
It's the hardest job I've had in my life to come into Anthropic. You need to understand that 50%, 60%, 70% of how you operate in the past, just throw it out the door.

**Lenny Rachitsky** (00:00:41):
One of the cleverest growth moves you all made was this idea of importing memory from ChatGPT.

**Amol Avasare** (00:00:47):
Activation is a really big challenge in AI. We are starting to look at how do we automate growth. Our growth platform team is driving this effort called CASH, which is Claude accelerate sustainable hypergrowth. How can we use Claude to automate growth experimentation?

**Lenny Rachitsky** (00:01:04):
And it's delivering results, you're basically living in the future.

**Amol Avasare** (00:01:06):
We always talk about the exponential. The product value that we will deliver in two years time is probably like 1000X, what it is today. The funniest thing is I've noticed internally, linear charts are just not cool. Everything is log linear. So show me at log linear scale.

**Lenny Rachitsky** (00:01:22):
Today, my guest is Amol Avasare. Amol is head of growth at Anthropic, which is on the most unprecedented growth run in history. In the past 14 months, they grew from 1 billion to over 19 billion in annual recurring revenue. Just in the past few months, their revenue doubled. They've been growing 10X year-over-year. This is unheard of at the scale. By the time this episode comes out, their revenue will be even higher. To put this scale in perspective, companies like Atlassian, and Palantir, and Snowflake, which have been around for 15 to 20 years, each do something like 4.5 to 6 billion in ARR. Anthropic is adding this much ARR every few months.

**Lenny Rachitsky** (00:02:04):
And if that isn't interesting enough to you, Amol who leads growth at Anthropic is an incredible human. He previously led growth at Mercury and MasterClass. Before that, he was a founder and an investment banker. And most interestingly, something that most people don't know about him is that Amol suffered a severe brain injury. He had to spend nine months relearning how to walk and work and just not be nauseous all the time. He shared this story in a guest post in my newsletter a number of years ago. We actually chat about this during the conversation. These are my favorite kind of conversations because Amol and his team are living in the future and he's come to tell us where things are heading and what's going to change.

**Amol Avasare** (00:03:22):
Pleasure to be here.

**Lenny Rachitsky** (00:03:24):
Head of growth at Anthropic. No big deal. I've had a lot of people come on this podcast from companies that claim to be the fastest growing companies of all time. And Anthropic actually is, if you look at the trajectory, I just have some of the numbers here just so people understand how absurd this is. So you guys were at a billion ARR at the start of 2025, then hit something like 4 billion mid 2025, then 9 billion ARR at the end of 2025. And the last number I've seen is you guys are at 19 billion ARR, which just to put a couple pieces of context here, one is that's from $1 to $19 billion in 14 months. I have so many questions. First of all, the story of how you actually landed this role is really interesting. Talk about how you got this role.

**Amol Avasare** (00:04:15):
Yeah, it's a little unorthodox. So it's funny, when I did my onboarding, they walked through what percentage of the cohort came through referrals, what percentage came through applying on the website, what percentage came through sourcing? And I was on none of those. And I was like, "Okay, this is interesting." And basically the way that I got to Anthropic was that I was actually a user of Claude and I was using a lot. I was like, "Man, these guys, great product, great company, but they really obviously don't have a growth team." And what I did was I just sent Mike Krieger a cold email. He was the chief product officer. I sent him a cold email saying like, "Hey, love what you guys do, love the product. I think you guys badly need a growth team. Want to chat." And I didn't expect he would respond.

**Amol Avasare** (00:05:02):
And he responds and says, "Hey, yeah, I'm interested. Let's talk." And it's funny, I didn't know. I wouldn't have known. They were not hiring for a growth team. There were no growth PM roles listed, but they were just at that time starting to think about hiring a growth team. So it was very good timing. But yeah, spoke to Mike and one thing led to another. He said, "I'm the only PM that he's hired from cold email." And I feel very lucky that he decided to respond to my email.

**Lenny Rachitsky** (00:05:31):
I did not know the story. That is another absurd fact. Clearly you're good at cold email. What did you do in this cold email to get his attention?

**Amol Avasare** (00:05:40):
I would say I've basically perfected cold email over the years. So when I was a founder, I had to get really, really good at this. So I sent a lot of cold emails out and just honed the subject line, the message, and the tone. And so basically in the subject line, the first thing is from a conversion standpoint, someone sees the email, they need to click on it. And so I have a copy that I've tested that is very, very high open rate. And so-

**Lenny Rachitsky** (00:06:10):
Wait, what is this copy? Or is this a secret?

**Amol Avasare** (00:06:12):
It's a secret. I think [inaudible 00:06:12].

**Lenny Rachitsky** (00:06:11):
Okay. We'll keep it a secret.

**Amol Avasare** (00:06:12):
It's a secret. So that's one, getting them to open. I think the second is then the tactics of you need to understand where are people getting outreach. And if everyone's getting outreach in one area and then you reach out to them there, then you're not going to get as high of a response rate. So you can think about LinkedIn, you can think about work email. These are things that everyone is emailing. So there's ways to get people's personal emails out there. And so that's one thing that I did. And so okay, I've got this personal email, I know the copy that works, and then it's just keeping it very short on here's who I am, here's why I'd be a good fit, and we should chat.

**Amol Avasare** (00:06:49):
And these things typically don't work. And then you should always follow up a few times. I think my role of thumb is like, if I really care about it, I should just keep reaching out to them until they tell me, "Please stop." And so I would've kept doing that, but he responded the first time.

**Lenny Rachitsky** (00:07:03):
It makes sense that a talented growth person would be very good at cold email and getting people's attention. So that's almost like an interview step is just, did I want to read this email?

**Amol Avasare** (00:08:36):
Yeah, I'd say it's very much a company-wide effort. So yes, we are the growth team. We have done great. I think we've driven a lot of impact. But honestly, man, we can't claim too much credit for the success of the company. We as Anthropic are really a model company and an intelligence company first and foremost. And so the lion's share of what has driven our success is our research team. We have, I think, the best research team in the world. We have great teams on inference and compute, and then there's many other teams like Claude Code, go to-market, et cetera, who I think deserve much more credit than us. I think just zooming out, going to some of what you said earlier, that the growth trajectory's just been insane. That 10X year-on-year revenue growth trend has been there since the beginning. I think 2023 was 0 to 100 mil, 2024 was 100 to 1, last year was 1 to roughly 10.

**Amol Avasare** (00:09:29):
And I look back to when I joined in 2024, revenue was in the hundreds of millions and just that trajectory through the end of 2024 and 2025, week two of when I joined, we're going into 2025 revenue planning and we have these base case and aggressive case scenarios and Dario's pushing the aggressive case scenario and people are freaking out being like, "How the hell are we going to hit that?" And Dario's like, "I think we can actually go much higher than that." And I'm coming in, this place is crazy, there's absolutely no way. And that happened. And then you get to the end of 2025 and it's like, okay, law of large numbers, there's going to be a pretty big slowdown here based on your baseline rate of 10 billion, how are you going to keep growing at this rate? And it just has not slowed down.

**Amol Avasare** (00:10:16):
And those numbers are public. The 19 billion number you quoted is from the end of Feb, so that is also out of date. And look, it's absolutely insane. The funniest thing is something that I've noticed internally is linear charts are just not cool. No one cares about linear charts. Everything is log linear. You have to show me at log linear scale, and that's a scale we think. And I think overall, we're just really hanging on by the seat of our pants. So we're trying to manage the growth and do the best that we can for our users.

**Lenny Rachitsky** (00:10:46):
I was talking to somebody at Anthropic about you, and they said that basically anytime they want something to grow, they ask you to help and it works. So you talked about just things are magical and amazing and Claude and all the tools you all built are amazing innately, and that's a big part of the reason they grow. I think many people listening to this will be like, "What do you even do, Amol, with a magical microgod that just can do anything for you? Why do we need a growth person? What do you even do?" Talk about just the stuff that you focus on and maybe a couple of the wins that your team has shipped that has helped accelerate growth.

**Amol Avasare** (00:11:21):
I would say they're not fully wrong. We're very, very lucky to have the best models in the world. We're very lucky to have products like Claude Code and Cowork. It certainly makes life a lot easier. Having said that, I would say this is the hardest job I've had in my life, and that's having been a founder, having been an investment banker and other things like that, it's tough. And if I look at what do we do as a growth team here, I think ultimately it's the same categories of things that you would think about at a normal company. So we care about acquisition, how are we getting more people in the door, the intent of the people coming through the door. We care about activation, the signup flow, funneling people to the right products, making them successful. We care about things like monetization, free-to-paid conversion, pricing and packaging, all of that stuff that the categories of work is the same.

**Amol Avasare** (00:12:13):
I think then probably the big differences is I would say that roughly 70% of what I spend my time on is what we internally refer to as success disasters. And that is where things have gone so well that other things are breaking now. And I think anyone who's worked at companies that have gone through rapid growth, you think like Facebook, or Uber, or DoorDash early on, they understand this viscerally where scaling this much just brings a lot of challenges. So if you think about each of those categories on acquisition, on activation, on monetization, there's just a ton of firefighting jumping from one urgent thing to another. And it's often extremely painful. And it's funny because you look at all the charts, all the charts are green, fully up onto the right, and everyone's just like, it can be quite tough emotionally still. And so you need to step back and just realize we're very lucky to have these problems.

**Amol Avasare** (00:13:07):
But that's 70% of my time, I'd say, is just these firefighting of success disasters. And I think the 30% remaining is just much more standard bread and butter growth work where it's more proactive. So you think about, okay, if we have limited resources, we have many different products, which of the products do we want to put some juice behind? What does our long-term pricing and packaging look like, especially given that the technology's changing a lot and behavior and engagement trends are shifting. And then things like we have a lot of new products coming up like, okay, you ship Cowork, now what? When is the right time that we should lean in as a growth team to start optimizing the core adoption funnel for Cowork? So it's probably 70% just crazy firefighting, 30%, more bread and butter stuff.

**Lenny Rachitsky** (00:13:53):
Okay. I'm going to dig into a lot of that stuff. One of the cleverest growth moves you all made recently was this idea of importing memory from ChatGPT where you just made it really easy and jumped on this trend of people getting really excited about Anthropic. Is there anything you could share about the behind the scenes story of that feature?

**Amol Avasare** (00:14:11):
We're just thinking about what can we do to improve the cold start problem and improve the new user experience. I think that activation is a really big challenge in AI. And so that's one example of something that we shipped that was very specific to a moment in time. But ultimately that you zoom out, it's like, okay, how do you really make it easier for people who are signing up to have Claude understand who they are and understand how Claude can help them and get them to the right place?

**Lenny Rachitsky** (00:14:43):
I want to follow that thread, activation. That's something that comes up a ton when I talk to people leading, driving growth on AI products. It's just there are so much stuff trying to get your attention these days for people to get to a place where they, okay, wow, this is really going to be something I want to keep using. It proves to be really hard. And it's also just unreliable sometimes, it's not going to be magical. It's AI, it's non-deterministic. I guess, one, is just how important is focusing on activation, getting people to that aha moment with AI products? And two, what are some things you've learned about how to do that well with Claude or AI in general?

**Amol Avasare** (00:15:19):
Yeah, it's a good question. I think that activation, it's critical and defining that as early activation, call it day zero, day one product experience. I think that historically anyone who's been in growth or been in product understands that that's usually one of the highest levers that you have to actually even increase longer term retention. And I think that the importance of that has just gotten exponentially higher. Now, zooming out, I feel like one of the biggest problems in the industry is capability overhang where the models are just getting better so quickly. And the real challenge is on the product side of how do we start to diffuse those benefits to people where even internally, there's new models coming internally and you're sitting there, you're so busy. And when a new model's available, you need to really carve out time to be like, "What can this do? How do I need to update my priors?"

**Amol Avasare** (00:16:14):
And if you think about more broadly for most people, you may have a model that is like, you may have AGI or some model that can do all sorts of crazy things, but if people's instinct is to come there and be like, "Hey, what's the weather in SF?" Then they're not going to get the most out of the product. And so I think that it's tough because the model capabilities are rising so much. So if I think about, okay, back when we had, I don't know, I want to say Opus 4, there's a series of things the model can do at that point, and Opus 4.5 unlocked a whole bunch of new things. You think about, okay, we sit there, we've got this new model, Opus 4. The time to then go and run a bunch of tests, figure out, okay, there's the capabilities from this new model, what are the right on ramps to guide people to those features?

**Amol Avasare** (00:17:03):
You run tests, you get the learnings, you then ship a new flow. By then, you may already have the next model, which unlocks newer capabilities that makes all these learnings irrelevant. So it's actually just a really difficult problem to stay on top of. I think that many of the same things, same old trends in growth and activation remain, I think, accurate where to me it's like ultimately some of the highest leverages from finding the right product or the right feature for the right user. And I think that one learning, seeing this time and time again across companies, actually the right friction helps and adding more friction usually works if you do it the right way. I think that's something I've consistently seen that we've seen here as well. So to me, I think it's really being able to identify what are the characteristics of a user that allows you to then recommend them to the right feature or product and not being shy about adding friction to do that, I think is probably the single biggest thing that's important here.

**Lenny Rachitsky** (00:18:05):
When I asked Ben Mann, one of the co-founders, former podcast guest, what to ask you about, and this is what he highlighted, is your experience, especially at Mercury redoing onboarding and making it magical. And basically he's in the same place as you of just how important it is for people to understand what the AI tool is capable of to help people decide to use it and stick with it. Is there an example of something you changed in onboarding that helped significantly improve activation?

**Amol Avasare** (00:18:33):
Yeah, it's a great question. And I like that it brings up Mercury. I talk about their product a lot. So worked on the growth team at Mercury, I think it's a fantastic product. It's something many people use, and the reason they use it is because the better banking experience than its-

**Lenny Rachitsky** (00:18:47):
Yeah, I'm a very happy customer just to put that out there. I love it.

**Amol Avasare** (00:18:50):
It's a great product. Highly recommend it. They have personal banking. Everyone should go and use it.

**Lenny Rachitsky** (00:18:54):
Right. They just launched that.

**Amol Avasare** (00:18:57):
And so I think that the interesting thing about Mercury is the core value is that it's a better experience. That's the reason you use it. You're not getting better other things, just it's a better product experience. And so that ethos is very, very deeply held within the company. It comes from a number of the founders. And I think that we had a big push one quarter when I was there on the onboarding flow. So onboarding flows for banking institutions and regulated entities are extremely complex. The amount of time I've spent on the difference between a registered agent address and a legal address and a physical address, these things are very, very complex. And we basically looked at the onboarding flow and we were like, okay, we've invested so much in quality and the rest of the product, but we haven't really done it here. And this is the first experience that people have.

**Amol Avasare** (00:19:48):
And so we said, forget metrics, forget growth, forget everything else. As the growth team on conversion, we're going to spend a whole quarter fixing quality in this flow. And so that's all we did. Forget the metrics. We're just going to make this as good of an experience as we can and fix all these. You go back from one field to the other field and adding in your beneficial ownership details. And it actually ended up being, and probably until I joined here, the single most impactful quarter that I've ever had as a growth PM in terms of the impact that it had. And so we saw a significant uplift on basically our onboarding started to completion from just focusing on quality.

**Amol Avasare** (00:20:28):
And so that to me is a broader learning around quality drives growth that I think I've tried to bring to Anthropic. I think for us at Anthropic, some of the things that we've done in the onboarding flow is basically we ask users questions around who they are, what their interest areas are. And we then use that to recommend different products and features. And number of people look at the flow and they're like, "You have so much friction. It's such a long flow." And I'm like, "We have the data. We're kind of happy with how that's performing."

**Lenny Rachitsky** (00:20:57):
What is your kind of philosophy on good friction versus bad friction?

**Amol Avasare** (00:21:01):
I've just seen time and time again at every job I've been in growth that adding friction and adding the right steps leads to higher conversion and higher funnel completion. So you want to get rid of... And especially if you have high volume, you should test the majority of this and just learn and see, does this apply to your business as well? But you want to get rid of annoying friction that doesn't add value. But I think the most simple understanding people have is just solve time for value, cut all the steps and just get them into the product. And that doesn't work most times. I think if you've really thoroughly tested your flows, I look at the companies I've been at, MasterClass. If you go through MasterClass's purchase flow right now, you'll go through all these steps in this quiz when you land on, when you're trying to buy.

**Amol Avasare** (00:21:57):
And you're like, "I came here to buy and it's taking me through all these questions, what are you here for, et cetera." I think it's easy to look at that and be like, "Why do they have this? This is a terrible thing. Just cut it all." And it's like, no, that's been thoroughly tested. And actually that was a significant revenue driver because it helps users feel that the product is for them by understanding what their interests are and then recommending the content and classes there. One of the growth PMs on our team left to join Calm, Calm.com, the meditation app. If you go to Calm's, their landing page and you go through their purchase flow, their login flow, you'll see a quiz. It's not a coincidence that at Mercury we also tested, I think Immad posted on Twitter, we broke out some steps in onboarding. And just having one screen, if you have five or six different form inputs and you often break that into two screens and reduce the cognitive load to people, that is something that performs well.

**Amol Avasare** (00:22:54):
We added steps into the flow there that actually performed well, same at Anthropic. So I think that the takeaway to me is cut friction when it doesn't add to the experience of helping a user understand why the product is for them. But if you can help users understand a product, why product is for them and how to use it and what's most relevant to them, and it's going to add friction, don't shy away from it. Test it, confirm that it works for you, but I think this is something that most growth practitioners deeply understand.

**Lenny Rachitsky** (00:23:28):
And for them is really important there, what you described is adding friction to better understand who they are so that you know how to recommend the right thing for them.

**Amol Avasare** (00:23:38):
Correct. Yes. And that done right, it just flows through. So it helps you with activation, but then it helps you with lifecycle. You know more about those users and why they're here. And most sophisticated businesses, you can then, even if someone drops off, you can do lookalike targeting and you can get them at the ad layer as well. So that initial piece of how you understand who the user is just like it's a juice that just keeps on giving if you then use it right for the down funnel.

**Lenny Rachitsky** (00:24:06):
Everyone's about to go do a bunch of tear downs of Claude's onboarding, MasterClass onboarding, Mercury onboarding. As a tangent, I was at this PM dinner recently and I was asking all the PMs, how has your role as a PM changed most with AI? Where has AI most impacted what you do? And one of the PM's answer that is actually doing competitive analysis, doing a bunch of teardowns of what other people are doing for pricing pages and onboarding. So it's easy to do now. Just, "Hey, Cowork..." I don't know, would you use Cowork for this or Claude? What would you use for that? Okay, this is good. Help people pick which tool to use. If you want to go do a bunch of teardowns of other competitors' onboarding flows, what would you use?

**Amol Avasare** (00:24:44):
You can use Cowork for this, right? So you have Cowork with the Chrome extension. So if you task Cowork with a Chrome extension, go and look for these flows and give me a view of what's working, what's not. That's definitely something that Cowork can do.

**Lenny Rachitsky** (00:24:58):
Cool. And I imagine that's one of the challenges is you have all these tools now, just which ones for me. By the way, the Chrome extension, I use it all the time. It's amazing. I want to drill a little bit further into the growth org. There's this whole meme on Twitter the other day of just like you have one growth marketer driving all growth at Anthropic and it's like, okay, that's crazy. How many growth people are there? What's the rough org structure of the growth team?

**Amol Avasare** (00:25:22):
We're roughly maybe 40 people now. And so we are, I think, structured very much like a traditional growth team in that we have horizontals of growth platform and monetization who think about the sphere of growth across the entirety of our products. And then we have more audience-focused growth pods. You can think about B2B growth, you can think about Claude Code growth, knowledge worker growth, API growth. So really these audiences to keep a narrow focus, which is the thing you have to do when you have so many different products. And then these horizontals that think about things across the board.

**Lenny Rachitsky** (00:26:05):
And is it across a team of engineers, designers, PMs? What's the functions within this growth org?

**Amol Avasare** (00:26:11):
Yeah, it's engineers, designers, PMs, data. I think that overall the shape of the org is quite similar to, I'd say a traditional growth team. Probably the things that are maybe different is that I think that we index a lot more towards larger swings as opposed to smaller optimizations. If I think about a traditional growth team, I would've probably done maybe 60%, 70% of my time on small to medium bets, 20% to 30% on larger swings. And I think that for us, we flip it a lot. We do much more the other way where it's 70-30 or more like 50-50 rather than indexing towards smaller bets. That's probably one of the biggest changes, I think.

**Lenny Rachitsky** (00:27:06):
Just to highlight that, what's interesting there is at the scale you guys are at, a 1% win is massive in the scheme of things. So it's interesting that even at the scale you're at, you're not focusing on these micro optimizations.

**Amol Avasare** (00:27:19):
It is easy. You could easily focus on these small optimizations and then you tally them up at the end of the quarter and you're like, "Look how much impact we made." And you could do that.

**Lenny Rachitsky** (00:27:26):
Another billion. No big deal.

**Amol Avasare** (00:27:27):
Yeah. But the thing is we've been tracking at 10X year-on-year, and that's the thing that we keep in mind. And I think it ultimately comes down to our fixation of this company about the exponential. I think if you look at anyone who's talking from Anthropic about basically anything, we always talk about the exponential. It's effectively as model capabilities continue to grow on an exponential and the tools around them enable a better job of diffusing that into useful use cases, you basically just keep unlocking new markets where the value of those markets significantly dwarfs what the value of the previous markets were. And agentic coding's a great example. It didn't exist a year, a year and a half ago. And then now just the value of agentic coding is bigger than the previous market of AI coding use.

**Amol Avasare** (00:28:22):
And so I think that is the core thing here where just that the future product value is in order of magnitude higher than it is today. And I think about, I don't know, a normal business, number of companies that I maybe mentioned, or you think about a trading app or a grocery delivery product, many of the leading companies, they're great businesses. But if I think about what is the product value that a company, like a standard, call it a grocery delivery app, what is the product value you get as an end user today versus two years from now? I look at it as like, okay, in two years from now, even if you're shipping all these new products, as an end user, the value you get-

**Amol Avasare** (00:29:00):
You're shipping all these new products. As an end user, the value you get from that product maybe goes up 30 to 50% if the company's done a really good job of shipping new features. It's not exponential though.

**Amol Avasare** (00:29:12):
And so if I think about, "Okay, you're here today. In two years, you're going to have 30 to 50% more product value." Then as a growth team, the relative differential of the product value in two years from now relative to today, I can actually capture a decent percentage of that with the small to medium optimizations that typically have higher conviction as opposed to larger bets.

**Amol Avasare** (00:29:36):
But for Anthropic, it's not really that way, where because of the exponential and our products being very, very, very ... The product value coming from AI, the product value that we will deliver in two years' time is probably a 1,000x, a 100 to a 1,000x what it is today.

**Amol Avasare** (00:29:58):
And so if I think about that, and it's like there's so much value on offer, you need to shift more towards, "Okay, we need to take larger bets and we need to not miss the forest for the trees." And so that's why we still do all the smaller optimizations. It really matters, and no one else is going to do some of these things and so we need to do it. The compounding value is not immaterial, but we do take on much larger core productey type of swings as well.

**Amol Avasare** (00:30:25):
So you mentioned the Chrome Extension. That is now the thing that underpins a number of use cases on Cowork and Claude Code as well. And that's something that the growth team built. That's a very AI-peeled product that is a very research-heavy product that we were just bullish on it. We had an engineer who was very bullish on it and we were just like, "Hey, no one else is doing it. We're going to do it." And so that's the sort of thing that I wouldn't have done at another company.

**Lenny Rachitsky** (00:30:53):
Oh, wow. I did not know that. So one takeaway here is there's stuff to extract from your advice that is only true in Anthropic and then there's, what can other companies learn from this experience that you've had?

**Lenny Rachitsky** (00:31:09):
So one is, is your sense that if you're working in AI, shift more of the pie chart towards bigger bets because in the future, the opportunity is so large, you want to find those as soon as possible versus micro-optimize?

**Amol Avasare** (00:31:25):
To be more specific there, I would say that if the primary value that your product delivers is underpinned by AI as a central element of it, then I think you should operate this way. So I don't know, companies like Lovable, Cursor, all these great businesses that are, as the exponential rises, their value props are also going to continue to rise significantly.

**Amol Avasare** (00:31:50):
If you're building a product where it's an AI-first product, then I would definitely operate in this way. I think if you're building a product where it's not necessarily an AI- first product and you have some AI features that are on the side, but it's not the core of your value, I don't know that I would operate this way. It would depend on how is the rest of the product org staffed and how is the growth org staffed in relation to that.

**Lenny Rachitsky** (00:32:14):
Okay, awesome. And then in terms of the way you are structured, I thought that was really interesting. It's a combination of different sorts of things. So there's the API growth, there's Claude Code growth, but then there's also personas, like a vertical of knowledge workers and B2B. Is that intentional, some specific bets and one just broad market opportunity?

**Amol Avasare** (00:32:35):
When you have one product, it's easier to have a growth team that's more purely on the funnel. It's like you have the conversion, you have activation, you have monetization. But as you start to get into having multiple products, I think that's harder because if you do that, then if you just have one activation team, for example, but then you have Claude Code, you have Cowork, you have all the other things. They're very different audiences and they're very different sets of cross-functional stakeholders internally.

**Amol Avasare** (00:33:01):
So we're kind of looking at, what is the thing? And all org structures are not perfect and they're right for a point in time, but we're looking for what is the structure that allows us to have as much focus. Focus is a really big thing, and on audience and problems.

**Amol Avasare** (00:33:19):
And also, the tie-ins to cross-functional partners is really, really important. The folks on our Claude Code growth team, they work extremely closely with Cat and Boris and the others on that team. And so that tie-in is really important as well.

**Lenny Rachitsky** (00:33:34):
So you've done growth at a lot of different companies, a lot of basically, let's call it traditional growth before Anthropic. How else is growth as a function and as a skillset changing with the rise of AI, AI products, and AI startups?

**Amol Avasare** (00:33:47):
I think if your core product value is very backed by AI, then it is shifting where you're skewing more towards larger bets as opposed to smaller, medium experiments. I think in other things, it may be a big thing related to this that I think will accelerate this, which I am really interested to see how it will play out, is we are starting to look at how do we automate growth, which I think is a really interesting area.

**Amol Avasare** (00:34:16):
So our growth platform team, we're very lucky we have Alexey Komissarouk who teaches growth engineering at Reforge, and he's just the guy on the team. And so he is driving this effort. The name is, it's a little cringey. I didn't come up with it. And it's called CASH, which is Claude Accelerates Sustainable Hypergrowth. I did not come up with that, but really it's an effort to look at how can we use Claude to automate growth experimentation?

**Amol Avasare** (00:34:48):
And it is still very, very small. It's still very, very early. We kicked it off only, I think, a couple of months ago. I think before Opus 4.5, it wasn't really possible. We were just not seeing the results. And more recently with Opus 4.6 we're like, "Okay, this is headed in the right direction."

**Amol Avasare** (00:35:07):
And so this, I think, it will happen more and more across the industry, where basically if you think about, okay ... I think this can happen all across product, but growth teams in particular because there's this whole body of work that is very small optimizations, I think are just more inherently suited to tackle this earlier.

**Amol Avasare** (00:35:29):
I think if you think about the lifecycle of shipping, there's four parts to it. One is identifying opportunities. How good is Claude at actually identifying opportunities based on different trends, based on previous trends that Claude has seen in the past? Second is then building the actual feature and getting it ready to ship. Third is testing and ensuring that it meets your quality bar and your brand bar. And then fourth is then once you've actually shipped the thing, analyzing the data, gathering the learnings.

**Amol Avasare** (00:36:02):
If you think about that as the loop of, "Okay, these are four things that you can eval and hill climb on each of these areas and understand how good is a model doing for you there." And we basically think about it in that four ways and we are scoring how good is Claude doing in each of those areas.

**Amol Avasare** (00:36:24):
And so we've been testing this at pretty small scale right now. It's been a lot of copy changes and some very minor UI tweaks. It's delivering results and it's like you can push it, press play with it. And it ultimately prints money where I'd say that the win rate is like, I would expect a senior PM to do better. I would say this is a junior PM, two, three years in. I would say this is the win rate that I would expect from a junior PM, but it's not quite at the senior PM level. Although, I think you look at the exponential, this wasn't available at all a couple of months ago. So it's getting better rapidly.

**Amol Avasare** (00:37:03):
And I think that it's going to change where you'll be able to do this for larger and larger types of experiments. But then you think about the largest types of experiments, I think that I mentioned the four pieces around identifying opportunities, building, testing and shipping. The one I didn't mention there, Lenny, is cross-functional stakeholder management.

**Lenny Rachitsky** (00:37:26):
There's still a need for human brains. There is.

**Amol Avasare** (00:37:31):
And I think that that one is going to mean that in my eyes, the work of PMs is not going away actually, anytime soon. And that piece, especially for larger projects. Usually, you don't need to do as much of it for smaller stuff. You can skip it. But for larger stuff, that piece is not going away.

**Lenny Rachitsky** (00:37:51):
Until the other stakeholders have their own little agents running around.

**Amol Avasare** (00:37:54):
I think that's right. I think that would be the point where it changes. It's funny, we had a difficult meeting a couple of weeks ago, and me and our head of design, Joel, we were debriefing afterwards. And he pings me, he's just like, "Amol, we will have AGI and it will still be impossible to get six people in a room to get to align." And I'm like, "Yeah, I think I can say that."

**Lenny Rachitsky** (00:38:16):
What's the harder alignment problem? Oh, okay. This is so interesting and this is exactly where I feel like things are going. So just to be clear what you shared here, there's basically this tool that comes up with experiments to run, to help grow Claude and all the tools.

**Lenny Rachitsky** (00:38:36):
So it comes up with idea, somebody looks at them, approves, "Cool, let's do these things." Builds it, ships it, tests the results, see how it's doing, and then comes back of, "Here's things that are working." Is that roughly right?

**Amol Avasare** (00:38:48):
It's roughly right. And right now, we have human in the loop approving, but the amount of time, I kind of think about scale in this way of just week on week, are things getting better in each of the areas? Are people spending less time on each of the areas? Are the results getting better in each of the areas?

**Amol Avasare** (00:39:04):
And as long as week on week, that's getting better, then you're like, "Okay, this whole initiative is scaling." And so that's roughly right, but you can think about it as, I think a lot of this can be automated where human review is not needed.

**Amol Avasare** (00:39:17):
So we care a lot about our brand, right? So that is something that we do look at right now. We don't want to be shipping something that goes against the brand, but then you can have a skill that contains your brand guidelines and very clear, yet dos and don'ts on brand.

**Amol Avasare** (00:39:36):
And so all of these types of accompaniments, I think are going to get better. The model's going to get better at understanding how to use them. And so over time, I think that the need to human review this really, really decreases significantly.

**Lenny Rachitsky** (00:39:50):
Yeah, and you could always unship it if it's like, "Oh yeah, that was actually not a great idea." And that's such a good point that we think we need people to do these things forever. And it turns out, "Okay, a skill could do this really well. Here's our brand guidelines, here's our vision, here's our mission, here's our goals, here's what matters to us. Okay, no, let's not ship that thing."

**Lenny Rachitsky** (00:40:06):
So the reason I think this is so interesting, I've just been watching the expansion of AI doing more of the product development process, in this case the growth process of just, okay, it went from helping you write code, to writing all your code, to reviewing your code. Now it feels like, what are the two ends around this? It's kind of going from the middle up. The top of that is coming up with what to do and then there's the alignment stuff's still very hard.

**Lenny Rachitsky** (00:40:32):
And then on the other end, it's reviewing the code and then shipping it and then get distribution. That's a whole other thing I want to talk to you about. So what I'm hearing here, and this is exactly what I thought was going to start happening, is AI is now getting really good at telling us what to do, not just taking our orders and building it.

**Lenny Rachitsky** (00:40:49):
And it feels like the growth version of this is where it starts because it's so much simpler, not that growth is easy, but just like it's data-driven, there's this loop that you talk about. So I think this is such an interesting sign of things to come across just generally, product.

**Amol Avasare** (00:41:04):
Yeah.

**Lenny Rachitsky** (00:41:05):
Just putting that out there. Okay. So something that I'm constantly thinking about along these lines is just the future of product PM engineering, how those roles shift over time based on the stuff we're talking about.

**Lenny Rachitsky** (00:41:18):
How are you working together as a triad and where do you see these roles going? What's most going to change, do you think, across these three roles?

**Amol Avasare** (00:41:28):
This is something that we talk about and think about frequently, and the picture changes rapidly. So sometimes when things break, execution, like the bottlenecks break, historically in the past it's like, "Okay, now you need to hire more engineers, you need to hire more designers," et cetera. And it's more just a lifecycle thing of, where is the lifecycle of your team and that specific pod to identify where the bottleneck is?

**Amol Avasare** (00:41:51):
But now when things break, you need to still look at it, of, "Okay, is it the actual ratio or is there also underlying technological shifts that are also causing this to break?" And so that's an interesting thing. I think that smaller companies, if I'm at a 15 or 20-person company, I'm the only PM there working with some designers and engineers, I think in the smaller companies, you'll see probably the biggest blend, where the PM will be doing all sorts of ... They'll be designing, shipping, et cetera, and I think you just have extreme bifurcation.

**Amol Avasare** (00:42:24):
You know, at larger organizations, more scaled organizations, I think the jury is still very much out. You speak to people even internally here, and different people and different teams will have different views of, "Okay, how much are these roles coming together versus how much are these roles going to be separate?" I think that it's not to say even the PMs, number of PMs are shipping, and themselves shipping and pushing PRs, et cetera.

**Amol Avasare** (00:42:51):
But if I look at, okay, across what I'm seeing, I think that it's clear that while PMs and designers are getting more leverage from AI, engineering is getting the most leverage right now. I look at tools like Claude Code, and the amount of leverage engineers are getting from them is higher than, I think the leverage that designers and PMs are getting from them today.

**Amol Avasare** (00:43:15):
Now, this is rapidly also changing, but that to me is my view today. And so if you think about, okay, a default team, which is, say five engineers, one designer, one PM. With Claude Code, that five engineers is two to 3xed. And the PMs and designers have also increased, but now they're managing what is effectively a much larger group of engineers.

**Amol Avasare** (00:43:42):
And so even though the headcount and the org structure hasn't changed, you're now just dealing with a situation of maybe 15 to 20 engineers in the old world, one and a half to two PMs, and maybe one and a half to two designers. And so we're seeing that that's putting a lot of strain on PM and design. And it's not everywhere.

**Amol Avasare** (00:44:04):
I look at teams like Claude Code and I think that, or because that product is so technical, it's probably just the right thing, where the PMs are all basically engineers themselves anyway. But we had a product, like a PM lead on site the other week, and we were all just talking about this where across the board we're feeling this, where PM and design is just squeezed. It's just absolutely squeezed.

**Amol Avasare** (00:44:26):
And we're like, "Is the right thing here, we just need to actually hire a ton more PMs?" And it could actually be where we land. On growth, how I think about it is, one, we are hiring a number of growth PMs. We desperately need people who are very, very good, and we are hiring. So if you are excited by what we're doing and you know growth, please feel free to apply. Would love to chat and-

**Lenny Rachitsky** (00:44:58):
Maybe craft an amazing cold email to you.

**Amol Avasare** (00:45:00):
Yeah, yeah, yeah. Feel free to craft that email. So that's one, is I think we are going to be hiring in a number of PMs. But then the second thing that we do is we very much hire product-minded engineers. I think this has always been the best thing to do in growth. You always want to have the engineers coming up with ideas, et cetera, especially people who can really step in as mini PMs if the PM is absent.

**Amol Avasare** (00:45:29):
And so we're basically more formally leveraging that right now because we are so stretched. So, the frame that we have is that if a project is two weeks of engineering time or less, then the engineer is on the hook to effectively be the PM for that. And so that means things like talking to security, talking to legal, talking to cross-functional stakeholders, and the engineer is very much driving that. The PM will get looped in and they'll advise if needed. And if something's wildly going off track, then they'll step in, but they're much more in an advisory capacity versus execution. If a project is more than two engineering weeks, then the default is that the PM should continue to be on the hook for making that go well. They'll still delegate more to eng, but they're squarely accountable.

**Amol Avasare** (00:46:19):
It's not fully clean-cut. It's like, use your head. If this is a one-week thing, but it's extremely controversial, the PM should probably still drive it. But that, I think is the approach that I expect more companies will start to do, which is just deputize the engineers to be mini PMs.

**Amol Avasare** (00:46:37):
Now, not everyone can do it. So the PMs, the engineers who are more product-minded, suddenly their value goes up significantly in order of magnitude. And then I think we will probably still be hiring a lot of PMs.

**Lenny Rachitsky** (00:46:52):
There is so much interesting stuff I want to follow up on here. Okay, so one is this idea of two weeks, just briefly. I always joke as a PM, you can go on vacation and be away for a couple of weeks from your team and things are going to be all right. There's a momentum, there's a plan, people keep operating, and it feels like that's kind of this rule of thumb you use of just, "Okay, if it's a two-week project, you'll be all right without a PM. You can handle it."

**Lenny Rachitsky** (00:47:16):
I love that those two connect. Okay. The other here is so interesting. So you're saying here that because engineers are so accelerated, and this all makes sense, PMs and design are kind of just like, "Holy." It feels like hard to keep up with this pace of engineering. And what you're saying is you need more and more PMs to keep up.

**Lenny Rachitsky** (00:47:33):
That's one route, or it's engineers that can PM essentially, which is so funny. It's just like, okay, great news for the product managers until more of the PMey stuff can be done by AI. But that's a really interesting trend. I don't know, is there anything else there just like, "Oh wow, we actually may need more PMs"? The ratio of more PMs, fewer engineers might be the future.

**Amol Avasare** (00:47:52):
Yeah. I think it just really depends on the industry, the size of company. Any company where you're building something that's much more developer-focused, you're going to rely on the engineers a lot more. Earlier companies, you don't have as much of this cross-functional coordination, stakeholder alignment nonsense that you need all these PMs for, so you can get by with less.

**Amol Avasare** (00:48:17):
But then as a company scales, and if I think about, okay, now you have this ratio where maybe the one PM became two PMs from productivity, that the five engineers became 20 engineers, the one designer maybe became three designers. If you think about what is the best use of time for that PM, I think this is a really interesting thing, of how much should PMs be actually shipping things themselves versus everything else?

**Amol Avasare** (00:48:46):
I think in the world where you're limited on engineering, the PM should definitely be shipping things. I think in today's world, it's a good way to get an understanding of the tools, which is really important. So the PM should be shipping for that reason. But if I'm one PM or two PMs and there's 20 engineers, I think about what is the incremental value I can add with my time? And is it actually shipping the 21st PM feature or is it saying, "How am I getting a little bit better at guiding the team on what the right opportunities are?"

**Amol Avasare** (00:49:21):
And so that's where I think in this world, you may have all these engineers who are like mini PMs, and the better that happens, that's where I would love to be doing more of. But still, if you then get a really good PM who can come in and can improve that, the why and the what particularly by 5%, that is such a high leverage higher.

**Lenny Rachitsky** (00:49:45):
This is such an interesting insight you're making. It's so counter to how a lot of people are thinking PM is evolving. What I'm hearing here is, because PMs are so behind, because engineers are just getting so much done, there's many people here, "Okay, you need to be prototyping, you need to be shipping PRs as a PM."

**Lenny Rachitsky** (00:50:01):
What you're saying, which I completely agree with, is your time is much better spent helping PM basically, and helping the engineers become better PMs themselves. And the leverage there is a lot higher than you spending time coding, shipping PRs in most cases.

**Amol Avasare** (00:50:17):
I think that's true in certain circumstances. I think that as a smaller company, I don't know that that's the case. In a smaller company where it's all hands on deck, I think you probably need to be shipping. I think if you're in a company where budgets are very tight, and engineers are very tight, and you're not able to just hire because money's unlimited, then you need to do what is needed to accelerate the impact your team's going to have. Right?

**Amol Avasare** (00:50:42):
So there's going to be a number of cases, where as a PM, the right thing to do is to be like, "Screw it. I'm shipping and I'm going it the whole way." But I'm talking here more about the larger companies, more scaled businesses.

**Amol Avasare** (00:50:58):
Yeah, if you have 20 engineers, is it the highest use leverage of your time to ship an extra feature, or figure out how do I up-level everything that we're doing, get the user insights better, et cetera?

**Lenny Rachitsky** (00:51:14):
Yeah. And I think there's also an element of shipping to learn, building a prototype so that you can have a better opinion. A lot of people talk about just, "I'm just going to try three things, see how it goes and that'll help inform the roadmap." This is now the PRD, is look at it instead of talking about it. So there's a lot of value there still.

**Amol Avasare** (00:51:29):
That's very true. I think that's a great point. So even for me now where we've got number of PMs, we've got many engineers, there are certain times when I'm like, "I want to articulate the idea I have in my head." It's just better for me to prototype it and show it. Right? So I think that is really important.

**Amol Avasare** (00:51:46):
And then we are very scrappy. So we're a big company by name, valuation, but we're extremely scrappy, and just the focus internally is just minimize bureaucracy and just go. And so probably 70%, maybe 60, 70, 80% of what we ship does not have a PRD. I'm averse to PRDs. I think I just hate documentation.

**Amol Avasare** (00:52:10):
I'm just like, "Go, go, go. Just cut the blockers." 20, 30% of stuff where it's like, it's important, it's really important to get right. The documentation should be really good and that people should spend a lot of time on it. But by and large, I think PRDs are just outdated at this point, and you can just kick things off with a good team without needing to do that sort of thing.

**Lenny Rachitsky** (00:52:34):
Say more about that. What do you do to help make sure, because people can build so fast, or spend a lot of time going in the wrong direction, ship things that are not what you're asking? How do you kick off a project and clarify, "Here's what we're doing"? Is it just a conversation or is there anything beyond that?

**Amol Avasare** (00:52:48):
It really depends on the size of it. And this kind of goes back to the two-week thing. So why we have that two-week thing, it's more like, how do I have some filter to say if we're investing heavily into something, we should apply more thinking behind it versus if it's a smaller set of investments, just go for it?

**Amol Avasare** (00:53:06):
And as a growth team, again, you do have a decent amount of these smaller things that you do. So for very small changes, like, "Oh, there's a thing coming. We need to have an upsell for it. What is it the thing we're doing?" This is just on Slack. This is just purely on Slack. It's just messages back and forth.

**Amol Avasare** (00:53:24):
And I think it also depends on having a good caliber of engineer in there, but engineers can understand, like, "Hey, I know you said this, but what about that for the audience?" And so we're lucky we have good product-minded engineers in that sense, but all these smaller things are very much just on Slack back and forth, and that's what you do.

**Amol Avasare** (00:53:45):
For the larger things, I think I very firmly believe in a proper kickoff. So we still do ... Just there's so much going on at this place. No one's got time, no one knows what's going on. And so doing a cross-functional kickoff, get legal, get safeguards, get everyone in the room and just be like, "This is what we plan to do. What do you care about? What do you care about? What do you care about?"

**Amol Avasare** (00:54:06):
That 30-minute meeting for larger things is just, I think, still so important to just streamline all the mess that may happen later if you don't do that work early on.

**Lenny Rachitsky** (00:54:17):
What's your approach to crafting that PRD in those cases? Is it ramble into Claude? Is it, do you have a template?

**Amol Avasare** (00:54:24):
Even in those cases, there are times I don't craft a PRD because everything's moving so quickly, right? So there's still some of those cases where I just set up the meeting and then five minutes before, I'll put it into Cowork, some of my thoughts, what credit. "Here are the things that I need to think about," spin up a basic doc and we use it to talk. Other times I won't even have a doc.

**Amol Avasare** (00:54:45):
But if I am creating a PRD, I have basically, a skill that they've created, and then there's projects with all the previous PRDs in there, and then it's pretty simple. It has the format down so I'll just say, "Here are the things I care about. Here's the why. Here's the problem," and flesh out the key considerations, flesh out the cross-functional stakeholders, those types of things.

**Amol Avasare** (00:55:12):
But again, my default is if I can avoid the doc and if we can just jump to action, then that's what we should do and increasingly just jump to prototyping the thing.

**Lenny Rachitsky** (00:55:24):
Yeah. And that's where I think it'll get so interesting once we can automate more of that, just like your assistant talking to the legal assistant, just ironing out all these little, what's important to you, what's important to the ...

**Amol Avasare** (00:55:35):
Yes, and it's coming. And I think the legal team has done good enablement around this. We work as versions of, how do you ... You can think about how can you mimic what someone might say and set up a Claude. Right? So there's things like that, that I think that we have now.

**Amol Avasare** (00:55:53):
And then as Claude gets more and more context and gets better at parsing long contexts, I think these are things that Claude will just get better at knowing. One of the things, Lenny, it's a slight tangent, but one of the, I think, most effective ways I use Claude, or one of the most interesting ways I use Claude, which I see a number of people doing internally is to help you identify misalignment.

**Amol Avasare** (00:56:17):
This is, I think something that I found really, really helpful. So with Cowork, you have the Slack MCP, and you can tell Cowork to say basically, "Look across Slack. You know the projects that I'm working on. These are the things that are top of mind. Go and find me areas of potential misalignment right now." And it does a really, really good job.

**Amol Avasare** (00:56:39):
So this is something that I've scheduled runs every week. Claude's looking at things and coming back to me and saying, "Hey, I think these things you should be aware of." And so you can think about in that shipping context, it's a similar thing where Claude can basically be looking at what's happening across the company and say, "You're thinking about shipping this thing. Here's who you need to talk to. Here's what you need to keep in mind."

**Lenny Rachitsky** (00:57:00):
That is so cool. I am so excited to tell you about this season's supporting sponsor, Vanta. Vanta helps over 15,000 companies, like Cursor, Ramp, Duolingo, Snowflake, and Atlassian earn and prove trust with their customers.

**Lenny Rachitsky** (00:57:16):
Teams are building and shipping products faster than ever, thanks to AI. But as a result, the amount of risk being introduced into your product and your business is higher than it's ever been. Every security leader that I talk to is feeling the increasing weight of protecting their organization, their business and not to mention, their customer data.

**Lenny Rachitsky** (00:57:35):
Because things are moving so fast, they are constantly reacting, having to guess at priorities and having to make do with outdated solutions. Vanta automates compliance and risk management with over 35 security and privacy frameworks, including SOC 2, ISO 27001, and HIPAA. This helps companies get compliant fast, and stay compliant. More than ever before, trust has the power to make or break your business. Learn more at vanta.com/lenny and ...

**Lenny Rachitsky** (00:58:00):
... your business. Learn more at vanta.com/lenny. And as a listener of this podcast, you get $1,000 off Vanta. That's vanta.com/lenny.

**Lenny Rachitsky** (00:58:10):
I feel like there's this like, what are the jobs of a product manager, and then how are they slowly going to be supported/done by AI? So there's this misalignment, just like fine misalignment, and then maybe one day, it'll be like, aligned people initially. You talked about this cash automation for growing, like, how do I grow this product? That's starting to happen. Another that I use myself when I'm building stuff is just asking, "How do I make this product better? How do I make this a better user experience?" And asking the AI to just give me a bunch of ideas, and they're actually really good.

**Lenny Rachitsky** (00:58:41):
So it's interesting how these little pieces are starting to be put into place to do more and more of this role. I'm curious what other automations you have and your team have that are effective. What I love about these conversations is you're basically living in the future. You're working on the most bleeding edge company with the most talented people, with the most cutting edge tools. And you can see where things are going and start to actually live in the future, build things that nobody else has even thought about or can do. I'm curious just what else is working, what else your team has done to help save you time, be more productive?

**Amol Avasare** (00:59:17):
We use it pretty extensively across the board, right? So there's this standard PM stuff like writing docs, brainstorming, looking at data. For data, I personally have like, Coworker runs on a schedule and looks at 20, 25 different charts every morning. And then so when I come in the morning, there's just so many charts, so many products to track. Cowork will tell me, "Okay, here are the things that you should pay attention to. Here's what is concerning, and here are just some interesting insights."

**Lenny Rachitsky** (00:59:45):
And it sends you an update in Slack, or what's the workflow?

**Amol Avasare** (00:59:49):
For me, it just shows, it comes up in Cowork. So Cowork has a schedule-

**Lenny Rachitsky** (00:59:52):
In the desktop app?

**Amol Avasare** (00:59:53):
Yeah. In the desktop app, you can have a scheduled task that you create. And so I have a bunch of Hex links that it will go and look at. It uses the Chrome extension for some things and it uses MCP for other things, and then it'll just give me a summary, and then I know... I saw this one, a few charts that I just like to look at because I was just like, "I'm a numbers guy. I just like charts."

**Lenny Rachitsky** (01:00:18):
They all open to the right too. So that one was, yeah, nice.

**Amol Avasare** (01:00:20):
Yeah. I like to see the chart. But then there's the long tail of things, and even the medium tail where it's like, you don't have time to look at it every day, that if Claude is proactively looking at it and you start to feel good over time of, okay, it's like the false positive rate is going down, the false negative rate is going down of the things that Claude brings to you, then you just get a little bit more confidence and peace of mind there.

**Lenny Rachitsky** (01:00:46):
This touches on an idea I've always had that Teams will have is a strategy bot, which just imagine an agent that's just constantly watching metrics, the market, the roadmap, what's working, what's not. And just like, Tamil, "Here's what I think we should do now. Here's the pivot we should take. Here's where we're going to win." It feels like we're very close to that.

**Amol Avasare** (01:01:08):
I think we're close. I think we'll get there later this year, to the point where that's very, very effective. That's my gut. I think that level of proactivity and looking across a bunch of context and distilling insights, I think is... The thing I mentioned earlier, learning about the alignment piece, that's like a version of it, right? Now you're just looking at across more data sources. This is something that I use. So I talked about some of the standard PM stuff, brainstorming, data, UXR. There's a lot of like, admin stuff. I just hate life admin and paperwork. I just hate it. And so I get Claude to book my meeting rooms. I got to book meeting rooms. Claude archives sort of my email first pass at clearing out my inbox. I don't do any of my reimbursements and expenses. Claude will go to Benepass and file the reimbursements. It'll go to Brex and file the expenses.

**Amol Avasare** (01:02:02):
So all of that side of things, I'm just like, just hand it to Cowork, just get rid of it. And then the stuff that's quite interesting, I think is the manager lens, where I talked about alignment is one thing. So I look also across my direct reports. Claude can look into what have they done this week. You look at our team goals and OKRs, look at the transcripts from our discussions and understand. It can basically ask for like, what are the key takeaways and observations I should keep in mind and what feedback do you think I should give them? And that's something that is like, again, you can just set that up weekly. The quality is hit or miss right now. It's decent on something. Sometimes you're like, "Holy shit, I am so glad that I caught this." And that's very, very helpful. And then I do that for myself as well. My manager, Ami Vora, was I think, a podcast guest of yours, right?

**Lenny Rachitsky** (01:03:00):
Yeah, yeah.

**Amol Avasare** (01:03:01):
So I say, "Hey, based on what you know of Ami both publicly, she's written extensively about product, and then internally, and then our discussions, based on everything that I've done or not done this week, what feedback do you have for me as Ami?" And I get that every week, right? So a lot of these things can already be done today. I think that as the models improve, I think it's just the accuracy and the signal of these things is going to continue to improve rapidly.

**Lenny Rachitsky** (01:03:31):
I don't think you realize just how much awesomeness you're sharing here. Everyone of these is like, "What?" Okay. So this Ami example, you have one on ones with her. Do you ask Claude Cowork to go through all of her writing, basically build like a model of her and you ask, "What should I be doing differently based on what you know about Ami"? Is that different?

**Amol Avasare** (01:03:58):
Yeah. Effectively, there's a number of ways you can do this. I think if someone has a public profile where they've written extensively, it's helpful because Claude can just get all that information. Otherwise, you can have a project or you can have a skill, but increasingly, Claude is better at just understanding. Because you can tell Claude like, "Look on Cowork." You can say, using the Slack MCP, "Look at everything that this person has said in the last week, et cetera." And based on that, what are their top priorities? What are priorities my manager has based on how they're spending their time that I don't know? And so all of this layer of stuff, which is like, I think about it as soft coaching, I think that that is unlocked, in my opinion already. I think it's just that you're working with a coach who is kind of like drunk at times. Not drunk, but sometimes says something, you're like, "Why would you bring that up? That's clearly wrong." But other times, you're like, "Wow."

**Amol Avasare** (01:04:57):
There's like, one of the guys, Scott, who leads our enterprise team. There was a few cases where he found major areas of misalignment that would've caused teams to spin their wheels significantly or do overlapping work. And you think about the impact of that. Your shipping in this world as bigger companies is going to be constrained often by all the cross-functional coordination, right? And I think we're now starting to see at this cross-functional coordination layer, some of that work AI is really being able to be used to reduce that foil. And I think that six months ago, that wasn't possible. And I'm like, "Shit, six months from now, what is going to be possible there?"

**Lenny Rachitsky** (01:05:45):
Oh, man. And I think the fact that all this data is there, Slack, there's Granola, or whatever people use, all these notes from conversations and discussions are really key to this working.

**Amol Avasare** (01:05:55):
Yes.

**Lenny Rachitsky** (01:05:56):
So for someone that wants to do something like this, how do you set this up? What's the steps?

**Amol Avasare** (01:06:01):
Yeah. You go on to Cowork, download the desktop app on Cowork, connect the Slack MCP. That's where you need to, depending on how big the organization is, you may need to get sort of team or enterprise admin permissions, someone with those permissions to enable that. But once you have the Slack MCP connected and on [inaudible 01:06:25], you just ask Claude. That's it.

**Lenny Rachitsky** (01:06:27):
Amazing. Okay. I'm going to go into a different direction. I want to talk about the focus that Anthropic has had over the years. So if you look at the numbers that you're all putting up, what's really incredible about it is the focus that you all have had. And I think this is the reason it has worked out so well. There's a certain competitor in the market that is realizing they should have done this and are starting to shift to a similar approach. As an external observer, it feels like Anthropic has been very good at doing very few things, but going super deep. So B2B, for example, just going deep on B2B, and then going really deep on coding use cases, Claude Code being an example. And it has worked out really well. Who's been driving that focus? Who has helped keep that focus from the beginning?

**Amol Avasare** (01:07:16):
Yeah. I think it's a foundational part of the company. I think it's been there from the very, very early days. And it really comes from leadership and I think they've just done a phenomenal job of distilling that. I saw this doc come up recently. I don't know where it was shared. It was something that Ben Mann, as one of our founders that you had on the podcast, had written. It's dated in 2021, I think a few months after they started the company. And it was like, "Here's why we should just focus on AI coding." And this was like, five years ago. This was long before anyone knew what the actual market opportunities were around this. And I think this is just like a deep focus that we have had internally from the start on the importance of coding and B2B.

**Amol Avasare** (01:08:10):
I think there's two lenses to it. It's like maybe a view of, "Okay, that this is going to be commercially beneficial to tackle, and then also, the side of it around accelerating research." So I'd say it's a pretty mainstream view now. I've now heard people from various labs talking about this, the importance of coding to accelerate research. But that has just been a very firm view that we have been laser focused on internally of, "Okay, if you have the best models, that's going to accelerate your researches and that's going to accelerate the research loop." And I think that's something that Dario has seen very clearly for a number of years. So I would say that that's probably one of a lot. I think a lot comes from Dario. I think a lot comes from leadership and just our DNA.

**Amol Avasare** (01:08:55):
I think the second though is probably just necessity, where it's now changed. We're a more well-known company, raised lots of money, blah, blah, blah. But historically, we're very much the smallest, least well-funded player in this space. In many ways, it's a complete miracle that I think, we've gotten to the stage that we have. We didn't have the free cash flow or the distribution of a Meta or Google. We didn't have the first mover advantage of an OpenAI. And so what do you do? I think there's this broader principle I have just around life of like, the freedom through constraints, that when you have a bunch of constraints applied on you, whether that's in personal life or at work, I think that it can bring a lot of freedom because it just frees up all this excess choice. So you're like, "Okay, this is clearly the path."

**Amol Avasare** (01:09:47):
And I think for us, it's like, "Okay, you don't have a ton of funding, you're a small player, you don't have distribution." You just have to really pick a very narrow focus, and even for a very generalizable technology, to maximize your chances of getting to escape velocity. And I think that that's also just related to how history played out, right? So it was well before my time, but Anthropic had a version of Claude. We had a chatbot before ChatGPT was launched. And we had ultimately chosen not to launch it for safety reasons. I think the team didn't want to kick off effectively like an AI global arms race. And ChatGPT launched and they got insane traction and that just naturally sort of pulled them towards consumer. There's another world where if Anthropic had launched Claude first, maybe did the other way around even with all that focused stuff. So who knows? It's always hard to say, looking back at some of these things.

**Lenny Rachitsky** (01:10:42):
Wow, I didn't know that. I think also, people just don't realize how far behind Anthropic was. Right now, it's like, of course, they're amazing. But like, I just remember when people were talking about Anthropic, we were raising money. I was like, "There's no way they're going to compete with OpenAI at this point. It's so over." Just like, "They're so far ahead." And it shows the power of focus and just, I guess, I don't know, all the things you all did. It is absurd how far you all have come and how successful and how things have changed so quickly.

**Amol Avasare** (01:11:14):
Yeah. And I would say, I very much agree. I think a lot of that comes down to our leadership team. We have a number of people who've worked at, call it the best companies you know in the world, very senior people. And I think almost uniformly, everyone was like, "This is the strongest leadership team out of any of those companies." And so I think a lot comes from them, and then we're just very lucky to have incredible people. I think that helps a lot as well.

**Lenny Rachitsky** (01:11:41):
On the coding piece, just to make sure that part is clear, I never thought about this, that the reason that the bet was so deep on coding is not just that's a huge TAM, but it's that this is a feedback loop that will accelerate us further and further. So if we get the best at coding, coding will help us do research, it'll help us build better models and it'll accelerate faster and faster.

**Amol Avasare** (01:12:02):
Yeah, that's correct. And this is something I checked. Dario has talked about this publicly, so I'm fine to [inaudible 01:12:07].

**Lenny Rachitsky** (01:12:08):
Okay, it makes sense. The safety piece is really interesting. So I want to spend a little time here. So famously, Anthropic, I think the official name of Anthropic is Anthropic, an AI safety research company. As a growth person, there's this balance I imagine you strike between growing and the mission being, don't grow at all costs. Our goal is AI safety and alignment. How do you balance those two things? How does that impact your job?

**Amol Avasare** (01:12:37):
Look, I think it's something we take very, very seriously, and it is the whole reason the company exists. And if you think about, it's all the way from... It's why they left to start the company. It's deep in our corporate structure itself. So historically, everyone raising money is like, "Go create a Delaware C Corp." And that's the structure you do. And with a corporation, you have a fiduciary duty to maximize returns for shareholders, maximize shareholder value. And from the beginning, they went a different way. We then created a public benefit corporation, PBC, which allows you to legally say that maximizing shareholder value is not the overarching umbrella goal of this company and you can optimize for public benefits. So really, I think it starts from there and it ladders down from there. For us, our purpose, our mission ultimately, is just to make sure that the transition to powerful AI goes well and is net beneficial for humanity.

**Amol Avasare** (01:13:46):
I think internally, we are very excited and I think, honestly, we're very, very optimistic about where this can go, but we also understand what the risks are. And so for us, that top line objective of, " This needs to go well for humanity. This just needs to go well for humanity," that is something that we are happy to take a significant commercial hit for. And we've done that time and time again, right? So we have it like back then, okay, you had Claude, but you don't want to release it because you're like, there's these safety risks. And so there's time and time again that I've seen, we've been happy to take that hit and it's actually worked out well for us in other ways.

**Amol Avasare** (01:14:26):
From like a growth lens, I look at it as like, growth teams can often push the boundaries of what is good user X, UX, et cetera, because they're trying to very, very much eke out metrics at times. When I think about if a controversial test is brought to me, I sort of look at it as like, there's two types of tests that are controversial. One is when that test is so controversial that you just should not run the thing, because the results don't matter because you would not ship it for a combination of brand and sort of customer friendliness and values. And then the second is where it's like, it's controversial. I don't like it. I certainly don't love it, but it's not like a red line.

**Amol Avasare** (01:15:15):
And so you're like, if someone comes to you with conviction and is like, "I have a really good hypothesis around this," and you're like, "I don't love it, but you can run the test and see what impact it has." And if it's a high level of cringe or ick, then I want to see a high level of return for the result for that. I kind of think about everything and like, is it in one or is it in two? And for every company, that one and two is different.

**Amol Avasare** (01:15:42):
I think for us, AI safety is very much in one. I think that it's like, "Yeah, that's why we exist. Yeah, it's fine. We're just not going to do this thing." I think then, there's other things that fall into two, where you're like, heightened sensitivity, but we can try it and see what happens. I think zooming out though, Lenny, one of the biggest mistakes I feel like I see growth teams make, and particularly just hardcore growth practitioners, is just trying to squeeze every last dollar. I think this is like a general principle also in life. If you're a founder raising money, you're just trying to squeeze that last dollar. You don't want to do that because you want people to come back next time as well, is my view.

**Amol Avasare** (01:16:23):
And I think in growth, I think it's really important that you just need to be okay leaving money on the table. And that's a core principle for us as a growth team, where we are very comfortable for going metric impact in order to prioritize safety, in order to protect our brand, in order to hold a high quality bar and to maintain a great user experience. And if you look beyond the short term and like, "Okay, what are the numbers for this quarter?" And you zoom out and you think about what are the very best products out there, you realize this is how they all operate. And that's actually the thing that's going to drive more growth long-term as well. And so I think that actually ties back to safety, where as the risks get higher and the stakes get higher, I think the fact that we are taking a stance and safety is critical to what we do, is actually going to become a significant, it's going to be a significant competitive advantage for us that I think is going to help us in the long run.

**Lenny Rachitsky** (01:17:19):
Yeah. And as you share all this, clearly it's working. Anthropic is killing it. So I love when someone doing something, someone approaching the problem that way, it actually works out. It's the same way I think about with my newsletter. There's so much more I can do to grow it. My philosophy is just focus on creating good content, nothing else. All these micro optimizations are not going to matter in the end. It'll grow through people sharing it if it's useful to them. And a very small scale, I have similar philosophy.

**Lenny Rachitsky** (01:17:51):
One of the things that people are probably thinking about as we talk, we joke about AI replacing parts of jobs here and there. It is pretty scary to a lot of people, just like, "What is the future of my job? Will I have a job? How do I stay relevant in this future?" So there's a couple of questions here. One is just like, for folks that want to thrive in this approaching AI future, as a PM, as a growth person, do you have any advice, things that they should be doing right now?

**Amol Avasare** (01:18:19):
To me, a couple of things come up. One thing that everyone says, is use the tools, you need to be on top of the tools. I think you need to be using Claude Code, you need to be using Cowork and understanding just each model release. What is the new things you can do with this? How can you apply this to your job? It'll work well in some things, it'll work terribly in other things. And then the model launched later, it's like, "Oh shit, that other thing worked." But if you didn't go back to try it, you would not have known. And now, many months have passed and you didn't know that that was possible. And so I think that being on top of the tools is really important, both for improving your own productivity, but also for getting product sense around AI products, which I think is just going to become increasingly important.

**Amol Avasare** (01:19:02):
I think then, zooming out beyond that, I look at it as like, just leaning into where you'll have a competitive advantage and an unfair advantage. And so to me, there are some people, some PMs who are really good at like, craft, for example. And there's others who you'll throw them into a situation with all these stakeholders who have all these strong opinions and there's no way they're going to mediate this. And they come out and it's like, everyone's swimming in the right direction. And so if you think about like, what is the major skillset that you have where you spike that can be tied to delivering, driving impact for a company in a product role, I would just double down on that and almost forget the weaknesses. Just what can you do to become the best person at that thing, because that's very, very valuable.

**Amol Avasare** (01:19:49):
And I think that ties to the notion of just leaning into being interdisciplinary. So going back to some of what we mentioned earlier on where it's like, "Okay, in this world of engineers are mini PMs, that the engineer who is highly product-minded is a unicorn, is an absolute unicorn." I think the same thing is true for PMs, where it's like, "Okay, now, in this ratio, if the designer's really stretched and you're a PM who can design, you are also a unicorn now." The chances of a company letting you go has gone down dramatically because you are now just so much more useful. And so I think that is just really, really important. I think if I look at what's benefited me, it's probably a version of this. I think that for me, I came from a founder background. So the mix of the founder background, the finance. I was an investment banker, so the finance background and numbers. And then sales, I almost became an account exec, instead of going into product. I was right on the edge of, "Should I go into sales or product?"

**Amol Avasare** (01:20:53):
And I think a combination of those, along with growth is probably what's led to like, there are certain areas and situations where I can just have outsized impact to other people. And so, understanding what that is for you is really important. I look at our financial services product. We've launched Claude for Sheets, Claude for Excel-

**Lenny Rachitsky** (01:21:15):
They kind of like, tanked the market, by the way. Everyone went crazy.

**Amol Avasare** (01:21:18):
I know. But the guy running that, Nick Lin, he came from investment banking, he came from private equity, and he just has such a competitive advantage where he is building that product and he's like, "I know this, I know this." He's built for this. And so I think just understanding what are those interdisciplinary areas you can lean into, to make yourself more just higher impact is really important. And then the last one is just being adaptable. Anyone who is trying to just keep applying old playbooks, I think you're going to make life a lot harder for yourself. So one of the biggest things you come into Anthropic, is you need to understand that probably 50, 60, 70% of how you operate in the past, just throw it out the door. It's not going to be relevant. And if you try to stick to that, you're going to have a lot of friction and it's not going to be helpful. So just being adaptable and understanding, "Okay, the job's changed this way, I'm going to go that way," is I think like, it's so, so important.

**Lenny Rachitsky** (01:22:17):
That is awesome advice. It matches a lot of what Jenny shared when she came on the podcast, the design leader on Claude and Cowork and all these things, of just the idea of going deep, becoming the best or one of the best at a very specific thing, and that not every company will need and you don't need all 10, but just going deep on something. I forget how she described it. Marc Andreessen said the same thing. I think we called it a sideways E, instead of just T-shaped of one thing. If you could have a couple of things you're really, really good at, there's a lot of power to that.

**Lenny Rachitsky** (01:22:51):
Oh, man. Okay. Before I get into something that I think will blow a lot of people's minds about how we actually met and kind of a big part of your journey, let me just ask you this. Is there anything else about Anthropic that might be worth sharing, might be worth talking about?

**Amol Avasare** (01:23:09):
The thing that maybe comes to mind is just our culture and the people that we have here. I really think it's our secret sauce. I think it's the thing that is the most defensible, the thing that no one else is going to be able to replicate. And I don't think it's an accident. Leadership has really invested in this a lot. And Daniela and Dario, they really believe in this a lot, and I think they've just created a very special culture. So I would say that this is truly a mission-driven company and I was not 100% sure of that when I joined. I was like, I think that this is an exciting company. I very much agree with their principles, but I didn't know anyone at the company. I didn't have any references on what it was like inside. So I was a little skeptical when I joined. I'm like, "At least they're talking about it, but I don't know. Are they serious about this?" And then I came in very early on, and I was like, "Oh, oh shit. Okay. Maybe they're even more serious about this internally. They talk externally."

**Amol Avasare** (01:24:14):
And so it's a mission-driven company where people viscerally, viscerally understand both the upsides and the downsides of the technology, and therefore, understand the divergent ranges of how this may go for humanity and how different of a future that could be. And I think when you understand that, of how different this could be as a future for all of us and our children and our grandchildren, et cetera, I think it leads to a lot of passion for what we do and it just leads to a lot of belief in what we're doing. And so I look at every other job I've had in the past, and there's some degree of people at the company who are just checked out, where it's like, "I'm here, I'm sick of this, but I don't have a better option or I'm getting paid too much to leave, et cetera." That is just not the case here. I have not met a single person. I'm saying a single person, who has checked out. Everyone is putting everything they have on the table. Everyone is pouring it out and leaving nothing behind and is just fully, fully in it.

**Amol Avasare** (01:25:22):
And so I think that leads to like, releases energy that is just very, very hard to describe. I think you have that energy, you have that mission-driven nature, and then it's such an open culture. So leadership is very, very transparent with us on things. Slack, it's a whole maze. There's so many things that play out on Slack. We're very open. Everyone has these notebook channels where you have your own Twitter feed in a way, where you're just talking about your thoughts about things. And so you can go and join the Slack channel, the notebook channels of people on research and all these other areas, and you can learn whatever you want and you can spend so much time getting lost in that as well.

**Amol Avasare** (01:26:05):
But that openness where we even encouraged people can just argue with Dario. There was an all hands. You said something where someone didn't agree, and the person goes onto Dario's notebook channel and just says, "Hey, I didn't appreciate how you said this and this and that." And then it sparked a whole big debate. But that sort of thing where it's encouraged like, "Go to leadership and disagree with them, challenge them publicly," I think that just leads to a level of trust. And all of that together, I think it just means that we have this very, very deep sense of togetherness that, man, I've never experienced anything like it.

**Amol Avasare** (01:26:44):
And then you get to the talent, right? I think that is the thing where the talent density is like, I feel like I'm playing for Real Madrid at times. I look around, I'm like, "Man, I'm playing for Madrid," where it's like, you just have the best people in the world. I think it's most the case on research. We have the very, very best...

**Amol Avasare** (01:27:00):
... the case on research. We have the very, very best researchers in the world. But even you look on product, we have Ami Vora, she is phenomenal. We have Mike Krieger. You're like, okay, casually started Instagram. He's here. On growth, we have John Egan, who's my engineering counterpart, who's the OG in growth engineering. He's great. We have Alexey, he's a guy who teaches growth engineering at Reforge. He's just another dude on the team. And all of that I think is just very special. I think my favorite here is in the [inaudible 01:27:33] a couple of months ago we had our onsite, company-wide onsite in October, and I'm walking around, I see this guy, he's just walking around eating popcorn by himself. I go up to him and I'm like, "You're Jeff, right?" And he's like, "I am." And I'm like, "You are literally the US ambassador to my country, Australia, and you are just an employee here." I'm talking to our prime ministers of our country and all these things.

**Amol Avasare** (01:27:57):
And it's just the talent combined with that culture, I think, is just this secret sauce that is the reason that I think we are as successful as we are.

**Lenny Rachitsky** (01:28:08):
This notebook channel is so interesting just as a tactical thing. So the idea there is Dario just shares... It's a little internal Twitter feed where folks just share what they're thinking about and what their priorities are and things like that.

**Amol Avasare** (01:28:22):
Yeah, that's basically where it's an internal feed where... It's not just Dario, everyone has one. And basically you share your internal thoughts. It's a way to keep people updated on things on what's working. It's a way where people share provocative things. I think from a leadership level, and we also think about that as it's a way to scale your beliefs and views across an org as it grows quickly, right? So if you're now adding a lot of people in the organization, you need to think about, "Okay, what are the behaviors that we want to model? What are the principles that are top of mind to us?" And if you think about, yeah, you can have a bunch of these meetings where you talk about it, you can model that behavior. But if you have a channel which is like, "Here's my top of mind," and you say these things, right, if I have a post, which I did the other week of this is the importance of being comfortable leaving money on the table.

**Amol Avasare** (01:29:14):
Now all the new engineers on growth who've joined have seen that and they're like, "Oh, okay, this is different to what we've known before." Right. So I think it's good for the openness, but it's also good as a leader of how you can scale your views as an organization to get people more up to speed on the way that things are done, which is I think really important to avoid that drift, which when you have so many new people signing up, that drift can lead to a lot of drift in strategy and sort of perception. So it just helps run a tighter ship in that way.

**Lenny Rachitsky** (01:29:46):
And more importantly, it's data for the agents everyone's got running to help them work with all these humans.

**Amol Avasare** (01:29:52):
Yes, that is very, very correct. It is something that goes to Claude. There are certain documents in onboarding where it's like the HR team has written before editing anything on this document, please check with this person because this is a document that Claude references as a key thing, right? And so more and more these types of things of, okay, how does the growth team think about this? How does safeguards think about this? You're arming Claude with that context to get better and better at helping in the future.

**Lenny Rachitsky** (01:30:20):
That's interesting. It feels like that's something that every company's going to have to start doing is just sharing their thoughts in a structured way so that all these agents that we've all got running have what they need to know. Another interesting side note here is just Slack. Okay. So there's all this talk of SaaS tools being replaced by AI and you guys use Slack. I think there was this famous tweet of you guys still use Workday and all these tools, all these SaaS tools. They're all going to be vibe coded out of existence. The fact that you all, at the cutting edge of what could be built with code, still use Slack and all these other tools, to me, that's a good sign that maybe SaaS companies will be outright in the future. I don't know if you have anything there to share.

**Amol Avasare** (01:30:58):
Yeah, I think it's a really complicated picture. There's a number of things that we just build internally ourselves. As time goes on, the ability for Claude to do that better increases. And at the same time, we use Figma a ton, we use Slack a ton, we use Workday, we use a lot of these products, and I don't see that changing in the immediate future. And so yeah, I think there's probably some truth to some of this. I think the other parts are like it's overblown. And many of these products, they're customers of ours. We value them a lot as customers and we use their products very, very heavily, and I don't see that changing in there.

**Lenny Rachitsky** (01:31:37):
And you have better things to do. Who's going to spend time building Slack at a... That is not where value is going to accrue. And I think it also helps you see how sophisticated these things are. There's been teams thinking about these problems for a long time. Anyway, that's a whole other tangent. Just coming back to the values thing, I just want to highlight something here that's really important. A lot of people criticize Anthropic for talking about the dangers to humanity, throwing out all these numbers about jobs going away, just creating all this fear.

**Lenny Rachitsky** (01:32:11):
And people think it's, "Oh, we're trying to raise money or we got to get people's attention or we're just trying to create headlines." But everything I've ever seen internally is always just this is what we believe in. We want people to know what it might be coming. Even if it isn't bad, we want people to understand, "Here's what might happen and we are trying to avoid it." And you might say, "Why is Anthropic even building AI if it's so dangerous?" And the understanding Ben shared is just like we think it's better that we go at this and try to build it the right way versus just stay out of it and just hope that nothing bad happens.

**Amol Avasare** (01:32:48):
Yeah. I think three things that come to mind there. First is I go back to something I said earlier, which is that we very much think about things from an exponential lens. And if you are thinking about things from a linear lens, you'll see the world very, very differently, right, because you look at where we are today and you're like, "Okay, but how much better can it be in two, three years?" I think if you're looking at it from an exponential lens and you understand how exponentials work, then you just realize that a lot of this stuff is actually going to be happening sooner than people think if you're looking at it from a linear lens. And then if you understand that there could be upsides and downsides and the range of outcomes here, I think we very much need to be talking about the downsides so we can avoid them and push towards the upsides.

**Amol Avasare** (01:33:36):
I think most people at the company are optimists. We're very optimistic about the future. I think it's just we understand the risk is like it is not a guaranteed that we end up in a good place. And not enough people are talking about the risks, I think, in productive ways and who have the know-how of the risks. I think there's people who may talk about the risks but are not in the game. And so they don't actually know fully. They're not surgical on what the specific risks are, but we're in the game, we understand what's happening. And so that's one piece. I think the second is, I think, we actually believe in this stuff more strongly than we say externally. So it is just such a key part of how we think internally that sometimes we just reword your statements because it's like people might just think we're being too over the top, but internally, that's how we think, and what we're putting out is a softer version of that at times.

**Amol Avasare** (01:34:28):
And then I think the third piece is going to what Ben said where we think a lot about driving the race to the top. And so it's like if you're not in the game and you're shouting from the sidelines, no one cares. It's just the reality of how the world works. No one really cares. If you're in the game and you're a leading player and what you're doing is working, you can influence people who are also in the game to take the right actions. And so that is the core of it. If we just pack up and go home, you have no influence on this thing. And if you stay in the game and you're like, commercially, you're doing great, and then you have ways to influence that, okay, these are the principles and put that into the conversation and make more people sort of believe in those things.

**Lenny Rachitsky** (01:35:12):
I could talk to you forever, Amol, but two more questions just to round out the conversation and touch on some stuff that I've hinted at a number of times. One is I want to take us actually to failure corner because someone listening to this may be like, "All right, look at this guy just worked at all these amazing companies, cold email, the CPO at Anthropic, got a job, joined this rocket ship. It's all been up and to the right, just killing it constantly." What's a story from your career where things didn't work out when you failed and what did you learn from that experience?

**Amol Avasare** (01:35:45):
I have a couple. I think it's very much not that way. I feel like it was a lot of squiggly lines to get here. The biggest I'd say is just founding a company, raising a bunch of money, having employees, and then having to shut it down and tell your investors that you've lost the money and that you had a vision of what you're going to do and that it's not going to happen. And so that I think is probably the biggest one. We spent three years on it. It was not like a, "Oh, we tried something part-time." It was like, "No, we went for it." We had spent three years, raised a couple of mil. We had maybe seven, 10 employees at our biggest. And it was something that we really believed in. It was around mental health and how you can quantify mental health to help understand or get early predictors of things like generalized anxiety, major depression. So it's stuff that we really, really believed in.

**Amol Avasare** (01:36:39):
But ultimately, in our early 20s, we had no idea what we're doing at the time and many things I do differently, but that was just a very, very, very painful process. I think the good thing was we kept our investors in the loop the whole time, so 20 founders who are struggling out there. Send those monthly investor updates. It's really easy to send those when things are great. It's really hard to send those when things are bad. You just bat it down. You sit down and send an update to your investors about why everything you talked about last month did not go to plan, but it's just the right thing to do, and it keeps people in the loop, and it avoids surprises. But it's still so tough when you're then calling up the investors to be like, "Hey, we're shutting down or making that decision," everyone who believed in you and it becomes such a big part of the identity. It's very, very tough.

**Amol Avasare** (01:37:29):
So man, that was just brutal. It's brutal. And it took me, I think, a number of years to truly get over. I think that it's a tough thing, but you get so much from that experience that it's hard to see in the moment. And I think without doing that, I would not have gone into this. I was not a PM before. I didn't have any of these skills. I'd never worked on products. I didn't know how to cold email really. And so it was through that job that I learned a ton of the skills that made this career path viable for me. And it's just really hard to see that in the moment when you're looking at a point in time. It's much easier to draw the line looking back.

**Amol Avasare** (01:38:07):
But I think that'd be my takeaway is just keep in mind that it's a long game and some of those things... I'm so grateful for that experience now. I'm so grateful that it failed and went that way, actually. It's very painful because it wouldn't have led to what I'm doing now. And so it's a tough thing, but the positives can come from it.

**Lenny Rachitsky** (01:38:25):
What I love about this is a lot of people have these times in their career where they're like, "It's all over. I failed in such a big way and my reputation's screwed and people were counting on me and now they see I'm an imposter. I never knew what I was doing. And after all, now they finally see." And just seeing that, and this was three years, I'm looking at your LinkedIn, you had seven employees, something like that, and then it's like masterclass, Mercury, Anthropic. I think it's inspiring to hear a story like that to know that you can have a big failure like that and things can work out. That is not the end. Okay. So at 2023, I was going to go on pat leave because my wife's pregnant and I was just like, "Wait, what do I do with the newsletter? I need to take some time off. That would be really nice to take a month or two off."

**Lenny Rachitsky** (01:39:13):
And so my plan was, "Okay, I'm going to do a bunch of guest posts where people line up." I put out a call for guest posts, people apply, I pick a few and then I kind of slot them in ahead of time so I could take time off. So I put out this call, "Hey, who wants to write a guest post for my newsletter?" I got 500 plus applications. One of those applications was from you and the pitch was essentially how a traumatic brain injury made me a better product manager. And I still remember reading the first draft you sent me and I was just like, "Holy shit, this story is incredible." It's just like you feel such feelings and it was just so tactically interesting and useful like, "Oh wow, this is actually going to make me a better product manager." Share the story of the brain injury that you went through and just the journey that you went on there because this is going to blow people's minds.

**Amol Avasare** (01:40:04):
It was the toughest time in my life. It made shutting down a company being like, "Oh, that was nothing actually." Just funny how perspective works that way. Back in early 2022, I had a traumatic brain injury. So I'd done MMA for many years. I'd done Muay Thai, which is a type of martial arts for many years, never had a problem. And it's just one of the things that happens, the wrong session. It's just a normal day of sparring, nothing crazy. You get the wrong hit to the head in the wrong way, and my whole life changed. And basically I spent nine months. I was off work for nine months. The first couple of months were brutal. It took me roughly half a year till I was comfortable walking again. It was very, very difficult. The first two, three months beyond just showering and going to the bathroom, my wife did everything for me, including texting my friends.

**Amol Avasare** (01:40:59):
I would listen to music for maybe 20 seconds and feel like I needed to vomit. I couldn't look at screens at all. And it was a very, very long recovery. It was not clear to me that I would ever work again for a while actually. And it was like we'd even discussed my wife, what would we do in that case, et cetera. And we had to think even on those levels. And through a lot of pushing and really working through myself, and you have to just slowly increase your tolerance to things. It's a brutal process, but you need to slowly expose yourself to different things and just get better and better at each little thing, actively work on that, don't push it too far, otherwise you have a big setback. It basically got to the point then where over nine months and then that it returned to work and then it slowly got better. And the part, Lenny, you don't know is in mid-2023, we posted that newsletter and a month later I got re-injured actually.

**Lenny Rachitsky** (01:41:59):
Oh, wow.

**Amol Avasare** (01:42:00):
And when you have a brain injury, until you're 100% healed, your risk of another concussion or a brain injury is elevated. When you're 100% healed, your risk falls down to that of a non-concussed population. But until that time, and even if you're like 95% healed, you're not 100% healed. And it was just an innocuous sort of in everyday life getting off a plane, a bag sort of hit me on the head type thing. And I was off work for two months when I... One month into joining Mercury, one month in, I'm like, "Sorry guys, I need to peace out for three months." And then it was a very, very long recovery from that. And I'm actually still not 100% healed. So I'm mostly good, but I have times when I have dizziness and headaches and other things that I need to work around. Overall, I feel like it's one of the best things that could have happened to me, and I think that keeping that mindset helps.

**Amol Avasare** (01:42:51):
And there's a point when you can take that too far when that view is detached from reality, but I think it's just made me so much better and more effective as a person. A lot of the same habits, I don't drink alcohol, I don't drink caffeine, I have to do a bunch of these things for my physical health. I just have to do them. So I keep doing them. I take breaks. This is a really big one. You might think even in a place like Anthropic, how do you survive in this way? It's like even on the craziest days, Lenny, between the start of the day and lunch and between lunch and the end of the day, I take a short break. Even on the craziest days with model launches, et cetera, I'm lucky we have a meditation area in the office that I'll go to.

**Amol Avasare** (01:43:29):
And then the whole side of things around meditation that I talked about in that post, I think both you and I have done a retreat at Spirit Rock and doing a meditation retreat changed my life. And it's something that I do at least once a year now. I have one coming up relatively soon as well. And just I think all of that has helped with better managing the physical side of it because this job is very taxing, and then emotionally having a little bit of space to what happens. So you have sort of awareness on one side, you have the reality on the other side. And reality's crazy here, man. Reality's insane. There's so much happening every day. There's so much noise, it's mind-blowing. And so that relationship between awareness and reality, that's where you have choice that you sort of learn from deep meditation on how to shift that and apply your choice there.

**Amol Avasare** (01:44:26):
I think that that is the thing that has helped me significantly with just keeping a more level head. I think a lot of staying in this game in this level of intensity is just keep your head, just don't lose your head in the crazy times. And I think all of that that I've gone through has helped me do this without resorting to unhealthy coping mechanisms.

**Lenny Rachitsky** (01:44:47):
Wow. Amol, you're such an inspiration in so many ways. There's so many reasons that you would not have been successful and things would not have worked out. And there's so many lessons to learn from just the stories you've shared in the journey you've been on to help people overcome challenges they're having. If you can come back from an insane... Was it like a kick to the head? Is that what happened?

**Amol Avasare** (01:45:11):
It was a kick to the head. That's correct. Yes.

**Lenny Rachitsky** (01:45:13):
Just feeling like you may not be able to listen to music to just leading growth at the fastest growing company in history. There's also just a lesson here of constraints. Again, you mentioned this idea of just the power of constraints. You're forced to take breaks, you're forced to go meditate in a way that's really helpful and it's a lesson for us all. This is actually really good for us all.

**Amol Avasare** (01:45:36):
Yeah. I think that freedom through constraints is one of the big takeaways I've had during that time. Because if you have these constraints, you're forced to adapt and it creates, gives you in a business setting, you have to focus more in a personal setting. And if the constraint is, "I can't do anything and I'm injured. I don't know what's going to happen. I don't know. I'm going to get better," you have two choices. You're like, one, are you just going to resist and fight with reality and really suffer from that, or are you going to accept the situation and not let that affect you emotionally? And it's not to say I did everything, man. I was like, every single thing I could do, diet, I was like, "I'm on it. Every action I can take, I'm on it."

**Amol Avasare** (01:46:16):
But then you have a choice of, are you going to let the impact of that define your happiness or not? And I think that that's the thing when the impacts maybe are not coming, you have to then adapt to, "Okay, what do I want my happiness to be?" And one of the meditation teachers said that true freedom in life is learning how to be content when you don't get what you want. And it's not to say you shouldn't do something when you don't get what you want, but I think that that takeaway of just can you be content and not have your happiness rely on getting something. It's a challenge. I'm not perfect at it, but I think it's probably one of the biggest takeaways from that whole thing.

**Lenny Rachitsky** (01:46:50):
Incredible. And we'll link to the post of folks who want to read this. Before we get to a very exciting lightning round, is there anything else you wanted to share, or should we just jump right in?

**Amol Avasare** (01:46:58):
I think we can jump into it.

**Lenny Rachitsky** (01:46:59):
Oh, we covered a lot of ground. Okay, here we go. I've got five questions for you. First question, what are two or three books you recommend most to other people?

**Amol Avasare** (01:47:09):
It probably ties to a lot of what I just talked about. I think a lot about meditation and my emotional state. What I spend most of my time thinking and reading and researching and working on outside of work. So my recommendations very related to that. The first is a book called Joy of Living by a Buddhist monk. His name's Yongey Mingyur Rinpoche. It's just really about how you can start to think about your life experience in a different way and have tactics of what to do to kind of change just how you think about things. This is one where I've recommended to people.

**Amol Avasare** (01:47:49):
Yeah, I've recommended to a lot of people and they've really, really enjoyed it. I think another one is Awareness by Anthony de Mello, which is a kind of similar thing but from a different angle. Those two I consistently recommend to people. And then the third one is more relevant to product in many ways is Thinking In Bets by Annie Duke. I think just being able to break down a situation when someone's like, "I don't know, it'll get done in time. Okay. Can you put a number to that? What percentage or likelihood is it?" Those types of things, I think, are just so tactically helpful in product.

**Lenny Rachitsky** (01:48:20):
Favorite recent movie or TV show?

**Amol Avasare** (01:48:22):
I think movie is probably Marty Supreme. It's one of the only ones I watched recently. I thought it was great. I thought it was just insane. Absolutely insane movie. It was ridiculous, but I loved it. TV show, I have not watched TV in a while. I think it's probably the Olympics would be the one, if that counts.

**Lenny Rachitsky** (01:48:38):
Is there a product that you love just like, I don't know, when you discovered recently or just one you have in your life that's like, "Oh, this is very cool. People might want to know about it"?

**Amol Avasare** (01:48:45):
Yeah. So this is a funny one. I was in Japan last week and I was sleeping in this hotel and I just really loved the pillow that I had in this hotel. It was very random. I just at times had neck and upper trap pain and sometimes I've been frustrated with my pillow because I sometimes sleep facing up, sometimes sideways and the height's not quite right. And I was just like, "This pillow is just great." And basically this pillow is full of beads. And so you can naturally shift the height of the pillow while you're sleeping even unconsciously without thinking. And so I looked at the tag. I was like, "What is this?" I ordered it to [inaudible 01:49:26] Amazon Japan, and I bought it back with me on the plane. And so I have the name here. It's called the Maruhachi Shinsui Maruhatchi Pro pillow, and you can only get it in Japan, but they're shipped to the US, no affiliation. And I think that has changed my life in the last week.

**Lenny Rachitsky** (01:49:42):
That is an awesome pick. Do you have a favorite life motto that you often come back to in work or in life?

**Amol Avasare** (01:49:48):
Main one I'd say is just she'll be right. This is a very common Aussie saying. It's like she will be right. She'll be right. It's a common Aussie saying when we're faced with a tough or difficult situation, you're kind of dismissing the severity of it in a way by saying like, "Eh, it'll be fine." And I think that that's just such a good metaphor. It's such a good tactic in many, many cases. And then I think the other one is just sometimes in life, you just have to go for it. And that is something that this guy, Eros Resmini, who is the CMO of Discord, who is a very close advisor to me as a founder, he would push me on this and that was something that he would often say is just like, "Just go for it." And I think that it's a very helpful thing of you can sit there thinking, "Should I do this, should I not?" And sometimes in life, you just have to go for it.

**Lenny Rachitsky** (01:50:34):
I love the combo of those two. Just sometimes just go for it and she'll be right. So good. Okay. Final question. Okay. So I'm curious, used to be into martial arts, that didn't go great. Do you have a new hobby that you find yourself loving? Do you make time for hobbies?

**Amol Avasare** (01:50:51):
I think I'm just quite tight on time for hobbies. I would say I think it's largely just work and have my body function and then take care of the most important relationships around me. I think maybe the one hobby I'd say is just I'm really into sports and I've gotten more into sports at football in particular.

**Lenny Rachitsky** (01:51:11):
Like watching.

**Amol Avasare** (01:51:12):
Watching. Certainly not playing. My wife's from Michigan and she took me to a game at the Big House and it just changed my life. From then on, I was like, I'm a Wolverines fan and big Wolverines fan, big 49ers fan. I just love football. So that's probably the one that comes to mind.

**Lenny Rachitsky** (01:51:29):
Amol, this was incredible on so many levels. I'm so thankful that you made time for this considering how much you got going on. Where can folks find you a line, say they want to apply for a job maybe on your team, or can they find that? And how can listeners be useful to you?

**Amol Avasare** (01:51:42):
You can find me on my LinkedIn. It's just Amol Avasare. I'm boring. That's it. You can look online to apply on our jobs page as it rolls across growth engineering, growth product, growth design. We are looking for great people on the growth team. So please come and join us. And I think being helpful to me is just two things, trying our products, giving us feedback, giving us harsh feedback in particular on what [inaudible 01:52:07] you better. And then please send great people our way. We are looking for the best of the best to join the team, and we would love to hear from anyone you know of as well who could be a fit for one of our roles.

**Lenny Rachitsky** (01:52:20):
Dream job for so many people. Amol, thank you so much for being here.

**Amol Avasare** (01:52:23):
Thanks, Lenny. Bye everyone.

**Lenny Rachitsky** (01:52:26):
Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
