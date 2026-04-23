---
title: "How Anthropic’s product team moves faster than anyone else | Cat Wu (Head of Product, Claude Code)"
date: "2026-04-23"
type: "podcast"
guest: "Cat Wu"
description: "How Anthropic’s product team moves faster than anyone else, covering team leadership, AI product work, and product design."
word_count: 16271
---

**Cat Wu** (00:00:00):
I think it is very hard to be the right amount of AGI-pilled. It's very easy to build the product for the super AGI strong model. The hard thing is figuring out for the current model, how do you elicit the maximum capability?

**Lenny Rachitsky** (00:00:13):
I've never seen anything like the pace folks at Anthropic are shipping at.

**Cat Wu** (00:00:17):
We want to remove every single barrier to shipping things. The timelines for a lot of our product features have gone down from six month to one month and sometimes to even one day.

**Lenny Rachitsky** (00:00:27):
You're interviewing hundreds of PMs and you just keep feeling like they're approaching it very incorrectly.

**Cat Wu** (00:00:32):
The PM role is changing a lot. It's changing really quickly. The thing that is extremely important for building AI-native products is iterating so quickly, figuring out a way for you to actually launch features every single week.

**Lenny Rachitsky** (00:00:44):
What do you think are the emerging skills PMs need to develop?

**Cat Wu** (00:00:48):
It comes back to product taste. As code becomes much cheaper to write, the thing that becomes more valuable is deciding what to write.

**Lenny Rachitsky** (00:00:56):
**Cat Wu** (00:01:35):
Thanks for having me.

**Lenny Rachitsky** (00:01:37):
I have so many questions. I'm so excited to have you on this podcast. I want to start with giving people an understanding of your role alongside Boris. Everybody knows Boris. His episode is the number one most popular episode on this podcast, no pressure. He created Claude Code. He leads the eng team, ships a bazillion PRs a day from his phone, just like... I don't even know what the number is anymore. I think people don't give you enough credit for the success that Claude Code has had and Cowork and all the things you all are building. Help us understand your role on the team, how you work with Boris, how you split responsibilities. Just like what does the PMO look like on the Claude Code team?

**Cat Wu** (00:02:16):
I feel very lucky to work with Boris. He's been an amazing thought partner. He's our tech lead. He's very much the product visionary, and he is great at setting, "This is what the product needs to be in three months, six months from now. This is what the AGI-pilled version of the product is," and a lot of my role is figuring out, okay, what is the path from where we are today to that vision three to six months from now? And I spend more of my time on the cross-functional, so making sure that our marketing team, sales team, finance, capacity, et cetera, are bought in on the plan and that we're all rowing the same direction and that once the feature is ready, that there aren't any blockers to shipping it.

**Cat Wu** (00:03:00):
I think in many ways it works well because we kind of mind meld, but it is actually remarkably blurry of a line. I think we're 80% mind meld, and then there's this 20% of things that maybe I care a lot more about than Boris, so I'll drive those and 20% work he cares a lot more than me and he just drives those.

**Lenny Rachitsky** (00:03:20):
**Cat Wu** (00:05:03):
I think before AI, technology shifts were a lot slower, so you could plan on these six to 12 month time horizons, and because you were shipping features at a bit of a slower rate, there was a lot more emphasis on coordinating with all the other partner teams to make sure that their shipping features that unblock your features because code at that time was very expensive to make. I think now with AI and with how much that has accelerated engineering and with how quickly the model capabilities are improving, the timelines for a lot of our product features have gone down from six month to one month and sometimes to one week or even one day. And with that, we actually need to make sure that products ship quite quickly.

**Cat Wu** (00:05:49):
And what that means is as a PM, there should be less emphasis on making sure that you're aligning your multi-quarter roadmaps with your partner teams and more emphasis on, okay, how can we figure out the fastest way to get something out the door? How can we figure out how to make a concept corner of our product suite where we can just... An engineer has an idea or a PM has an idea, and by the end of the week, we are able to get into our user's hands. I think the PMs who do the best on AI-native products are the ones who can figure out, how can I shorten the time from having this idea to actually getting the product in the hands of users and help define what are the most important tasks that need to work out of the box for my product?

**Lenny Rachitsky** (00:06:37):
So what I love about this is what you're saying is just like people haven't grasped how fast they need to move and how much of the job now is helping the team move fast. What helps do that? What do you do, what does your PM team do to help them move this fast other than have access to the most advanced models?

**Cat Wu** (00:06:57):
I think the first thing is to set clear goals. Because LLMs are so general, that actually creates a lot of ambiguity in who we're building for, what problems we're trying to solve, what the top use cases are. And so I think a great PM is able to say, "Okay, our key user is professional developers. The main problem that we want to solve for this feature is maybe there's too many permission prompts and people are feeling fatigue, and the use case is we want professional developers at enterprises to safely get to zero permission prompts." And that actually sets a pretty clear goal because it rules out a lot of potential approaches for reducing permission prompts so that people can get a lot more done with one prompt.

**Cat Wu** (00:07:42):
And then I think the second thing that's very important is figuring out some repeatable process for getting these features shipped. So for Claude Code, what we do is we actually ship almost all of our features in research preview. We clearly brand this when we ship something so that users know that this is an early product, this is just an idea, this is just something that we're trying to get feedback on and iterating on, and that this might not be supported forever. And what this does is it reduces our commitment for shipping something. We can just get something out in a week or two.

**Cat Wu** (00:08:17):
And then the third thing that a PM should do is help create the framework for the team so that they know when to pull in cross-functional partners and what those cross-functional partners' expectations are. So for example, we have a really tight process between engineering, marketing, and docs. So when engineers have a feature that they feel is ready and that we've dogfooded internally, they post it in our evergreen launch room, and then Sarah, who leads our docs, and Alex who leads PMM, Antaric and Lydia on DevRel just jump in and can turn around the marketing announcement for it the very next day. And because we have this really tight process, it lowers the friction for any engineer to ship something, and PM is the role that should be setting this up.

**Lenny Rachitsky** (00:08:59):
How do PRDs fit into this and the fact that you said that goals are a really important part, just like being aligned on what does success look like? Who is this for? Who's this now for? Are you writing PRDs, is it just a couple bullet points? How's that evolved in the world of a PM?

**Cat Wu** (00:09:12):
So there's two things that we do. One is we have very rigorous metrics and we do metrics readouts with the entire team every week. The goal of this is to make sure that everyone deeply understands all the facets of our business, what our key goals are, how they're trending, and what drives them. The second thing that we do is we have this list of team principles, and this includes who our key users are, why those are our key users, and the reason that we articulate all of this is so that everybody on the team feels like they understand how our business works, they understand what's important to us and what we're willing to trade off, and it lets people make decisions by themselves without feeling like they're blocked on PM or any other stakeholder.

**Lenny Rachitsky** (00:09:12):
I love how so much of this is like, okay, we still need PMs in the future, and there's so much talk of why do we need PMs? We're just going to ship and build. We need engineers.

**Cat Wu** (00:10:05):
Oh, we actually do PRDs sometimes. So I think for features that are particularly ambiguous, it does help to write out just a one-pager on what the goals are, what the delightful use cases are, what the failure modes currently are that we need to fix. And there are occasionally some projects, especially things that require heavy infrastructure that do take many months, and for those situations, we do write PRDs still.

**Lenny Rachitsky** (00:10:29):
I want to drill a little bit further into just how you're able to move so fast. I've never seen anything like the pace folks at Anthropic are shipping at. Someone made this calendar of launches across Anthropic, and it was literally every day there was a major feature or product. So one question people had online is you guys just launched this, not launched, but built this incredible model Mythos that is still in preview because it's so powerful, people are a little afraid of what it can do. Have you guys been using this? Is this part of the reason you've been able to move so fast?

**Cat Wu** (00:11:03):
We've been moving pretty fast for several quarters now, so I think it's not fully Mythos. Mythos is an incredibly powerful model. We do use the models internally, and I think this has increased our rate of shipping a little bit, but I don't think it explains the bulk of the increase. I think a lot of it is the process and the expectation on the team. So we're very low on process. We want to remove every single barrier to shipping things. We want to make sure every single person on the team feels empowered to take their idea from just an idea to out in the world in less than a week, sometimes even in a day.

**Lenny Rachitsky** (00:11:41):
Cool. Oh, man. What an advantage to have the best model and also be building product. That's so cool.

**Cat Wu** (00:11:46):
We are very lucky to be able to work with the frontier models.

