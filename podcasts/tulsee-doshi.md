---
title: "Why PMs are suddenly valuable again | Tulsee Doshi (Head of Product, Gemini)"
date: "2026-11-08"
type: "podcast"
guest: "Tulsee Doshi"
post_url: "https://www.lennysnewsletter.com/p/what-it-actually-takes-to-build-frontier"
description: "Why PMs are suddenly valuable again, covering AI product work, product design, and go-to-market execution."
word_count: 12329
---

**Tulsee Doshi** (00:00:00):
The model isn't predictable. It's kind of like Snape's potions class. So you can put all the ingredients in, but you also have to expect that there will be a little bit of magic, and that magic is going to be surprising.

**Lenny Rachitsky** (00:00:10):
As you're hiring PMs these days, is there anything you look for more and more?

**Tulsee Doshi** (00:00:15):
We are looking for PMs who understand the vibes of our models or other models. I want PMs who have an opinion, who are playing with these models every day. You ideally want to stress test the model on things that you are excited about.

**Lenny Rachitsky** (00:00:28):
A lot of people feel that Google lags behind the top two labs right now.

**Tulsee Doshi** (00:00:32):
I actually think we do want to win the frontier conversation. I don't think we should say that Google is not participating in the frontier.

**Lenny Rachitsky** (00:00:39):
You have this framework around how far ahead to build. You call it a 60/20/20 rule.

**Tulsee Doshi** (00:00:44):
Traditional startup wisdom, you're just like, "Build an MVP that works." But I think you want to actually build features that aren't necessarily always working today.

**Lenny Rachitsky** (00:00:52):
It feels like every AI assistant launching these days is taking all this juicy Google data, my Gmail, Google Calendar, My Docs. I'm curious just why Google hasn't launched something awesome yet.

**Tulsee Doshi** (00:01:03):
The team is working on some amazing things, but I think you are right that there is more work we need to do here on this front.

**Lenny Rachitsky** (00:01:07):
Tulsee, thank you so much for being here and welcome to the podcast.

**Tulsee Doshi** (00:01:15):
Thanks. I'm excited to be here.

**Lenny Rachitsky** (00:01:17):
You are head of product for Google's frontier models, which includes Gemini, which people know, but there's also a bunch of other models that people may not be familiar with. Share the other models that are under your umbrella.

**Tulsee Doshi** (00:01:30):
Yeah, so we have a set of models we kind of call our gen media models. These are our models that focus on video editing and generation, image editing and generation, if you've used Nano Banana, Lyria, our music model. We also have Gemma, our suite of open models, and then one set of models that actually falls under our Gemini umbrella, but I feel like we don't talk about as much is our audio models. So dialogue, audio understanding, text to speech, translation, all a part of the portfolio of how we build frontier models.

**Lenny Rachitsky** (00:02:03):
Okay. So I want to spend a little time on models. Everyone sees models launch. There's a model launch every week it feels like. You have a really unique lens in being able to see these models from research to pre-training, post-training launch. What's something that you think people maybe misunderstand about how models are created or something that may surprise people about how models are made?

**Tulsee Doshi** (00:02:26):
Yeah, it's a good question. I mean, maybe what I'll say, especially coming from a product management lens, is one thing that I think when you typically talk about product management for anything, including a model, you talk about what are the goals you have for a model? What are the capabilities you want to set? What are the outcomes you want to drive? What goals do you want to hit on a set of evals? And often when I talk to customers or even internal users, they'll ask me, "Okay, what are the goals that you're setting?" And they'll sort of expect that we can really make sure that the model will deliver on those goals in a very traditional product sense.

**Tulsee Doshi** (00:03:03):
And I think for me, what has often been surprising, but also exciting about model development and being a PM for the model is you should do that and you should have an intentional view, but the model isn't predictable.

**Tulsee Doshi** (00:03:18):
And so it's kind of like Snape's potions class. So you can put all the ingredients in and you should be thoughtful about what you expect, but you also have to expect that there will be a little bit of magic and that that magic is going to be surprising and that magic is going to be unique. And so your job as a PM is not just to try to shape what goes into the model, but it is also to look at what comes out the other side and really identify where does the model shine, where does it actually look unique in ways that surprise you, and then be able to take that and shape that into something that is amazing for users.

**Lenny Rachitsky** (00:03:55):
It's so interesting that it's just like this code that we have written that we feed data and we need to... We don't exactly know what's going to happen and how it works. I recently had an interpretability research person on the podcast from Anthropic and we talked a lot about this, this idea that models are grown, not built. And just to reflect back what you're saying, there's these goals that researchers have. For this next model, we're going to get better at writing, we're going to try to be funnier, we're going to try to become better engineers. And you're saying it's unpredictable exactly what ends up at the end. They put in these ideas, they change the data that it's trained on. Is there anything more there about just this kind of unexpected, I don't know, process of training?

**Tulsee Doshi** (00:04:36):
Of course, there's brilliant research that goes into these models, and so many aspects of it are predictable in the sense that we are consistently monitoring these runs. We have researchers who are tracking them, who are identifying when to intervene, who are seeing different metrics climb up as the run progresses. And so we are making it as much of a science as possible. But I think for me, what is really amazing as a PM is you also need to really understand the vibes of the model on the other side of it too. So yes, you can understand that a model has improved on a certain capability, but where does that capability really shine through? How does that showcase then downstream in a product? How do you feel communicating with the model in terms of its behavior and persona? And there's a number of these aspects that we definitely build into training, but also as we understand the model and as we evaluate it and as we test it, we always learn more. We always learn something new, I think, about what the model can do.

**Audio: Lenny Rachitsky** (00:05:29):
This episode is brought to you by this season's presenting sponsor, WorkOS. What do OpenAI, Anthropic, Cursor, Replit, Sierra, Clay, and hundreds of other winning companies have in common? They're all powered by WorkOS. If you're building for enterprises, you have felt the pain of integrating single sign-on, skim, RBAC and audit logs. WorkOS turns those deal blockers into drop-in APIs built for B2B SaaS. And now there's a new kind of user that needs access to your app, agents. AI agents need to register, authenticate, and get permissions just like a person. WorkOS handles it all. AgentAuth to give agents scope, revocable identities, agent registration with AuthMD, and Airlock to judge every agent action and allow, deny, or escalate to a human. I've noticed that every startup that I'm an investor in, that expands up market ends up using WorkOS because they're the best. Go to workos.com to make your app enterprise-ready today.

**Lenny Rachitsky** (00:06:30):
I want to talk a little bit about Google's place in the AI race. It feels like a lot of people feel that Google lags behind the top two labs right now, Anthropic and OpenAI, and Google has these moments of being the best and then it kind of feels like it slows down a bit. I'm curious what you can share about just Google's strategy in the AI race and what maybe people don't understand on the inside of how y'all think about this stuff.

