---
title: "OpenAI Codex lead on the new shape of product work | Andrew Ambrosino"
date: "2026-06-28"
type: "podcast"
guest: "Andrew Ambrosino"
post_url: "https://www.lennysnewsletter.com/p/openai-codex-lead-on-the-new-shape"
description: "The new shape of product work, covering product design, engineering tradeoffs, and AI product work."
word_count: 13903
---

**Andrew Ambrosino** (00:00:00):
90% of people at OpenAI use Codex. Not 90% of engineers, that's 90% of the entire company.

**Lenny Rachitsky** (00:00:06):
Yeah, this tweet the other day where you said that you intend to make Codex the best desktop app that has ever existed.

**Andrew Ambrosino** (00:00:12):
Yeah. The quality bar for Codex had to be so high that there was never a hesitation that you have opening this app to do the next thing. That this was your natural choice. Just like people have kind of come to open a browser tab, right?

**Lenny Rachitsky** (00:00:24):
That's true. I know there's numbers constantly coming out about the records you guys are setting for usage.

**Andrew Ambrosino** (00:00:28):
I don't know. We'll see. A lot of people seem to like the app.

**Lenny Rachitsky** (00:00:31):
Why do you think AI and the top frontier models are just not good at design?

**Andrew Ambrosino** (00:00:36):
I think design's a little bit harder to grade because the human aspect of taste is part of the feedback mechanism you need. That is still feeling a little out of reach with the current technology.

**Lenny Rachitsky** (00:00:46):
What does the shape of product team look like now versus a couple years ago?

**Andrew Ambrosino** (00:00:50):
Everybody at OpenAI is very agentic, has great ideas, and so everybody's building everything. And it's not that people are doing fundamentally different roles or focusing on different things, it's that it's backwards. The implementation is actually not the expensive part anymore. It's, dare I say, taste.

**Lenny Rachitsky** (00:01:05):
Do you feel like there's this collapse coming where everyone's everything and that's just the feature? Or do you think we're going to continue to be mostly divided up?

**Andrew Ambrosino** (00:01:11):
There are some things that I'm afraid of. I've heard a lot of companies be like, "We're getting rid of the product role and everybody's just going to be a builder." And then what happens is...

**Lenny Rachitsky** (00:01:22):
Today, my guest is Andrew Ambrosino, product and engineering lead for the Codex app at OpenAI. Codex is quickly becoming people's go-to app for building products and also for non-product work like organizing files in your computer, drafting documents, doing data analysis, reading your emails, and a lot more.

**Lenny Rachitsky** (00:01:39):
If you stick around for the end of this episode, we actually have a little clip from after we stopped recording where the producer in the room started talking about how he uses Codex in his editing work.

**Lenny Rachitsky** (00:01:49):
Since this January, Codex usage has grown 6X. They currently have over five million weekly active users. I suspect this number is quickly going to be out of date. Internally at OpenAI, nearly 100% of their employees use Codex weekly and that is not just the engineers.

**Lenny Rachitsky** (00:02:06):
Andrew is a designer, turned engineer, turned product manager, who's building the app that more and more of the world is using to build their own products.

**Andrew Ambrosino** (00:02:37):
Thank you for having me.

**Lenny Rachitsky** (00:02:38):
This is a rare in-person podcast. I rarely do this kind of thing. We'll see how it goes.

**Andrew Ambrosino** (00:02:42):
We'll see.

**Lenny Rachitsky** (00:02:42):
We'll see if people like these more. When we were preparing for this chat, I asked you what's the biggest thing you want people to get out of this conversation? And you said that it was how AI is changing the shape of product work.

**Lenny Rachitsky** (00:02:52):
You're working at maybe the most bleeding edge, AI-pilled software team there is. So you have a really interesting lens into where things are heading, where other teams are going to be in a year or two or more. What does the shape of product team look like now versus a couple years ago?

**Andrew Ambrosino** (00:03:09):
One of the hardest things to do right now as a leader building these products is just sort of the inversion of the process in my mind, which I think a lot of people have talked about, which is that anybody can build anything. I generally believe now that starting from scratch, if you talk to these models, ours, anybody else's really, you can stand up whatever feature you want. And that's not necessarily a hard part of software, but that's really cool.

**Andrew Ambrosino** (00:03:44):
And I think that has created an environment where people are making all of this. You give people unlimited tokens. Everybody at OpenAI is very agentic, has great ideas. And so everybody's building everything. Whereas I think you look back at product process that we've all run for a long time and it's been a little bit opposite. It's been kind of research, ideation, maybe there was some prototyping. But it was even when we got past waterfall, it was still kind of flavored of the implementation is expensive.

**Andrew Ambrosino** (00:04:20):
And so what you want to do is you want to de-risk all implementation upfront through documents, through research, through prototypes. Because prototypes and designs are cheaper was kind of the assumption there. And that's changed. That's totally changed.

**Andrew Ambrosino** (00:04:35):
And right now I'm sure there are 90 different explorations for... There's this feature that we desperately need to do that I'm sure there are 90 different uncoordinated teams implementing and trying, right?

**Lenny Rachitsky** (00:04:48):
Yeah.

**Andrew Ambrosino** (00:04:50):
So I guess the short answer is it's backwards. And it's not that people are doing fundamentally different roles or focusing on different things or that even skillsets have vanished or that roles have just disappeared. It's that it's backwards. The implementation is actually not the expensive part anymore. It's, dare I say, taste.

**Andrew Ambrosino** (00:05:07):
But it's the curation process. It's like of those 90 attempts, what's good about these? What should we fold into other aspects of this? How should we frame this? Should it be part of this other feature? How many segments should be in the toggle? All of those things.

**Lenny Rachitsky** (00:05:23):
**Andrew Ambrosino** (00:06:46):
Yeah.

**Lenny Rachitsky** (00:06:46):
Here's what we're going to build, here's the feature, here's the strategies, PRD. Today, what you're describing, which makes all the sense, is people just create a prototype. And what you're saying is people across the company have kind of similar ideas. And now instead of a doc, they create their little prototype. And that leads to kind of 90 different things people can look at and maybe pick here's a direction we want to go down. Is that the idea?

**Andrew Ambrosino** (00:07:05):
Yeah. There's a lot of this. And it's not just happening here. You've seen many product leaders say PRDs are dead and prototypes are in. And I actually don't believe this at all.

**Andrew Ambrosino** (00:07:17):
I think that one of the interesting things that is happening right now is that because implementation has gotten so cheap across every medium, it's very tempting to jump straight to a prototype. Especially if you're not an engineer. Especially if you've never been able to write code or never been interested or never had the time, it's really tempting to say like, "PRDs are dead. Let me just show you what I mean."

**Andrew Ambrosino** (00:07:45):
What I've also noticed though is that for engineers, it's really tempting to write a lot of documents, a lot of documents that are not worth reading. This is no shade on people writing documents. It's that if implementation is abundant, then it's really important to pick the right format for the point you're trying to make.

**Andrew Ambrosino** (00:08:05):
If that point is product clarity around a vague area, then it might actually be a document. If what you're trying to do is get something in people's hands to try out and to stress test an interaction pattern, it's a prototype. But I think this is kind of the funny thing now, which is that it's really important to pick the medium.

**Lenny Rachitsky** (00:08:28):
There's this term that a podcast guest shared that I think about when you say this, which is it's called the primal mark. When a designer or a painter or an artist just creates the first mark on a painting or a piece of art, that mark is what you start to respond to. And so everything kind of trickles down from that first mark you make.

**Lenny Rachitsky** (00:08:47):
And what I'm hearing you saying is sometimes the prototype is the wrong first thing to do because then you're just responding to this prototype versus a different idea versus a bigger idea. So I love hearing this. So everyone's just like, "Okay, forget it. No more writing, no more docs, no more PRDs." You're saying, "They're actually still useful for specific use cases."

**Andrew Ambrosino** (00:09:04):
Yeah. I think too, there's this part of the previous world was that the medium implied it had baked in a lot of signal around where in the process something was. So if you're seeing something that feels like the app in production, that means that it's late in the process. That assumptions have been de-risked, that design has looked at this, that this is a good business goal.