**Lenny Rachitsky** (00:11:49):
Oh my God, what an awesome advantage, just build a thing and then use it and then accelerate faster. It's so interesting. There's a couple of these other side things, I want to just go on these sidequest on this conversation. There's so much happening with Anthropic, and I just am so curious to get your insight. One is a week ago or so, the whole source code of Claude Code leaked. Somebody got it out there. I think it was a mistake someone made. Is there anything you comment there, just like what happened? What went wrong? What should people know?

**Cat Wu** (00:12:15):
So we immediately looked into this when we saw it. We realized that this was the result of human error. There was a human working with Claude to write PR. This was just an update to how we release our packages and it actually went through two layers of human review, and so this was a result of human error and we've hardened our processes to make sure that it doesn't happen in the future.

**Lenny Rachitsky** (00:12:40):
Is this person still at Anthropic? Are they doing all right?

**Cat Wu** (00:12:42):
Yes, yes. It's a process failure, and the most important thing is to just learn from it and to add more safeguards so that doesn't happen again, and so that's what we've been focused on and most of those have shifted.

**Lenny Rachitsky** (00:12:54):
Okay. Another question I had is OpenClaw. So recently there's been this move to keep people from using Claude's subscription with their OpenClaws. People got really upset. They're confused why this is happening. It feels like there's harm caused to the open source community. What do people need to understand about what went into this decision?

**Cat Wu** (00:13:18):
So we've been seeing a lot of demand for Claude, and we've been working very hard to both scale our infrastructure and also to make our harness more token efficient so that you can get more usage out of it. It wasn't designed for third-party products, which have different usage patterns than our first-party ones. We spent a bunch of time trying to figure out what is the most seamless transition that we can offer, and so I was very happy to be able to say that everyone gets some credits alongside their subscription. But yeah, we did have to make the hard decision that we needed to prioritize our first-party products and our API, and so this is the decision that resulted from that.

**Lenny Rachitsky** (00:14:01):
Yeah. To me, it makes so much sense. You guys are subsidizing this usage at 200 bucks a month and it's basically unlimited use of this. And I think people don't understand. Businesses are trying to make money. We're trying to be profitable here. We can't just give away compute when it's so in demand. So I get it. Coming back to the PM team, what does just the PM team look like at Anthropic? How many PMs are there? How are they kind of organized?

**Cat Wu** (00:14:26):
Yeah, so we have a few PM teams. I think we're maybe around 30 or 40 PMs right now. So we have the research PM team who Diane leads, and this team is responsible for understanding all of the feedback from our customers for our models, and then feeding that to the best research team to act on it, and they also shepherd the model launch. There's the Claude developer platform team that maintains the APIs that Claude Code is built on top of, and they also release things like Managed Agents, which is a way for you to build your agents and we can host it on your behalf. And then there's Claude Code that works on both Claude Code and the Cowork core products.

**Cat Wu** (00:15:08):
There's enterprise that helps make Claude Code and Cowork easier to adopt for all of our enterprise customers, and so this is everything from cost controls, our back security controls, and just making sure that these enterprises feel very confident and comfortable using our tools. And then we also have our growth team that is responsible for growing across our entire product suite. So we work very closely with them on Claude Code and Cowork growth. And I know they also work with our other teams on CDP growth, so growth of people who use the Claude API.

**Lenny Rachitsky** (00:15:43):
So speaking of growth, so Amol was just on the podcast. You have this really interesting insight that most people haven't been sharing. There's always this sense that we need fewer PMs in the future. Why do we need PMs? Engineers can do ship. His take is that because engineers are moving so fast, PMs and designers are squeezed. There's less time to stay on top of everything that is happening. There's a feature shipping every day. So his take is he needs more PMs because it's hard to keep up. What's your take there? Do you feel like there'll be an increase in hiring of PMs? What do you think is going on with the PM profession long-term?

**Cat Wu** (00:16:15):
I think all of the roles are merging. PMs are doing some engineering work, engineers are doing PM work, designers are PMing and also landing code. You can either hire a lot more engineers who have great product taste, or you can keep your engineering hiring the same and hire a lot more PMs to help guide some of their work. On our team, we're pretty focused on hiring engineers with great product taste. This way, we can reduce the amount of overhead for shipping any product. There are many engineers on our team who are fully able to end to end go from see user feedback on Twitter through to ship a product at the end of the week with almost no product involvement. And this I think is actually the most efficient way to ship something.

**Cat Wu** (00:17:05):
So I think engineer and PM are kind of overlapping and you will get a lot of benefit from having more of either. I think product taste is still a very rare skill to have, and we'll pretty much hire anyone who we feel has demonstrated this strongly.

**Lenny Rachitsky** (00:17:25):
And your background was in engineering, right?

**Cat Wu** (00:17:27):
Yeah, I was an engineer for many years. I was then a VC very briefly before joining Anthropic, and actually almost all the PMs on our team have either been engineers or ship code here on Claude Code, and so that's one of the things that I think helps build trust with the team and also just enables us to move a lot faster. And then actually our designers also have been front end engineers before.

**Lenny Rachitsky** (00:17:54):
Wow. Because that's the big question, there's definitely this emerging that's happening, the Venn diagrams are combining. I think the big question for a lot of people is if you're coming from engineering or product or design, which of those core skills is going to be most valuable? I could see it Anthropic and on Claude Code, engineering is very valuable. I'm curious if other companies, if you have a design background becoming a PM is more valuable or just a PM-PM.

**Cat Wu** (00:18:16):
I still think it comes back to product taste. As code becomes much cheaper to write, the thing that becomes more valuable is deciding what to write. What is the right UX for this feature? What is the most delightful way that a user can experience it? We get tens of thousands of GitHub issues asking for every single thing under the sun, and it takes a lot of care and taste to figure out, okay, which of these is worth building and what is the right way to build it? And I think that skillset can come from any background, but I think that's the most important thing.

**Cat Wu** (00:18:53):
I think the reason why an engineering background is particularly useful, at least for the next few months, is if you have an engineering background, you have a better sense for how hard something should be, and that's often a factor in what you choose to build. So if something is very easy to build, then maybe instead of debating it, you just spend an hour doing it, but if something is harder to build and you know that upfront, then you know that, okay, this will just cost a lot more for our team to get this out the door. So it helps a bit with the prioritization.

**Lenny Rachitsky** (00:19:27):
You said for the next few months, is that just because the models will get so good potentially in the next few months, you may not even need to know that as much?

**Cat Wu** (00:19:37):
I think the valued skillsets does change quite frequently, and so it's really hard to predict more than a few months out. So it's less a commentary on what shift I think will happen and more of a commentary that I think large shifts will happen.

**Lenny Rachitsky** (00:19:53):
So you're not saying that's when Mythos comes out and will change everything and that we don't need to know anything about engineering?

**Cat Wu** (00:19:59):
No, I'm just saying that every few months it seems like there's a large increase in coding capability, which then changes what other roles are valuable. I think the most important thing is to be able to have this first principles thinking where you can figure out how the tech landscape is changing, what the team really needs from you, and to jump in and fix that hole because I think the work is becoming more amorphous, which means that a great PM is able to understand what all the gaps are to figure out what the highest priority ones are, and then to just figure out, okay, how do I learn that skillset or what is the skillset that I have that I can apply to this challenge? So I think the current environment values people who are able to wear a lot of hats, are able to swap them, and are very low ego about what work they do to help the team move faster.

**Lenny Rachitsky** (00:21:06):
I love this answer. There's this question I've been asking people in your shoes, folks that are kind of at the bleeding edge of what AI is capable of and building with the latest tools, which is just where will human brains continue to be useful and necessary for a while until we get to super intelligence. What I'm hearing here is essentially picking the things to work on, knowing where the market's going and figuring out what to prioritize essentially, and then it's knowing if the thing you've built is good and right and getting it out there in some early version at least. Does that sound right? Is there anything else of just where human brains will continue to be useful for at least the next few months?

**Cat Wu** (00:21:43):
I think humans still provide a level of common sense that the models don't, and there's a thousand moving pieces to any product launch, some of them are very small, but there's always a lot that could potentially go wrong. I think the model doesn't always have a great sense of who all the stakeholders are, how they relate to each other, what their preferences are, what are the right venues to communicate with them, to keep them on board. I think a lot of this more tacit common sense EQ kind of knowledge is still very valuable. Of course, we want the models to get better at this and I think they will be, but right now I think there's still gaps.

**Lenny Rachitsky** (00:22:27):
How do you just deal as a human going through so much constant change, just being on the inside of the tornado, maybe it's calm there, but just like how do you stay on top of what's going on? How do you stay sane through all this craziness that we're moving through?

