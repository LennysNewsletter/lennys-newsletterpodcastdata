---
title: "Why companies are becoming a series of loops | Anish Acharya (a16z)"
date: "2026-09-06"
type: "podcast"
guest: "Anish Acharya"
post_url: "https://www.lennysnewsletter.com/p/why-companies-are-becoming-a-series"
description: "Why companies are becoming a series of loops, covering AI product work, product design, and engineering tradeoffs."
word_count: 16574
---

**Lenny Rachitsky** (00:00:00):
There's a lot of fear and worry about the future with AI. I want to talk about this idea that if you fall behind, you're going to become part of this permanent underclass.

**Anish Acharya** (00:00:09):
It's a funny dark fantasy that we seem to have as Silicon Valley collectively. Things have never been better by almost every measure. This is a technology that really amplifies our agency, it kind of unbundles skill from desire. Not only can we dramatically drive productivity, we can dramatically drive ambition.

**Lenny Rachitsky** (00:00:25):
Can you get too ambitious? Is there a limit?

**Anish Acharya** (00:00:27):
In the old days, three years ago, we would see a company, and if what they were trying to do was too ambitious we would not engage. Today, we're almost seeing the opposite problem. An idea that's too small is not something that we want to engage with.

**Lenny Rachitsky** (00:00:39):
Do you have this interesting take that company building more and more is going to become this kind of series of creating loops?

**Anish Acharya** (00:00:45):
We're going to see this sort of cascading set of everything from a loop per person to loops that can run large parts of the company. With that said, I think humans are a critical ingredient. The loop will help you climb to the local maxima, but then it plateaus. You need human intuition, you need somebody to actually help you land at the base of the next hill.

**Lenny Rachitsky** (00:01:03):
We have this take that the big opportunity is this idea of, "Loop, make me happier."

**Anish Acharya** (00:01:07):
We believe that people want to be more productive, but they don't. I think more people want to spend time than save time. So, I think that the opportunity for this technology is the basics of consumer need. How do we feel more connected, more loved? How do we make progress? How do we have fun? I don't think it's a model or a capability challenge, it's just a product design challenge.

**Lenny Rachitsky** (00:01:29):
Today, my guest is Anish Acharya. Anish is general partner at a16z, where he focuses on consumer investing. He is one of the most insightful, thought-provoking, mind-expanding, in-the-weeds product investors I've met. He's been at a16z for over seven years now, and unlike a lot of VCs, and why I loved having Anish on the podcast is that he is a longtime product builder and founder. He founded a company called SocialDeck, which he sold to Google, and then ended up leading a number of efforts within Google. Then he started a new company called Snowball, which he then again sold, this time to Credit Karma, where he moved to VP of product and then GM of the broader consumer product and the whole entire credit card business. This conversation will get your mind buzzing. Before we get into it, don't forget to check out lennysproductpass.com for a free year of the hottest and most beautifully crafted AI products in the world available exclusively to Lenny's newsletter subscribers.

**Anish Acharya** (00:02:33):
Thank you, Lenny. I'm so excited to be here, thrilled.

**Lenny Rachitsky** (00:02:36):
I want to start with a very light topic. I want to talk about this meme of the permanent underclass. It's kind of this joke that people half joke about, this idea that if you fall behind and aren't just on top of all the latest AI tools, aren't becoming the most productive person ever, you're going to become part of this permanent underclass and fall behind and have a really hard time. And some people joke about it, I think a lot of people take this really seriously and stresses a lot of people out. How real of a concern do you think this really is? How seriously do you think people should take this?

**Anish Acharya** (00:03:09):
Not very seriously, and it's a funny dark fantasy that we seem to have as Silicon Valley collectively. Things have never been better, really by almost every measure, by how distributed all the opportunities are, by the kind of technology we have access to, to the types of ambition we're allowed to have, and to the number of companies that are independently working on things that are winning. And yet there's this sort of discussion of permanent underclass, being outside of the light cone, I've heard it. And it's not just something for deep insiders or outsiders, it feels like there's a real fear from researchers at foundation model labs all the way through to the Silicon Valley layman. I mean, here's a couple of points that I think are really important. So first, I think the last era of tech was a lot more centralized. If you look at network effects, that's sort of the gold standard.

**Anish Acharya** (00:03:58):
You worked on a network effects product, that's the gold standard of businesses from the mobile era, and those things led to dramatic centralization. Of course, all of them are definitionally sort of N-of-1 networks. If you look at what's happening now, it's like every part of the stack there's not even two relevant players, there's 20. You've got labs, you've got open weight, you've got different variations within both. If you look at coding agents, we were talking about it, your mental model for two years ago should have been, would've been, I think it should be winner take all, and yet Claude Code, Codex, Lovable, Replit, Wabi, they're all sort of working. 

**Anish Acharya** (00:04:35):
So it's really, really encouraging to see that. The second thing, you've heard all the kind of economic data, everything from radiologists who are supposed to be cooked every year for I think about 20 years now. And of course, job postings are higher than they've ever been, as well as programmers. So, I don't know that the empirical data bears it out. I think the final thing is that there's this sort of discussion about RSI, and I know RSI is like recursive self-improvement is a fun term to throw around, but if you ask the most sophisticated individuals at the labs, it's not actually RSI that's occurring, which could lead to some sort of runaway winner because they were an epsilon ahead of the others. It's auto catalytic effects, which just means you're using the technology to improve your process, but it's not truly recursive. So, I think everything from the most empirical to the most technical view points in the other direction, and yet we can't seem to let go of this fantasy.

**Lenny Rachitsky** (00:05:26):
Something I've been thinking about recently, even seeing these crazy stories about OpenAI's models hacking Hugging Face, all these stories to me feels like there's always been this question of are we on the fast takeoff or the slow takeoff scenario? And it feels very much so that we are on the slow takeoff scenario, because every one of these milestones it's like, "Holy shit, it hacked ..." We had no idea it was doing this, but we're catching it, we're watching it, we're observing it, we're iterating, evolving. There's always this fear, "Okay, but tomorrow it's going to take off." What I'm hearing from you is that's probably not the case, which I think is the source of a lot of people's fears, this idea that all of a sudden it's going to become super, super intelligent and then we're in big trouble.

**Anish Acharya** (00:06:05):
That's right. The line of reasoning for that case is always everything up until now, then something happens that no one can quite articulate and then fast take off. So, I don't believe that that's going to happen. I do think that model progress is happening faster than ever before, but if you look at something like economic diffusion, I grew up in a small town, I went back home last summer, people's lives haven't changed that much. So if nothing else, the sort of slow rate of economic diffusion will catch it. I think the other thing that's under discussed, Lenny, is how many problems are truly intelligence bound? If you had a data center of PhDs working at FedEx or Domino's Pizza, are they going to be exponentially dominating supply chain and pizzas? I don't think so. So, I think we might be overestimating how many problems are intelligence bound versus bound by other things.

**Lenny Rachitsky** (00:06:54):
**Anish Acharya** (00:08:24):
I mean, I have so many thoughts on this. I don't think we give the average employee enough credit. I think we have this abstraction of a white collar employee. The white collar manager, the abstraction is like some Dilbert-esque manager who's just shuffling paper all day long. We have this abstraction of consumers that they're sort of these low agency NPCs. Of course, that would never apply to us or our friends. We have this abstraction that everybody else's job is super automatable by AI, but of course ours is not. So, I think when you actually get into the details, a lot of people are actually excited to better themselves, get more leverage. And you see this with, of course, sophisticated companies like Google, but even a company like Kavak where they sell used cars in Mexico, they've got this concept of a Jedi academy where they're teaching everybody at the company, including the mechanics, how to use the new tools and technologies and at the end of the six-week course they ship a cutting edge in-production agent. 

**Anish Acharya** (00:09:17):
So, I actually think that more people are embracing the technology than we sort of like to discuss. I think a big change is going to be using AI versus reorganizing your entire company around AI. And a great example of this is if you look at the diffusion of electricity as a technology, it took 40 years for us to get from the inception of electricity to reorganizing factories. And that means burning the buildings down and starting from scratch versus taking what was previously coal and simply swapping it with electricity. So, I do think that the most ambitious companies are rethinking everything around the models, and those that are a little less ambitious or perhaps a little earlier are thinking more about how do we give people in existing orgs, existing job functions, access to the technology.

**Lenny Rachitsky** (00:10:01):
So, kind of a theme I'm hearing so far is we can be a little less stressed about where things are going and the future of your job, your careers.

**Anish Acharya** (00:10:10):
I think so, man. I mean, I think if you even just think of the kind of incentives for the CEO and executives, Sundar running Google, he doesn't want to run a more efficient $4 trillion company, he wants to build a $40 trillion company. So anytime you have an economically productive unit, it's rational to, especially if it gets more productive, to maintain that sort of presence in your organization. And then, I don't know what you hear, but anecdotally, I talked to a good friend who's an executive at Google and I said, "Hey, have you laid anyone off?" And he said, "No, we didn't. What we instead do is now rip through our roadmap." So, two years of roadmap happens in three months, and we're actually our hardest problem is knowing what to add to the roadmap, which by the way is every PM's fantasy. How much emotion has been drained on prioritization conversations between you and I?

**Anish Acharya** (00:10:55):
So yeah, I actually think that people shouldn't be as stressed and I think they should feel really empowered. And by the way, the best way to do it is just to ship stuff. I mean, Claire is my muse. She's so awesome because she's-