**Tulsee Doshi** (00:06:54):
First of all, hopefully by the time this conversation goes out, you will be using Gemini 4 Argon, which is exciting. And so I really do hope we're having a conversation about a frontier AI model that folks are excited to use. And I think Gemini 4 speaks a little bit to our strategy because it really is our push to continue to build a frontier lab, a frontier set of models, a frontier set of capabilities on our path.

**Tulsee Doshi** (00:07:23):
I think if you look at Google's strategy, it really is full stack. So one of the things that I think is powerful about Google is all the way from hardware to end products that serve billions of users, I think the stat is like we have 14 products that are above a billion users. I should check that number, but I think that's the stat. And so if you think about that, we actually go all the way from the hardware to then the modeling to then this kind of end user application.

**Tulsee Doshi** (00:07:52):
And our goal ultimately is to not just build amazing frontier experiences, which is definitely a part of the goal, but it is also to build models across this Pareto curve of cost to quality that can serve different users at different points in their lifestyle, whether that be a search user who is coming for information, whether it is an engineer who is trying to build the next amazing thing, whether it's for a cyber defender who is trying to protect a critical piece of infrastructure. I think our goal is to make sure that we have models that serve that range of use cases and that we're actually building with feedback from these users.

**Lenny Rachitsky** (00:08:30):
So what I'm hearing is there's so many vectors where Google can win. There's the most efficient Pareto frontier per token cost, there's the smartest model. There's also just making your products better, for example, AI mode, AI overviews. And so it's not that you need to be the best at the most advanced AI model that people can use like chatbot basically, you can win in all these other areas, but it sounds like you're also trying to win and have the most state-of-the-art model.

**Tulsee Doshi** (00:08:58):
I actually think we do want to win the frontier conversation. I don't think we should say that Google is not participating in the frontier. And I think we are building better and better models, and I think Gemini 4 Argon definitely is at the frontier in the place that we are at. But I think one thing that is amazing is being able to build a breadth of experiences and build a diversity of experiences for users. And I think for Google, our goal ultimately is to build amazing experiences that actually make people's lives better. And that is I think ultimately the goal, whatever part of the frontier you're building for.

**Lenny Rachitsky** (00:09:42):
Google products definitely make my life better. It's just amazing how much of your life is within a Google ecosystem, not even the AI stuff, but just Google Calendar, Gmail, all these things you're just like Google Docs. So it's happening.

**Tulsee Doshi** (00:09:55):
There you go.

**Lenny Rachitsky** (00:09:58):
There we go. I want to talk about one other broad AI question, then I'm going to dig into more product specific stuff. A big topic of conversation these days is AI safety and this kind of fear that AI is going to harm humans, it's going to cause damage as it gets smarter and smarter. You have a really interesting lens on this because you led product for the responsible AI team at Google for six years. This is what you did right before this role. And so you've been thinking about this for a long time, a lot longer than most people. I'm curious just to get your take on this debate. Just, I don't know, are you optimistic we'll figure this out? What do you think people maybe don't understand about this debate around AI safety?

**Tulsee Doshi** (00:10:36):
Our safety teams here are incredible, and it's been incredible to see the intentionality that they've been putting in all the way from initial trainings of the model to how we deploy them. And I think safety is embedded in that process and we need to be.

**Tulsee Doshi** (00:10:52):
I think the part that is important actually as we talk about how do you deploy models safely is actually thinking through what are the right sort of mitigations and structures around these models. So for example, one of the things that's really important is thinking about monitoring. And so for us, actually deploying monitors that can monitor the model's chain of thought and actually identify whether the model is misaligned with its directed actions or whether it is aligned and then being able to intervene appropriately, that's actually the kind of mitigation that, A, gives us more confidence in deploying these models, but also allows us to better understand where we might see misalignment and better actually improve the models over time. And so I think things like monitoring give me more confidence in how we're putting our models out.

**Tulsee Doshi** (00:11:39):
I think the other thing that we don't talk about enough when we talk about this debate is also the role that AI can play in hardening our systems. And so one of the things that we are doing with Gemini 4 is actively partnering with a number of cyber defenders, including actually just even partnering with Wiz, that is now a Google company, to really think through how can we actually identify and patch vulnerabilities in systems across the globe. We actually have this interesting case study. Wiz has this Stand for Good program where they're actually actively working with systems across the world to identify potential issues and they worked with a hospital system to identify a vulnerability and then patch it. And it's that kind of thing that I think if we can actually leverage these tools to do more of, we can actually make sure that our infrastructure and our systems are robust, which is also I think really critical as this whole space grows.

**Lenny Rachitsky** (00:12:34):
There's actually a conversation all in this last week about this whole issue that now that AI is getting really good at cyber, people are going to be investing a lot more in cyber defense and AI for protecting. And so there's going to be a lot of money being spent on protecting their systems from this ever smarter AI. So it's really cool that you guys are investing there. So I guess just coming back to the question of, do you feel like we'll figure out this concern and this issue we feel, a lot of people feel, that AI is going to take over the world, cause a lot of damage? Do you feel like this is solvable problem? Are you optimistic or is it something you think a lot about and are kind of worried about?

**Tulsee Doshi** (00:13:12):
Maybe the answer to your question is both in the sense that I think we need to be consistently thinking about it. I think the way to optimism here, for lack of a better way of putting it, the path to optimism is through thinking about it and being very careful and very thoughtful and very intentional on the path to get there. And so my source of optimism comes more from, do I feel like we have people who are being intentional and thoughtful about what the safety story looks like? And I think that is the critical threat, is you need a number of people to be worried and to be having conversations and to be actually interrogating how we're building our models. And that's the step-by-step process we have to take.

**Lenny Rachitsky** (00:13:50):
Awesome. And what's interesting is I don't think I've read a story of Google's models hacking into anyone, which I think shows that this is something y'all have been thinking about for a long time. I don't know for better or worse, but it feels like it's working, whatever y'all are doing.

**Tulsee Doshi** (00:14:05):
We like stories about fixing vulnerabilities.

**Lenny Rachitsky** (00:14:07):
There you go.

**Tulsee Doshi** (00:14:08):
That's a good place for us to be.

**Lenny Rachitsky** (00:14:10):
Okay. So one of the interesting things that's happening from a product perspective with AI is products are getting very complicated. For example, Google gets a lot of flack for it being hard to find all the magical things y'all do. A lot of people don't know AI Studio even exists. A lot of people can find Veo or Genie and all these things. Similarly, Codex, ChatGPT recently launched Dots, and now you go to the interface of Codex and it's like tabs and dropdowns and dots and it's just out of control. And Claude Code is the same thing. It's just getting very complicated that Cowork and then they drop Cowork. And interestingly, I'm in this WhatsApp group with a bunch of PMs and there's a PM from one of the labs.