**Cat Wu** (00:22:39):
I think our team is still people who lean into the chaos. So we try to face every challenge with a smile because there's always so much going on. There's always so many risks and tricky situations that if you get too stressed about anything, you'll burn out, and so we really look for people who can kind of look at a challenge, be like, "Whew, that's going to be hard, but I'm excited to tackle it and I'm going to do the best that I possibly can. And I know I won't be perfect, but I'll be able to sleep at night knowing that I did my best."

**Lenny Rachitsky** (00:23:12):
That's an interesting answer to just what skills will be important in this future because it's... I forget who said this, maybe Ben Mann, that this is the most normal the world will ever be.

**Cat Wu** (00:23:23):
Yeah, it definitely gets harder. I feel like there are a lot of weeks where maybe Sunday night there's some P0 and then by Monday there's a P00 and by Monday afternoon there's a P000 and you're like, "Wow. I can't believe I was so worried about that P0 from Sunday." But I think you just have to acknowledge that there's only so much that you can do that you need to sleep well so that you can make good decisions next day and just brutally prioritize where you spend your time, what's the most important thing to get right and be okay letting things go. There's products that we ship that aren't as polished as I wish they were, but our top goal is to help empower professional developers, and if a product isn't successful, as long as it's not blocking the core use case, it's okay because we'll hear the feedback and we'll fix it in the next release.

**Cat Wu** (00:24:17):
Launching a feature that is buggy is the kind of thing that would have kept me up at night, but it is something that I'm now able to live with knowing that, okay, we're going to get that quick feedback and we're going to fix it in the next release.

**Lenny Rachitsky** (00:24:31):
What I'm imagining is there's that GIF. I think it's maybe from Pirates of the Caribbean where it's this guy walking down a pair of stairs on a ship and the whole ship is just being demolished around him and he's so chill, just strolling down the staircases as everything's falling apart. And that's interesting because everyone I've met from Anthropic is just so chill and just so optimistic. Yeah, I think that's a really interesting insight is just like having this calmness and optimism versus just like, "Oh my God, everything's crazy and going nuts."

**Cat Wu** (00:25:00):
Yeah, I think if you don't have it, you'll get pretty burnt out. I think we also tend to hire people who have been in the industry for a while and have experienced lots of ups and downs and have a good sense for what gives them energy and how to maintain their energy over time, and I think that's helped us a lot.

**Lenny Rachitsky** (00:25:20):
So interesting. Something that I wanted to ask about is, so there's these roles blurring, engineers are becoming PMs, everyone's dogs are cats, everyone's everyone. What do we lose in that world? Do we lose career ladders and clear career paths? Do we lose design consistency, code quality? There's probably some downsides. What are some things you find are just like, okay, that's something we're sacrificing for the greater good?

**Cat Wu** (00:25:42):
We're sacrificing product consistency. Historically, when code was expensive to write, you would carefully plan out everything in your product suite, how every product relates to each other, what the use case for every single one is, how they integrate, and you would pretty much have one product for each use case, and now with AI moving so quickly and with so many ideas that we need to test out, we do sometimes have features that overlap with each other. A lot of the times it's because there's two form factors that we love internally and we want the external audience to tell us which one is better. What that means for someone who's a new user though is a new user might not know, okay, what is the best path to accomplish X? There is more education we need to do to help people understand what the core features are and what the best practices are for using them.

**Cat Wu** (00:26:41):
I think this is the cost of launching a lot of features. I think users also feel like it's hard to keep up with the latest. Usually in traditional PM, you ship a feature every month or quarter, and so it's really easy for a user to understand, okay, I just need to check in on this once a month and I'll learn some new things, and if I ignore it for six months, it's fine, I don't feel like I'm missing out. I think with these agentic tools, not just Claude Code and Cowork, but across the whole ecosystem, people feel this need to check Twitter every single day to see what the absolute latest thing is, and I think there's more we can do to help people feel less like they're on this ever increasingly fast treadmill and that they feel like... I would love people to feel like they can just open these tools, the tools will educate them or teach them what they want to know, and that they can just feel more bought along.

**Lenny Rachitsky** (00:27:48):
Yeah. I saw you launch this really interesting feature the other day. I think it's /powerup where it basically walks you through all the cool ways and basically all the best practices to use Claude Code. Is that kind of along these lines?

**Cat Wu** (00:27:57):
Yeah, exactly. So in the past, we didn't actually want to do something like powerup, because we felt like the product should be intuitive enough that you don't actually need to go through any tutorial, and over time, we've just realized that there's just so many features and there's so much demand for a built-in onboarding experience that we diverged a bit from our original principle saying no onboarding flow and added this because there's just so many users who wanted to know there's a hundred features, what are the 10 that I absolutely need to use? And so we put that together.

**Lenny Rachitsky** (00:28:32):
Yeah, it's such a bizarre world. So Anthropic has been really successful with B2B enterprises where traditionally you don't launch a bunch of stuff, you just kind of have quarterly release maybe, and it's like the opposite of every day we got some new... So just maybe following that thread, the run Anthropic has been on as just otherworldly. Anthropic was way behind when it started. It was, Amol shared this, just like one of the least funded companies, didn't have distribution, wasn't the first to go, OpenAI was way ahead and it was just like no way Anthropic has any chance to compete significantly long-term. Now it's just killing it, just beating the biggest companies, teams. So much just like the growth is just... $11 billion in ARR in one month growth. By the time this comes out, it'd probably be even higher. Just being on the inside, what are some ingredients that have allowed Anthropic to be this successful and kind of come from behind and do this well?

**Cat Wu** (00:29:29):
The two most important things are, one, this unifying mission. It's hard to state how important this is. We hire people who care most about bringing safe AGI to all of humanity, and this is actually something that we reference frequently in our decisions about what our entire product org should focus on shipping. And because we put this mission above any individual product line, we're able to make Make very fast decisions that cut across the entire org and execute on them in a unified way. So I think this is something that I've never seen at a company of our scale.

**Lenny Rachitsky** (00:30:12):
And so just to make sure that's clear, so essentially having the number one mission is safety, alignment, making sure AI is good for the world, and you're saying just having that as a clear mission makes decisions a lot easier to make.

**Cat Wu** (00:30:24):
If there's two competing priorities, we'll talk about which one is more important for Anthropic's mission, and it makes it a lot easier to decide which of the two we prioritize and then everyone will stand behind the one that we decide. And so sometimes that means that, hey, we want to ship something on Claude Code, but this other thing is more important, and so we deprioritize shipping this and we just wait until later.

**Lenny Rachitsky** (00:30:47):
What's really interesting about that is that explains, I think, versus another company maybe rhymes with OpenAI did a lot of different things, and what I'm hearing here essentially is like, okay, we're not going to launch a social network, we're not going to launch a feed of interesting information because it's not aligned to this mission, and that has kept Anthropic focused, which seems to be a core ingredient to the success.

**Cat Wu** (00:31:10):
Well, when I think about mission, I think about putting Anthropic's goals ahead of any individual org or any individual product. And so for me, it's... I think the second thing that we're very good at is focus. I think mission to me is slightly different. Mission means that teams are willing to make sacrifices that hurt their own goals and their own KRs in service of Anthropic's goals and Anthropic's KRs, and people are very happy to make those trade-offs. So an extreme example is if Claude Code failed, but Anthropic succeeded, I would be extremely happy. And the whole team is very willing to make decisions that follow that chain of thought.

**Lenny Rachitsky** (00:31:58):
I don't know if you can talk about this in depth, but do you feel like the OpenClaw decision is a part of this, just like, okay, this is not furthering the mission of Anthropic, we need to stop this because it's not working in the way we want it to work?

**Cat Wu** (00:32:11):
I think one of the most important things for Anthropic is to grow the number of users that we're able to reach. One of the ways that we're able to do this is with the Claude subscriptions with our first-party products. And so we just very much want to double down on that, but that does come at the expense of third-party products sometimes.

**Lenny Rachitsky** (00:32:29):
So we've been talking about Claude Cowork, all these things. Something that I want to make sure people get, and I'm curious just how you use these tools. So there's Claude Code, there's Claude desktop/web, there's Cowork. What's the best way to understand when to use which? When do you use each of these three?

**Cat Wu** (00:32:44):
So I tend to use Claude Code in the terminal when I'm just kicking off a one-off coding task, and I want all of the latest features. The CLI is our initial product surface, and it's also the one where our features often land first, and so it's the most powerful of all the tools. So that's what I tend to use when I'm just trying to kick off one or maybe a handful of tasks at a time. I think desktop really shines when you're doing something that requires front end work, and so one thing that I love to do is to use our preview feature.