**Lenny Rachitsky** (00:11:07):
Claire Vo?

**Anish Acharya** (00:11:07):
... always shipping. Yes, Claire Vo, she's shipping, she's trying things, she is not afraid to be a little embarrassed by it. And if you just see her whole kind of affect, she feels like the best version of herself that she's ever been and I think we all have an opportunity to be that.

**Lenny Rachitsky** (00:11:23):
I love that. I want to be Claire Vo when I grew up.

**Anish Acharya** (00:11:25):
Totally.

**Lenny Rachitsky** (00:11:26):
Kind of along those lines, you have this interesting take that company building more and more is going to become this kind of series of creating loops and creating series of loops. Talk about that.

**Anish Acharya** (00:11:36):
Yeah, yeah. Well, I think the broad concept and the loops concept kind of gets teased a little on X because at sometimes it feels like maybe we're big braining it. I know there was a big meme around graphs, like the next stage of loops is graphs, but let me make the kind of steel man for it, which is we had prompts and then we invented agents. Agents of course are just models in a loop with tools and memory and skill files. And then we had sort of loops, which are sets of agents that are doing tasks. If you look at a lot of work in coding, coding is such a great domain because you have the best models and you have the most sort of technically apt customer, plus you have these established loops, like bug fix, or a bug report comes in, repro gets generated, bug fix gets created, bug fix gets reviewed.

**Anish Acharya** (00:12:24):
If high risk, then humans should confirm that it's okay to ship to prod. And if low risk, it just gets shipped. And maybe you even email the customer and say, "Hey, we fixed the bug you reported." That happens in five minutes. There are many loops like that in engineering, everything from bug fixes to customer feedback, to sales demos, to new feature development. So, coding sets itself up well. So, you have a coding loop and the kind of change it makes is to the code base. My question is what are the business loops? So if you're the GM of a business, you're looking across many job functions and you've got loops running in coding, and marketing, and sales, and support, and legal, the output of all of those loops is something that is itself a loop that you should be able to optimize for.

**Anish Acharya** (00:13:07):
And I think the strong form of this is that it sends a message to the CEO saying, "Hey, we need to actually make a change to one of the physical aspects of the business, or to our business model, or to our strategy." So, I think we're going to see this sort of cascading set of everything from a loop per person, loop per job function, loop across entire business units to loops that can run large parts of the company. With that said, I think humans are a critical ingredient. I just don't think that most work in the organization can be done fully autonomously. When you think of what a human will do in this AI native company, sales, support, strategy and exceptions.

**Anish Acharya** (00:13:45):
And all those things are super critical. We've seen one thing, Lenny, it's that the ability for models to do new thinking out of distribution thinking is still really limited. And I don't actually take the point that some of the new thinking in math is actually representative of new thinking in domains like business. So, you're still going to need a person to say, "Hey, here's the thing I think we should make," and have them be right about it.

**Lenny Rachitsky** (00:14:05):
Let me just kind of make sure this point is really clear, because it's so interesting. What you're saying here is engineering and building more and more is becoming this loop of input, feedback, support ticket, whatever, input of just what to build. And then AI more and more is taking that, deciding, "Here's a PR. Here, is this ready?" And then shipping it. And you're saying that you expect that to spread to say go to market, legal, growth, support. So, maybe describe what that loop looks like or may look like within a company.

**Anish Acharya** (00:14:38):
I mean, a great example is a growth team. You worked on the growth team at Airbnb, right? 

**Lenny Rachitsky** (00:14:41):
Yeah, yeah.

**Anish Acharya** (00:14:41):
Supply growth.

**Lenny Rachitsky** (00:14:42):
Yeah, that's right. 

**Anish Acharya** (00:14:42):
Awesome. 

**Lenny Rachitsky** (00:14:42):
That's right. 

**Anish Acharya** (00:14:45):
I don't know how you ran your team, but I'm guessing it was something like you got everyone together, you built a list of possible experiments, you prioritized them, you built them, you ship them, you measure them-

**Lenny Rachitsky** (00:14:53):
Brainstorming. Yeah. A lot of brainstorming-

**Anish Acharya** (00:14:54):
Correct, right?

**Lenny Rachitsky** (00:14:55):
... a lot of spreadsheets.

**Anish Acharya** (00:14:56):
So, the loop version of that should be that every variant gets generated, every variant gets measured. Once you get to stat sig with a high enough P-value, you converge and ship that variant. You then have a long-term holdout and you start working on the next experiment. And then you're going to hit some local maxima, and I think this is really important. The loop will help you climb to the local maxima, but then it plateaus and you need some sort of out of distribution thinking, you need human intuition, you need somebody to actually help you land at the base of the next hill.

**Lenny Rachitsky** (00:15:26):
Yeah, you have this chart. I don't know, maybe we'll show it over later as we talk about this, which is such an interesting way of thinking about it. This idea that agents will help you hill climb and reach some new plateau, and then you need a human there to think about a bigger idea, kind of unlock it, and then it keeps going and going and there's kind of this agent to human kind of back and forth.

**Anish Acharya** (00:15:47):
Yes. Yeah. And you know what really illustrates that? If you've ever tried to have an agent come up with a business idea for you, like, "Hey Claude, make me a million dollars, make no mistakes," why doesn't that work? And it's because you sort of need to set it in the right direction, and nothing in the technology has shown us that that is not needed.

**Lenny Rachitsky** (00:16:06):
Yeah, it's interesting. I've been hearing more and more. I just saw a tweet that I think at OpenAI, the go-to-market team now is using Codex more. More of the go-to-market team is using Codex more often than even the engineering team.

**Anish Acharya** (00:16:19):
Yes. And think of how happy that makes them. What does the go-to-market team want to do? I mean, this is a caricature but I'm going to stand behind it, which is they want to hit the gym, they want to go to steak dinners, and they want to raise the trophy up for being salesperson of the quarter or of the year. So, I actually think that this is a distillation of their job into the thing that they're the best in the world at, that they're the most interested in, and all the administration that goes around doing that core work is now handled for them. So, that's where go-to-market is going, and it's going to be awesome.

**Lenny Rachitsky** (00:16:51):
This reminds me of a PM friend who had this really funny take that as a PM, you're constantly having to say no to all these ideas that are coming at you and you have to like, "I'll put it on the roadmap, we'll prioritize it." He's like, "Okay, I'm going to flip this. I'm going to say yes to everything. I'm going to build everything and then simulate every idea with Simile," or all these products that are launching where you could simulate how a user will react, and then that'll tell you, "Should we build this?" What a hilarious way to rethink PM.

**Anish Acharya** (00:17:21):
And you know what's so beautiful about that? Actually, there's two things, and I'll tell you maybe the one that's less obvious to me, which is I feel like every PM at every company feels like they're a true zero to one thinker, but they're held back by the heavy hand of management, and executives, and founders, and engineering capacity. And in a world where every story gets told, every product story gets told, every feature gets tried, I think a lot of PMs are going to realize they're actually not that good at zero to one and it's much more fulfilling to work on someone else's good idea than your own bad idea. So, I think even things like that are going to lead to a lot more organizational health than we've had in the past. Not to mention the fact that the idea that ends up winning doesn't have to be the one that's came up with by the person who can sell it best to an executive. It just gets tried, and the best idea wins.

**Lenny Rachitsky** (00:18:09):
So coming back to this loops idea, the way I'm thinking about it is how can every function start to think of their function as setting up an agent to be able to just go from input to some kind of impact? And what this makes me think about is something actually Claire tweeted recently, this point that people always used to joke that soft skills are the least valuable and engineering skills the most important valuable because they're so concrete, and turns out that's what AI is the best at, the things that are verifiable and you know what success looks like. And so, the question I think about now is just which skills can you not just turn into a loop because the output is so hard to verify?

**Anish Acharya** (00:18:50):
Yeah, I think that's right, and I think that those are going to be the rate limiting factors because you can only do one steak dinner a night. I guess you could do a steak lunch, but to some extent there's going to be these rate limiting factors in every system. I think a useful way to think about it is anytime the model's making a mistake or doing something you wouldn't do, what do you know that it doesn't know? And there's a really interesting example I heard from Ale at Kavak. He's probably the most sophisticated thinker on this stuff that I get to hang out with, where he said anytime their agent, they have an agent per customer, they sell used cars online, and when the agent gets stuck it actually calls a human, and the human will coach the agent through. Now, the magic of that is not only does it unblock the agent, but of course the agent then captures all the traces and learns from it. That's a really interesting mental model.

**Anish Acharya** (00:19:36):
It's either a knowledge gap or a data gap that you have to give the agent, and the next time it shouldn't have to call you.

**Lenny Rachitsky** (00:19:42):
I love that example. Basically, the takeaway here is you need to start thinking about every function as an agent loop, and the job is to figure out where it gets blocked, where it goes wrong, and give it more context, more insight, more direction, basically.

**Anish Acharya** (00:19:58):
That's right. Yeah, that's right. And then hopefully a lot of your day-to-day work, when you come up with a new idea that works, the kind of implications of that idea, if it's a product, there's marketing work, there's sales work, there's product marketing, there's communication, there's legal, all of that should be largely handled for you. And your job is to go take a hike and dream the dreams and come up with the next hill to climb.