**Andrew Ambrosino** (00:09:32):
And now those things are sort of divorced. And the reason it was that way is because it was hard to get resources to build the thing until it was properly de-risked. And now that's just out the window. And so I think it's really important to start saying, "Look, we can have prototypes. We can have documents. Are we clear around what this is doing?"

**Andrew Ambrosino** (00:09:51):
Because to your point, you do not want to over anchor on this thing that was meant to be an exploration, but now it looks so production ready that, oh, visually it's ready for prod. But it's not actually the right model of where the research is going or what users are asking for or what's right for the business.

**Andrew Ambrosino** (00:10:08):
Not to overdo the taste thing, but it's once again, it's like the taste to know what to work on, how to present that information, how to achieve the goals, what medium to use is emerging as the most important thing to do. And that's in every field.

**Lenny Rachitsky** (00:10:26):
What is taste when you talk about good taste? Is it what you described deciding here's the thing we're going to invest in? Is it also once you have a thing, is this right? Is this the thing to shift?

**Lenny Rachitsky** (00:10:37):
Talk about when you think about what is good taste, good judgment, what is that concretely? Because people hear this word, they're like, "Oh, I have good taste. I know it." What does it look like in practice?

**Andrew Ambrosino** (00:10:46):
Yeah. It's funny. There was a tweet, I'm too online. There was a tweet, I think it was yesterday from the head of product at Linear, I might be getting that wrong, sorry to anybody, who said, "People overemphasize the aesthetic part of what taste means." And they used, Paul Graham's great, but they used him as an example. Saying, "Paul Graham clearly has great taste and wears cargo shorts."

**Andrew Ambrosino** (00:11:11):
We got to tease out what taste means a little bit and there's a lot of nuance here. I think it's all of the above to what you mentioned. There is an aesthetic part to it, but there's also a systems thinking part of it, like how does this fit in the system? There's a where are we going and what theme is this part of? There's how to present this.

**Andrew Ambrosino** (00:11:35):
A lot of it is wider context. And obviously there are parts of taste that are like, "Hey, this interaction animation doesn't fit in the semantic meaning it's supposed to." It's too snappy for what it's actually trying to convey. And that's incredibly important and I focus probably too much on that.

**Andrew Ambrosino** (00:11:52):
But there's the like, "What should this be?" If we can build anything, what's the goal here and how do we get there? That I think is actually the real taste question here.

**Lenny Rachitsky** (00:12:06):
When I hear things like this, I always wonder where will human brains continue to be valuable as AI becomes stronger and better and doing more of the work? And it feels like taste is a part of it. Something I think about along these lines is just AI is still very bad at actual design. The output of AI is not great.

**Andrew Ambrosino** (00:12:24):
Yeah.

**Lenny Rachitsky** (00:12:24):
Rarely is it like, "This is it, they nailed it." And it's always like, "Oh, this is Claude Design, this is Codex Design." Why do you think AI and the top frontier models are just not good at design today? And do you think they'll get there? Do you think we'll get to a place of like, "Holy moly, we're done."

**Andrew Ambrosino** (00:12:40):
Yeah. I tend to think that there are some practical reasons why it's lagged and also some harder problems to crack. I'm not in our research org, I'm sure I'll get yelled at for saying us. I think design's a little bit harder to grade than software. And that creating a loop where you can train the model and what's good design and what's bad design is just a little bit more tedious and onerous than does the code compile, does it do what it's supposed to?

**Andrew Ambrosino** (00:13:09):
Because the human aspect of taste is part of the feedback mechanism you need. I also think that the labs historically invest in making their models good at things that accelerate AI research. And that in the early era of coding models, it was very clear that the model being able to write correct code would accelerate research. In a way that you can't really make the same case for design. Not that getting good at design isn't important, it's that it's not directly in that flywheel.

**Andrew Ambrosino** (00:13:46):
Those are practical reasons and those will go away. These models will get pretty good at design. There are some kind of murkier things that is going to be really tough. I have kind of a short list of them. One is there is an aspect of culture to what is considered good design. In that you remember it was probably what last year where every new website that came out was just a copy of Linear's website.

**Andrew Ambrosino** (00:14:15):
Linear's website, great design, great taste. If a model did that, I'd be like, "Wow, this is incredible leaps here." If I have a model that outputs Linear's website every time, that's not the challenge here. There's an amount of novelty that is more important in design than it actually is in software engineering. Software engineering, you must want it to over-index unknown patterns. Whereas design, it's like, "No, there's an element of randomness here and novelty."

**Andrew Ambrosino** (00:14:48):
To me, I spent a lot of time writing code or supervising code on the early Codex app. And even as the models get good at design, there's sort of an abstraction layer that is an interplay between the software design and the code that's being written. This thing over here in this corner should share X, Y, and Z in the code base with this thing down here.

**Andrew Ambrosino** (00:15:14):
And that's a little bit different than saying the model needs to be a better designer. Especially that is visual design, but it is significantly deeper. It's about the abstractions in that like, "Oh, if tomorrow our company did a rebrand, the shallow version of this is that we have to update 263 components one by one." The deep version is the semantics between these two things that look different. They're both in list that have this style, that convey this interaction pattern to the user.

**Andrew Ambrosino** (00:15:48):
And I think that is still feeling a little bit out of reach with the current technology, that abstraction layer. So I think as we've gone through this process of, we started the Codex app in November. And we weren't using it full-time, now we use it for everything. That's been a journey. But now it's like the things that we actually do while using it are different things. So what was the question?

**Lenny Rachitsky** (00:16:17):
I know, that was an amazing answer. Speaking of design and being creative, the Codex app when it came out, it's like such a new thing that nobody had seen before. It's not a terminal thing, it's not an ID thing. It's like this chat thing that codes and you could see code.

**Lenny Rachitsky** (00:16:32):
To your point, it feels like it'd be hard for AI to be like, "Here's a whole new paradigm for how to code." And that feels like where human brains continue to be valuable for now is creativity almost in coming up with something new versus patterns of things that have been done before.

**Andrew Ambrosino** (00:16:47):
Yeah, I mean, I totally hear you. Let's give it up for the human brain.

**Lenny Rachitsky** (00:16:50):
For now. As we were getting ready for this, you said that you were listening to the episode with Jenny who does the head of design for Claude Code and Cowork and such. And she had this whole kind of thesis that the design process is dead.

**Lenny Rachitsky** (00:17:02):
There's no time for design. Things are moving too fast. Just build now and design is kind of steering things as things move along. You're implying you have kind of a different perspective on the design process.

**Andrew Ambrosino** (00:17:13):
We probably agree on a lot of this, Jenny and I. I wasn't a fan of the design. The design process proper, I agree with her take that it is dead. I genuinely was not a fan of this process before AI.

**Lenny Rachitsky** (00:17:27):
Can you describe the process real quick just from people think about the design? What does that mean?

**Andrew Ambrosino** (00:17:31):
Yeah. So I mean, when I ran a startup a number of years ago, we would do design hiring. And there was this sort of snarky article that came out about the case study factory. And it was like mid-SERP era stuff and it was that designers were being taught about this process and valuing that above all else, above all outcomes even.

**Andrew Ambrosino** (00:17:55):
And if something went through this process that two things were true. One, it would be good and the process would guarantee quality and guarantee impact. And also that if something, the thing was good if it went through that process, even if you don't like it and nobody uses it.

**Andrew Ambrosino** (00:18:13):
And it's like the process of user research and the divergence and the convergence, it's the right framework. It was always a little academic. But I think this is really exposing some areas where it falls down, especially because of the speed of implementation.

**Andrew Ambrosino** (00:18:31):
And once again, that process is sort of predicated on the assumption that implementation is expensive and that you can really only afford to build once. And so you need to fully, exhaustively go through the problem space and the solution space before implementing.

**Andrew Ambrosino** (00:18:51):
And then we saw with Figma and Origami and all of these tools that you can fast-forward some of the insights by pulling interactive prototypes earlier into the process. That you can simulate production. And there ended up being sort of a meme about executives just being like, "Well, can we just do a prototype and then expect it to work?"