**Cat Wu** (00:33:22):
So if I'm building a web app, I'll often use Claude Code and desktop. I'll have the preview pane open on the right-hand side so that I can actually see the web app that I'm making in real-time as I'm chatting with Claude. It's also really great for people who want something a bit more graphical. A terminal can feel very unfamiliar to someone who's non-technical. You get a bunch of these scary popups on your machine and you can't click around the way that you're used to in pretty much every other product that you use. So there's a lot of people who just don't feel comfortable in the terminal, and if that's you, I would highly recommend checking out Claude Code on desktop. Desktop is also great for getting an at-a-glance view of everything that's happening. So you can see your CLI terminal sessions in desktop, you can see your other desktop sessions, you can see your sessions that you kicked off on web and mobile. So it's a one-stop control point where you can see all of your tasks.

**Cat Wu** (00:34:16):
I think the benefit of web and mobile is that it's really great for kicking things off on the go. So CLI and desktop both require you to be on your local laptop, and this is constraining because sometimes you're out and about, you're touching grass, you're going on a walk and you don't have your laptop open, and I can't count the number of people who I've seen holding their laptop open, like tethered to their phone while they're outside. And this just means that we're missing a product that solves that need. And so for me, what mobile lets you do is kick off these tasks on the go so that you don't need to bring your laptop everywhere and make sure that your laptop's open wherever you are.

**Lenny Rachitsky** (00:34:57):
I love that. I've seen people on plane. It's just like such a meme now. Just I need to let this agent finish. I can't shut this down. I need WiFi.

**Cat Wu** (00:35:06):
Exactly. And then I think for Cowork, the role that this fills is there's a lot of work that everyone does where the output isn't code. So whether that's like getting to Slack zero or inbox zero, or whether that's creating a slide deck for some customer meeting that's coming up, or whether that's writing a quick doc on what the goals of a feature are or what the launch plan for a feature is. All of these tasks produce outputs that are non-code and Cowork is best positioned for that. So the way that I split the products in my mind is if I'm building something where the output is code, I'll use Claude Code or desktop or Claude Code on mobile, and if the output is anything that's not code, I'll use Cowork for it.

**Lenny Rachitsky** (00:35:48):
People are just sleeping on the success that Cowork is having. It's just growing incredibly fast, and I think people still don't understand maybe what it's for. And so what if you give us a couple use cases just in your work as a PM? What are some really interesting, maybe unexpected ways you use Cowork to save you time, get more work done?

**Cat Wu** (00:36:08):
If you are getting started on Cowork, the first thing that you really need to do is connect all the data sources that are relevant to your role because Cowork can only do a great job if it has access to all the context that it needs to be able to curate the output for you. So what that means for me is I connected to my Google Calendar, I connected to my Slack, to my Gmail, to my Google Drive so that it just knows... It has the flexibility to find relevant context, to ask questions, to pull in threads, and this substantially improves the quality of the result. The kinds of things I use it for are like last night we have this Code with Claude conference coming up and there's a few talks that I'm giving there.

**Cat Wu** (00:36:54):
And one of the talks that we're doing talks about the transition of Claude Code from an assistant to a full-on agent, and one of the things that I wanted to do in this talk was to showcase all of the products that we've been shipping that enable this transition, and also to figure out, okay, what are the success stories that people have had internally that we can use as demos? And so I have my Google Drive connected, I have Slack connected. Alex, who's our product marketer, put together a draft of what the points that he thinks we should cover are.

**Cat Wu** (00:37:33):
And so I just fed this all into Cowork. I told Cowork the narrative that I wanted to tell, and it actually just worked for an hour. It looked through Twitter to see what we launched, it looked through our evergreen launch room, it looked in our Claude Code announced channel, which is where our team posts demos of how they've been getting the most value out of Claude Code, and it synthesized all this together to this 20-page deck that I woke up to this morning and I read through it and it was like pretty good. There were a few tweaks, so I did have to give it a round of feedback. I like my slides to have extremely minimal words and it was a little too wordy, but it was far faster than what I would be able to produce. And because Cowork has access to our whole design system, it actually looks like an Anthropic designer put it together. When you visually see it, you're like, "Oh, this is incredibly polished."

**Cat Wu** (00:38:29):
So these are the kinds of things that are so much faster. Making this slide deck would've taken me hours, but instead it turns out a draft that is actually quite good so that I could focus on making sure that the demos are amazing that we plug into it.

**Lenny Rachitsky** (00:38:45):
This sounds like a dream come true to PMs that... Putting decks together, so annoying.

**Cat Wu** (00:38:49):
It's so slow.

**Lenny Rachitsky** (00:38:51):
And I love people will see this deck whenever you present this. This will be out in the world. Obviously it's not the one-shotted version, but you've iterated on it. So just to help people try this for themselves, so step one is connect their... What did you say? Slack. What else do you suggest they connect?

**Cat Wu** (00:39:07):
Slack, Google Calendar, Gmail, GDrive. You should connect your communications tools and where you store your source of truth data for what your team cares about, what you care about and what you're working on.

**Lenny Rachitsky** (00:39:21):
Okay. And then what was the prompt roughly that you put in there to generate this deck?

**Cat Wu** (00:39:25):
So I just wrote make me a slide deck for the code with Claude Conference. This is what our PMM suggested it should cover. This is the current draft that I made that I don't like. This is one that I made manually that I don't like, but I linked it. Can you start by creating a proposed outline with details? Also, make sure it doesn't overlap too much with a keynote talk, which is more important. And then Claude read a bunch of the links that I sent to it and created a proposed outline. So then I read through its proposal and all the different ideas that I had generated for what we could cover, and I just made a decision on what I wanted to actually be in the final deck, and I think this is an example of what the role of the PM still is today.

**Cat Wu** (00:40:07):
It's like Claude is a great brainstorming partner. It's able to synthesize a massive amount of information really quickly and present all of the possibilities to you, but the role of the PM is still to make the end decision of, okay, what should belong in the final product? So for this, what I ended up deciding was that I wanted the talk to cover the progression from making local tasks successful to making every PR green, to helping engineers land more PRs, and for each of these, which demo would be the most compelling. And then after this decision about the outline, Cowork just went off for a few hours and built the whole slide deck.

**Lenny Rachitsky** (00:40:50):
This is so awesome. What an awesome part of the job to not have to do anymore, and it feels like you're talking to essentially a deck designer that also has actual knowledge about what you've worked on and can make it actually the content what you want it to be, not just make it look really nice. How did you do the design system piece? How does that work? How does it know the design system of Anthropic?

**Cat Wu** (00:41:15):
So what I did for this is we actually already have a standardized deck that we use across all of our external engagements. And so I just gave Claude access to that, and so it's able to see what colors we use, what fonts we use, the different kinds of, what's it called, like slide formats that are possible, and so it has 20 of these example slides.

**Lenny Rachitsky** (00:41:37):
So give an example, got it. So you upload, here's our template, work from this. Yeah.

**Cat Wu** (00:41:41):
You can also connect to your Figma MCP if you have your slide format save there and it can pull that in.

**Lenny Rachitsky** (00:41:48):
Along those lines, something I'm always curious about is what's kind of in your stack of tools as a PM at Anthropic? Obviously Claude Code and Cowork and all the Anthropic tools. What else are you using? What other... Slack you mentioned. Is there anything else?

**Cat Wu** (00:42:02):
So my stack is pretty heavily Claude Code, Cowork and Slack. Anthropic largely runs on Slack. I feel like it's the core OS of our company. And day-to-day, I would say maybe 30% of my time is pushing the boundaries of what Cowork and Claude Code can do so that I have a very strong sense of what we're not good at, and I spend a lot of time talking with the model to understand why it makes mistakes that it does. We actually have a lot of internal tools that we make. I think one of the things that Claude Code has really unlocked for our entire company is it really lowers the barrier to making any custom app that you want, and so we've seen this surge in personalized work software that people are building for custom use cases instead of using tools that don't perfectly fit the use case.

**Lenny Rachitsky** (00:43:06):
I got to hear more. What are some examples? What are things you've built, other people built that are really popular and useful?

**Cat Wu** (00:43:12):
One of the sales folks on Claude Code, he realized he was making these repetitive decks over and over and over again, and so he actually has this web app that he built with the examples of the core Claude Code decks that we know work well, so like a 101, 201 and mastering Claude Code, and then he has a way to input specific customer context that pulls from Salesforce, that pulls from Gong, that pulls from other notes so that we can customize the decks for specific customers. And so we'll pull out things like, okay, this customer is using Bedrock or Claude for enterprise or console, which affects what features are available to them. It'll pull out things like, okay, this customer is concerned about the code review stage of the SLC, and so we'll add a slide about our code review features there. It'll pull out things like, okay, this customer needs to be HIPAA-compliant or needs X, Y, Z security controls, and so we'll make sure to add a slide or two in their deck about that.