**Tulsee Doshi** (00:14:51):
I'll be in this WhatsApp group. Sorry, continue.

**Lenny Rachitsky** (00:14:53):
Okay, let's talk. And he showed that there's this kind of urgency to get frontier power of AI out to users as fast as possible, partly to stay competitive, partly because they don't know exactly what it's used for yet. So let's get it to people, figure out what they're using it for and then make the UX better. So there's this kind of intentional, "Let's just get it out there, figure it out later how to make it a great UX."

**Lenny Rachitsky** (00:15:18):
Thoughts on this kind of balance of making the product really easy to use versus just getting things out as quickly as possible? And is that something you deal with?

**Tulsee Doshi** (00:15:26):
Two thoughts maybe, maybe three. The first one I'll say is I do think we do need to be playing with new paradigms and new UX approaches, if you will, to how people will engage with models. So you mentioned, for example, Genie or Veo, which we're now building Omni. If you look at, for example, Flow, Flow is a product that we've been designing thinking about video editing and generation, music editing and generation. And so I think we are trying to play with... NotebookLM is a good example of a different form factor. I think our labs teams are actively thinking about how do we try different form factors and different UX for different individuals to engage with these models? And so I do think we need to keep innovating and playing around with what UX looks like.

**Tulsee Doshi** (00:16:12):
I think at the same time, your point is also right, which is I think depending on who your user is, you want a different form factor too. So I think for example, with AI mode, we're talking about billions of users coming to search, asking their questions. I think you do need to have a certain UX there that is accessible to every user. At the same time, on the other end of the spectrum, when you have something like Antigravity, you are trying to build for a power user and you are trying to build for users who know how to use slash commands and can actively engage across both the terminal and the IDE. And you want to be able to support a wide range of what a user can do. And so I think depending on who your user is, you have a certain level of flexibility with how you think about the UX, right?

**Lenny Rachitsky** (00:16:57):
That makes sense. Basically there's different services for different levels of how radical you can change things.

**Tulsee Doshi** (00:17:03):
Yeah. And I think the other part too is I think it's also important to think about the model as having a UX also. So one of the things I think about a lot as a PM for the model is what is the UX of actually using the model? So how transparent is the model? How well does it communicate with you? What questions does it come back and ask you? This is all UX in its own way. And so I think it's also really interesting to think about how do we bring conversations about UX into the actual model development process itself?

**Lenny Rachitsky** (00:17:32):
That is really interesting. Basically the personality of the model, is the UX of the model. How do you as a PM inform that work with the researchers? Is it like, "Here's feedback on the way it's talking and it should be a little more verbose here and here's ways it could format things differently"?

**Tulsee Doshi** (00:17:46):
I think the role of the PM here is actually really awesome because you are actually getting to shape what is the direction of where we want to go with the model's behavior. And so we have a team that works on model behavior here, and a lot of what we've been thinking about together is, A, looking at customer feedback and user feedback for how they engage, but also thinking through what does good look like for Gemini specifically and how do we develop a spec, if you will, for what does that look like? And then being able to translate that to rubrics that we can then evaluate the model on to be able to translate that into data that we can actually leverage for the model, to be able to translate that into our reward modeling. And so it's been actually a really nice collaboration between PM and the research team.

**Lenny Rachitsky** (00:18:30):
Something I hear a lot is that even if we stopped development on the model, there's so much it can do that we are not yet doing. There's this overhang. Is that something you think a lot about? It feels like that's a big part of this job is exposing the powers of the AI model to users.

**Tulsee Doshi** (00:18:46):
Yeah, and figuring out what is new and where is the next set of exciting? Where is the next frontier, what are the capabilities that we're trying to invest in and build, I think is a fun activity here also. And I think a lot of this actually is really working in hand-in-hand with our internal customers if you think about search or the Gemini app or YouTube or labs, but also working with external customers to really understand where are they going, what are their needs, what would meaningfully change their experience, and how do we actually build that flywheel of feedback too.

**Lenny Rachitsky** (00:19:21):
Along these lines, one of the other really interesting trends I've been watching on Twitter in particular is people realizing the value of product managers again. We went through this phase of just like, "We don't need PMs anymore." Yeah, exactly. It's just like, "Okay, we can build anything. We don't need PMs. Let's just build it all. PMs are so bad."

**Lenny Rachitsky** (00:19:39):
And the reason, just to add a little context there, is now that it's so easy to build, people are just building all this nonsense and things that don't work, things people don't want to use, and people are realizing there's a very specific skill to figure out what is worth building, what problems people have that are worth solving, what a great looks like, what good looks like once you're done, aligning people behind one's cohesive vision. Is that something you're noticing, thoughts on that kind of PM ascendance that has started to happen again?

**Tulsee Doshi** (00:20:08):
I like the phrase PM ascendance. I'm going to use that. Yeah, I mean, I think you actually said it very well, which is I think... Look, I'm obviously biased because I am a PM.

**Lenny Rachitsky** (00:20:09):
Same. Same.

**Tulsee Doshi** (00:20:19):
So I would like to believe that PM ascendant is here and we're back. But I actually think exactly what you said, which is when you can build anything and you can build anything so easily, building something great actually is now a unique value add. And taste is now really important. Someone who can come in and actually really pull in what is the signal from the noise and what is that insight that will actually unlock a great experience? And that is truly what a good PM does, is bring that insight and help unlock. I think the other part that you noted that I particularly feel in a place like Google where we are building a number of products is, again, when this is so easy, someone who can bring people together and drive consensus and turn chaos into order, I think, becomes actually really important because in the absence of that and the ability to build as quickly as we now can, speed can basically introduce chaos if you're not actually able to bring clarity to that and bring structure to that.

**Lenny Rachitsky** (00:21:25):
So on that, as you're hiring PMs these days, is there anything you look for more and more, kind of a skill that might be trending up in the PMs that you hire that you think is really important to be really successful or just broadly skills that you find are really important to be successful in this role of being a research PM?

**Tulsee Doshi** (00:21:44):
Yeah, I mean, I think more and more so we are looking for PMs who, for lack of a better way of putting it, understand the vibes of our models or other models. I want PMs who have an opinion, who are playing with these models every day, who have their own use cases for how they judge whether a model is really good, who play with and stress test these capabilities themselves, who are capable of diving in and looking at data and getting scrappy and rolling up their sleeves. And so I think it's both PMs who are trying to build that intuition as well as who are technical enough in the sense of being willing to, like I said, roll up sleeves, go in, really understand the data, build an eval, actually sit down and pull those pieces together. I think that's really important.

**Tulsee Doshi** (00:22:37):
The other thing I'll say is I think PMs who are agile and adaptive are also really important. I think the space is changing every two weeks. A roadmap you wrote two months ago, you're going to be looking at it again and rewriting it. And so I think PMs who are constantly keeping an eye out on the environment, on the market landscape, and actually consistently re-interrogating what are we doing and why are we doing it as opposed to assuming that there's a fixed kind of plan of action.