**Lenny Rachitsky** (00:20:20):
And this begs the question a bit of just what will separate the companies that win in this world where AI is kind of doing a lot of this? I imagine part of the answer is the human in this local maxima coming in with a better idea. Is there anything else that you think becomes a differentiator in this world where AI is doing so much of the work that humans are currently doing?

**Anish Acharya** (00:20:39):
I mean, I think one thing that's under discussed is that it's unclear that the sort of competitive equilibria that exists in a lot of industries will really change. So, let's say Pizza Hut, and Domino's, and Papa John's, and Roundtable all get a data center of PhDs, and they're all going to either adopt it or have a CEO change and adopt it. So, it'll be a rocky period and there'll be some relative shuffling, but I think that they're all going to embrace the new technology because most companies do. I don't know that one of them is going to have 99% of the market. So, I think what's under discussed is that yes, in the near term I think there'll be winners and losers based on adoption of the technology and how ambitiously you adopt it. But I do think there's a lot of industries that will sort of maintain their current competitive dynamics because they're not intelligence bound.

**Anish Acharya** (00:21:29):
I think the most useful question to ask yourself as a founder CEO is just, "Hey, if we assume these things are infinitely intelligent and astonishingly cheap, how would we reorganize the company?" Because that's where we're going?

**Lenny Rachitsky** (00:21:42):
Kind of along those lines, you have this interesting take about this kind of split that might be coming within companies between these generalists and specialists, and how AI plays into that. Talk about that.

**Anish Acharya** (00:21:52):
Yeah. Well, I think that there's so many interesting things that this touches on. One is the question of open weight versus frontier. So I'm sure, are you familiar with Pareto efficiency? I'm sure you are.

**Lenny Rachitsky** (00:22:03):
Please explain.

**Anish Acharya** (00:22:04):
Yeah, so Pareto efficiency is just for price performance, for example, the efficient frontier is what's considered the optimal trade-off of a unit of performance for a unit of price. And if you're along that curve, you're always paying the rational amount for the performance. And what's interesting is that frontier models are actually irrationally priced in that, first of all, Mythos is infinite dollars a token, you can't use it. But if you look at even something like Fable 5, for one IQ, conceptually one IQ of extra intelligence you're paying 100X more than Opus 4.8. So it's not rational, but I think there's a lot of jobs in which you have unbounded upside, like drug discovery. And if that one IQ point lets you discover the next statin, it's a trillion dollar outcome. So, it's sort of rational to pay for the highest intelligence in these types of jobs and industries.

**Anish Acharya** (00:23:01):
Now on the other hand, I'm going to pick on maybe legal. There's perhaps only so much upside to be had in legal or finance. And for those jobs, you actually do want to be very Pareto efficient and probably pay for good performance at a good price, not infinitely priced, infinite potential upside performance. So, I think what we're going to see is a split between job functions that demand kind of mid-IQ intelligence, and those will often be open weight, sort of biased with reinforcement learning, things that make the models even cheaper, more performant for a narrow job, along with incredibly "expensive but performant" frontier tokens for sales, support, research, engineering. So, I think you're going to end up having both architectures, and we can touch on this in a little bit but I do think there are these sort of comparative advantages amongst model families, and then also amongst, of course, individual models that we're seeing more and more of. It's not going to be one or the other.

**Lenny Rachitsky** (00:24:01):
Such an interesting insight. So, just to make sure I understand what you're describing here, you're thinking there's going to be this split between within an org of function and model, where specific functions that have a lot more upside and potential leverage go for the frontier models, and you described these kind of product sales, engineering research roles. And then, for other functions you don't need Mythos, you don't need Astra, I think is that the latest one that's coming?

**Anish Acharya** (00:24:29):
Yes, Astra. Yeah, yeah.

**Lenny Rachitsky** (00:24:30):
And so it's both, you're saying the AI doesn't need to be the frontier model and the people don't have to be the smartest people in the world to do really well in that world.

**Anish Acharya** (00:24:37):
Yeah, and I don't want to be diminutive. There's extraordinary people in those job functions. I just think that they're bounded upside problems that they work on. You can only kind of close the books correctly, you can't close the books 100X better. So yeah, that's exactly what I'm saying.

**Lenny Rachitsky** (00:24:53):
I wonder if it's connected back to that discussion we had earlier about it's verifiable. If it's a lot more verifiable, you don't need the frontier model versus, I don't know, the potential upside.

**Anish Acharya** (00:25:04):
I'm not sure. I mean, I think for a ... Verifiability is a good question because I think for a drug development company, you have infinite upside, it is verifiable, but closing the books is also a verifiable problem, which has limited upside. I think the question is really how much upside is there and how hard is it to calculate it? Here's a nuance. Customer support, a customer may call in and report a bug. That bug may actually be the first breadcrumb to a thing that changes our entire organization. And if the CEO was on that call or the smartest person, they could follow the trail. But if we actually have this "mid-IQ generalist," then not, that actually makes the case for as a basket of problems always use frontier intelligence. And I can of course make the case for the mid-IQ basket as well, which is simply that we've crossed an intelligence threshold for almost every economically useful problem, and anything beyond that threshold is simply waste.

**Lenny Rachitsky** (00:25:57):
Yeah. And I think the point people forget is that the models that are not the frontier models, that was what the frontier was, I don't know, six months ago, and we were so impressed and we loved it. It was like, "Holy shit, it can do all this." And now just because there's something better, we don't give those models as much credit.

**Anish Acharya** (00:26:12):
You're right, because it's sort of like, "This thing is so crazy. This is AGI." And then, a day later it's like the old thing that you throw in the dustbin.

**Lenny Rachitsky** (00:26:22):
So along those lines, I hear people jokingly call you a model sommelier. Tell us with your sommelier credentials, what's the current state of the model art? What is each model great at? What are model's terrible at?

**Anish Acharya** (00:26:38):
Yes. Well, as you know, the secret of every sommelier is 10,000 hours or maybe 10,000 bottles. So, I think that the secret of being a model sommelier is just using them all. 

**Lenny Rachitsky** (00:26:47):
Drinking them all.

**Anish Acharya** (00:26:48):
I push myself really hard to ship something with every new model that comes out, and I think you learn so much. I think for people who believe the models are commodities or totally fungible, you just haven't actually used the models. And for example, in the last few weeks I've been obsessed with Qwen 3.8-Max. Qwen is an awesome model. It's very good at long horizon tasks, and it's actually really creative. It's a great storyteller. So, I've been using it to create these impossible documentaries, mostly of planets of the Star Wars universe. I did Tataouine, which turned out great. I did Bespin last night, and it can just work for four or five hours.

**Anish Acharya** (00:27:27):
It tells a great story, it generates all the video using the MiniMax model via Fal, generates audio via Eleven. It actually directs the movie, the five-minute movie, and then it cuts all of the clips in. It overlays it, it watches it. It's just extraordinary. It's got a totally different shape than GLM-5.2. GLM-5.3 just came out, which I used for a bunch of product work. It doesn't have a vision component, and it's sort of like this neurotic PhD you put in the corner, and they both have the role. This is a little bit of these tension of models. It's not that one is ahead of another, one is more intelligent, it's rather one has a mind that's shaped in one direction, perhaps creativity and openness for Qwen, and others that are shaped in other directions like neuroticism and precision like GLM-5.3. So, I just make something with every model and that's how I build my intuition.

**Lenny Rachitsky** (00:28:22):
How important is this habit, do you think, for people? Because I hear a lot that it's really important to be using these models. And a secondary question is how do you come up with what to do with these models? Because a lot of people want to try these things. They're like, "Okay, what do I do?"

**Anish Acharya** (00:28:37):
I know.

**Lenny Rachitsky** (00:28:37):
Any suggestions?

**Anish Acharya** (00:28:38):
Well, I think almost all of us have got ... The most insufferable thing for a long time was your app idea friend. Every time you went to have a beer they're like, "Let me tell you my app idea." You're like, "Oh, here we go again." We have got to be the app idea guys now, and all the silly ideas, actually, especially the silly ideas, because those are the ones that often have the most alpha, are the ones that we should all be building. So, I've probably got two dozen apps that I've built, I've got one or two large apps that I iterate on. And I think that if you don't have a chassis with which to use the models, it's just really hard to come up with an idea from scratch every time. So, I'd say work on something. It's actually better if it's not important with a capital I, and then keep finding new ways to invest in it and add to it with a model as a kind of tool rather than as a goal. Does that make sense?

**Lenny Rachitsky** (00:29:27):
Yeah. Maybe even zooming out, I've been thinking more and more one of the most important habits to build right now is to, whenever you're about to do something, ask yourself, "How can AI do this for me?"

**Anish Acharya** (00:29:38):
Totally.

**Lenny Rachitsky** (00:29:38):
I'm visualizing this input to response, the whole idea of there's a space between input and response, and meditation helps you think more deeply before you respond. And I feel like the trick now is insert in that moment, "How can AI help me with this?"

**Anish Acharya** (00:29:53):
I mean, I'm also a longtime meditator. We should talk about that if you like, but yeah, I think that's right. I think in our day-to-day knowledge work, sometimes it's less obvious to me. I guess my mind is I've always been a consumer product person, I love products. So for me, it's easier to think of a new feature to add to my DJ streaming app or my Google Reader for X that I use than it is to find a part of my life to automate. But you're right, there's some fun examples. I posted about one a few weeks ago where I had my laptop transcribe everything that was happening in the kitchen, and then it would award or detract screen time from my son's iPad depending on whether he was being good or bad. So, it was a fun little social experiment. It also had a fun outcome, which is that he recorded a video of himself saying, "I love you, Dad," over and over, and put it next to the mic.