**Andrew Ambrosino** (00:19:15):
But this thing was real that this became part of the design process proper. We pulled prototyping into that. The problem now is that you can pull all of the implementation into that and there's a mismatch between, I think a lot of assumptions.

**Andrew Ambrosino** (00:19:31):
Again, you see this fully polished prototype that looks like it's ready to go out the door. And enough people at a company see that and they're like, "Can we release this now?" But the appropriate, we're actually in that early design process stage and nobody's just saying that. This is where we are with a bunch of multiplayer exploration.

**Andrew Ambrosino** (00:19:52):
90 people will have this idea. It'll look really polished, but it's like, "No, this is actually..." That's the design process now. Tying the design process to mediums, media, that's the scary part. It's that designers have more tools now to do this process with.

**Andrew Ambrosino** (00:20:12):
You can put stuff into the current product and you can A/B test it or just use that as a prototype. Many companies right now have this idea of a baby version of the product. Like baby Cursor, you've seen this on Twitter. We have baby Codex, a dramatically simplified code base that approximates all of the interactions of the production app. And therefore is a lot quicker to vibe code over. Because you can be like, "Well, what if the sidebar worked like this? Or what if a pane came in and had a group chat here? What if X, Y, Z?" That's a huge tool that's part of the design process.

**Andrew Ambrosino** (00:20:46):
So to say that the design process is dead, I feel like it's both true and false. It's that if you are tied to the tools and the exact day-to-day specifics of the process, then yeah, it's dead. You're not going to have a good time. But to throw the process out completely or throw the overlay of the process, the like, "Hey, we are at this point in the process." That is still more important than ever.

**Lenny Rachitsky** (00:21:11):
It's really interesting because you have a background in every function. If people look at your LinkedIn, it's like engineer, designer, product manager, founder. Now you oversee the desktop app. And I think design is not under your purview, is that right? Is there a separate design team or are they under your?

**Andrew Ambrosino** (00:21:25):
Depends on the week.

**Lenny Rachitsky** (00:21:26):
Okay.

**Andrew Ambrosino** (00:21:27):
We worked very closely together. We believe in, while sitting together, being embedded. Reporting line, I don't know.

**Lenny Rachitsky** (00:21:35):
They shift weekly. What does the design process look like on the Codex app?

**Andrew Ambrosino** (00:21:38):
Yeah, there's been a lot written about role collapse, existential role collapse. There are no roles anymore. We haven't seen that. We have seen more role collapse in the Codex org than I think other parts of the company and other parts of the economy. I think part of this is that this was a technical product for engineers. And so our designers speak engineer, our product managers speak technical language and write code.

**Andrew Ambrosino** (00:22:08):
Alexander has a master's degree in computer science, which is, I do not have a master's degree in computer science. So we've seen a lot of role collapse. And I think that one of the ways that we describe how the groups work together is that there's significantly more overlap in the roles than there used to be. And everybody's sort of defined less by the fence and the boundaries of where design stops and engineering starts, but more the average of where they're working.

**Andrew Ambrosino** (00:22:37):
So if you average up all of the things that somebody on our design team does, there's plenty of code writing things. There's plenty of things that are product work, but on average there are dots over here if you draw it out on a diagram. And this sort of speaks to the process too, especially because the entirety of the Codex app has been informed by the dog fooding loop.

**Andrew Ambrosino** (00:23:02):
There is a desire among all of us to try to do as much as possible in the app even when it's not the best tool, so that it can become the best tool. And so a lot of design we all work on by using the app and say, "Okay, what's broken about this?" This is a whole thing we do, which is that we often don't improve our process so that we can make the product better to do it, which is a deeply uncomfortable place to be in. But week to week, it's changing.

**Lenny Rachitsky** (00:23:30):
I love this point so much that what are you? It's your role is the average of what you spend your time on. If most of your work is PM-y work, then okay, you're PM for now. If it's engineering, you're an engineer for now. I feel like, was OpenAI the first company to call people member of technical staff?

**Andrew Ambrosino** (00:23:46):
No, I believe that this might've started with Xerox. First company I interned at, it was a company called Upthere, did the same thing. This has been around. But it's much more common now, but it is kind of a tradition in research focused companies, right?

**Lenny Rachitsky** (00:24:01):
Okay, got it. So it emerged from research. But I feel like it's such a, I don't know, sign of where things might be headed, this idea of we're just going to call everyone member of technical staff, your function isn't set. You're not in this bucket of the PM org or the eng org or the design org.

**Lenny Rachitsky** (00:24:16):
Do you feel like that's where we all head long-term? Do you feel like functions will continue to exist? There's still the PM skillset and the eng skillset and the design skillset. And people are, "I'm a designer." Or do you think this is like, people call it builder. Do you feel like there's this collapse coming where everyone's everything and that's just the future? Or do you think we're going to continue to be mostly divided up in quadrants?

**Andrew Ambrosino** (00:24:38):
Yeah. There are some things that I'm afraid of. And I think that some companies like to be very extreme about getting onto the bandwagon of whatever people say is going to happen. And I think part of the danger in eliminating the concept of roles is that it can dangerously eliminate the idea that things are specialties with knowable best practices.

**Andrew Ambrosino** (00:25:10):
I've heard a lot of companies be like, "We're getting rid of the product role," which I think is by the way, a terrible idea. And everybody's just going to be a builder. And then what happens is this whole discipline of product that's been built up and has real best practices, real things that have been tried and failed, and real processes, that just gets abandoned. Because people are like, "Oh, I wrote some code." That's not a great place to be in.

**Andrew Ambrosino** (00:25:37):
I think that the boundary of so and-so, this isn't your lane. I welcome that part going away. But there's a balance here where it's like not everyone can work on everything, for one, both in terms of breadth and depth rate. This is why managers are not going to go away.

**Andrew Ambrosino** (00:25:58):
Not everybody can work on everything. And also every discipline has a skill component to it, which I think a lot of engineers are guilty of not recognizing that, "Well, engineering has a skill to it. It's writing code and other roles are just people vibing." It's like, "No, that's not how it works." Yes, you can use Excel, but you cannot work on the finance team, that kind of stuff, right?

**Lenny Rachitsky** (00:26:24):
Yeah. I think there's also just like, "Do you want to be doing this work?"

**Andrew Ambrosino** (00:26:27):
Yeah.

**Lenny Rachitsky** (00:26:27):
Do I want to be?

**Andrew Ambrosino** (00:26:28):
I think more of it's that actually now, is it's easier to switch roles. It's easier to learn the best practices. It's easier to not tie your effectiveness in a role with the ability to use the exact tool. It's more of like, "Can you get yourself into this mindset, learn which things work and which don't, and then focus on it?"

**Andrew Ambrosino** (00:26:52):
I spent so long feeling like I should not be a software engineer because I didn't care about assembly language or memorizing type scripts and texts. And it's like there have always been parts to these roles that are that sort of gatekeeping. That are like, "Well, no, being good at this role is being good at this tool." And I think that's what's kind of starting to erode. I think people take this, they hyperbolize all of this.

**Lenny Rachitsky** (00:27:22):
What does your team look like on the Codex team? How many engineers, designers, PMs? What's kind of the makeup of the team right now?

**Andrew Ambrosino** (00:27:29):
Every time people ask me how many people are on the Codex team, do you remember my answer to this? I'm like, "It's somewhere between 10 and a few thousand." I mean, it's like a fake answer, but it's real in that we do see this as the culmination of what everybody works on here.

**Andrew Ambrosino** (00:27:45):
Everything that goes into model research, everything that goes into how models are good at CUA and browser use. Everything about how model personality. All of the product work around front end infrastructure, all of the user, all of it is this product. At the same time, we are not accepting PRs daily from thousands and thousands of people on whatever they want.

**Andrew Ambrosino** (00:28:07):
So we got a team, double digits of engineers, probably half that on the design side. A few product people, although product here is kind of more of a zone defense play. And I think one thing that is very common among everybody on the Codex side or on the desktop side is agency and taste, right?

**Andrew Ambrosino** (00:28:29):
A lot of former founders or people who were at larger companies doing founder shaped things. A lot of people with immense taste. At OpenAI, we let teams get very large. So we haven't said, "Hey, there's no management," but the teams are quite large. It's mostly ICs and I think that's good.