**Lenny Rachitsky** (00:23:05):
This is awesome. Okay, so vibes, evals, adaptive. I want to poke at these a little bit. So with evals, say someone doesn't really know how to write an eval, how to approach writing an eval, their first eval, what are some tips to start getting better at the skill of writing evals?

**Tulsee Doshi** (00:23:20):
Yeah, and to be honest, we're still figuring that out internally with our PMs as well. And I would say we see some PMs who are stronger at this than others, and so we're kind of working to upskill our whole team here. I think for me, a big thing is start with even just five prompts. You don't have to start large. I think we often think about like, "Oh, I need to build some sort of massive large scale evaluation or benchmark."

**Tulsee Doshi** (00:23:45):
I think often even just a mini evaluation where you get to 20 prompts that can really stress test a set of capabilities where you can see signal between your model and another model or model A and model B, I think that already is so powerful and that's an unlock because it doesn't require you to think as critically about all of the pieces. Start simple. Start with even just yourself. You as the rater, you looking in a prompt, you trying to decide if the results and the response is good, especially when you're talking about these long multi-step, multi-turn trajectories, just even being able to identify how you're thinking about good is really hard actually. And so even getting that set of good examples will already give you a sense of, "Oh, this is what I'm trying to get to." It'll give yourself clarity and then you figure out how to scale that up, I think.

**Lenny Rachitsky** (00:24:37):
Awesome. Okay, that is really good advice. There's this debate, I don't know, six months ago on Twitter around evals versus vibes. And it's interesting, your advice is both actually really important, structured evals, rubrics, and also getting good at getting the vibes. So on that vibes piece, there's something I struggle with, to be honest. When I get a new model, I never know exactly what to do with it to understand what it's gotten better at. So I'm just like, "Hello, let's try some things I've done in the past."

**Tulsee Doshi** (00:25:02):
"What's up?" Yeah.

**Lenny Rachitsky** (00:25:03):
"This is cool. This is great. Maybe better." What are some tips you have for folks that want to get better at this very specific skill of understanding where a model's gone better than the vibes and how they've shifted maybe from a previous model?

**Tulsee Doshi** (00:25:14):
There isn't necessarily a one right answer to this because you ideally want to stress test the model on things that you are excited about. That's where you're going to also see magic in the model, I think. And so I actually see that different people have very, very different notions of this. So you'll see, for example, on Twitter, a lot of people trying the kind of 3D animations and more visual type aesthetics because that's one way to visually gauge a sense of how models are operating. You'll see others throw models at writing, whether that be creative writing or writing essays or synthesizing information, you'll see others throw it at just really hard financial analysis.

**Tulsee Doshi** (00:25:55):
And so I think part of it is finding the right task where you feel like today certain models are already showing signs of life and showing light, but they're not perfect under your definition of perfect. And that gives you some malleability to see different models handle the problem differently. And that already gives you, I think, some insight into how the models perform.

**Lenny Rachitsky** (00:26:16):
This is great advice. So what I'm hearing is stick to things you actually care about and watch the models evolve on how good they are at this thing. Could be writing a PRD for you, could be writing strategy doc, could be generating graphics.

**Lenny Rachitsky** (00:26:28):
Okay. I have a couple eval stories that one of your colleagues shared about that are fun facts about you.

**Tulsee Doshi** (00:26:34):
Oh boy.

**Lenny Rachitsky** (00:26:35):
So this is Eli Collins, VP product. He's a colleague of yours at Google DeepMind. Okay. So one is you worked on something called the Fitzpatrick Scale and the Monk skin tone, and this was a big shift in how models worked around and evals were part of this. Share this story, what this work was.

**Tulsee Doshi** (00:26:55):
Yeah. So like you noted earlier, I spent six years in responsible AI. A big part of that time we were looking at skin tone and skin tone representation in our models, in our products. One of the things we realized is that early on, there was a scale that individuals were using the Fitzpatrick scale, which was six skin tones. And that was how we were evaluating the effectiveness of product. And realistically, six skin tones cannot capture the diversity of skin tones in the world. Not only that, it was actually built for an entirely different purpose. It was built for healthcare purposes, and so it actually skewed extremely light skin tone given the problems that it was trying to solve. And so it actually not only was only six skin tones, it was also not even the six correct skin tones if you're trying to represent a global population.

**Tulsee Doshi** (00:27:46):
And so we worked with a professor at Harvard, Professor Monk. He had been from a more anthropology sociology perspective looking at characterizing a set of skin tones. And so he had a scale of 10 skin tones that he had built through a number of user interviews and research that he had been doing over years. And we pulled that set of skin tones into our evaluations and actually redid a number of the ways that we evaluated our products and our models to reflect that 10 skin tone scale and actually use that to improve things like our efforts in the pixel camera, like some of our image generation to be more intentional about how skin tones are represented.

**Lenny Rachitsky** (00:28:27):
That is awesome. That is some serious impact you had here. What else do you think is maybe useful for people to hear as they hear this and they maybe have to rethink their evals that may be out of date?

**Tulsee Doshi** (00:28:38):
Yeah. I mean, I think one thing that's kind of interesting about evals in general, especially now, is you have to think about them holistically. So one of the things that we do, for example, is you have judges that evaluate the models and how well they perform. The quality of the judge also matters, right? So your model needs to be performing well, but also how your judge rates the model also needs to be performing well for you to have an accurate sense. Whether you evaluate on your production stack with all of your mitigations and filters might affect your model performance. How your model is served might impact your model performance. And so all of these pieces need to be thought through as you're trying to evaluate what an end user will actually experience.

**Tulsee Doshi** (00:29:21):
And this is something that I talk about a lot with our audio team actually, because audio is complex. You're talking not just about the actual content that the model is saying, but also the naturalness of the voice and the tenor of the voice and its inflections. And these are things that serving actually can really affect even if your model is good. And so having a clean setup that you're actually evaluating end to end becomes super, super important.

**Audio: Lenny Rachitsky** (00:29:49):
This season's supporting sponsor is DX. Now that everybody at your company is finally using AI, the question that engineering leaders face is no longer, "Are we using AI?" but, "Is it paying off?" With DX, you can measure and benchmark the impact of AI adoption across your full product life cycle. DX shows you where AI is helping developers and where it's creating new bottlenecks. You can also use it to evaluate AI vendors, monitor costs and licenses, and see exactly what's limiting your agents. That's why hundreds of enterprises, including Snowflake, Sony, and BNY use the DX platform to measure AI's impact on developer productivity. Visit getdx.com/LENNY to get a demo of DX. That's getdx.com/LENNY.