**Lenny Rachitsky** (00:30:42):
To hack the metrics?

**Anish Acharya** (00:30:43):
To hack the metrics. So yes, anything becomes a measure it's no longer useful, but it was just a cool little social experiment. I think those things are super fun.

**Lenny Rachitsky** (00:30:54):
That is hilarious. So, one of the measures was how often he said, "I love you," and that was going to give him more free time?

**Anish Acharya** (00:31:00):
Is he saying things that are positive and pro-social-

**Lenny Rachitsky** (00:31:00):
That is so funny. 

**Anish Acharya** (00:31:03):
... or negative and antisocial? And saying, "I love you," is very pro-social.

**Lenny Rachitsky** (00:31:07):
That's so funny. I had a friend who built this little device that measured how often he and his kid laugh throughout the day.

**Anish Acharya** (00:31:14):
Oh, that's nice.

**Lenny Rachitsky** (00:31:15):
Yeah. He hacked one of those Limitless pendants to do that, and then they just look at that metric every day.

**Anish Acharya** (00:31:21):
And this is what I mean, man. I think we spent a lot of the time on the show so far really intriguing, talking about productivity, job loss, all these heady, important topics with a capital I, but what you just described, how often you laugh, that's not a startup, that's probably not an economically consequential idea, but it is for the quality of our life. And I think we tend to think that happiness is fixed, but what if it's not? If you and I were doing jobs 100 years ago, what would our jobs be? I promise they'd be less cool than they are right now, and maybe 100 years from now they'll be that much cooler. So, I think that the thing that gets often missed, and this is why I'm a fan of Claire and others, is just how can this thing add texture to our human lives even if they don't have economic consequences?

**Lenny Rachitsky** (00:32:05):
Yeah. Along these lines I saw somewhere you have this really interesting take that the big opportunity, maybe just in consumer, but broadly is this idea of, "Loop, make me happier."

**Anish Acharya** (00:32:16):
Yeah.

**Lenny Rachitsky** (00:32:17):
Talk about that.

**Anish Acharya** (00:32:18):
Oh, yeah. I mean, I think that we believe that people want to be more productive, but they don't. I think more people want to spend time than save time. There's a reason the biggest products in the world are entertainment and social. So, we get at the heart of how do we deliver the value to the consumer? I think for most consumers, sometimes I tease and I say it's like the Instagram AI user versus the X AI user. The X AI user is fearful of being outside of the permanent underclass, is really opinionated on GLM-5.3 versus Kimi K3. They're just so pilled. And then the Instagram person is like, "Oh, this is like a better Google search. Kind of. It's cool." They don't get what all the hype is about. And it's really a product design failure. We have the capabilities to radically transform people's lives.

**Anish Acharya** (00:33:05):
I mean, Lenny, in many ways we spent 40 years building a technology that enables better spreadsheets. We built this technology that extends our intellect, but nothing to extend our soul. And I think that we have a little bit of a spiritual hunger, especially as a lot of these cultural institutions have gone away that fulfilled that, especially in the rest of America where you don't have as many hot yoga classes, and Pilates, and fasting, and Friendsgiving. So, I think that the opportunity for this technology is like, hey, the basics of consumer need, how do we feel more connected, more loved? How do we make progress? How do we have fun? The things that we all aspire to, the basics, how do we apply this technology to those areas? That's what I want to see more of. And again, I don't think it's a model or a capability challenge. It's just a product design challenge.

**Lenny Rachitsky** (00:33:50):
I love this so much. We talked about this idea of, "Loop, grow my business. Loop, find me more sales. Loop, close support tickets." But the way you're describing here, I think you, the way I had it in my notes here, just like, "Loop, improve my health," or, "Loop, make me a better friend." And there's no reason AI can't just think deeply and hard about all those things and figure out a way to actually do this.

**Anish Acharya** (00:34:11):
Yeah. And also, look, we have to dial this in, but I think there's a way that AI can challenge you, can push you, can be disagreeable. This is also why I think startups are advantaged over incumbents. The idea those 1,000 Google committees who would roll in their graves at the idea that they're going to release a model that's disagreeable, or God forbid it should be sexually suggestive, but guess what? Those are all parts of human existence. So, I think exploring the kind of uncomfortable parts of our social existence are things that startups are uniquely set up to do.

**Lenny Rachitsky** (00:34:42):
And I know you spent a lot of time investing in consumer companies. What I'm hearing here is this is a big opportunity for consumer businesses to basically build an app product that is exactly this loop around improve my connections with my friends and family.

**Anish Acharya** (00:34:56):
I think that's right. I think the thing that's held back consumer so far a little bit, and it maybe held back is too strong, because if we put this into iPhone terms, we're in iPhone 2010. What is iPhone 2010? I think it's pre-Airbnb, pre-WhatsApp, pre-Uber, pre all the important consumer companies. So it is early days, but what's held us back is I think three things. One is that the models have been expensive, so if you want to do a kind of free to use product, that hasn't been easy. The second is that we've had an interface problem. Chat makes sense if you're the highest agency person in the world, which is Elon and Sam, but for the average consumer, their ideal interface is TikTok. So, we need to find something between Chat and TikTok. And then the fact that the technology has been so much more focused on productivity than things like human connection and entertainment, I think all those things are kind of up for grabs.

**Anish Acharya** (00:35:50):
The open weight models mean things are way cheaper. I think that we're starting to have conversations about things like, "Loop, make me happier." And I think that founders like Eugenia, who you should have on the show, she's tremendous, are thinking really ambitiously about user interfaces. Brian Chesky from Airbnb, I think he started a foundation lab focused on next gen user interfaces. So, I think all those problems will get solved or they're at least in a better position to be solved than they were two years ago.

**Lenny Rachitsky** (00:36:15):
I want to come back to the whole space of consumer and AI and things like that, but I want to follow this thread a little bit more about just the optimism around where things might go. There's a lot of fear and worry about the future with AI and just generally. Mark Andreessen when he came on the pod had this really interesting take that AI came just in time to save us, because population is declining, productivity's going down, there's all this war, climate change and all these things, and we would be in big trouble if AI wasn't here to fill that gap. Talk about just your bigger picture perspective on why you think maybe people are underestimating the positive and optimism around AI.

**Anish Acharya** (00:36:58):
One, I think it's a potential for it to be a sort of emotional spiritual interface on which we can get leverage and explore aspects of ourselves that have been really buried. If you look at the kind of effect of the industrial revolution, it's that there are these scale advantages which are insurmountable. And as much as obviously I'm very pro-capitalism and I love the economy that we live in, I think that centralization, it sort of discourages the individual in some ways and it maybe detracts from their identity. So, I think one of the really magical things is this is a technology that really amplifies our identity, our agency, it kind of unbundles skill from desire. For example, if you want to make music, you can make music now. You don't have to know how to play the piano. If you want to be a programmer and make software, you can make software now.

**Anish Acharya** (00:37:42):
So it really amplifies our individuality, it allows us to explore aspects of our lives that we were never able to explore before. And just in terms of the nuts and bolts, we have been in this sort of morass of 2% GDP growth. Who said that we have to be there? Why can't we be 10 or 15 or 20%? And this is a technology with which not only can we dramatically drive productivity, we can dramatically drive ambition. Maybe this is a caricature, but the 1950s and 1960s we believed that we could do anything. We were coming out of World War II where the entire economy, the entire world mobilized in a way that we didn't think was possible. And one of my theories, Lenny, is that when the stakes are high we are awesome. When the stakes are low we are at our absolute worst. And in a lot of ways, I think the world we lived in five years ago felt like a low stakes world, which is why we collectively had a lot of these side projects as a society which weren't necessarily productive or making any of us happier.

**Anish Acharya** (00:38:38):
And now you've got, it's not just Elon doing everything he's doing, but I think everybody feels like they're climbing the ambition ladder. You ship your bad ideas so you can discover your good ideas. And if you want to build software, great. If you want to build a bridge, you don't have to be a civil architect to know how to do that anymore. So, I really think that we have the makings of a sort of dramatically happier, more fulfilled, more productive society, and yet we're here talking about permanent underclass.

**Lenny Rachitsky** (00:39:05):
I love all of that, that all feels so right. It's so hard to really believe that. But if you actually look at how things have gone so far with the rise of AI, unemployment's down, people are making a lot of money. Obviously a lot of people are struggling, there's a lot of downsides, data centers causing problems for people, things like that. A lot of issues, but it feels like as an economy and as a country feels like things are going well so far. They just almost cured some kind of cancer the other day.

**Anish Acharya** (00:39:33):
Yeah, you're right. Moderna just did. I mean, the fact that Dario can write a blog post and say, "What happens when we cure every disease?" And then we debate it as a serious topic, what world are we living in here? I also think that we're collectively worried always, these abstractions, the world, the average worker, the middle manager, the person who lives in the vicinity of a data center, these are abstractions, but our actual lives seem like they're getting more fulfilled, we're more capable, we're more empowered. So, I think that's also something that the revealed preferences tend to show how people are experiencing it individually, and the stated preferences tend to show how people are sort of observing it or believe it's playing out societally. If you ask people if they want a data center in their neighborhood, most will say no, but if you ask them if they use ChatGPT today, most people will say yes. So, that's kind of the dissonance.