**Cat Wu** (00:44:14):
And then for example, if this is a customer that's on Vertex or Bedrock and doesn't want to use Claude for enterprise, then we'll just take out some of the slides that are Claude for enterprise-only features. And so normally this is manual work that could take 20, 30 minutes, and so people will either spend that time doing it or they'll just decide not to do it and use the general deck. With this, it takes a few seconds and you get a tailored deck.

**Lenny Rachitsky** (00:44:42):
What's interesting about this Slack is the tool that nobody's... It's just like nobody's trying to create their own. Slack just continues to win, and this is just like the way you describe it as the OS of so many companies. It's so interesting. People talk about Salesforce as just SaaS. We don't need SaaS software anymore. We're going to build our own. It's like Slack is a durable tool that nobody wants to try to compete with and build a better version.

**Cat Wu** (00:45:04):
I think it's pretty important communications infrastructure, and I think they do the core task of helping everyone get real-time updates incredibly well.

**Lenny Rachitsky** (00:45:13):
Yeah, people hate on Slack, but it's really great at what it's trying to do, and the most cutting-edge teams are hooked on it. It's so interesting.

**Cat Wu** (00:45:21):
Yeah, and I also love how easy they've made to customize it. And so we love making Slack bots and this kind of hackability means that we're able to integrate with Slack the way that we want to. So really appreciate Slack's work on that.

**Lenny Rachitsky** (00:45:38):
Time to buy some CRM stock.

**Lenny Rachitsky** (00:45:40):
I am so excited to tell you about this season's supporting sponsor Vanta. Vanta helps over 15,000 companies like Cursor, Ramp, Duolingo, Snowflake, and Atlassian earn and prove trust with their customers. Teams are building and shipping products faster than ever thanks to AI, but as a result, the amount of risk being introduced into your product and your business is higher than it's ever been. Every security leader that I talk to is feeling the increasing weight of protecting their organization, their business, and not to mention their customer data. Because things are moving so fast, they are constantly reacting, having to guess at priorities, and having to make do with outdated solutions. Vanta automates compliance and risk management with over 35 security and privacy frameworks, including SOC 2, ISO 27001, and HIPAA. This helps companies get compliant fast and stay compliant. More than ever before, trust has the power to make or break your business. Learn more at vanta.com/lenny. And as a listener of this podcast, you get $1,000 off Vanta. That's vanta.com/lenny.

**Lenny Rachitsky** (00:46:49):
Okay. So you talked about all these different teams and how they use Claude Code and Cowork to operate. Which teams do you find other than engineering... Imagine engineering is the biggest token spender, but if not, that'd be really interesting. What's the second place function right now for tokens?

**Cat Wu** (00:47:04):
Oh, Applied AI is amazing at pushing the boundaries of what Claude Code and Cowork can do. A lot of our Applied AI team spends time with our customers helping them adopt our API, and so sometimes our Applied AI team will, for example, make prototypes on behalf of these customers, which Claude Code makes so much faster than it used to do. They also have the dual goal of needing to manage a lot of customer comms, a lot of customer inbound and historical context, call notes, and so they're both extremely heavy on Cowork and on Claude Code.

**Lenny Rachitsky** (00:47:42):
And just to understand Applied AI, is that forward to play engineering sort of role? How would most people describe what the Applied AI team is doing?

**Cat Wu** (00:47:52):
Yeah, it's helping our customers adopt the latest API and model features across their company, both for powering their company's products and also for internal acceleration.

**Lenny Rachitsky** (00:48:05):
Got it. So it's like customer success, go to marketing, kind of for deploy engineering sort of thing.

**Cat Wu** (00:48:11):
Exactly. It's like a very technical go to-market person.

**Lenny Rachitsky** (00:48:13):
Got it. Okay, awesome. So you're saying that might be the second org that uses the most tokens?

**Cat Wu** (00:48:19):
Yeah. And then we also see them pushing the boundaries of what Cowork can do. So for example, if... So a lot of these folks cover multiple customers and in any given day can have five to 10 customer engagements on a high day, and so what they often use Cowork to do is the night before, they'll ask it to summarize, okay, what are all my customer meetings that are coming up the next day? What are all the things that this customer has asked me for? What's top of mind for them? What are the action items from the past meetings? And Cowork will just put together this dossier, this brief of what they should be aware of going into the next meeting. And Cowork can also research answers. So if a customer asks, "Okay, when is feature X going to launch?" Cowork can help the Applied AI person research through Slack to get the latest ETA, add that to the notes so that during the customer call, the Applied AI person has the absolute latest. And these are just workflows that people are building for themselves and sharing with other people on their team.

**Lenny Rachitsky** (00:49:25):
So cool. Something that kind of this question, this trend, I don't know, question topic comes up a lot recently, which is tokens spend exceeding people's salary where people just use AI and it costs more than how much they're making. Are there any numbers floating around Anthropic of just how much tokens spend, say, engineers spend, I don't know, a month, a day or PMs, anything like that?

**Cat Wu** (00:49:50):
It is clear to us that as the models get better, people delegate far more tasks to it and they spend a lot more hours in tools like Claude Code and Cowork, and so we do see the token cost per engineer or per any knowledge worker increase every time that there's a model jump or a substantial product improvement. I think it's still much lower than what the average engineer salary is, but we see the percentage increasing over time.

**Lenny Rachitsky** (00:50:22):
It's such an interesting... We talked about how you have access to the most cutting-edge models and other advantage of working Anthropic, I believe you guys have basically unlimited tokens. You can use as much as you want. Is that right?

**Cat Wu** (00:50:33):
We can use a lot of tokens. Some people do run into limits, so-

**Lenny Rachitsky** (00:50:37):
Okay, there's a limit. Okay. Boris, shut it down. Okay. It's so interesting how many advantages come from having the most advanced model. It's such an interesting flywheel that starts to kick in.

**Cat Wu** (00:50:49):
I think we also believe a lot in empowering our internal teams to build as fast as possible, and we also trust that everyone understands how much capacity that serving these models truly costs, and we trust our team to use the tokens responsibly. So it's very frowned upon to waste tokens, but we do trust individuals to make that judgment call.

**Lenny Rachitsky** (00:51:14):
Awesome. Coming back to the PM role, we talked a little bit about this, but I think this will be really interesting for people to hear. Just what I want to understand is what do you think are the emerging skills that PMs need to develop/you most look for, AI companies most look for when they're hiring PMs these days?

**Cat Wu** (00:51:35):
I think the hardest skill is being able to define what the product should look like a month from now. I think there's a lot of ambiguity in what models are capable of in that timeline and how user behavior will change, but I think there are patterns that the best PMs can see based on how users are abusing the limits of the existing product and the best PMs can sense that, can set a direction and can steadily execute towards it and change the path if the model capabilities are much better than or worse than what they'd originally expected. I think it is very hard to be the right amount of AGI-pilled because I think everyone can see this future where the models are extremely smart and can do almost everything, in which case you actually don't need that complicated a product, you can actually just have a text box again where you tell the model what you want and it's so smart that it can add any tool or add any integration that it needs to get the job done. It knows when it's uncertain, it can ask clarifying questions.

**Cat Wu** (00:52:45):
It's kind of very easy to build the product for the super AGI strong model. I think the hard thing is figuring out for the current model, how do you elicit the maximum capability? How do you help users go get onto the golden path? How do you guide users to interact with the model's strengths and patch its weaknesses? This skill is pretty rare.

**Lenny Rachitsky** (00:53:19):
And how do you build that skill? Is it just using each... Basically understanding the limits of each model? You talked about taste, understanding, having taste into what the model maybe is capable of, what it's great and not great to at, where it's changed?

**Cat Wu** (00:53:32):
Think it's spending a ton of time talking and using the model. One of the things I really like to do is to ask the model to introspect on its own behaviors. So sometimes when I notice that the model does something unexpected, like for example, there's situations where the model will make a front end change and run tests, but not actually use the UI. It's actually pretty useful to ask the model to reflect on why I did this, and sometimes they'll say that, "Hey, there was something confusing in the system prompt," or, "I didn't realize that the front end verification was part of this task," Or, "Hey, I delegated the verification to this subagent and the subagent didn't do the test and I didn't check its work." A lot of times just being very curious about why the model made the decision that it did will show you what misled it so that you can fix the harness in order to close this gap.

**Cat Wu** (00:54:31):
The other thing that helps is to figure out who are the users who you trust the most to give you accurate feedback about the model. Usually there's a handful of people who are much better than others at articulating what makes a specific model or model harness combination good, and there's a lot of people who will give you feedback, but not everyone's feedback is as qualified. And so finding a group of those five people you trust is really important for getting very fast feedback. I think the third thing that is useful, but not everyone loves doing is building evals. You don't need to build hundreds of evals for them to be useful. Just building 10 great evals is important for helping the team quantify what the goal is and what their progress towards it is and what they're missing, and so I think evals is this underappreciated thing that more PMs, more engineers should be working on.