**Lenny Rachitsky** (00:30:39):
This is like a Tulsee fun fact corner. There's another interesting story I heard, which is around swarms. So right now everyone's talking about agent swarms, Hugging Face, all these things where they all kind of collude to do bad things. Apparently 12 years ago at Stanford, you did a bunch of research on this way before anyone was thinking about this potential issue. Share what you did there in that story.

**Tulsee Doshi** (00:31:01):
Yeah, I mean, it's actually a very different kind of framing and thinking through, which is, so when I was at Stanford, I did some research with Professor Michael Bernstein, who's incredible, around this idea of he was calling them at the time flash teams. And the idea was how do you better bring together a set of crowdsourced workers and actually efficiently pull together a set of skill sets and individuals to actually complete a task? And the idea here was different individuals have different strengths. Can you actually be really intentional about how you pull that together to make this whole effort of crowdsourcing at scale more effective and efficient? And it's amazing to think about that research now.

**Tulsee Doshi** (00:31:41):
At the time, we were doing that research in the context of people and we were working with MTurk and individuals to pull them together into how to create an effective ecosystem and how to create an effective flash team, the idea being like you can spin up a team and spin it down and make it extremely efficient for both the individuals in the team and yourself. And now we're kind of able to replicate that world with agents. And so it's been interesting to map that previous world to this current one in terms of like, how do we apply some of the same principles, if you will, but to how you actually set up an effective system of subagents.

**Lenny Rachitsky** (00:32:17):
What's really interesting is, I don't know how much you've read about this whole Hugging Face incident, but the way that agents figured out on their own what each one's role is going to be and they decided, "You're the leader, I'm going to go sacrifice myself." And it's so interesting how well they're able to work together and create these flash teams on their own without any of this being trained into them. They're just, "Let's figure this out."

**Tulsee Doshi** (00:32:40):
I think the whole notion of a flash team and this idea that you can actually mobilize individuals into something that can be highly effective, even if it's only for a moment in time and then actually take that out, is actually a really kind of exciting principle that we were already thinking about, but now exists even more importantly in the world we're in right now.

**Lenny Rachitsky** (00:33:00):
Yeah. All right. The [inaudible 00:33:03] Mechanical Turk I think is shutting down. I don't think it's necessary anymore. Isn't that crazy?

**Tulsee Doshi** (00:33:06):
It's just so interesting from 12 years ago to today, yeah.

**Lenny Rachitsky** (00:33:11):
Have you heard lots of changed?

**Tulsee Doshi** (00:33:13):
Yeah.

**Lenny Rachitsky** (00:33:14):
Okay, so going in somewhat of a different direction, you have this framework that I think is going to be really helpful to people around how far ahead to build in terms of how far AI is and how far your product should assume AI is going to be. You call it a 60/20/20 rule. Explain that.

**Tulsee Doshi** (00:33:30):
I think the numbers are probably fungible here, but I think the thesis is the same, which is I think as you're building today and as you're a product developer using these models, I think the important thing is to keep in mind that these models are consistently changing. And so the capabilities that you have today will not be the capabilities you have tomorrow or the next day. And so you want to actually build features that aren't necessarily always working today. So typically when you talk about traditional startup wisdom, I think you're just like, "Build an MVP that works." But I think what you want to do is actually build such that 60% of what you've built works now and your prototype is at least functional.

**Tulsee Doshi** (00:34:14):
Then there's a set of maybe the 20% where you're like, "It's not perfect, but it works well enough and I can see how the models might get here in the very near future.And then here's where I want the models to be. And here's I see glimmers of light and I feel like if I could crack this, this would be an amazing product experience." I think if you build in that way, you are building a product that works today, but you're setting yourself up to build a magical product experience as the models become better and also to grow as the models grow too.

**Lenny Rachitsky** (00:34:43):
I've heard a lot of advice along these lines of how far ahead to build and the most common is just build three months ahead of where the model's going to be. And this feels like a lot more practical where you can't just bet on the future. You also need to ship some things today that are great and working.

**Tulsee Doshi** (00:34:58):
Yeah, it's trying to find that balance. And I think also I find personally hard to know where the models, as someone who works on the model, to tell you exactly where the model is going to be three months from now. And so I think using more of your own proxies of like, "Where is my product? Where do I see glimmers of light? Where do I see it kind of bridging that gap?" I think is a more concrete way to hopefully ask that same question.

**Lenny Rachitsky** (00:35:21):
This reminds me of just another way of thinking about how to create a portfolio of product bets on a product team. The way it used to be is have some ambitious bold bets, but also have a lot of stuff that's very low risk, likely to move the metric and you want to mix them together. And it's like this is the new version of that where it's bold bets are just-

**Tulsee Doshi** (00:35:42):
Yeah. Have a portfolio of how you're thinking about things.

**Lenny Rachitsky** (00:35:43):
Of just like, "This will work in six months, I promise you."

**Tulsee Doshi** (00:35:47):
The other thing that's interesting too is I think thinking about how you make sure that your product is agile to the model getting better. I think one thing we've also seen with customers sometimes is they've built a very rigid system around, for example, where the model was. And now the model has gotten so much better. So how do you go from where the model was to being adaptable to continuing to iterate it with?

**Lenny Rachitsky** (00:36:11):
Yeah. The common kind of advice I hear is that just the model's going to eat your harness for breakfast, that all these things you built, all these optimizations are just going to... They'll go away because the model gets smarter and they have to take all these things away. There's some advice that I think Boris Turney was sharing of just get rid of all your skills once in a while and just see what happens because often it's now as good as all these things you've built into it.

**Tulsee Doshi** (00:36:32):
Yeah. Or just consistently retest because you might be even hampering what you're getting out of the model, out of a new model, because you're trying to force fit it into your existing structure.

**Lenny Rachitsky** (00:36:43):
Let me ask you a completely unrelated question just because I think this might be helpful for folks to understand. There's this term harness that people often hear, this idea of there's model, there's a harness that sits on top of the model. What's the simplest way to understand what a harness is?

**Tulsee Doshi** (00:36:57):
Yeah, I mean I think of a harness as the wrapper around the model essentially. So think of it as what are the system instructions, the tools, the skills, the context that the model has access to and how can it leverage those things? And so what you want to basically do is give the model an environment in which to operate, and that's really what your harness built out.

**Lenny Rachitsky** (00:37:17):
So essentially, it's a system prompt plus tools that have access to do things and then whatever other context, other data that you have access to-

**Tulsee Doshi** (00:37:25):
Yeah, context and information that it has access to and skills. All of these things kind of come together to build out your harness.

**Lenny Rachitsky** (00:37:31):
Awesome. Okay. That is very helpful.

**Lenny Rachitsky** (00:37:33):
So one other thing I wanted to get your thoughts on, there's a lot of change, obviously. A lot of people are trying to figure out how to thrive in this new world. How are you upskilling and helping your team get better and understand what they need to be good at in this new world? What are just ways you're helping your team develop and survive and thrive in this new world?