**Lenny Rachitsky** (00:28:47):
You use this term zone defense for product work and that's really interesting. It kind of maps to the design kind of shift also, just like you're there to manage and coordinate. Talk a little bit more about what that looks like. What does zone defense look like for a product person?

**Andrew Ambrosino** (00:29:00):
Yeah. And I have had a lot of conversations with Alexander about this analogy, which is that if two product people are working too closely, that's often not a good signal. And that you kind of want, as a product org, you sort of want to do this force directed activity. Where you're like, "Where are the gaps?"

**Andrew Ambrosino** (00:29:22):
Especially in this new world where curation and steering and alignment is a lot of things. Where you're like, "There's a ton of chaos happening on people throwing ideas all over the place." The whole top down, year long planning thing, not going to work.

**Andrew Ambrosino** (00:29:36):
And so now it's like we need the taste makers to guide things from inception to what the product should be. And that means you basically want company coverage. And so you spread out and you say, "All right, who's best at what? Let's create some space between us so that we got full coverage." And that's kind of how it goes.

**Andrew Ambrosino** (00:29:55):
And then you fill in the gaps and you're like, "Look, we want to hire engineers who are product-minded." We don't want it to be that we've got a bunch of people writing a bunch of code that needs full team reviewing it for product coherence. We want everyone to have these skills, but I think what people go deep on has to change.

**Lenny Rachitsky** (00:30:14):
This is definitely a thread I've been noticing over and over with talking to folks like you. Is the most valuable person right now, one of the most valuable, is someone that could take an idea from idea to done with the taste to know this is great.

**Andrew Ambrosino** (00:30:28):
Yeah.

**Lenny Rachitsky** (00:30:28):
Just shepherding throughout, this obsession with making it awesome. This kind of high agency, high taste person exactly as you described. Is that kind of the way you think about here's who we're hiring, here's who's going to do really well in this new world?

**Andrew Ambrosino** (00:30:40):
Yeah, I think that's the core piece right now. And it also speaks to how I sort of see IC versus management, which is that it's not that management is going away. It's not that everyone's an IC, but everyone's kind of both now. If you are an IC, you're not typing code out character by character. You are managing something. You're managing agents. You are managing work that is happening that comes together to do a certain thing.

**Andrew Ambrosino** (00:31:14):
If you're a manager of teams, you're doing the same thing just at a different granularity. I generally look for obviously command over the discipline, but then the taste to say, "Hey, you're going to have unlimited tokens and we can't just be doing slop." You need to be able to determine what signal, what's noise in a world of just infinite content.

**Lenny Rachitsky** (00:31:38):
Mention planning. At the pace things are moving, it's become very hard to plan roadmaps. I imagine, especially in your world.

**Andrew Ambrosino** (00:31:47):
People are very frustrated with me all the time on this. Yes.

**Lenny Rachitsky** (00:31:50):
Because things are just constantly shifting, things are changing. How do you plan on your team? How far ahead are you thinking and what does a plan look like? Is it a spreadsheet? Is it MD file? What's the output of a plan?

**Andrew Ambrosino** (00:32:00):
Yeah, I don't think we do anything revolutionary on that. We're not clever about planning. I think the basic gist is, the shorter term something is, the more detail it needs. And then it's not that we don't plan for nine months out. It's that that just has to stay very hazy.

**Andrew Ambrosino** (00:32:17):
Because any amount of precision that you add to a nine-month plan right now is false precision and you're just going to waste time. You can say stuff, but nothing that we planned. I think research is different. So I'm not speaking for research here, but on the applied side when we do product, anything that you could have planned in November may have been true for December, but isn't what happened.

**Andrew Ambrosino** (00:32:41):
So it's hard. It is really hard to do planning. We generally need to know what do we think models are able to do on what timeline?

**Andrew Ambrosino** (00:32:49):
And my last company, I kind of saw this shift where we were starting to use the models to drive features. And the product process fell down. It basically had to be like, "Let's list out all of the things that we think we are interested in doing for the next year or two." Let's prototype all of them, decide which things are ready now, and then just let the others sit and bake.

**Andrew Ambrosino** (00:33:18):
And then every time there's like a new leap in models, let's try that thing again with it swapped out. Because the whole premise of whether features were good or not were based on whether they were smart enough, not the shape of them.

**Andrew Ambrosino** (00:33:31):
So this is a great story about the Codex app. I am very confident that the Codex app that we released in February, if that had been ready in November, it would've absolutely failed in the market. And the only difference was the models between November and February. And I think there's a lot to that, that this product with the exact same shape, I think its outcomes were totally different depending on just a few months of timing.

**Lenny Rachitsky** (00:34:04):
**Andrew Ambrosino** (00:35:39):
Yeah, I think we have a lot of that. I think sometimes the challenge is you have to be very clear again about what stage of the design process that's in. People still have this muscle memory of like, "Oh, I wrote the code for this thing, therefore we should put it out there." It's like, "No, no, no." That means you have an artifact now that we can test against for into future models.

**Andrew Ambrosino** (00:35:57):
This happens with the in-app browser in the app that we have. We had a kind of a working version. I mean, go back to Atlas, we had agent working inside of Atlas and that was pretty cool. We had Operator before that in ChatGPT. That didn't work out. Very cool idea. There's some thread that you can draw between Operator, Atlas, Codex, ChatGPT that's fundamentally the same feature. But the re-releasing of it with different intelligence totally changes the outcome here.

**Andrew Ambrosino** (00:36:28):
And so I push people not to be stubborn about like, "No, this isn't working so it's a bad feature." It's like, "No, it might not be ready yet."

**Andrew Ambrosino** (00:36:37):
There's also this aspect of, especially in research, there's always a desire to be the most ambitious. And to say, "Okay, but at the limit the model can just do this." And that just doesn't work on the product side.

**Andrew Ambrosino** (00:36:52):
If you go back to the original Codex release, basically what it was is it said, it was Codex web and it wasn't good for interacting with. It was like, you give the model a task and it's going to go off, do the task, come back to you with it finished. It doesn't sound that radical. The problem is it didn't do the task that well. It wrote code, it was good, but it was like that form factor was too early.

**Andrew Ambrosino** (00:37:15):
And then the Claude Code comes out. Totally local, not hooked up to the cloud, doesn't pretend to be as... It's not as AGI-pilled. It's going to ask you questions, it's going to sit there. You can't just delegate your life to it. That worked way better because that's the point that the models were out there.

**Andrew Ambrosino** (00:37:32):
So we were too AGI-pilled for the moment. And I think about that lesson a lot on this stuff. It used to be that failing in market told you all these things about the shape of the product, about the communication of the product. And now it's like, "No, you might need to release this thing six different times before it works." And the shape might not change at all.

**Lenny Rachitsky** (00:37:55):
It's so interesting to hear about all the variables you have to think about building product now. There's the timeline for the models and the research and how smart it gets. There's people's ability to even understand this is how you could build software in the cloud and this is the future. Get people prepared for this new feature and then just what you can build as a team.

**Lenny Rachitsky** (00:38:13):
And I love that Codex example because it comes back to this idea of ambition. And I want to hear if there's anything there for you, of just this thread of just be more ambitious because these models can do so much more than you even imagine. And sometimes it's too ambitious for the market and they're not ready for it.

**Lenny Rachitsky** (00:38:26):
But you think about that at all, just pushing your team to be more ambitious because it's so much easier to just do things that maybe felt crazy hard in the past.

**Andrew Ambrosino** (00:38:34):
Yeah, this is a core challenge. Once there's a product that exists or a feature that exists, it's really easy for people to find paper cuts and-

**Lenny Rachitsky** (00:38:43):
Micro-optimize.

**Andrew Ambrosino** (00:38:44):
And they should. And people on Twitter like to remind us of this and I thank them for that. People should be focused on the features that exist and make them more reliable and better. But this is why we also have a culture of bottoms up exploration here.

**Andrew Ambrosino** (00:38:56):
Because sometimes in the same way that Codex app came and disrupted ChatGPT in some way, this thing will get disrupted by a future effort. And that's part of the design is that. You can't always as one team be good at both the disruptive piece instead of maintaining a product and its quality piece. At some point, you have to design a process that allows for both.