**Lenny Rachitsky** (00:40:26):
The obvious issue is just the PR around AI has not been great. There's a lot of fearmongering. Thoughts on that, what's going on there? Do you think that'll change?

**Anish Acharya** (00:40:34):
The most important thing that we can do with AI to change the kind of conversation around it is make important things cheap. There's two things that are extraordinarily important in America that have only gotten more expensive, healthcare and education. If you look at healthcare, 45% is administrative. So, if you take a lot of that administrative burden out, you can actually see deflationary healthcare costs, also things like curing every disease. That sounds awesome. GLP-1s, also obviously not an AI thing but I think is a reason to be optimistic about deflationary health costs. And then, education as well. I think education now has the strongest form of competition, sort of traditional education that it's had in 200 years. And I think it's going to be very, very good to kind of unbundle learning from institutions. And also by the way, status from credentials. You don't need a Harvard degree, you just need to get, and that's pretty cool.

**Lenny Rachitsky** (00:41:30):
**Anish Acharya** (00:43:10):
I mean, without commenting on OpenAI specifically, I think that maybe I'm a little skeptical on some of these things where I think the aura that Anthropic got from having a model that was too dangerous to release was extraordinary. And maybe they had a GPU shortage. Now, maybe the capabilities were more advanced than they actually wanted. Maybe they actually wanted to keep that proprietary model internal to extend their own lead. So, I think there's a lot of sort of confounding factors that would cause you to pull back a little bit. Look, I do take the points about offensive cyber seriously, which is we should harden all of our systems before we make them trivial to penetrate. But I think the sort of concept of the model that's too dangerous to release, it kind of conflates marketing, inference capacity, and then also economic considerations like do you want to externalize your competitive advantage or use it to make yourself better?

**Lenny Rachitsky** (00:44:06):
Yeah, I always think about that when I have folks from Anthropic and OpenAI on the podcast, just how an advantage they have when they have the best model-

**Anish Acharya** (00:44:14):
It's crazy. 

**Lenny Rachitsky** (00:44:15):
It's crazy, right? Just that's a loop right there is just have the best model for longer and they can move so much faster.

**Anish Acharya** (00:44:20):
It's crazy though, to take the other side for a moment, it felt like Anthropic was unassailable and now OpenAI's had an amazing six months, and open weights are also ripping. So, despite the sort of scary concept of this supremely intelligent model that's totally proprietary to one company, so far the kind of industry trends haven't played that way at all.

**Lenny Rachitsky** (00:44:41):
Yeah. Grok Bot just came out of nowhere and is now the most amazing AI kind of assistant tool. I'm just hooked on it.

**Anish Acharya** (00:44:48):
Oh, man. I mean, we should talk about the personal agents thing. Actually, the three big products that I love here, Grok Bot's totally nailed it, and also the model underneath it is awesome. They came out of, you're right, out of left field. And that's I know a lot of the good work the Cursor team did. I think ChatGPT Work, it's kind of buried in the UI but it's really, really good. It's one of the best products they've released. And then there's a startup that's really getting some buzz called Instinct, which has made some more aggressive and interesting trade-offs, but all in the same domain.

**Lenny Rachitsky** (00:45:17):
That's amazing. I don't know if it was a strategy for someone tweeting this vague tweet about how awesome it is and everyone's like, "What the hell are you talking about?" That was really effective, because I was like, "How do I get that?"

**Anish Acharya** (00:45:29):
[inaudible 00:45:29]

**Lenny Rachitsky** (00:45:29):
ChatGPT Work, the episode that will come out right before this is the PM in charge of that, Tara.

**Anish Acharya** (00:45:36):
Oh, really?

**Lenny Rachitsky** (00:45:36):
Yeah.

**Anish Acharya** (00:45:37):
Oh man, they did such a good job on it. I don't know how much you use it, but it's really well done.

**Lenny Rachitsky** (00:45:44):
What is better than Cowork there? Is it that it runs in the cloud? Is that the big differentiator?

**Anish Acharya** (00:45:49):
It runs in the cloud, it does a good job of caching browser credentials so it's not as aggressive as Grok or Instinct. And it also, the remote feature, it's got the full duplex voice mode. So, you can actually just call it and it could see all your threads, and you can just talk to it and say, "Hey, what's happening across all my coding agents, across this? Can you change that?" So, just because the full duplex voice is so good, you really feel like you're calling your assistant who knows everything that's happening in your world. Whereas with Grok, it's a sort of one-way transcription. Or with some of the other assistants, it's a text. So, the voice plus the kind of model of it can see all threads is really well done.

**Lenny Rachitsky** (00:46:25):
Awesome, okay. I'm going to come back to this AI assistant consumer stuff, but just something I wanted to close the thread on. I feel like in terms of jobs and the economy as a result of AI, I see it almost as the spectrum of, there's the Dario end of the spectrum of 50% of knowledge work will be disrupted and we're going to have massive unemployment, to the David Sacks spectrum of it's going to be incredible, jobs are going to be fine. So far everything is pointing in a good direction. Clearly you're closer to the Sacks direction. Is there anything else just along the lines that you think might make people feel better about jobs in the future?

**Anish Acharya** (00:47:04):
I mean, I think that the entire trend of human existence has been that our desires grow faster than our ability to fulfill them. If you look at the things that are expectations today, they were unimaginable luxuries 500 years ago, even 50 years ago for things like therapy or things like antibiotics 100 years ago. I mean, didn't matter how rich you were, you simply didn't have access to it. So, I think we're underestimating human ambition, human desire. People are going to be mad that they don't have a vacation home in Mars in 20 years. Really mad, viscerally mad. They'll be seeing it on Insta and be like, "Come on, babe. We got to work harder and make this happen." Every CEO is going to want to build a much bigger company. So, I don't think already it feels like we're living a much larger form of human existence than we could have imagined 100 years ago, and there's no reason that trend won't continue or accelerate.

**Lenny Rachitsky** (00:47:53):
This idea of ambition, I'm glad you brought that word up again, it's something that's coming up a lot on this podcast that not only is AI making it easy to be a lot more ambitious, it's almost making us have to be more ambitious, because everybody else can just do all the easy stuff now. And now what separates us is just how big can you go? Okay, I'm going to make a personal website. Okay, it's cool. It'll be this white, simple background. No, okay, I'm going to make it this 3D game where you have to walk through a world and discover all the things they do. Everything is just getting more epic. Thoughts on just this idea of ambition becoming a bigger, I don't know, skill and habit.

**Anish Acharya** (00:48:27):
A lot of things get conflated, because when you and I say ambition on this pod I think people have a very specific idea of what that ambition is. Ambition to be a founder, ambitious to build a beautiful software product. Those are types of ambition, but there are other types of ambition. Let's talk about creative ambition. When you're five nobody says, "Lenny, you're good at painting but you're bad at drawing." You just have an ambition or a desire to make something and you make it. That's something that's very unique and can now actually be encouraged. Think of very local ambition. So, they have the NHS in the United Kingdom. I think it's a sort of treasured institution that's not working well. Maybe the way AI shows up in their society is making the NHS as good as the iPhone. That's very specific and local to them, or simply the ambition to be more connected to our family, to be more present parents.

**Anish Acharya** (00:49:15):
So, I think ambition doesn't have to be sort of ambition in the narrow economic sense, it can be really anything that we want to do more of, and who doesn't have that in their bones?

**Lenny Rachitsky** (00:49:23):
Yeah, my example is so dumb now that I think about it. It feels like the thing we have to unblock in our brain is like, "Okay, AI, solve cancer." That's where we can start to think now, and it's so unnatural to us, especially as product people that always have to think about the MVP and the constraints. Now we have to think big. Okay, what's the 10X, the 1,000X version of this?

**Anish Acharya** (00:49:46):
Yes. I know, right? In a way, we have to think small because this thing that ... Our whole lives have been built around how precious software and intelligence is, and now it's totally not precious, that probably will be a harder change for you and I.

**Lenny Rachitsky** (00:49:58):
Yeah. So, all these new little habits I think a lot about on the Claude Code team, they have a principle. "You know what's better than me doing it? It's Claude doing it." And that just created this habit in everyone on the team, "How do I have Claude do this thing for me?" And I feel like that's a thing we all have to start to build in our head, and Grok Bot's really good at that. And not an investor, no affiliation, but it's just so simple and good at this stuff.

**Anish Acharya** (00:50:22):
I also think that there's so much learning that happens through doing. It's funny, if you look at the number of people that are talking about vibe coding versus the number of people that are talking about their projects, people are a little embarrassed. I'm a little embarrassed to talk about a lot of my projects because they don't seem important or substantial enough, but so much of it is learning through execution or shipping, or being fulfilled through execution and shipping. I don't think we can underestimate that either.

**Lenny Rachitsky** (00:50:45):
I have a guest post coming together from someone at Google that works on a lot of their lab stuff, and I don't want to give away the goods but just broadly her concept is that building is now the new reading, where you build to learn and infuse and experience, and it's totally okay for most of it to get thrown away because that's still building your muscle.

**Anish Acharya** (00:51:07):
So well said. Yeah, it's building as an activity rather than an outcome, right?

**Lenny Rachitsky** (00:51:13):
Which I think a lot of people feel bad. "I shipped all these things, but no one's using it. I never use it." And I think that the key here is that's actually okay, that's totally fine.