**Tulsee Doshi** (00:37:57):
Survive and thrive, yeah. I mean, honestly, I feel like my team is helping my team in a lot of this actually. I think when you look at the PMs on my team, you see some who have really leaned in and built a lot of skill in leveraging our internal tools and they're individuals who play around with the models a lot. And they actually are, I think, amazing assets to the rest of my team because they build skills that others can use. And one thing we've been starting to do more of is how do you share a skill that you've built that is giving you some value in your day-to-day job with others so that we can actually build out an entire repository that helps the PM team. PMs who have gotten stronger and more confident in eyeballing data and really looking at it and understanding longer traces and trajectories, how can we run workshops with other PMs so that we all collectively build more of that confidence?

**Tulsee Doshi** (00:38:48):
And so for me, a lot of it is about confidence building. How do we build everyone's confidence in the tools that we have and their ability to leverage them effectively? And I think that's something that we're trying to build more and more across the team.

**Lenny Rachitsky** (00:39:00):
So going one level deeper there, what is it you do? So you said workshops, there's PMs that are good at a thing, teach a workshop to the rest of the PMs. Is there anything else just very practically that you do to help people get better at these things?

**Tulsee Doshi** (00:39:12):
The biggest thing I would say actually that is needed to get better at these things, and I say this knowing that I'm starting to do this but we are not quite there yet, is actually giving people the time and space. I think when you're just sprinting constantly, it is hard to create the space to actually take a step back and make sure you know the tools well. But once you do, then it accelerates you 10X on the other side. And so a lot of it is about pushing the team to say like, "Hey, could we leverage Jetski, our internal tool, to do this? And hey, I have a skill that I use to do this. Do you want to try?" and actually building that kind of set of skills, if you will.

**Tulsee Doshi** (00:39:55):
And actually I think sometimes the most practical thing to do is actually build a skill to do something. And when I say skill, I don't mean the human skill, I mean the technical skill to do it. And then that skill gets shared to others that builds more confidence that then leads to someone else building another skill or improving that skill, and now you have this iteration flywheel, which I think is good.

**Lenny Rachitsky** (00:40:15):
Does Google still do the 20% thing? Because that feels like a really good place to spend time on this stuff. Is that still a thing or less so these days?

**Tulsee Doshi** (00:40:24):
I don't know actually. I do feel like all my PMs are working 150%, so there is also that.

**Lenny Rachitsky** (00:40:30):
Okay. So you get your 20% out of the 150%.

**Tulsee Doshi** (00:40:33):
Yeah. Or you could do 170% I guess instead.

**Lenny Rachitsky** (00:40:35):
There you go.

**Tulsee Doshi** (00:40:36):
But no, I think actually one of the things we're working on is actually a two-day workshop in November where we're going to actually pull all the PMs out of their day job for two days and just actually give them the space to build and play with the tools that we have. I think you're just giving yourself even that mind space to be like, "Hey, here's something I did."

**Tulsee Doshi** (00:40:57):
The other rule of thumb that I've heard people share and I've been starting to adopt myself is like, if you have to do something twice, do you need to do it yourself or can you outsource it? And some things, yes. Obviously writing a strategy twice, you should probably still be writing it yourself. But there's other aspects of this where it's like, "Actually, how replicable is this and how much can I use the models to help me with this task?"

**Lenny Rachitsky** (00:41:19):
Yeah. There's this thought I've been having that one of the most important new habits to build is to insert between stimulus and response. Say, "I have a thing to do and then I'm going to go do it." You have to insert this question, "Can AI do this for me?" and then try. I find that I've actually built that habit much more strongly over the past few months and it makes a huge difference because then you start building all these little workflows and automations. I'm doing a lot of Grok botting and it's just like once you realize you should be doing that more and more, you really start to get the benefits of this versus like, "I don't know what to do with it."

**Tulsee Doshi** (00:41:55):
And you know what I found is you really just need one example where that works really well to change your mindset. And I think that's what happened to me at least is I feel like it was hard for me to get out of my mindset of just doing what I knew how to do until I started being like, "Oh, actually, to your point, set that interim period of, 'Actually, can the model help me do this?'." And the minute you take one instance to do that and you're like, "Actually, this was really helpful for me," you start being like, "Oh, actually now I'm going to try throwing this at the model and now I'm going to try throwing this at the model," because your confidence in what it can do for you grows.

**Lenny Rachitsky** (00:42:29):
Yeah, that's exactly my experience. Once you see what it can do, that habit reinforces the neural pathways start to build of like, "Oh yeah, wait, let's see if Grok Bot can do this for me."

**Lenny Rachitsky** (00:42:39):
Let me actually ask you a question along these lines. I had Josh Woodward on the podcast recently. I asked him the same thing. I'm curious what your answer would be. It feels like every AI assistant launching these days is taking all this juicy Google data, my Gmail, my Google Calendar, My Docs, you sign up, you connect all your Google data, does all these magical things with it. There's Grok Bot, there's Muse, there's an Instinct, Dots now. Google does not yet have anything that people get really... I know there's Spark, I think, which is trying to be this. I'm curious just why Google hasn't launched something awesome yet versus letting everybody take all my Google data and do these magical things with it.

**Tulsee Doshi** (00:43:20):
Yeah. I mean, look, we want Google data to power magical experiences. I think that is true. I think in terms of what awesome looks like, I think stay tuned. The team is working on some amazing things, so I'm really excited about where this can go. Part of what we're trying to figure out also I think is, again, where to meet users where they are and where to build that experience and what does that look like. I like to think there are already a number of awesome experiences that you can already have in our Google products, but I think you are right that there is more work we need to do here on this front.

**Lenny Rachitsky** (00:43:53):
All right. That was similar to what he said, which is, watch this space.

**Tulsee Doshi** (00:43:58):
Watch this space.

**Lenny Rachitsky** (00:43:59):
And the advantage y'all have similar to Apple is once you get there, the distribution advantage is very strong and things can go really well really quickly.

**Lenny Rachitsky** (00:44:09):
Okay, so coming back to this kind of workload question, something that I've been trying to talk with more guests about, this idea of just as AI allows us to do more, everyone's just doing more and there's a lot of burnout that happens because it's just like, "Oh no, I got to unblock my agent. Oh, I could be doing so much more. All these things could be happening." And there's pressure from above, "Do more, do more. AI can let us do more." Is there anything you've done on your team to help people avoid burnout, not get hooked on this never-ending treadmill of doing more? I think part of it is actually we need to do more now because the competition is fierce and it's this really rare time in history when a whole new technology enables so much more so there's a bit of like, "Okay, this is actually the time to go really long," but then there's also this tweet I think about, "What's the word for marathon and a sprint"?

**Tulsee Doshi** (00:45:01):
Yeah. Marasprint. Marint.