**Lenny Rachitsky** (00:39:18):
Kind of zooming out a little bit. If you think about the progression that we've been on of AI impacting how we build product, it's insane how far we've come from. As you said, we used to write all our code by hand, artisanally created human code. To AI writing 100% of our code, to you actually put it this way that now coding is steering the AI.

**Lenny Rachitsky** (00:39:41):
And when you think about what percentage of my code is written by AI, it's almost like how many times did I have to steer it in the right direction as the AU version of coding? And now that there's agents and loops and all these things, what's kind of the latest frontier from what you've seen of how people are building? Is it loops? Is there something else of just the most AI-pilled, AI forward teams, here's how they operate now that people may not be aware of.

**Andrew Ambrosino** (00:40:07):
Yeah. I mean, loops are so last week, man. I mean, we talked about this. One of the big questions is always, "Well, how much of the product is AI written?" And it's always hard to answer that question because if you're using the goalposts from last year, it's like, "Well, 100% of our product right now is AI written code." So the question is more like, "Well, okay, fine. Is the code written supervised versus unsupervised?" And that's a totally different thing.

**Andrew Ambrosino** (00:40:36):
I welcome the moving of goalposts because that means we're making product progress. There have been a lot of explorations here around autonomously developed software. A lot of harness engineering stuff, a lot of different explorations on like, "Okay, well, what if you came in overnight and did garbage collection of the code base to clean it up?" One thing that I think all models suffer with right now is just they usually increase complexity.

**Andrew Ambrosino** (00:41:01):
If research is listening at any company, please make the models better at deleting code. But that becomes a problem right now when you try to put development completely on autopilot and it's both on the human side and the code base side. So feature requests. How do you teach a model which features to build, which ones to ignore, which ones to group together and reframe a little bit? How do you teach to model how to build the right abstractions?

**Andrew Ambrosino** (00:41:31):
All of this is getting better. I don't think we're at place yet where we're like, "We're just going to set up a loop that's like improve the app." And listens to Twitter and listens to Slack and listens to email. We're not there yet, but we're trying to make it happen.

**Lenny Rachitsky** (00:41:49):
Do you think we'll get there? Do you think we'll get to a place where it's just like grow, win?

**Andrew Ambrosino** (00:41:54):
Slash goal, make money, make me a billion dollars.

**Lenny Rachitsky** (00:41:58):
Win the market.

**Andrew Ambrosino** (00:41:58):
I don't know, man. I am not in the business of saying never or always or whatever.

**Lenny Rachitsky** (00:42:05):
Yeah. How are you using AI in your work as product leader, eng leader?

**Andrew Ambrosino** (00:42:10):
Yeah.

**Lenny Rachitsky** (00:42:11):
What are some ways that you use it that maybe people may not be aware they can use AI for?

**Andrew Ambrosino** (00:42:15):
Yeah, I think I have the best job in the world right now. But one of the things that makes it very fun is that when we were developing the original Codex app, the goal for me personally was to make it the thing that I wrote the code with. I was like, "I need to make this so good at development that I can build the Codex app with this." And the Codex app at that time was a development tool.

**Andrew Ambrosino** (00:42:39):
And we did that super quick dog fooding loop because you've got your personal dog fooding loop. Where you're like, "Oh, I can't do this thing. I should fix that so that I can do the thing. Now I can do the thing, now I can do more things." We released that.

**Andrew Ambrosino** (00:42:54):
And then the next challenge was, "Hey, people are starting to do some different shaped things with this. And now I need to grow this and so I need to hire a few people and help." So then my role changed at the same time that the role of the app needed to change.

**Andrew Ambrosino** (00:43:07):
I'm like, "Okay, I need to do more product discovery here. I need to figure out the right loops for seeing what everybody's working on and steering things that are off track." And so all of a sudden that's what I started using the Codex app for. I did still write code.

**Andrew Ambrosino** (00:43:22):
I've tried to align my own usage of it with the problem that we're trying to solve. And now I'm like, "I need to build a spreadsheet that models this out." I need to do internal deep research on all of the efforts that have gone into this area of research for the next version of this.

**Andrew Ambrosino** (00:43:41):
There was a release or a series of releases in May-ish that introduced the in-app browser, computer use, and artifact creation to the Codex app. That was, I think our Codex is for almost everyone release. And everybody knows the term vibe coding. I think that was our first vibe coordinated release.

**Andrew Ambrosino** (00:44:01):
Where I had a Notion Doc somewhere with everything that needed to happen. And I was automating, going out to gather updates from pull requests, from Slack channels, and updating the status tracker. And now this is pretty commonplace, but at the time I felt like I was at the bleeding edge of how to manage a product release.

**Andrew Ambrosino** (00:44:22):
In short, the way that I use the Codex app is basically like, what has my job grown into and how do I make this thing able to do everything I need to do? I will get up in the morning, I will see the daily brief that I have from everything from the 3,000 Slack channels that I'm in. Which things need my attention. I can kind of message back and be like, "All right, give me five questions and I'll answer them." And I can do that.

**Lenny Rachitsky** (00:44:49):
How do you set that up? What's the workflow for somebody to set that up? Yes, that sounds amazing.

**Andrew Ambrosino** (00:44:53):
Again, I think we're still in the discovery phase on a lot of this. And so right now it's like I'm making an automation that says, or scheduled task that says like, "Go through my Slack channels, these are the things that I care about and think are most important." So I'm still kind of defining that.

**Andrew Ambrosino** (00:45:12):
These are things to watch out for different categories, here's some context. And that'll get set up as an automated task and then first few times it runs it might need some steering. And luckily with this app, I don't have to find out how to edit the instructions.

**Andrew Ambrosino** (00:45:27):
I can just be like, "Hey, next time this runs, can you please worry about this instead? Or can you de-emphasize this work stream? Or, hey, this thing happened and it didn't come up in a brief, can you make sure that stuff in this shape?" So I can kind of coach it along the way. It'll update the way that it notifies me, stuff like that.

**Lenny Rachitsky** (00:45:44):
Amazing.

**Andrew Ambrosino** (00:45:45):
I think in the future though, this has been a core problem with the chatbot shape, is that I know how to set this up. I have time to set this up because for me, it's product discovery to set it up. But if you're not working at OpenAI, not developing this, you don't want to have to figure out all this stuff. We need to figure out that shape of things.

**Lenny Rachitsky** (00:46:06):
Yeah. What I'm hearing here is I don't think people realize that your app can act a lot like OpenClaw, people were so excited about. You just talk to it, set up this thing, check on this thing for me every day, and then tell me what's going on.

**Andrew Ambrosino** (00:46:19):
Exactly, yeah.

**Lenny Rachitsky** (00:46:20):
It's starting to become a part of all the products, which is amazing. So the way somebody would set this up is they just talk within the app and say, "I want to set up an automation to do this. Look at my Slack and these are the things I want to do."

**Andrew Ambrosino** (00:46:20):
Yeah.

**Lenny Rachitsky** (00:46:32):
Great.

**Andrew Ambrosino** (00:46:32):
Yeah. And the app will say it'll set it up for you. If it doesn't have a Slack connector, it'll say, "Can I add the Slack connector? Yes or no?" You can hit yes to that.

**Andrew Ambrosino** (00:46:43):
The least that we can do is make it so that if you don't know how to do something in the app, that you can just ask it. I don't think that's enough, but I think that's the least we can do.

**Lenny Rachitsky** (00:46:52):
Yeah. A good example of this, I built this little app that filters spammy email from my inbox. So every email that comes in, and I built this in Codex, every email that comes in, it looks at it and decides is this unsolicited, kind of cold emaily stuff that I don't want to look at? And labels it and puts it somewhere else.

**Lenny Rachitsky** (00:47:08):
And to set that up, one of the steps was you have to go into the Google Cloud console and set up all these hub, sub, hubbub, API things, and triggers. I don't know if you've ever used that interface. It's so annoying and slow.

**Andrew Ambrosino** (00:47:20):
Right.

**Lenny Rachitsky** (00:47:20):
So I was like, "Wait, what if I ask you to do it?" And I was like, "Okay, cool. Do this for me." And it just... You described computer use. I've never actually seen this happen on my computer before. It just takes over my computer and starts going there.