**Lenny Rachitsky** (00:55:33):
We've covered evals a bunch. There's this trend of just like, that is the future of product management's writing evals because essentially it's what does success look like. Okay, cool. Let me actually concretely define it and then we'll know. How much of your time are you spending writing evals, would you say?

**Cat Wu** (00:55:46):
I think the importance of evals varies a bit based on the feature that you're working on or what the problem you're trying to solve is. So there are a lot of folks on our team who do spend a lot of time working on evals. We have a small pod of folks who collaborate very closely with research to more precisely understand our Claude Code behaviors and what the largest areas of improvement are and trying to measure those pretty concretely. I personally jump into evals when there's a feature that I think needs a bit more product definition, and often the output of this is, "Okay, here are five evals that I made. This is how you run them. These are the ones that succeed and these are the ones that don't, and this is the prompt that I've used to increase the success rate." It varies a lot though based on the exact feature. Not every feature needs it, but I think features such as memory benefit a lot from it.

**Lenny Rachitsky** (00:56:46):
This point you made about people being very good at evaluating models so interesting. It's almost like a human eval of just like, okay, they understand where it's spiking, where it's maybe lacking. Is there anyone specific that you want to shout out that's very good at this?

**Cat Wu** (00:57:01):
Two people who I think are incredible at this are, one, Amanda, who molds Claude's character. It's just such a hard role because the task is so ambiguous. Even coding is easier because you can verify the success, whereas crafting the character requires a very strong sense of conviction in who Claude should be, and I think she has an incredible ability to not only mold the character, but also to articulate what the goals are, what the character, what's successful and what's not. The other group of people who I really trust is just the Claude Code team.

**Cat Wu** (00:57:46):
So we often have team lunches and whenever there's a new model we're testing, one of the fastest ways for us to get feedback is to just at these team lunches, just go to every single person and just be like, "Hey, what is your vibe on the model?" And oftentimes we'll get feedback like, "Okay, this model is not fully explaining its thinking. It's too abrupt," or like, "Hey, this model just loves writing a ton of memories, but we're not sure if the memories are high quality or not," or some people will notice that, "Okay, this model loves to test itself, which is great, or this model isn't testing itself enough." So that informs what data we look at to verify, okay, is this a larger pattern? So we have a ton of data, but it is very hard to extract insights, and so the feedback from this group helps us inform, okay, what are the hypotheses we want to test, and then we're able to extract data to test that.

**Lenny Rachitsky** (00:58:45):
This point you made about the character of Claude, I had Ben Mann on the podcast, co-founder, and he talked about this, just the character, the constitution of Claude is such an important part of Claude. And I didn't realize until afterwards just with OpenClaw actually, one of the reasons people are sad is the personality of your Claude is... Because Claude's personality is so good and fun and interesting unlike other models. And the way he put it is the personality is what makes Claude so good at so many things. It feels like this trivial side thing. Okay, it's going to be funny and interesting and talk in a fun way, but it's so core to the success of Claude. Is there anything get shared there about just what people may not understand about why the character, as you described, and the personality is so key?

**Cat Wu** (00:59:34):
When you reflect on everyone you've worked with, there's just some people where you're like, "I really like their energy. I really like their vibe," and when people think about Claude and Claude Code, this is one of the things that people bring up the most where they just really love that Claude, it's lighthearted and fun, but it also is extremely confident at your task. People really like that Claude's low ego, and so if you tell it, "Hey, you did this thing wrong." It's truly sorry. It's like, "Oh, shoot. Thanks for telling me. Let me fix it. Let's work together." It's also very positive. So if you're feeling like, "Oh, this is an insurmountable task. I don't know how to get started," Claude is like, "Okay, it's okay. These are the steps that I think we should take. Do you want me to get started on it for you?"

**Cat Wu** (01:00:28):
I think part of what makes a great Coworker is this positivity, this bias towards action, this ability to give you earnest feedback, not just agreeing with every single thing that you say, and so we try to imbue this into Claude because we think it makes it a lot more enjoyable to work with.

**Lenny Rachitsky** (01:00:45):
There's something I want to come back to. You talked about how when new models come out, you often have to revisit things you've built. That's so interesting and so frustrating maybe, just like, "Oh, Goddammit it. Reshipped this thing, now I have to rethink it." Talk about just how often you have to come back with a new model and they're like, "Okay, we have to redo this product that we launched a few months ago."

**Cat Wu** (01:01:03):
A lot of the changes that we make with a new model is removing features that are no longer needed. So a lot of times we add features to the product as a crutch for the model because it's not naturally doing itself. So the classic example for this is the to do list. When we first launched Claude Code, people would ask it to do these larger factors and Claude Code would say, "Okay, cool. I need to change these 20 call sites," and it would go and change five of them and then stop. And then we were like, "Okay, how do we force it to remember to get every single one of these 20?" And so Sid on our team was like, "Okay, what if we just think about what a human would do? A human would make a list of everything that they need to change. Similar to how in VS Code, you would look up all the call sites and it would be a list on the left side and you would go through them one by one and replace all. How do we give this kind of a tool to Claude?"

**Cat Wu** (01:01:55):
And so he added the to do list and we found that with that, Claude was actually able to fix all these 20 call sites. But then with Opus 4 and later models, we realized that we didn't need to force it to use this to do list, it would naturally use itself. For the earlier models, we had to keep reminding it, "Hey, did you finish everything on the to do list? You can't finish until you're done with everything on the to do list." And for the later models, without prompting, it's just naturally thinks to do everything on the to do list. These days, the to do list is still nice to have as a user because then you can more clearly see what Claude is working on. But honestly, it's such a de-emphasized part of the product right now that the model may use it, the model may not use it. It's really not necessary for it to make thorough changes anymore.

**Lenny Rachitsky** (01:02:44):
I forget who said this on the podcast, that the model will eat your harness for breakfast, and what I'm hearing here is essentially you remove things over time that you've had to add on top of the model where it was not operating the way you wanted. And essentially, as the models get smarter, it becomes simpler and simpler for it just to do the thing you want it to do.

**Cat Wu** (01:03:03):
Yeah. We can remove a lot of prompting interventions every time the model gets smarter. And we actually do this every time we launch a model, we read through the entire system prompt and we reflect on, okay, for each of these sections, does the model really need this reminder anymore, and if not, we'll remove it. The most exciting thing that new models unlocks though is just entirely new features. So there's a lot of features that we've been testing out with prior models and the accuracy wasn't high enough for us to want to launch them, and so one example of this is code review. We tried to build a code review product a few times and we've launched simpler versions of code review, which is the /codereview command in the past, and it was only with the most recent models that we felt like, okay, this code review is so good that our engineering team relies on this code review to pass before we merge PRs.

**Cat Wu** (01:03:58):
And we found that this was... We've always dreamed of Claude being able to be a reliable code reviewer that we can confidently feel catches the majority of bugs, and it was only with Opus 4.5 and 4.6, and Sonnet 4.6 that we felt like, okay, we are now able to run multiple code review agents simultaneously to traverse the entirety of the code base and to synthesize a set of real issues that an engineer needs to address before merge. And so this is a new capability that the newest models have unlocked.

**Lenny Rachitsky** (01:04:39):
This is another trend that is very common on this podcast of build something that will possibly be possible in the next six months, be kind of at the edge of what's working sort of, and then it'll catch up and then it'll be an amazing product and you'll be ahead of everyone.

**Cat Wu** (01:04:52):
Yeah, exactly. It's pretty important to build products that don't necessarily work yet so that you know, okay, what is missing for this product to work? And then with the newest model, you can just swap it into the prototype you've already made and see, okay, does this new model close that gap?

**Lenny Rachitsky** (01:05:12):
How much are you able to speak to just where things are going with Claude and Cowork as the vision of it? I imagine you don't want to give away too much about the goal, but it feels like there's all these awesome features being added on top, dispatch, control from phone and all these mobile app, all these things. What's kind of just a way to understand the vision for all these things long-term?

**Cat Wu** (01:05:32):
We think about this in terms of building blocks. So for both Claude Code and Cowork, the core building block is making individual tasks successful. So you wanted to produce some output, you give it a prompt description. Is it able to consistently produce acceptable output that you're able to either merge or share with your colleagues or external audience? So the task is the core building block. As the models get smarter, the task access rate gets a lot higher, and then we see people moving towards doing multiple tasks at the same time. So multi-Claudeing was this big thing towards the end of 2025, and it's only increased since then. And so we see this as, okay, great. One task works, and now you can do six tasks at a time. As the models get even smarter, the way that we are extrapolating this is, okay, next, maybe you're going to run 50 Claudes at a time or hundreds of Claudes at a time, and so what is the infrastructure we need to build to enable that?