**Anish Acharya** (00:51:21):
Oh, man. And it happens in every other domain. I make a DJ set and three people listen to it, and I listen to it 100 times, and it's very fulfilling. It doesn't matter.

**Lenny Rachitsky** (00:51:31):
We're going to talk about your DJ stuff later.

**Anish Acharya** (00:51:31):
Okay. Okay.

**Lenny Rachitsky** (00:51:35):
Okay, let's come back to consumer stuff. So, you focus on consumer at a16z. What's happening in consumer these days? What's the landscape? What are you excited about?

**Anish Acharya** (00:51:45):
So, I think there's three big areas. We're very early, as we kind of discussed. The labs have done a good job, but there aren't as many sort of independent mass market consumer products. Coding agents are awesome and I think a total lightning bolt. I think it's easy to say most people don't want to make code, but the big change in my thinking is that coding agents are a way to interact with the world generally. And you've seen a lot of this on X, people use Claude Code to edit videos, or Codex to create a game that they play with their kid on an airplane ride. It's sort of this general problem solving tool that consumers can use in very unique ways. And probably the best example company we've invested in is Wabi, where it's sort of a platform for many apps. People can create them, consume them, share them.

**Anish Acharya** (00:52:30):
So, coding agents is one big area I think that's important. Personal agents, we had this incredible moment around OpenClaw, but guess what? OpenClaw is a dev thing. And Hermes, of course, and Moltbook, all of that is now getting distilled into mass market consumer and enterprise agents that people understand, which is what we discussed previously. And then the last is, I'm going to call it entertainment, though that doesn't fully do it justice. I think that it's a lot of creative tools. Suno has done such an amazing job. It's companionship products, all that. That entire area is uncomfortable to talk about so I think it's under discussed, but there's some huge fast-growing products there. So, I think those are the three big areas that we're watching right now.

**Lenny Rachitsky** (00:53:13):
That's really interesting. Just thinking of these three buckets, coding agents, AI assistance, OpenClaw but much simpler and easier and more reliable. Sounds like basically the three described there that you're excited about are Instinct, Grok Bot, and ChatGPT Work.

**Anish Acharya** (00:53:30):
That's right.

**Lenny Rachitsky** (00:53:31):
And then, Wabi I guess would fit in that first one. It's like a personal coding agent that can build whatever you want for you.

**Anish Acharya** (00:53:36):
Yes. Yeah, that's exactly right. Yeah.

**Lenny Rachitsky** (00:53:38):
And then entertainment is the third bucket, like AI girlfriends and that kind of stuff. Yeah, those companies, it's crazy. You guys put out these market maps and five of them are these different companions.

**Anish Acharya** (00:53:47):
That's right. Though actually, to be accurate, it's more boyfriends than girlfriends actually. The majority of people using companion products are women that are in their 40s and 50s actually.

**Lenny Rachitsky** (00:53:58):
Interesting. Okay, cool. So, those are the three areas you think the biggest opportunities will come from. And it's interesting that they connect to this idea of loop, I don't know, make me happier. Yeah, they're just kind of like the jobs to be done for humans. Make me happy, make me healthier, make me live longer, that kind of stuff.

**Anish Acharya** (00:54:18):
Yes. Yes. Give me a channel for my ambition, a channel for my fulfillment, and then a thing to do when I'm not doing everything else.

**Lenny Rachitsky** (00:54:27):
That makes sense. Okay. The other question I have for you along these lines is there's so many companies and so many startups, so many products everyone's launching. The speed at which companies and products are shipped is 1,000X-ing. How do you think about durability and moats when you look at a startup? Because a lot of founders get that question. Everyone's getting that question. "How am I not a rapper?" What are signs that tell you this might be a durable thing?

**Anish Acharya** (00:54:54):
Well, I think there's two important ideas. One is something that Jesse from Decagon said, which I love, and that is that moats are most often discovered, not designed. I think it's really easy, I've done this as a founder, to get in your own head about, "Hey, I need a business plan that survives scrutiny from MBAs and VCs. I've got to have some really sophisticated idea of what my moat will be." And for that team, they just started shipping and it developed over time. Another great example of this is Cursor. They were criticized a lot for not having a moat, but it turned out that initially being a high NPS DAU product was really good. And over time they captured all the reasoning traces, they trained their own models, the Composer 1 2 models, and so on and so forth. We know how that story plays out.

**Anish Acharya** (00:55:38):
So moats can be discovered, they don't have to be designed is one. And then, I think the other is that we seem to have forgotten that the classic moats, none of the classic moats are based on how hard it is to make the software. We're not building self-driving cars, most of us aren't. So it's network effects, it's scaled advantages, it's brand effects, proprietary sort of data or what was historically called a cornered resource. Every moat from five years ago generally is still a good moat. We just need founders that have ambition in those directions. We need more multiplayer products, we need consumer social, we need products that get dramatically better the more you use them like Town, so on and so forth.

**Lenny Rachitsky** (00:56:15):
So, still read Hamilton Helmer and all that stuff still applies?

**Anish Acharya** (00:56:20):
Yes. Love his book. 

**Lenny Rachitsky** (00:56:22):
Yeah, he's been on the podcast.

**Anish Acharya** (00:56:23):
What?

**Lenny Rachitsky** (00:56:23):
Yeah.

**Anish Acharya** (00:56:23):
I got to watch that. Yeah.

**Lenny Rachitsky** (00:56:23):
It was recent. 

**Anish Acharya** (00:56:25):
I feel like there's only five real business books in the world, every other one is in the business of selling business books and they're fake, and his is on my list of five.

**Lenny Rachitsky** (00:56:34):
Are there any other on this list that come to mind real quick while we're on the topic?

**Anish Acharya** (00:56:37):
Oh, I mean, the two that are so obvious are High Output Management, which is like that is as good as it ever was. And then Ben's book. Hard Things is, it was the first emotionally honest book about business that was ever written, and that's why founders love it. That's why I love it, because you read it and you're like, "Wow, I'm not the only one that's anxious and feels like a failure, and can't tell anyone what I'm going through." Ben went through it too.

**Lenny Rachitsky** (00:57:01):
Two of the most mentioned books on this podcast, turns out.

**Anish Acharya** (00:57:04):
I'm not surprised.

**Lenny Rachitsky** (00:57:05):
So on this moat idea, so say you're a founder and you're putting a pitch together, trying to pitch you or other VCs, what's the best way to talk about a moat? Can you just say, "We're going to discover it. We're not sure. Nobody really knows yet"?

**Anish Acharya** (00:57:19):
Yeah. I think that we would happily take a bet on a product that doesn't have a "moat" or durability story if it has a lot of momentum, a lot of craft, a lot of growing engagement. It's actually a thing I've learned over the years, I used to be very worried about people stealing my idea, but I've learned that the big ideas are always supported by a dozen small ideas that are invisible. And even if somebody replicates your big idea, they never see the small ideas that make the big idea work. So, I actually think that there's just something special in the water with certain products that make them incredibly successful despite extraordinary competition. I mean, look at Granola. Two years ago it was really criticized, and I don't know that they have a super strong durability story today, and yet it is beloved and dominant. I listen to what the customers are saying more than what the business books say.

**Lenny Rachitsky** (00:58:11):
You get a free year of Granola if you become a subscriber to Lenny's newsletter. I should do this more often when it's part of this product pass, lennysproductpass.com. Get a free year of all these amazing products, including Granola. I just saw RAM put out a report of the fastest growing companies according to their data, and Granola is number two or three.

**Anish Acharya** (00:58:28):
It's a tremendous product. The craft is really high.

**Lenny Rachitsky** (00:58:31):
Yeah. I think about that a lot these days because there's so much, there's Cowork, there's ChatGPT Work, there's Cursor, there's Grok Bot, and it's crazy how quickly one can switch from one to the other. And the underlying model is not that different. All it really is, most of it is the harness/UX of the product. And so to me, that tells you there's so much opportunity in the actual user experience being a moat, or at least giving you a lot of time to find something that is durable.

**Anish Acharya** (00:59:01):
100%. And I think for the people that are at the edge, they pay for all of them because they all have the respective areas of specialization.

**Lenny Rachitsky** (00:59:08):
Yeah. I have many $200 a month plans right now.

**Anish Acharya** (00:59:10):
I know, I know. Right. So it's a little painful, but yes, me too.

**Lenny Rachitsky** (00:59:14):
And I think Cursor has a $300 a month plan now.

**Anish Acharya** (00:59:17):
So does Grok. Oh yeah, you're right. Yeah, that was the Grok plan.

**Lenny Rachitsky** (00:59:20):
Yeah, Grok slash-

**Anish Acharya** (00:59:21):
Yeah, it was Grok Heavy.

**Lenny Rachitsky** (00:59:22):
Yeah. RIP Cursor, I think they've transitioned away from that brand. Something I've been talking a lot about is the distribution. I call it distribution is new moat, but it's always been a moat. But it feels like more and more that is actually a massive advantage because everybody is ... There's 1,000 launch videos a day. Everyone's launching, launch, launch, launch. And really the ability to get your stuff into people's feed, get them continue to be reminded of your products feels like increasingly is powerful and important. Thoughts on the rising value of existing distribution being a big lever for growth and success.