**Andrew Ambrosino** (00:47:32):
It's like, "I don't care if you don't have a connector, man, I'll just start clicking."

**Lenny Rachitsky** (00:47:35):
Yeah. And it figures it out. It's crazy just to watch it doing this thing.

**Andrew Ambrosino** (00:47:39):
Designing the decision boundary between connectors. When to use the in-app browser versus your Chrome extension that's connected versus computer us was interesting. And all done through just feeling it out.

**Lenny Rachitsky** (00:47:52):
I saw a great Twitter thread the other day where they describe all these three and what you use it for. So this person described it really well.

**Andrew Ambrosino** (00:47:58):
These personal workflows are really interesting because some of them really click. People are trying all sorts of stuff. Everybody's making these personal systems. You ask everybody here what they do and everything's going to be different. And then certain themes arise and we're like, "You know what? That should be a first class experience on the app. We should take this thing that everybody seems to be setting up and just make that work."

**Andrew Ambrosino** (00:48:23):
And I think memory is sort of in the shape where we've had a lot of people, and a lot of people at other companies too are like, "Well, I set up an Obsidian base or a Notion area. And I tell it how to basically build my mind palace and how to put..." It's like, "I don't know if everyone..." You shouldn't have to do that. There should be a memory feature that does that for you, that's pretty generic.

**Andrew Ambrosino** (00:48:45):
So that's one. But then there are other things like they're your process of your job. And there's something that like, "Yeah, you should set that up." But I think we're constantly wading through what's working for individual people, what should enter the product? Versus stay, no, that's just how you do your job, right? What should become a primitive, what shouldn't?

**Lenny Rachitsky** (00:49:06):
Yeah. This is the taste and judgment you spoke of earlier deciding these things. I want to talk about this browser use piece a little bit because I think people don't realize how powerful this is and what it could be used for. Reminds me, I don't know if you watched when Dan Shipper was on the podcast, from Every. He had this prediction that we're going to start using Codex to run our SaaS apps inside out. So instead of going in Chrome-

**Andrew Ambrosino** (00:49:29):
I know, he Slacks me about this every day asking for stuff.

**Lenny Rachitsky** (00:49:33):
Do you feel like this is where things go?zeolite Where we're just working within the Codex app using Notion and Linear and Salesforce inside with your agent kind of helping you along? Or do you think that's a kind of a different direction?

**Andrew Ambrosino** (00:49:46):
Yeah, it's been really interesting because obviously we've had a few attempts at browser shaped activity. And Operator and ChatGPT agent mode and Atlas. And now we have the in-app browser inside of the desktop app. We also have the ability to install a Chrome extension where the app connects to Chrome.

**Andrew Ambrosino** (00:50:07):
We've had a lot of shapes of this and I think we've learned a lot of different things. There's a lot at play. There's a lot of really boring things at play. We originally launched the app, it's an electron app. The things that you can do with in-app browsers in there, it's kind of janky.

**Andrew Ambrosino** (00:50:22):
So the in-app browser was for development, it was for testing your front end on development. And we were like, "It's not really for anything else, guys. It's a developer tool." And then we switched over to our Owlstack, which had powered the Atlas browser.

**Andrew Ambrosino** (00:50:37):
And so now it multi-tab. And we've got enterprise security so that you can actually log into all your websites if you're... So we've been iterating on this. I think the tough thing has always been, what should the shape of this browser be? Is this something that is only for the agent?

**Andrew Ambrosino** (00:50:54):
That you've got Chrome, you open Chrome, you do your thing in Chrome. If you ask the desktop app, it opens up this browser that it can control really quickly, doesn't have the latency of Playwright, whatever. Or are we trying to say, "This app is for everything and we want you to use this as a browser."

**Andrew Ambrosino** (00:51:11):
And those have a lot of trade-offs. It's not super well-traveled path. Most browsers are browsers at the top level. They've got browser tabs. This creates a lot of really boring but tedious problems like keyboard shortcuts, right? Are we trying to do key mapping to VS code or to Chrome or to our own thing? Or to Linear?

**Andrew Ambrosino** (00:51:33):
We want to have some sort of muscle memory that carries over, but got all these things that have sub-shapes of different products out on the market. What do we do?

**Lenny Rachitsky** (00:51:42):
And this just highlights how extra challenging this app is where you have to allow it to work. For somebody that's never built anything from the more basic user, to power like Peter, OpenClaw trying to code with it.

**Andrew Ambrosino** (00:51:58):
I'm not convinced I'm going to get Peter to use the app. I think he might be the last-

**Lenny Rachitsky** (00:52:02):
He's a terminal hold out.

**Andrew Ambrosino** (00:52:04):
... terminal hold out.

**Lenny Rachitsky** (00:52:04):
Okay.

**Andrew Ambrosino** (00:52:05):
But I'm going to keep trying.

**Lenny Rachitsky** (00:52:06):
Okay. Let me zoom out for a moment and talk about the big picture of where you're taking all this. What's the vision for Codex? Where does this go? What's it going to look like, I don't know, a year or two, 10 years?

**Andrew Ambrosino** (00:52:18):
We had Codex as a CLI and then we decided to build this app. And we were a little uncertain about the app but had a lot of conviction in what it could be as to start a developer tool.

**Andrew Ambrosino** (00:52:35):
And it wasn't going to be an ITE, it was going to be this right sized surface. Where it was sort of a chatbot but it was more than that and you could see the code but we weren't going to let you edit the code.

**Andrew Ambrosino** (00:52:45):
There's a really interesting thing that happened at OpenAI in January and February. And it was before we actually released the Codex app, which is that we'd started to dog food the Codex app. And what we were finding, we were converging on some pretty clear internal PMF on engineering and research workflows.

**Andrew Ambrosino** (00:53:08):
They were thrilled. They were loving it. We were like, "All right, we just got to get the quality bar up before we release it to the world. We're convinced that this will be a thing." But then at the company, we spun up a few other workflows to say, "Hey, this Codex effort is onto something with these coding agents."

**Andrew Ambrosino** (00:53:23):
And we have people from marketing, from comms, from finance, from legal, from basically every discipline, who are using this Codex app, even though it is actively hostile to these people. It is trying to show them code. It's trying to ask for approval to run RG on the...

**Andrew Ambrosino** (00:53:41):
It's doing all of these things that are actively not the right product surface for them. So why don't we take our other surfaces and add Codex to them? Let's add it to the ChatGPT desktop app. Let's add it to the Atlas browser. And let's essentially take the lessons of Codex and make it more general for a general knowledge work tool.

**Andrew Ambrosino** (00:54:02):
And those efforts went for a little bit. And the most annoying problem happened, which is nobody would leave the Codex app for the apps that were allegedly for these other personas. I think the lesson in all of this was just that the whole developer tool versus general knowledge work tool, there's a lot of nuance here that isn't just one or the other.

**Andrew Ambrosino** (00:54:25):
I think we believe really strongly in this. And that there are certainly, in the same way that we talk about the average of your role as what your role is now, this is true on the product side too.

**Andrew Ambrosino** (00:54:36):
People who are doing Excel work don't want to see Git repository information. We know that, but we also know that we can tell a lot from what they're doing about what kind of work they do. And we can start simple, grow the product to complex as we feel is needed.

**Andrew Ambrosino** (00:54:53):
It doesn't mean we don't have modes. You might want some modes for organizing your stuff and to sort of be legible about the ways that you enter the experience. But we really believe strongly that what we've built here is the right shape to take on really deep, vertically focused things.

**Andrew Ambrosino** (00:55:13):
We work deeply with our finance team, with our team working on science, team working on legal. And we say, "If we can build the right extensibility primitives in the right general model, then you can do anything with this." And then our challenge is, well, how do you generalize it?

**Andrew Ambrosino** (00:55:33):
But this is kind of going back to the best desktop app that we can build. What does that look like? And so it was Codex the developer tool, ChatGPT, where's this going? This is how we think about it.