**Cat Wu** (01:06:30):
At that point, you're probably not going to run everything locally on your machine anymore. There's just not enough RAM to do it. And so we're thinking about how do we make it easier for you to manage all these? These will probably run remotely. How do we build the interface so that you as a human know which tasks you need to look into? How do we make sure that the agent is fully verifying its work so that when you look at a task and it says it's done, you can very quickly verify and fully trust that it is done to your spec. And how do we make sure that this process is self-improving so that when you do see a task that isn't done to your liking, you can give it feedback and the model will know for every future run to incorporate that feedback so it never makes that mistake again? So this is the progression that we're bringing our users along for.

**Lenny Rachitsky** (01:07:23):
There's a lot of people listening, a lot of product managers, a lot of maybe founders, a lot of other cross-functional folks listening. There's a lot of worry about just how their role... Just the future of their careers. What advice would you have for just people to not just survive this transition to this very AI-driven world, but to be really successful to essentially just to thrive in this future? What are just things people need to hear, need to be doing?

**Cat Wu** (01:07:49):
I think AI gives everybody a ton more leverage than they used to, and so I would push you towards anytime you realize that you're doing some manual task multiple times, think about how you can use Claude Code, Cowork, or other AI tools to automate that for you. Most people have creative parts of their job that they absolutely love and then tedious parts of their job that they really hate doing. I think the beauty of AI is that it can do those tedious parts for you. It can learn from every time that you've done that manual task and generalize and then run it automatically and so that you can focus on the creative parts and that means you can do a lot more than you used to be able to do.

**Cat Wu** (01:08:32):
So I think my immediate push for people is figure out the repetitive parts that you can pass to Claude, iterate on those automations until the success rate is very high, and then focus on, okay, what more can you be doing for your team, for your product, for your company that people haven't had the bandwidth to pick up so far, or what is that pet project that you always thought the company should do that you've never had bandwidth to do? If AI can take care of the grunt work, then you have this extra 20% time now that you might not have before. So my push is to lean into these tools, hand off the work that you're not excited to do, figure out how it can accelerate you, and then as a result, you'll be able to do so much more.

**Lenny Rachitsky** (01:09:19):
Something core to what you just shared, which I fully agree with is find problems to solve with AI. There's all this potential what all these tools can do. For a lot of people, the hardest part is just like, "What should I actually do?" And what you're saying here is just pay attention to things that you are doing constantly you can automate, pay attention to just ideas that have been floating around that you haven't had time to do. It's basically it's like solve a problem for yourself is kind of the core advice there.

**Cat Wu** (01:09:46):
Exactly. I would also push listeners towards focusing on bringing your automations from, okay, this is a cool concept to like, hey, this actually works 100% of the time. Sometimes I see users trying to automate something, getting it to 90, 95% accuracy and then giving up on it, and if an automation doesn't work 100% of the time, it's not really an automation, and that last five to 10% does take more time. Also, building the automation is often a lot slower than you doing it yourself. I would encourage listeners to put in that time to scope some automation that you really want to get to 100%, put in the elbow grease to teach Claude your preferences, to give it feedback so that it can improve its skill so that it can get to that 100%, and then really then you'll be able to rely on it. There's just not much value in a 95% there automation.

**Lenny Rachitsky** (01:10:48):
I am super guilty of that. This is really good advice for me.

**Cat Wu** (01:10:49):
I am guilty of this too. I've been teaching Cowork to try to get me to inbox zero for Gmail, and it has been very time-consuming and it is definitely not there as you probably realize.

**Lenny Rachitsky** (01:11:02):
Yeah. Funny enough, that's exactly where my mind goes. I have this workflow I set up where every email I get, it looks for things that are spammy, which is just all these like, "Hey, can I come on your podcast?" Or, "What about this?" All these things, I'm just like, "I don't have time for these sorts of things," and I have it categorized it into a folder called Spammy and it's just like, it's 95% great, but then there's like, oh, wow, I missed an email because it went in there. So this is a good push for me to like, I'm going to work on this. I'm going to get it to perfect.

**Cat Wu** (01:11:28):
Yeah. We also are working on making the flow for customizing these commands a lot easier because right now I think you have to know too many concepts. You have to know to define a skill, you have to know to use this skill and give it feedback, and then you have to know to tell Cowork to update the skill based on all the feedback that you gave, and then you also have to know where to read the skill to make sure that the feedback was incorporated the way that you want. It's also our job to make this flow really seamless so that it doesn't feel painful to do.

**Lenny Rachitsky** (01:11:57):
Amazing. Is there anything else, Cat, you wanted to share? Anything else you wanted to leave listeners with? Anything you wanted to double down on that we haven't already touched on before we get to our very exciting lightning round?

**Cat Wu** (01:12:08):
I see a lot of people playing around with AI and building prototype apps and tinkering with building workflows. I would really push people towards building apps that you're actually using every single day because I think only through that usage are you actually getting the value. If you build a prototype app that isn't helping you get more done, then the AI isn't really adding value to your day.

**Lenny Rachitsky** (01:12:38):
And there's only so much you learn from that when it's like, okay, I just did one-shotted something, oh, that's cool, and then you never come back to it. You're not learning a lot.

**Cat Wu** (01:12:45):
And you're not getting much leverage from it.

**Lenny Rachitsky** (01:12:47):
And actual leverage. Yeah, that's such a good point.

**Cat Wu** (01:12:49):
I also think there's a lot of people who spend a lot of time customizing their workflow. So I think there's two ends of the spectrum. One is people who never customize or never build automations, but there's this polar opposite end of people who obsess around customizing their tool, adding a ton of skills and MCPs and these workflow improvements, and I think sometimes that can even distract from your core goal of launching some product or building some feature. I think there's a lot of fun in customizing and we definitely want to make our products very hackable so that you can make it work really well for you, but there is a limit to how much it's useful, and I think there's a camp of people who maybe spend so much time customizing that they're not sleeping and not doing the core task that they originally set out to do.

**Lenny Rachitsky** (01:13:41):
I see a lot of that on Twitter. Just like, "Look at my setup. It's out of control. It's so optimized," and what are you actually building? No, but my setup is so awesome. It gets so much done.

**Cat Wu** (01:13:52):
I think the simple setups actually work better.

**Lenny Rachitsky** (01:13:56):
/powerup. Level up a little bit.

**Cat Wu** (01:13:58):
Yeah,

**Lenny Rachitsky** (01:13:58):
Yeah. There's this Karpathy tweet that just came out yesterday where you talked about this divide that's interesting between people that tried ChatGPT, Claude back in the day, it was like, okay, and they're like, "Nah, this is terrible," and they kind of gave up on what AI could do for them and they're just so cynical of like, "No way, it's not actually that big of a deal." And then there's people that are using it to code essentially who see the full intense power of it and how good it is and people on both sides don't understand the other side and how they see the world. And so your advice is really good here to just actually use it for real things and see how good it actually has gotten.

**Cat Wu** (01:14:38):
Yeah. I think the big shift is that the 2024 generation of products were chat-based and the Claude Code generation of products is action-based, and the big aha moment people have is when Claude can just do things on your behalf. It is an amazing feeling to know that the agent is capable of doing so much more than telling you what to do. The agent can actually just do it itself, and when people feel that, I think that's the eye-opening moment.

**Lenny Rachitsky** (01:15:10):
Shout out Chrome Extension, the Claude Code Chrome Extension, which you could just watch it doing stuff and you'd be like, "Fill out this form for me," and I'm like, "All right, here I go."

**Cat Wu** (01:15:18):
Exactly.

**Lenny Rachitsky** (01:15:19):
Okay. Anything else before we get to our very exciting lightning round?

**Cat Wu** (01:15:22):
No, let's do it.

**Lenny Rachitsky** (01:15:25):
Let's do it. Cat, I've got five questions for you. Welcome to the Lightning Round. There's this animation that plays, I have to make sure to say it. Are you ready?

**Cat Wu** (01:15:32):
I'm ready.

**Lenny Rachitsky** (01:15:34):
First question, what are two or three books that you find yourself recommending most to other people?

**Cat Wu** (01:15:38):
I really like How Asia Works. It's a story about economic development and what are the policies and governments that make long-lasting successful economies. The other books that I'm really into are The Technology Trap. So this is actually about the past few technology revolutions, so the Industrial Revolution and the Computer Revolution and how this has affected workers. The reason that I really like this is because I think there's a lot we can learn from history to make sure that this transition goes well. And maybe on a fun note, I really like Paper Menagerie. It's just a book of short stories about coming of age and AI and just self-discovery.