**Anish Acharya** (01:00:03):
This is so important. And I asked Chris Dixon about this because he sort of authored the famous come for the tool, stay for the network. I think the issue is that our entire generation of founders and CEOs were trained on the theory of networks and network building. And as a result, every network that exists today is hyper-trained to ensure no one else builds a network on their network. So, I actually think that the sort of network effect has gone back to this grassroots true word of mouth. When somebody is getting a ton of mentions on X, and on YouTube, and on Instagram and all of these places organically, that is probably the best form of the sort of third party network effect that you can hope for today. And actually just like the web 2.0 era, unlike the mobile era where you had the app store and you had growth hacking, and you had all of these sort of little cottage industries, we have to build our own channels off of that word of mouth growth.

**Anish Acharya** (01:00:56):
So, in a sense it's a purer growth problem, but a harder one than we've had in a couple of product cycles.

**Lenny Rachitsky** (01:01:03):
And to get word of mouth you need to build something. I always think about Seth Godin's line, build something remarkable, something that is worth remarking about, which is basically build an amazing product that people want to talk about, which is very hard to do. And it makes sense that because there's so much happening, people are just going to pay attention to what are my friends using and saying is worth paying attention to.

**Anish Acharya** (01:01:24):
Well, here's the one thing I would say that here's the hopeful point, which is I always say that nobody has a growth problem these days, they have a product problem. And the reason for that is you can build such a wildly ambitious product in any direction, functional or emotional, you can charge a lot of money for it. So my challenge is like, hey, is it that you have a growth problem or is it a failure of our collective imagination? If we imagined our product cost $1,000 a month, $10,000 a month, what if our product was a software Birkin bag? What would it have to do to justify that? Okay, let's figure out how we build that.

**Lenny Rachitsky** (01:01:59):
And it comes back to the ambition question.

**Anish Acharya** (01:02:01):
Yes.

**Lenny Rachitsky** (01:02:02):
And still though, you still need some advantage to get in front of people to get it out there, at least initially, because there's like 1,000 things launching every day. Imagine that's still a big opportunity and I don't know, advantage, which to me makes me feel like incumbents have a huge advantage. They have the products, they can tell you, "Hey, go use Gemini and every time you go search Google." I guess, do you feel like it's harder for startups now because of this distribution challenge?

**Anish Acharya** (01:02:28):
I don't know. I think it's easier, because Gemini, despite all the kind of heavy cross-selling Google has done, nobody would say they're winning.

**Lenny Rachitsky** (01:02:35):
That's right. 

**Anish Acharya** (01:02:37):
Startups can build in directions that incumbents are uncomfortable building in, like everything we talked around companion, but there's many others. 

**Lenny Rachitsky** (01:02:44):
That's true. 

**Anish Acharya** (01:02:45):
Prices can be pretty high. People are open to paying 200 a month or in the enterprise they're open to signing million dollar ACV contracts without really knowing what they're getting. So, I think the floodgates are open. It feels like Christmas 2009 where everybody got their iPhone and wanted to download new apps, that'll change at some point. People will feel like they're done and they're tired and they don't want to try any more apps, but the windows are open for now. I think it's easier for startups.

**Lenny Rachitsky** (01:03:09):
That's a really interesting insight. And you're lying about how it's not a distribution or growth problem, it's a product problem is such an important one, because if your product was that good people would talk about it and share it and use it.

**Anish Acharya** (01:03:21):
**Lenny Rachitsky** (01:03:22):
Yeah, yeah.

**Anish Acharya** (01:03:35):
They're awesome, right? They're sort of like this creative studio that uses technology as their medium, very web 2.0 in that way actually. Many of the Ev Williams, the Kevin Roses, they were painters except technology was their canvas. So, they created this very funny product called Card V Card where they shipped, I think 100,000 people a debit card. And then every day they would text those people with a location that they had to spend the money at and they would put $100 on the card, and everyone would rush out to spend the money, and one or two would be able to spend it and everybody else would get declined. And it was just this hilarious social experiment that went hyper viral. And for me, it was always inspiring in the world of FinTech because it was like, wow, why don't we build more products like that?

**Anish Acharya** (01:04:16):
Money is inherently social and yet all the financial products we have are so dry and personal and embarrassing. I think there's a sort of similar moment happening in AI right now where we can build these wildly ambitious products that touch on many of our social nerves, we just have to do it.

**Lenny Rachitsky** (01:04:29):
So, let me follow that thread. You get to see tons of companies both pitching you and also companies you're working with, that you're investor in. What are some counterintuitive lessons you've learned from watching the companies that operate well and have succeeded? Lessons that maybe go against typical wisdom, startup wisdom?

**Anish Acharya** (01:04:51):
I'll tell you the biggest one. In the old days, which is three years ago, we would see a company, and if what they were trying to do was too ambitious we would not engage. Just too crazy, too complex. And implied by that is you wouldn't do $100 million seed because just it's too much money for almost any problem. It's too much money for any person to actually manage. It's too much money to build this sort of talent to absorb. It doesn't make sense as an inception round. I think today we're almost seeing the opposite problem where an idea that's too small is not something that we want to engage with. And you can talk about how you put $100 million to work in the seed productively. Now, I'm not recommending you raise $100 million, but I think that there's this sort of no ceiling on ambition is also showing up in how we're picking companies and maybe how they're picking us as well.

**Anish Acharya** (01:05:41):
Because when we invest, we tell every founder, "We're here to help you build the strongest form of your vision." Mark told this to me when him and I were talking about coming here and he said, "Anish, the way we told our story when we were raising our first fund was we were going to the moon or we were going to leave a moon size crater in the ground, and there was no other option." That's sort of how we want to work with our founders as well.

**Lenny Rachitsky** (01:06:05):
I love that point. So, can you get too ambitious? Is there a limit? Obviously you look at the team and what they're ... But the key lesson here is be more ambitious. It's like the opposite of what used to be of here's our wedge, here's where we're going to go. What you're looking for is just how big is the idea.

**Anish Acharya** (01:06:22):
I mean, look at Adams. How crazy is Adams? I mean, what an incredible hero's journey for all of us collectively, but also what they're trying to do is something that 5 or 7 or 10 years ago would've felt insurmountable. And now it's like, okay, it's challenging. Let's see.

**Lenny Rachitsky** (01:06:38):
Interesting. Is there anything else that has changed or I guess you've changed your mind about around what you think it takes to build a successful company these days?

**Anish Acharya** (01:06:46):
I mean, I think that the kind of old wisdom around consumer products have to be free. I'm almost taking the opposite take, which is let's think about consumer products that are extraordinarily expensive. I think every part of consumer discretionary spend is up for grabs right now, and I think are really useful, because price is a measure of product market fit, a really useful product exercise is what is the Birkin bag 10,000 a month, 1,000 a month version of our product. So, I think expensive consumer software is something new and important that we wouldn't have thought about five years ago.

**Lenny Rachitsky** (01:07:18):
I love that framing, because it just pushes you, again, to be more ambitious. You mentioned Mark and you work closely with Mark Andreessen, Ben Horowitz.

**Anish Acharya** (01:07:26):
Yes.

**Lenny Rachitsky** (01:07:27):
What's one thing you've learned from each of those guys?

**Anish Acharya** (01:07:32):
They're such extraordinary leaders, founders. I mean, the thing that I actually feel so grateful to be a part of that they really embody to their core, I think is a feeling of stewardship for the technology industry, and for really the country and maybe the Western way of living and thinking. And if you look at a Ron Conway or Brook Byers, Tom Perkins, there was this feeling I think of obligation to leave it better than you found it from an industry perspective. And that sort of aspiration goes way beyond just being the best investor in the world, though we want to do that too. I see them both show up that way over and over again where they want to do hard important things that don't directly benefit the firm, or at least not singularly because they're just sort of important. Ben has done a lot of that in the direction of the industry, and Mark in the direction of the country, though of course both work on both.

**Anish Acharya** (01:08:34):
Another really cool thing is just to see how I think Mark and Ben, but maybe the firm a little bit, has shaped our collective ambition as a founder community. I think if you look at 5 or 7 or 10 years ago, deep tech was deeply unpopular. It wasn't a high status thing to be working on, it was very fringe, and now it's become very popular, high status and mainstream. And I think there's a lot of firms that have of course pulled in that direction, but I think that someone like Mark has been very full-throated in his support of working on sort of capital I important work in the national interest, and all of Silicon Valley has changed as a result.

**Lenny Rachitsky** (01:09:10):
And you guys have had some big wins in the past couple of weeks investing wise too.

**Anish Acharya** (01:09:15):
Yeah, thank you.

**Lenny Rachitsky** (01:09:16):
Congrats. Final question before we get to our very exciting lightning round. What's your advice to product people who are trying to think about what they might want to shift in how they work, how they think, how they operate to be more successful in the future in their careers and with their companies?

**Anish Acharya** (01:09:35):
Just make more things. And I know it sounds silly, I know everybody says it, but just please come up with a project. You don't have to tell anyone about it, it can be totally unimportant, but use it as a chassis to use all the new models, ship things, talk about them, build your own intuition. I promise you're one sort of slightly frustrating and then very fulfilling week away from being as pilled as anyone. So, you just got to use the technology. And if not now, then when, right? This is all of us got in the game to build the products we saw in our mind's eye, and now we have a chance to do it. So just please, please use the models and tell me what you built. Text me, tag me. I will reply and respond and engage with you, and so will everyone else because the magic of Silicon Valley is that it's a very positive sum mindset.