**Lenny Rachitsky** (00:55:47):
It is so interesting, the point you made that the Codex app was so, you did such a good job getting people to be aware it existed. And so good to use and fun to use that everyone's starting to use that versus the ChatGPT app. So clearly the direction is combining them so that you're not creating this confusion, which I know is things people have been talking about, this idea of come bringing them together.

**Andrew Ambrosino** (00:56:06):
Somebody called it a super app and wish they hadn't said that because now I have to hear about the super app all day, every day. We'll get past it. Great.

**Lenny Rachitsky** (00:56:17):
Okay. But is that kind of the... Let's not call it a super app, but the idea is one place people go to do all the things. Is that the general idea? Or TBD?

**Andrew Ambrosino** (00:56:23):
Yeah. I think what we see here is that it's a great home base. It's a great place to keep track of all of the things that you have to do across different surfaces. And some of those things, you do all of it in the app. Some of those things the app opens other apps to do. The app can connect to Excel so that yes, it has a spreadsheet editor inside the app.

**Andrew Ambrosino** (00:56:47):
Is that good enough for people doing financial modeling at OpenAI for raising billions of dollars? Probably not. And so the app talks directly to the add-in Microsoft Excel on your desktop. When it's done, you can close Excel.

**Andrew Ambrosino** (00:57:03):
And so it's not just about, "Hey, we're drawing a rectangle on the screen and everything needs to happen in that rectangle." It's, "This thing should be a home for you where you start work, you end work, you automate work, and it uses whatever you need to do."

**Andrew Ambrosino** (00:57:21):
There's a great story about, we had some videos that we shot in this room for the original launch of the Codex app. And our in-house DX videographer, Brent, then was tasked with editing all these videos. And he edited all the videos with Codex, which was one of the early like, "Whoa, what are people doing with this thing?"

**Andrew Ambrosino** (00:57:41):
And the process for why he decided to start using Codex was really interesting. He started just because he was curious if Codex could edit videos. And so Codex is not a video editor per se. It doesn't have any of that UI in it, but it was able to understand that he used Premiere Pro. It could do some edits by editing the files that were backing what was on-screen in Premiere Pro, but it couldn't do everything.

**Andrew Ambrosino** (00:58:08):
So naturally what Codex then did was built itself an extension that could be installed into Premiere Pro. That it could then talk to and say, "Hey, Premiere Pro extension, can you please change this marker inside of the Premier Pro app?" That was pretty nuts when we saw that happening.

**Andrew Ambrosino** (00:58:28):
It's a great model. There are these specialty tools that specialize in things. And so we're trying to do two things at once with Codex and with now with ChatGPT. One is how can we seamlessly interact with these tools that you're already using? And say, "We don't need to build a better video editor for you."

**Andrew Ambrosino** (00:58:47):
But Codex and ChatGPT can use that video editor. It can interact again, can hand stuff off to it. So how can we do that? And that's often through connectors or computer use or even extensions in this case.

**Andrew Ambrosino** (00:58:59):
And then there is Dan Shipper's thing, which is, "Hey, I have these web apps that you can click around and use, but I want to be able to open these in Codex and have Codex do extra stuff with it." And so those are kind of like two models that are almost inverse of each other that we're doing a lot with both at the same time.

**Lenny Rachitsky** (00:59:18):
This Premiere story is interesting to me because it's another example of just be more ambitious with these AI jobs. You may not know, maybe they could do this thing. It's almost just like, "Go try, go try out, see if it figures it out."

**Lenny Rachitsky** (00:59:31):
I'm going to take us to a recurring corner on the podcast that I call Fail Corner. And so the question for you is people see people like you just killing it, just growing. Everything's winning. Codex is doing so great, this crazy career, everything's up and to the right.

**Lenny Rachitsky** (00:59:48):
People may not see the times that things didn't work out and things that you launched that were failures. And so these stories are really important for people to hear, that it's not all just win all the time. What's a story of a time you failed in your career that taught you something really important?

**Andrew Ambrosino** (01:00:03):
It's funny to hear that description played back at me. And this is perhaps the first time I've not felt like I was failing. I mean, I was a startup founder for a long time. I ended up selling the company for parts essentially. It was years, it was a slog, it was heavily regulated spaces. The whole thing felt like a constant failure.

**Andrew Ambrosino** (01:00:28):
I went to this other startup and we were trying to do some AI tools in this also pretty locked down, regulated industry. And that felt like just time after time of trying things and it not working. So to me it's been like, "Oh, I've failed actually quite a lot." And sometimes it's just a point in time where things line up like skillset, passion, point in the market, line up.

**Andrew Ambrosino** (01:00:52):
With this project to bring what we've learned with the Codex app and marry it with ChatGPT, there have been, I don't know how many micro failures on this. Where we're like, "This is the shape it should look like." And then throw that in Slack and there's like a 2,000 message thread about how stupid we are.

**Andrew Ambrosino** (01:01:13):
This is the thing I love about OpenAI, is people will just tell us that. There's no holding back on when we fail with product things internally. It's why the external product has been pretty great is because it goes through these cycles of-

**Lenny Rachitsky** (01:01:27):
2,000, this sucks.

**Andrew Ambrosino** (01:01:28):
I failed for, I don't know, somewhere between 10 and 15 years before getting to this point. So I'm still surprised every day that things are going well. And I know it.

**Lenny Rachitsky** (01:01:38):
I think this is really important for people to hear. That you can have a lot of things not work out and then things start to work out super well and it's just keep going and keep learning. I imagine is a lesson.

**Lenny Rachitsky** (01:01:48):
Well, with that, we reached our very exciting lightning round. I've got five questions for you. Are you ready?

**Andrew Ambrosino** (01:01:53):
Great.

**Lenny Rachitsky** (01:01:54):
[inaudible 01:01:54]. What are two or three books that you find yourself recommending most to other people?

**Andrew Ambrosino** (01:01:59):
See, man, I'm a parent now. I'm a parent of young kids.

**Lenny Rachitsky** (01:02:02):
Nice.

**Andrew Ambrosino** (01:02:04):
I don't know. There's one called The Gruffalo, I read to my kids.

**Lenny Rachitsky** (01:02:07):
Oh, my God. Our kid just got obsessed with The Gruffalo.

**Andrew Ambrosino** (01:02:10):
Yes.

**Lenny Rachitsky** (01:02:11):
We have a bedtime chart and now it's like pajamas, brush teeth, books, Gruffalo, on blankie.

**Andrew Ambrosino** (01:02:18):
Yeah.

**Lenny Rachitsky** (01:02:18):
Yeah. It's so good.

**Andrew Ambrosino** (01:02:19):
So other books I'm reading right now are that style.

**Lenny Rachitsky** (01:02:23):
Okay, the soft stuff.

**Andrew Ambrosino** (01:02:24):
Actually, The Gruffalo is not a terrible one.

**Lenny Rachitsky** (01:02:25):
No.

**Andrew Ambrosino** (01:02:25):
I feel like there's some lessons in it.

**Lenny Rachitsky** (01:02:26):
It's so sweet. Yeah. Although every kid's book is about death. Someone's eating someone, someone's killing. There's always bad murder and destruction.

**Andrew Ambrosino** (01:02:35):
Kids like violence. Even when it doesn't feel like violence to them, the words...

**Lenny Rachitsky** (01:02:40):
It creates an arc and excitement.

**Andrew Ambrosino** (01:02:42):
Yeah.

**Lenny Rachitsky** (01:02:42):
Yeah. Okay. Great choice, Gruffalo.

**Andrew Ambrosino** (01:02:44):
I currently have a book backlog. I need to read all of them.

**Lenny Rachitsky** (01:02:49):
Any other children's books then that your kid likes?

**Andrew Ambrosino** (01:02:52):
Okay. Yes, actually. I am well versed on children's space. My favorite children's book ever is a very old one and it's called The Big Orange Splots or something along those lines. Look it up. It's great. Go get it. If you hate HOAs, go get it.

**Andrew Ambrosino** (01:03:09):
It's about this guy, Mr. Plumbean, who lives on a street where all the houses are the same. It's a very neat street. And then one day a bird drops a large can of orange paint on his house and he says, "Eff it. I'm going all in." So he goes to the store, he gets paint, hammocks, alligators, and he totally redoes his house.