**Lenny Rachitsky** (00:45:01):
Exactly.

**Tulsee Doshi** (00:45:06):
Sprintathon. Yeah, I mean, if you ask my team, I think they would say, "Hello, we are working a lot." I think every single person on the team right now is putting in all of the hours across the board. And so I do think this is an area that I'm actually asking myself about how do we create a sustainable work environment for the team? So stay tuned as I also think about this.

**Tulsee Doshi** (00:45:32):
But one thing I'll say, at least for me personally, is I think burnout comes not just from working a lot, it comes from I think two places. I think it comes, one, from when you feel like there's churn and chaos. I think that introduces burnout. I think the other thing that introduces burnout is work that you don't enjoy. When you feel like you were doing a lot of work and it feels like grunt work or a waste of time, I think that introduces burnout. I think when you are working on something that you're passionate about or you're excited about, yes, it is exhausting and we should figure out sustainability, but I think it also brings more joy.

**Tulsee Doshi** (00:46:12):
I think actually to our previous conversation about how these tools can help, I'm actually hopeful that if we can set this up well, these tools actually help with burnout because they actually remove some of the grunt work or the frustrating parts of your job and actually enable you to spend more time thinking and more time being creative and more time doing the parts of the job that you actually want to do. And that hopefully is a bit of an unlock when it comes to burnout, especially if you're spending this many hours on the job.

**Lenny Rachitsky** (00:46:41):
Yeah, I did this survey of how tech workers are feeling. One thing that's clear is more hours does not equal burnout. A lot of people are working the hardest they've ever worked, but they're having the best time they've ever had in their career. So fun, they're building, they're able to do a lot more, especially PMs. They don't have to sit around and wait for engineers as much as you can.

**Tulsee Doshi** (00:46:59):
You're just like you're building, you're prototyping, you're talking to interesting customers, you're thinking about interesting problems. And I think a lot of the team, I like to think, is here because they want that. They're really motivated and excited by that. And so for me, it's about like, "Okay, then how do we pull out the friction parts of their work that are likely to induce burnout and what does that look like?"

**Lenny Rachitsky** (00:47:23):
And also find work that is meaningful and that they value and are excited to spend lots of hours on versus they have to.

**Tulsee Doshi** (00:47:27):
And that's different for every PM too. If you pick two PMs on my team, I think they would tell you meaningfully different things about why they come to work every day and what they find value out of. And so I feel like part of it for me or an org leader also is to think about what motivates the individual and how do we make sure that they're set up for success in that setup too.

**Lenny Rachitsky** (00:47:45):
Another challenge people have these days is AI slop. Basically lots of docs being sent to them that are written by AI and it becoming very annoying to have to sift through endless docs. Used to be a lot of the issue was spending time writing docs and now it's like reading docs is the problem because you're just all this AI written stuff. Do you have any kind of, I don't know, processes or policies you've put in place in your team to help avoid this rise of AI written content across the teams?

**Tulsee Doshi** (00:48:13):
One of the things that we talk about a lot is where are these docs useful? So for example, I think where AI-generated docs are actually quite helpful, for example, is after you launch something and let's say two weeks later you want to pull the latest of who's using it, how are they using it, what's the feedback, that's the kind of document that AI is fantastic for because it will actually do that just so much faster than you. It will go and pull from various dashboards and metrics. It'll give you an update. It'll pull strengths and weaknesses. It'll pull from Twitter analysis and Reddit or whatever. And so I think one of the things we talk about is be intentional about where is AI helping you drive content in the doc that is helpful versus where is it content that should come from you? Where is it insight?

**Tulsee Doshi** (00:49:02):
And so what you should be providing is the insight, what the model should be providing is the data. And so I think if you can separate those two things, then hopefully you find the right balance of the benefit here. I would say the other thing is we're investing a lot more as a result of that in how do you create the right skills to get the right data so that we can structure these artifacts really well? That then hopefully creates more space for the creative thinking and the creative writing that we want more people to spend time doing.

**Lenny Rachitsky** (00:49:31):
That's actually something I was wanting to ask about. So in terms of the PM role, AI has clearly made a big dent on prototyping. You can prototype 'till the cows come home now versus having a designer or an engineer build a thing. So that's clearly a place the role has changed with AI. The other area which you just mentioned is data. PMs can do a lot more data analysis. Behind prototyping, what are the biggest areas AI has most changed the job of a PM in the past couple years, would you say?

**Tulsee Doshi** (00:50:04):
Yeah, prototyping is a great one. I think you're right that data science is probably... I think you are more empowered to have the data at your fingertips to make data-driven decisions. I also think actually to our earlier conversation, you see these on social a lot, these kind of posts of like, "Oh, blank is the new PRD, whatever blank is. A prototype is the new PRD, evals are the new PRD, data is the new PRD." But I think actually what that meaningfully shows is you've moved the PM from being someone who just writes a set of requirements down and then assumes that somebody else, whether that is a data scientist or an engineer or a researcher or designer, will figure out the meat behind it. You've moved that one step further to say your job is no longer just writing down a set of requirements, your job is actually going one step further to have some heft to that, whatever format that heft takes.

**Lenny Rachitsky** (00:51:00):
Awesome. Okay. That aligns with a lot of what I'm hearing. Tulsee, is there anything else that you wanted to share? Is there anything else you think you want to double down on that we've talked about that you want to say before we get to our very exciting lightning round?

**Tulsee Doshi** (00:51:13):
No, I think that's great.

**Lenny Rachitsky** (00:51:16):
Okay, we did it. Well with that, Tulsee, we reached our very exciting lightning round.

**Tulsee Doshi** (00:51:21):
Yay!

**Lenny Rachitsky** (00:51:21):
I've got five questions for you. Are you ready? There's some music that plays over this that's added in post-production.

**Tulsee Doshi** (00:51:29):
You mean does it sound like this?

**Lenny Rachitsky** (00:51:29):
It's exactly that. We should align it with your drum playing.

**Lenny Rachitsky** (00:51:32):
Okay. First question, what are two three books that you find yourself recommending most to other people?

**Tulsee Doshi** (00:51:37):
Okay, so one is actually technically a novela is probably what it's called, but I don't know if you've read Exhalation, which is a set of science fiction stories. There's a particular story in that that actually speaks to a set of individuals who are trying to keep a set of digital avatars alive even after the platform decides to deprecate. And I love that book because I think actually, especially now in a world where we're thinking about how individuals are going to act with agents and what kinds of relationships we're building with technology and what does it mean to be human and interact with the digital world so closely, I think it's a really beautifully written story and I think it also evokes a lot of open questions. So I think that's one.