**Anish Acharya** (01:10:27):
Everybody's building on each other and vulnerability is really rewarded, so I definitely would encourage people to use the models.

**Lenny Rachitsky** (01:10:33):
What's a good heuristic if you're doing this enough? Is it build something once a month? Is it some number of hours per day sitting, talking, building? Anything that you think might help people be like, "Okay, you're doing a good job"?

**Anish Acharya** (01:10:46):
I mean, just ship something once a week, and it doesn't have to be crazy. For example, when I was playing around with Codex I had it build a slide deck for Mother's Day for my wife that pulled from my text messages. It looked at my photo gallery, it set some music to it, created a 20 slide deck of our relationship and pulled some cool old texts from when I first asked her out. It was a really nice Mother's Day. I mean, it wasn't important, it wasn't something that we might come back to, but it was shipping something. So, it can be that small.

**Lenny Rachitsky** (01:11:18):
I know that you're our mutual friend, Nikhyl Singhal, you worked at Credit Karma with him, he had a really good way of thinking about this. He finds that people flip on AI and how they feel about it once they find some moment of joy that it had created for them, and this Mother's Day idea is such a good example. And so, I think that's kind of a tip I always think about is just what's something that just will bring you joy if this works.

**Anish Acharya** (01:11:44):
What's something you can do for someone else? Maybe that's a good starting point as well.

**Lenny Rachitsky** (01:11:47):
I love that. Anish, before we get to our very exciting lightning round, is there anything else that you want to share? Anything else you want to double down on before we get into the lightning round?

**Anish Acharya** (01:11:58):
I don't think so, I've loved the conversation so far.

**Lenny Rachitsky** (01:12:01):
Me too. And with that, we've reached our very exciting lightning round. I've got five questions for you. Are you ready?

**Anish Acharya** (01:12:06):
Okay.

**Lenny Rachitsky** (01:12:07):
Here we go. What are two or three books that you find yourself recommending most to other people?

**Anish Acharya** (01:12:12):
Yeah, so okay. Conquest and Cultures is my very favorite book. It's Thomas Sowell, and it just talks about how conquests have led to culture change in different societies around the world, sometimes positive, sometimes negative. I think to me, it's just the best historic view of culture as the biggest driver of outcomes, and I've experienced a lot of that as somebody who was born in Canada and moved here to America, which has a very different culture of ambition. There's that word again. So, Conquest and Cultures is great. 7 Powers you mentioned is actually just an awesome book. I think it's a very intellectual distillation about moats and business theory and compounding advantages. I really like it. Maybe the third is the one that Mark ... I actually thought that he was maybe punking me when he sent this to me before I started. I said, "Mark, are there any books that I should read?" And he sent me a couple.

**Anish Acharya** (01:13:04):
And one was a book, a textbook called Increasing Returns to Scale, which I think is Brian Arthur is the author. It's an awesome book. It's a slightly dense study of why things like software have such outlier economic effects, but it really helps put things in perspective, or it helped me in terms of why does our industry work in the way that it does? Why does our culture work in the way that it does? Why are we so positive some? I'd love to say that we're better people, but I think it may be a sort of better system and structure we work with it.

**Lenny Rachitsky** (01:13:33):
Favorite recent movie or TV show you have really enjoyed?

**Anish Acharya** (01:13:37):
Oh man, I watch trashy movies and TV. I mean, we-

**Lenny Rachitsky** (01:13:39):
Acceptable.

**Anish Acharya** (01:13:40):
... watched House of Dragon, which is pretty cool.

**Lenny Rachitsky** (01:13:43):
That's not trashy. Yeah, that's great. 

**Anish Acharya** (01:13:45):
I don't know. Yeah, maybe. It's not highbrow. It's not important with a capital I, but it was awesome. We loved that. And then I did see Odyssey. I saw it in London. I was there for a board meeting in an IMAX theater packed with people drinking pints and having fun. 

**Lenny Rachitsky** (01:13:45):
Amazing. 

**Anish Acharya** (01:14:02):
And it was cool because it was just a whole ... The movie was great, but it was just like a theater experience, like a weird social experience kind of alone together. Those are two recent ones.

**Lenny Rachitsky** (01:14:12):
I have not been able to get tickets to The Odyssey at an IMAX. I actually have a Grok Bot just watching the site constantly and-

**Anish Acharya** (01:14:12):
Perfect. 

**Lenny Rachitsky** (01:14:20):
... finding me good seats.

**Anish Acharya** (01:14:21):
Perfect.

**Lenny Rachitsky** (01:14:22):
Perfect. They've got the dumb CAPTCHA though on AMC website that it hasn't been able to get through.

**Anish Acharya** (01:14:27):
Really?

**Lenny Rachitsky** (01:14:28):
It's like a tricky one. It's a really tricky one.

**Anish Acharya** (01:14:31):
Is it the select the fruits? Anyways.

**Lenny Rachitsky** (01:14:33):
Yeah, it's like you have to click three different matching shapes, which come on, you can't do that? Hopefully by the time this comes out I've seen it. I think it's a few podcasts in a row I'm like, "I haven't seen it yet." Oh, man. Okay. Favorite new AI product? I don't know, favorite AI product recently that they've given you joy.

**Anish Acharya** (01:14:54):
Oh man, I've spent a lot of time with the personal agents. I think Grok's okay, I'm going to give it to Grok Bots only because it's just so unhinged for it to be so ambitious about caching credentials and getting work done on your behalf. I love it and I expect it from a startup, but they actually are doing things that I think no other sort of big company would do. It's really, really well done. It's a really thoughtful UI. It's got a really powerful foundation model. I think it also is like, okay, wait, maybe this is not a two-horse race on the sort of model side. So, I just think the product is fun and ambitious, and is sort of taking risks that other products like that wouldn't take.

**Lenny Rachitsky** (01:15:31):
Two more questions. Do you have a favorite life motto that you often come back to in work or in life?

**Anish Acharya** (01:15:37):
Oh man, I've got one. I learned this or this is from my founder days but it also is something that's very true of parenting, which is don't discover things through painful experience that somebody can just tell you. And I unfortunately have had a bad habit of discovery versus learning from somebody who's just a few steps ahead of me, and I find my children have that habit too.

**Lenny Rachitsky** (01:15:59):
What's one example of something that you wish someone had told you?

**Anish Acharya** (01:16:02):
I mean, for my kids it's don't touch the hot stove. For my startup, it was like-

**Lenny Rachitsky** (01:16:02):
Like literally. 

**Anish Acharya** (01:16:08):
Literally. For my startup, it was don't build a product and a platform at the same time. If you're going to be a platform company, build one. Our first company we tried to build a social platform for mobile games and be a gaming studio, and somebody wise told me right away, "Look, being a studio is so hard, much less being a studio and a platform. Pick one." And we did, and it took us years to figure out we were wrong.

**Lenny Rachitsky** (01:16:30):
Final question. I asked Ben Horowitz what to ask you about, and he just said, "Ask him about his DJing. He's very good." And I found your DJ site. I don't know if that's you call it on SoundCloud/illscience. 

**Anish Acharya** (01:16:43):
That's very good. Thank you.

**Lenny Rachitsky** (01:16:44):
I'm just listening to it while I work. Any tips for somebody that wants to get into DJing? Any tools you found useful? Any, I don't know, insights that might help someone become better at this?

**Anish Acharya** (01:16:56):
Totally. I mean, I think that this is why I love music models so much. I mean, I love DJing, I've been playing for 30 years now, since '95, actually 31. Wow. And it's an awesome way to express yourself musically if you're not a classically trained musician. You select the music, you pick the records, you mix them together so it requires some technical skill. But now I think you can go a step further and just make music with the models. And the best part is when you can come up with music ideas and have the models do the kind of strong form of them. So, I think music is just such a visceral, satisfying way to experience and provide experiences in the world. So, whether it's DJing or making music, I just suggest everyone do it.

**Lenny Rachitsky** (01:17:37):
I hadn't though about how DJing has changed now that you have Suno and things like ElevenLabs and all these things where you could just generate the music, not have to just splice together existing music.

**Anish Acharya** (01:17:46):
I mean, think of the history of it. You went from, okay, first you could only hear music if you were there with a person playing on an instrument, recorded music on the phonograph. The big change in music actually from a medium perspective was the cassette tape, because the cassette tape was really the first time you could create. You could actually compose your own "album." I think a lot of why music struggled in the 2000s is that went away and we went back to broadcast, and now that people are making music again I think the music industry is going to be bigger than it's ever been.

**Lenny Rachitsky** (01:18:17):
Wow. Man, so much disruption. Anish, this was incredible. We covered so much ground. Final question, how can listeners be useful to you?

**Anish Acharya** (01:18:27):
I mean, show me what you're building. Please don't be despondent. Build something and then tag me, and I'd love to see it. If you're interested in hearing more stuff like this, please follow me on X. I try to kind of engage and follow back. And otherwise, make sure you check out all the amazing folks in Lenny's network. Claire is a star, Alina is so, so good, and there's just so much compelling content here.

**Lenny Rachitsky** (01:18:49):
Nikhyl, which we talked about.

**Anish Acharya** (01:18:50):
Nikhyl's the best, man. That guy is everything.

**Lenny Rachitsky** (01:18:55):
Amazing. Anish, thank you so much for being here.

**Anish Acharya** (01:18:58):
Thank you, Lenny.

**Lenny Rachitsky** (01:18:59):
Bye everyone. Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review, as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