**Lenny Rachitsky** (01:16:30):
Favorite recent movie or TV show you have really enjoyed?

**Cat Wu** (01:16:34):
I really like Drive to Survive. There's no deeper meaning to it. There's just something very satisfying about people being so obsessed with a singular engineering goal and just the purity of the pursuit. And I also really love Free Solo, which is about Alex Honnold climbing El Capitan without a harness, and I think similarly, it's just such a pure achievement to be able to climb this extremely challenging, dangerous route and to be able to have the mental focus to do it knowing that if you make a single mistake, you die.

**Lenny Rachitsky** (01:17:17):
It's insane. Yeah, that movie's out of control. And it's interesting how these relate in some way to the work you do.

**Cat Wu** (01:17:22):
I actually am a rock climber, but I first watched Free Solo before I climbed rocks. And so I thought it was impressive, but I didn't understand how impressive it was. It's one of the rare movies where the more you know about it, the more you're blown away by how insane this is. The kinds of moves doing on the wall are things that I don't think I will ever be able to do in my lifetime if it were set in a gym one feet off the ground.

**Lenny Rachitsky** (01:17:47):
With a rope.

**Cat Wu** (01:17:48):
With a rope.

**Lenny Rachitsky** (01:17:50):
Did you see the documentary in that other guy, the younger one that went on ice mountains?

**Cat Wu** (01:17:54):
I did. That one was very sad.

**Lenny Rachitsky** (01:17:56):
But that was wild. Okay, favorite product you've recently discovered that you really love.

**Cat Wu** (01:18:01):
The product that has most changed my life outside of Claude products is probably Waymo. I'm a diehard Waymo user, use it twice a day, get to and from work. So the two things that I really like about it are, one, I don't feel bad if a Waymo is waiting for me, and so I feel less pressure to be right at the curbside the moment it arrives, and the second thing is I feel like it lets me be a bit more productive. When I'm in the car with another human, I typically try not to do any work calls. I feel a little rude if I'm on my laptop the whole time. But one thing I really appreciate about the Waymo is I can call into a work call. I'm not worried about someone overhearing me. I'm not worried about, "Hey, is this rude? Am I talking too loud? Do I need to ask someone to change the music?" And so I feel like this has given me back 30 minutes every day.

**Lenny Rachitsky** (01:18:55):
All these second order effects of technology, it's so interesting.

**Cat Wu** (01:18:59):
Yeah. I always saw Waymo needed to be priced lower than Uber and Lyft to succeed, but actually I'm very happy to pay a 2X premium for it.

**Lenny Rachitsky** (01:19:07):
I love Waymo. It's just like once you see it, you're just like, "This is insane." And then you get used to it. You get in there, you're like, "This is crazy," and then you forget about it.

**Cat Wu** (01:19:18):
Totally. And I think it's also changed the vernacular. A lot of people at Anthropic love Waymo, and I think in the past you'd be like, "Hey, let's call our rideshare app," and now everyone's just like, "Okay, is Waymo here?"

**Lenny Rachitsky** (01:19:30):
Okay, two more questions. Do you have a favorite life motto that you often come back to in work or in life?

**Cat Wu** (01:19:35):
Just do things.

**Lenny Rachitsky** (01:19:36):
That tracks. That tracks.

**Cat Wu** (01:19:38):
I think there's a lot of value in first principles thinking, and if you know what you're optimizing for and you have strong first principles, then you can normally deduce what the right course of action is and be able to clearly articulate that to all the stakeholders, and then you should just do it. I think jobs are fake. If you understand the constraints, you can figure out what you can do and then just try to do it quickly, learn from the mistakes and apologize or fix them if you did something wrong.

**Lenny Rachitsky** (01:20:08):
You could just do things, whoever said that.

**Cat Wu** (01:20:10):
I think it's liberating actually to tell people this. I think in a lot of companies, roles are very strictly defined like, okay, this is what the PM does, is what the designer does, this is what an engineer does, and then even team scopes are very rigidly defined. So hey, this corner of the code base we touch and this corner, we're not allowed to touch, and I think what just do things lets people do is they feel empowered to make these decisions, empowered to operate across team boundaries just to get something done.

**Lenny Rachitsky** (01:20:38):
That feels like a big important skill to be good at. People call it agency, just do the things they need to do.

**Cat Wu** (01:20:45):
Bias towards action.

**Lenny Rachitsky** (01:20:46):
Bias towards action, all these ways of describing just don't wait for permission.

**Cat Wu** (01:20:50):
Yeah. I think this is my favorite reason to work at a startup at some point in your life because one thing that was very life-changing for me was actually working at scale when we were 20 people, and so there was just no process and we had really big problems that we needed to solve. And I really appreciate Alex and the rest of the team for empowering me and the rest of the team to just figure things out without any boundaries for what sales supposed to do, what ops supposed to do, what engineer is supposed to do. Just like you have all the tools at your disposal, you have some ambitious hairy problem statement and you can do whatever you need to get to a good solution.

**Lenny Rachitsky** (01:21:28):
You almost need that experience to build that skill to feel comfortable doing that because a lot of people, they go through school or in college and all these do the thing we tell you to do and then you will get a good grade, and you have to kind of unlearn that of like, okay, I'm just going to do the thing that needs to be done, and even if people think it's dumb, I think it's the right thing to do.

**Cat Wu** (01:21:46):
Yeah, exactly.

**Lenny Rachitsky** (01:21:47):
Okay. I actually have two more quick questions, two more final questions. One is when Claude thinks there's all these, I don't know if you call them verbs, what's the term for these things?

**Cat Wu** (01:21:56):
Thinking words.

**Lenny Rachitsky** (01:21:57):
Thinking words. And interestingly, these all leaked in the source code. Do you have a favorite thinking word?

**Cat Wu** (01:22:03):
I really like manifesting. It's also like the sticker that I have on my laptop. It's my favorite.

**Lenny Rachitsky** (01:22:10):
Clearly the winner. Okay. Final question. Asked Forest this too, with AGI potentially arriving in our lifetime, when you don't potentially have to work, what are you going to do? What are you going to do with all your time?

**Cat Wu** (01:22:23):
I think it will take a long time for AGI to diffuse across society. So I think the immediate thing is actually just helping bring the world along. I think my non-serious answer for it after this happens is I'll probably just do a lot of rock climbing. I'll probably just live in some... I'll probably move to Fontainebleau and just live amongst 10,000 boulders and climb for a bit. There's also so many books I want to read that... My goal is to be able to read one or two books a week, and I'm currently at probably 0.5. The backlog is pretty big. I think there's just so much we can learn from history and so much that I don't understand as well as I would love to. I don't know anything about physics or robotics or any hardware or aerospace or... There's just so many interesting topics. So I'm excited to learn, even knowing that the AGI will already know it.

**Lenny Rachitsky** (01:23:26):
Cat, this was amazing. You're awesome. Two follow-up questions. Where can folks find you online if they want to reach out and just follow what you're up to, and how can listeners be useful to you?

**Cat Wu** (01:23:35):
The best way to reach out is I am _catwu on Twitter. Feel free to tag me in things. Feel free to DM me. I read all my DMs. I don't always respond to every single one, but I will read them all. And then the thing that is most helpful is tell us where Claude Code and Cowork aren't working well for you. We are very grateful for the amount of positive feedback, but the thing that we thrive on is edge cases, errors, like specific tasks that we can reproduce where Claude Code or Cowork fail, because if you're able to share that with us and we're able to reproduce it, then this is something that we're able to actively improve for our next generations of models and for our next harnesses.

**Lenny Rachitsky** (01:24:25):
Extremely cool. Everyone on... People on Twitter are not shy with sharing this feedback, so keep it going.

**Cat Wu** (01:24:30):
Yes, please share the problems that you're having with us.

**Lenny Rachitsky** (01:24:34):
Yeah, and it's really cool to see all your team being so active on Twitter and responding to people. And so what I'm hearing, this is actually stuff you guys actually see and react to.

**Cat Wu** (01:24:44):
Yeah. We appreciate everyone being so engaged with us. It gives a team a ton of energy. We have this channel of user love, and so whenever you guys share a success story, we post it there and whenever you guys share issues with our product, we put it into our feedback channel, that way our broader team is able to act on it.

**Lenny Rachitsky** (01:25:02):
That is so cool to know. Thanks for sharing that. Well, Cat, thank you so much for being here.

**Cat Wu** (01:25:08):
Thanks for having me.

**Lenny Rachitsky** (01:25:09):
Bye, everyone.

**Lenny Rachitsky** (01:25:11):
Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