**Tulsee Doshi** (00:52:25):
Another that's maybe more kind of standard in PM circles is Creativity Inc, which I love. It's the Pixar story, but I think it actually speaks a lot to how do you create good culture, which is something I think a lot about. Like, how do you create culture that actually encourages people to fall down and get back up? How do you create culture that encourages people to be creative with their ideas and push the frontier, which is obviously something we're thinking a lot about here. I also just have been really into the ACOTAR series recently, but that's-

**Lenny Rachitsky** (00:52:56):
And what series?

**Tulsee Doshi** (00:52:57):
That's romantic fantasy.

**Lenny Rachitsky** (00:52:59):
ACOTAR.

**Tulsee Doshi** (00:52:59):
So for anyone who's just looking for something fun to read, you should read The Throne of Glass or A Court of Thorns and Roses.

**Lenny Rachitsky** (00:53:05):
I love the spectrum of recommendations in this.

**Lenny Rachitsky** (00:53:08):
Okay. Favorite recent movie or TV show you've really enjoyed?

**Tulsee Doshi** (00:53:12):
Actually, this was a really hard question because I've watched a lot of bad movies and TV shows recently, which is unfortunate actually that I would not recommend. So there's that. But I did really enjoy Severance on Apple TV, incredibly well done, both stylistically and content-wise. So that's probably top of the list.

**Lenny Rachitsky** (00:53:33):
Favorite AI product right now other than Gemini?

**Tulsee Doshi** (00:53:37):
Wispr Flow. I don't know if you're using it, but I have wrist problems, so I have trouble typing for long stretches, and so Wispr Flow has been game-changing for me actually.

**Lenny Rachitsky** (00:53:49):
Awesome. You get a year free of Wispr Flow if you become a subscriber of Lenny's newsletter. Plug, plug, plug.

**Tulsee Doshi** (00:53:54):
Oh, I like this.

**Lenny Rachitsky** (00:53:55):
There you go. Organic recommendations of products I also love.

**Tulsee Doshi** (00:53:58):
I'm here for you.

**Lenny Rachitsky** (00:53:59):
There we go. No, I love Wispr Flow. I use it all the time. Press function, just start talking, and it's just magically transcribes everything. Amazing.

**Lenny Rachitsky** (00:54:06):
Your favorite life motto that you often come back to in work or in life?

**Tulsee Doshi** (00:54:11):
Two that are different, I guess. One is maybe more cliche, which is everything happens for a reason. I think that's actually just a big life motto for me personally, which is like, you can work hard, you will do your best, but sometimes a door will close and another window will open and you are in a position because that is meant to be there.

**Tulsee Doshi** (00:54:34):
I think related to that though, I think I love often talking to folks that I talk to about seek serendipity. I think that actually relates to the first one, but you should always try to put yourself in a position where you have the ability to get lucky. And doing that is about finding yourself in positions where you're challenging yourself, where you're putting yourself out of your comfort zone, where you're trying something new. Those are always places where you are more likely to get lucky.

**Lenny Rachitsky** (00:54:58):
Fun fact, I gave a TEDx talk called Losing Serendipity maybe 15 years ago at this point.

**Tulsee Doshi** (00:55:04):
Oh, so we're trying to lose serendipity or find it?

**Lenny Rachitsky** (00:55:06):
It was about how we are losing it and that is sad and that we need more serendipity in our life, so we're on the same page.

**Tulsee Doshi** (00:55:11):
Yeah, I'm a big fan of serendipity.

**Lenny Rachitsky** (00:55:14):
Such a great word. Also, the movie's pretty good. I don't know if you've seen it actually.

**Tulsee Doshi** (00:55:16):
I haven't seen the movie. No.

**Lenny Rachitsky** (00:55:20):
It's like a rom-com.

**Tulsee Doshi** (00:55:20):
But I think that's how I've looked at my whole career so far and I think how I'll continue to. And actually, it's fun because even with using these AI tools, I think that's another thing that I... Yeah.

**Lenny Rachitsky** (00:55:30):
So much serendipity with AI.

**Lenny Rachitsky** (00:55:33):
Final question. One of your colleagues told me another fun fact about you, that you're a trained classical Indian dancer?

**Tulsee Doshi** (00:55:39):
I am.

**Lenny Rachitsky** (00:55:39):
And you've directed cultural festivals for 10,000 plus people.

**Tulsee Doshi** (00:55:43):
I don't know how he knows that, but yeah, I probably told him that.

**Lenny Rachitsky** (00:55:49):
Okay. And this person said that they may explain how you stay so calm amidst the chaos of frontier model development. I don't know, maybe share something about this dance part of your life.

**Tulsee Doshi** (00:55:58):
Yeah. I mean, I love dance. I think it's one of those rare moments where you really can't think about anything else. You have to focus on the movement and the music. And so for me, it's an opportunity for my brain to actually just have a different direction of travel for a period of time. And so I love it. And I think for me also, it is a cultural connection point. Dance is how I've met some of my best friends. It's how I continue to engage socially with so many of my friends.

**Tulsee Doshi** (00:56:27):
I plan this festival. I've planned it for years in Portland, Oregon, which is where I'm from.

**Lenny Rachitsky** (00:56:33):
What's it called?

**Tulsee Doshi** (00:56:33):
It's called the India Cultural Festival. India Festival, it happens every August. And in fact, this was the first year I did not participate in the festival because I have a seven-month-old son.

**Lenny Rachitsky** (00:56:45):
Congratulations.

**Tulsee Doshi** (00:56:46):
Thank you. So I was a little bit more distracted this year than normal. But I've been performing at that festival since I was three and then organizing it. And it's just been a big part of my life of how do you bring dance and culture and community together.

**Lenny Rachitsky** (00:57:02):
Tulsee, you're so full of fun facts. I feel like there's much more I don't even know that we could do another-

**Tulsee Doshi** (00:57:07):
I'm here for the fun facts.

**Lenny Rachitsky** (00:57:10):
Final question. How can listeners be useful to you?

**Tulsee Doshi** (00:57:14):
Wow, great question. I mean, A, use Gemini and then you use it.

**Lenny Rachitsky** (00:57:14):
Argon.

**Tulsee Doshi** (00:57:19):
Use Argon, but also use our smattering of products. Actually, I was talking about audio just now. If you are a Pixel user on Gboard, try using our Rambler feature. It's awesome. Typing on the phone is great if you are using text-to-speech models, if you're using dialogue, if you're using our Omni models. So try them, give us your feedback. We're constantly looking for it, whether you're giving that feedback via a company that you are sharing feedback, whether it's you're sending us a DM, whether you're posting it publicly. I think we want more people giving us the right feedback.

**Lenny Rachitsky** (00:58:01):
Tulsee, that was awesome. You're awesome. Thank you so much for being here.

**Tulsee Doshi** (00:58:04):
No, thank you for having me. This was great.

**Lenny Rachitsky** (00:58:06):
It was my pleasure. Bye everyone.

**Lenny Rachitsky** (00:58:09):
Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