**Andrew Ambrosino** (01:03:29):
And the neighbors, they're up in arms, right? HOA, property value, whatever, whatever. It's not about HOAs, but I'm a very anti-HOA person. It's just really cool. And then one by one, the neighbors go talk to him, have what they refer to as lemonade, but it's a very convincing lemonade. Because one by one, they all start redoing their house. One guy does a boat.

**Andrew Ambrosino** (01:03:49):
I think that's a good book. I think people need to read this when they're, especially NIMBYs.

**Lenny Rachitsky** (01:03:54):
What I hear from this is agency.

**Andrew Ambrosino** (01:03:56):
Agency, exactly. You can just do things.

**Lenny Rachitsky** (01:03:59):
Just do things. Amazing. Okay. We'll keep going. Favorite recent movie or TV show you've really enjoyed if you've had any time?

**Andrew Ambrosino** (01:04:05):
So The Magic School Bus is back on Netflix. It's a new animated. It's got Kate McKinnon because Ms. Frizzle is now Professor Frizzle and she's around, but she's not the main Frizzle now. Kate McKinnon plays the main Ms. Frizzle. Yeah. I always liked the Magic School bus. It's back and very-

**Lenny Rachitsky** (01:04:22):
I've never seen or heard of it. Cool.

**Andrew Ambrosino** (01:04:24):
Personally, I don't have time for movies. So what I do is watch hour-long Netflix things back to back. You know that thing that people do?

**Lenny Rachitsky** (01:04:33):
Like binge watch?

**Andrew Ambrosino** (01:04:34):
I couldn't sit down and watch a whole movie and then watch hour-long episodes and keep... Idea. There's something addicting about that way.

**Lenny Rachitsky** (01:04:41):
Favorite product you've recently discovered that you really love?

**Andrew Ambrosino** (01:04:44):
Well, this is a terrible answer. I feel like I'm discovering our product every day.

**Lenny Rachitsky** (01:04:49):
Beautiful.

**Andrew Ambrosino** (01:04:49):
That's terrible.

**Lenny Rachitsky** (01:04:50):
That's so corny but-

**Andrew Ambrosino** (01:04:50):
I think Linear does a great job. Until this, Linear was my favorite, at least software product.

**Lenny Rachitsky** (01:04:59):
Is that what you guys use to plan and coordinate?

**Andrew Ambrosino** (01:05:01):
Well, in theory.

**Lenny Rachitsky** (01:05:04):
Do you have a favorite life motto that you find yourself coming back to in work or in life?

**Andrew Ambrosino** (01:05:07):
I want to ask everyone who works with me this because I feel like I'm not a motto person and then people tell me stuff I say all the time.

**Lenny Rachitsky** (01:05:16):
Yeah. When we were chatting ahead of this, there's so many little nuggets that stood out to me that I've integrated into this chat. So I totally hear that.

**Lenny Rachitsky** (01:05:23):
Okay. Last question. You've been a PM, you've been a designer, you've been an engineer. Which is the toughest role of the three, which is the hardest?

**Andrew Ambrosino** (01:05:33):
Trying to start a war?

**Lenny Rachitsky** (01:05:35):
Yes.

**Andrew Ambrosino** (01:05:35):
I don't know. I think they're all very different. I think the things that make it tough for one person make it easy for others. There's a lot. There's so much, so many takes on this and this triad, what's going to happen with this triad? Designers are done or should designers code? Are PMs cooked? Do we not need engineers anymore because PMs are going to write all the code? Or are designers going to PM now?

**Andrew Ambrosino** (01:06:03):
And everybody's cooked and everybody's so back. And I don't know. There's some convergence, there's some fluidity that is being introduced that I think is refreshing and great, especially for people with agency that want to be able to just do the thing that needs to get done. And at the same time, like we talked about, there are some things that shouldn't go away. But I think people should find the stuff that's worth working on and go figure out what to do on those things.

**Lenny Rachitsky** (01:06:32):
That is a beautiful way to end it. Andrew, thank you so much for being here.

**Andrew Ambrosino** (01:06:35):
Thank you.

**Lenny Rachitsky** (01:06:36):
Bye, everyone. Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.

**Speaker 3** (01:07:02):
I love that thing about Brent and the Premiere.

**Andrew Ambrosino** (01:07:04):
Yeah.

**Speaker 3** (01:07:04):
That's cool. I've actually used Codex to edit edits as well.

**Lenny Rachitsky** (01:07:07):
There we go.

**Speaker 3** (01:07:09):
It's basically simple stuff like, "Oh, could you just cut this into the three breaks?" If there's a pause in conversation, the second, and Codex understands it.

**Andrew Ambrosino** (01:07:19):
Basically every job we feel like starts with a story like this, which is the product's not designed for it, but it's sort of a blank chatbot that can write code. So it can do everything, but what are the useful things for it to do?

**Speaker 3** (01:07:34):
Right. I mean, people just have to have curiosity about the project. They have to have an intentional outcome and use Codex as the platform for that just to see what happens because there's no risk at all.

**Andrew Ambrosino** (01:07:34):
Right.

**Lenny Rachitsky** (01:07:34):
Just a few tokens.

**Speaker 3** (01:07:49):
A few tokens. But of course, if you're working for OpenAI, there's less risks on that regard.

**Andrew Ambrosino** (01:07:59):
You asked one of them, or a lot of them actually, what skills are important? And then you've also had conversations about the cracked new grad versus the...

**Lenny Rachitsky** (01:08:06):
Right, yeah.

**Andrew Ambrosino** (01:08:07):
I don't know if you're married to the exact process you have right now. I don't know what advice to ever give, but if there's one piece, it's like, "Do not get married to your exact process." Get married to the outcomes that you are uniquely able to deliver and then do things like change your process to try things.

**Lenny Rachitsky** (01:08:28):
You just keep doing more nuggets.

**Andrew Ambrosino** (01:08:29):
If you're like, "I'm the best at understanding Figma auto layout." What are you doing?

**Lenny Rachitsky** (01:08:33):
Right. Because AI is going to be better at that also.

**Andrew Ambrosino** (01:08:36):
Yeah.

**Lenny Rachitsky** (01:08:36):
You just keep spouting interesting things.

**Andrew Ambrosino** (01:08:38):
Keep it in.

**Speaker 4** (01:08:39):
It's crazy the level of self-awareness that's required to be successful with AI.

**Andrew Ambrosino** (01:08:39):
It is.

**Speaker 4** (01:08:39):
Yeah.

**Andrew Ambrosino** (01:08:46):
It's also why I'm nervous to ever say, "This is how something's going to be." Because I think about my parents are open-minded people. They are into their careers, but just the stuff that works here, it's not going to work with everybody. There's no nice way of saying that.

**Speaker 4** (01:09:00):
Yeah.

**Andrew Ambrosino** (01:09:01):
But the people who are here are self-selecting for like, "Oh, I am somebody who just figures out the next thing to do." And that's just not... Most of the population will not be an early adopter of things.

**Lenny Rachitsky** (01:09:13):
And there's also just, it's kind of a bummer to have to relearn things all the time.

**Andrew Ambrosino** (01:09:13):
Yeah.

**Lenny Rachitsky** (01:09:18):
It's like, "God damn it, just to learn a new thing again."

**Andrew Ambrosino** (01:09:22):
I hate repetition. This is a me thing. This is why I'm not ever the best media person either because I hate repeating myself.

**Lenny Rachitsky** (01:09:31):
Perfect.

**Andrew Ambrosino** (01:09:32):
Sucks to be a founder when you hate repeating yourself because you have to.

**Lenny Rachitsky** (01:09:35):
Repeater in chief.

**Andrew Ambrosino** (01:09:36):
And so to me, I'm like, "If I can come in and do my job in a different way every day, love it." But that's not...

**Lenny Rachitsky** (01:09:44):
You found product market fit for your job.

**Andrew Ambrosino** (01:09:46):
Yes. Yeah. No, that's how it... I can't negotiate because I'm like, "Well, I don't want other jobs."

**Lenny Rachitsky** (01:09:54):
Amazing, man.

**Andrew Ambrosino** (01:09:55):
Yeah.

**Lenny Rachitsky** (01:09:55):
Well, thank you.
