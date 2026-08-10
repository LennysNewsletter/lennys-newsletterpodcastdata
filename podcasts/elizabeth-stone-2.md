---
title: "Netflix CPTO on AI and the future of product and tech roles | Elizabeth Stone"
date: "2026-07-19"
type: "podcast"
guest: "Elizabeth Stone"
post_url: "https://www.lennysnewsletter.com/p/netflix-cpto-on-ai-and-the-future"
description: "AI and the future of product and tech roles, covering product design, engineering tradeoffs, and AI product work."
word_count: 13081
---

**Lenny Rachitsky** (00:00:00):
Everyone can be everything now. PMs can ship code, designers can write PRDs, engineers can product, and there's this confusion and frustration of what is my job anymore.

**Elizabeth Stone** (00:00:08):
Anytime a new technology comes along, you go through a storming phase before you go through the forming phase of things. We are in the middle of that right now. I don't think that means we should put AI back into the box and say, "Let's not use it."

**Lenny Rachitsky** (00:00:23):
If we all become builders, will we still need separate functions?

**Elizabeth Stone** (00:00:26):
I still see a craft excellence that's really important that I don't think is going away anytime soon. I still find great engineering to be scarce, great data science to be scarce, great creativity to be scarce.

**Lenny Rachitsky** (00:00:38):
If you look at the early culture deck of Netflix, high agency, autonomy, paying top of market, this is what I hear constantly now from how the top AI labs operate.

**Elizabeth Stone** (00:00:47):
Netflix's culture has always been excellence as an operating system. It's a resistance to do the thing that a lot of bigger companies would do and to feel comfortable in that discomfort very often.

**Lenny Rachitsky** (00:00:58):
What are the ingredients to make this happen?

**Elizabeth Stone** (00:01:00):
Talent density is the non-negotiable, being very comfortable with risk-taking in cases where things are not going well and not assume that process is going to fix it.

**Lenny Rachitsky** (00:01:09):
What have you added to the career ladders within this AI world?

**Elizabeth Stone** (00:01:13):
We need more systems thinkers, people who can look across all the business domains and abstract that to here's the building blocks we're going to need.

**Lenny Rachitsky** (00:01:23):
How do people learn this?

**Elizabeth Stone** (00:01:23):
Small trick. Each problem you're trying to solve, step out one click to the what am I assuming is true about the broader space.

**Lenny Rachitsky** (00:01:34):
**Elizabeth Stone** (00:02:33):
Thank you. I'm honored to be here, once and now twice.

**Lenny Rachitsky** (00:02:37):
That's right. That's a rare treat for me. I don't know if you know this, but your first visit to the podcast, your episode ended up being my second most popular episode. You're right behind Brian Chesky for the longest time.

**Elizabeth Stone** (00:02:50):
Wow. I am pleasantly surprised and also mildly competitive of how do I get to the first spot.

**Lenny Rachitsky** (00:02:58):
[inaudible 00:02:58], I guess.

**Elizabeth Stone** (00:02:58):
But I'll set that aside for now.

**Lenny Rachitsky** (00:03:01):
This is our shot.

**Elizabeth Stone** (00:03:02):
Brian's amazing, so I'll let that one go.

**Lenny Rachitsky** (00:03:04):
Yeah, he is. And then there's just all these fancy AI people that are just coming in hot. So, it's been two and a half years at this point. A lot's changed. Obviously, AI. Something AI is allowing people to do is everyone can be everything now. This idea of PMs can ship code, designers can write PRDs, and engineers can product and everyone's everything. There's a bunch of elements of this conversation. One is that I've heard from people that there's also this kind of confusion and frustration of what is my job anymore. What am I responsible for as a PM, as a designer? Is that something you've experienced?

**Elizabeth Stone** (00:03:44):
I hear it within Netflix for sure. I think anytime a new technology comes along, especially one that's as transformative as GenAI, you go through a storming phase before you go through the forming phase of things. And I think we are in the middle of that right now. I don't think that means we should put AI back into the box and say, let's not use it, because this is complicating all of our preconceived notions about our roles. But I do think it means we have to be much more thoughtful about how do we get the benefits while reducing the costs. I think it's a great thing that people are experimenting with. How can I develop an idea faster, prototype an idea, put together an initial set of code that would allow us to test it? Do I believe that means anyone should be shipping code to production, that everyone should actually be doing everything?

**Elizabeth Stone** (00:04:40):
Probably not, but I think that it's good for people to be exploring what's possible. And then like I mentioned earlier, the benefit of having product and tech teams together, is that if the business problem is clear, I think it's okay and it's healthy for there to be some fluidity in the roles that people play. Because instead of having to wait for the engineering team to be ready, to be able to prototype something, product and design can move faster on it, but they should still work with their engineering partner to think through, how should we productize this? How do we scale it? What are the guardrails for it? So, I don't think it makes the functional expertise obsolete. I think it means that teams have to be more comfortable with maybe this helps us move faster in a certain direction. From an organizational perspective, things I think about to make this more coherent or less frustrating, are some of the things that have to be in place for us to get the benefits rather than the cost.

**Elizabeth Stone** (00:05:36):
So, that includes clarity on source of truth data, guardrails on shipping code to production or testing, before we make large changes. Thinking about opportunities where we can trust the output of AI versus we should have a process or review that helps us check that we're getting high quality outcomes. And the importance of reiterating that humans are still responsible for what happens. So, it can be that an agent wrote the code or I helped to do an analysis when that's not really my background, but it doesn't make people not have the responsibility that comes with what they've created. So, I think investing in some of those core infrastructure and practices, and reiterating the accountability and responsibility for the outcomes, helps to balance some of what's possible with what we should actually be doing.

**Lenny Rachitsky** (00:06:27):
**Elizabeth Stone** (00:08:13):
So, you've mentioned some of the things, so I'll reiterate them and then maybe build. So, I have found that PMs, designers, data scientists, are able to get farther in the product development lifecycle before engineering really needs to be front of the line in unlocking things than was true a couple years ago. I say that with some caution, because like we were talking about, I don't think it's great to all of a sudden have thousands of prototypes, if they're not aimed at this is an important problem to solve for the business. And the engineering partners are aware that we're solving that problem. And that designers and product managers are going to take the lead in starting to shape the idea, but it's not working in a vacuum and it's not throwing a bunch of spaghetti at the wall to see what sticks. But when it's the right problem, approach in a thoughtful way with some alignment on that.

**Elizabeth Stone** (00:09:07):
I've seen product design data science move faster in the direction of let's get to something that's testable on this hypothesis. So, that's prototyping, that's writing code. The other thing I've seen, has been very valuable is we have a lot of information running around in the virtual walls of Netflix. We have experiments we've run over decades. We have insights from consumers. We have input from stakeholders across the business. And that was a problem that really presented a challenge of, how do we get the most out of that long history of knowledge and learnings, to say, let's apply that to the problem we've got now to move faster in this is a promising path or this is something that we've learned something about and we could leverage here? And AI is very powerful at distilling information, looking across a broad set of things, doing an analysis around it, getting to the core of here's some insights to start with.

**Elizabeth Stone** (00:10:04):
I would hesitate to rely on that exclusively, but I think it's a head start. And I find even in my own work day-to-day, instead of sending an email that disrupts someone of like, remind me what research did we do in what year and what was the question and what was the test we ran? I can find that almost instantly. Then I can form my own, here's what I find interesting about this. And I've now skipped a couple steps towards, is there something actionable here? So, that's data analysis, it's modeling, it's distillation of information. And I'm seeing more people do that, to your original question. So, instead of that needing to be only the experts who were here for 20 years and saw every experiment or know where to find it, we're now able to do that faster within product and tech across all functions. And a big unlock for us is our business stakeholders, sitting in finance and content and advertising, can do that as well. And then bring back an initial hypothesis where they want to work more deeply with the data scientist and engineer and so on.

**Elizabeth Stone** (00:11:03):
So, there's something there about the hypothesis generation, prototyping, thinking deeply about problems, that feels like it's accelerating and that functions are able to do that in a more fluid way. But I still see comparative strengths. So, data scientists are still going to be experts at, can we trust this data? Are we interpreting it the right way? What's the data versus judgment that we should be applying here? A product manager is still going to be exceptional at saying, have we really framed the what of this, the problem we're solving in the right way? An engineer still has a craft around the how. How does this scale? What does high quality look like? What problems is this going to create for us based on how we build and deploy something? So, I still see the nuggets of that comparative advantage. It's just that we're able to move more fluidly in a lot of steps that normally we would have blockers on.

**Lenny Rachitsky** (00:11:55):
There's so much interesting stuff here. One is this last point you made, something I've been thinking about. If we all become builders, will we still need separate functions? There's this member of technical staff trend that is happening across AI, where it's like, all right, we don't have a title. You could be anything. You don't have to be in a bucket. What you're saying here is you believe we will continue to have specialties, product person, engineer, data science, designer. While they do more of other functions, there's still a lot of value, and tell me if I'm hearing you correct, in having this specific discipline and skill and background.

**Elizabeth Stone** (00:12:26):
I still see a craft excellence that's really important in the disciplines that I don't think is going away anytime soon, even if there's fluidity or blurring of the work across the functional lines. It goes back to what I mentioned earlier of you still have humans who have to make sure that what we're doing makes sense. We're solving the right problems in a way that is best for Netflix members or business stakeholders. And that if I talk to an engineer, a data scientist, a designer, yes, they speak more languages now than they used to because they have the benefit of these AI tools, but there's still something that is not replaceable when I think about the craft and how they think about what good looks like. And that feels true across all levels. And I still find great engineering to be scarce, great data science to be scarce, great creativity to be scarce. So, yes, some things are easier, but that hasn't dissolved in my mind.

**Lenny Rachitsky** (00:13:27):
Are there functions that you are finding you are hiring more of, like the pie chart pie expanding, say for engineering or PM or design or something, and then functions you're need less of with AI tooling and LLMs rising?

**Elizabeth Stone** (00:13:43):
I'm not sure that it matches exactly to functions, but I can tell you what we're seeing more of, we need more of. We need more systems thinkers in a world with AI. That looks a little bit different across functions, but I could play out a couple examples. So, in our core infrastructure team at Netflix in central engineering, a lot of what made Netflix successful over time was that local teams with specific business problems could move fast to deliver. They very often were not feeling like they needed to be on a central paved path. They built the stack that they needed to solve the problem and have the impact. In a world of AI with agents operating across multiple systems, wanting source of truth data, the importance of having preferred paved paths that get the most of the benefits and produce some guardrails so we can make sure we're doing good work.

**Elizabeth Stone** (00:14:45):
Common infrastructure, common paved paths, solving problems once with a core set of capabilities becomes more important. So, we are hiring more people who can look across all the business domains and abstract that to here's the building blocks we're going to need in a world with AI. So, that's one of the lenses, but also just with a lens of what got Netflix here doesn't get Netflix there. And we're going to have to have a stronger set of infrastructure to move quickly in this future. So, that means that engineering profiles are more distributed systems, more infrastructure, more of that system thinking mindset than a local business expertise. Though, of course, we still have people who are deep in personalization and advertising and content delivery. So, it's more something additive for us to have that core infrastructure and systems thinking.

**Elizabeth Stone** (00:15:35):
If I take another example, like design, it's extremely important that our experienced design team is developing templates and again, systems thinking for what does great user design look like at Netflix, so that they can enable lots of people, including those who are not designers by training, to develop products that are coherent, that fit into the end-to-end member experience. I get really nervous about having different design languages or different types of user interactions and shipping Frankensteins, basically. So, designers need to then be the people we're hiring again for design systems thinking. How do we think about templates and expression of the brand? And what a good user experience looks like. And what is Netflix and the Netflix differentiated special sauce?

**Elizabeth Stone** (00:16:24):
So, there's more people on our design team that have to think that way now than, could I help to design a specific feature for a specific product? So, there's this stepping back to look at the big picture that I think is happening in every single function. And that requires some reorientation of skills among the existing team and also hiring people who've got that type of expertise. And across all of it, it's a mindset shift. So, we are not hiring people who are not excited to explore, try new things, understand lots is changing and feel comfortable with that ambiguity, be comfortable that there's a blurring of how we work and how we partner. That's true for people who are already at Netflix and people who we are adding to the team, that that curiosity innovation mindset, it's not been more important, at least in the time that I've been working in this field.

**Lenny Rachitsky** (00:17:22):
On the systems thinking piece, is the reason this is becoming more important, that people are moving so fast that you need to invest in platforms and frameworks and design language, and basically teach people to fish so they can not be blocked or are there other reasons?

**Elizabeth Stone** (00:17:38):
I think it's probably velocity. So, platforms do have a benefit of leverage. So, in general, that's an opportunity with or without AI, for a platform to get most teams 80% of the way there. And then they don't have to reinvent those building blocks. We have more bets that we're making across the business, more things we're trying to build. So, platform mindsets are good, and it's something that is relatively more recent for Netflix to think about that being a real critical enabler. There is also the sense of a scaffolding in a world of AI. So, not just the higher velocity, but you have more people doing more types of work that are different or new, like we were talking about. And there's risk that comes with, how do you think about access and identity in that situation? How do you think about security in that situation? How do you think about shipping high quality code and design and user experiences?

**Elizabeth Stone** (00:18:34):
And so, I don't think it scales well to have each person who's building something have to go figure out, could you remind me what good looks like here? And what are the bumpers or guardrails I should keep in mind? I think we need to encode that in our paved paths and our ways of working. And for a data science or analytical field to encode, here's the source of truth data, here's how to interpret it, here's how to access it, here's what to do with it or not to do with it and to be careful with certain types of data.

**Elizabeth Stone** (00:19:03):
An organization that has thousands of people can no longer rely on tribal knowledge or I'm going to find the one person who knows this. So, this was a challenge that was there before AI. It's probably a more urgent challenge with AI. And I like the idea of using AI or any new tech to motivate... We knew this is work we needed to do. No time like the present to invest in that more heavily across the team.

**Lenny Rachitsky** (00:19:27):
I wonder if another reason for this becoming more valuable is because agents are now doing a lot of work. And giving them the context, giving them the scaffolding, giving them the design language, just speeds all that up?

**Elizabeth Stone** (00:19:38):
Yeah. And one of the visions we have at Netflix is we will have so many agents that are contributing to doing work that you need to be able to reason and rationalize throughout that. The humans are the ones guiding what's the problem we need to solve. Do I feel like what we're producing is impactful and high quality output? But the work will be done by both humans and agents. And that creates velocity and benefits and it creates risks. And I think that's important, especially from an engineering perspective, that we figure out how to manage that in a way that lets people move quickly, but doesn't create undue downside or risks for the company.

**Lenny Rachitsky** (00:20:20):
This connects so directly with... Jenny Wen was on the podcast. She was Head of Design for Claude Code and Cowork and had this whole design process is dead kind of thesis. And the pitch there is just there's no time for design, the design process. And instead, as a designer, you're just kind of steering people and pointing them in the direction and adjusting and also thinking big pictures when you have the time. And it feels like that's what you're describing here is create the platform for people to move fast and then there's no time for design process of a specific new feature.

**Elizabeth Stone** (00:20:51):
I have mixed feelings about that, because we do want to enable with infrastructure and systems thinking, more people to do great work with strong design as part of it. Why not take that opportunity that the new tech provides? But for our most important priorities, design is critical to solve things in the right way. So, we do still make time for important design work. It can move faster. The designers themselves have more tools in their toolkit, so they can do incredible work at a faster velocity, show more options, learn, iterate, test more quickly. But I think it would be a mistake to say design and deep design expertise and thinking gets squeezed out, just because we can write code faster, we can do data analysis faster.

**Elizabeth Stone** (00:21:43):
At least for a large scale consumer product like Netflix, I feel like we would lose one of the things that makes Netflix great, which is the product technology and design makes a lot of complexity invisible and makes for a seamless customer experience. That's a design mindset that has to be core to it. So, the work itself might look different, but I don't think we lose the mindset.

**Lenny Rachitsky** (00:22:06):
That's an awesome counterpoint. So, what I'm hearing is trending up skills, attributes you look for, systems thinking. And this mindset of being comfortable, and excited about change, and what's coming, and not being stuck in your own ways. What are you finding is trending down? What are you less looking for that you used to value more highly?

**Elizabeth Stone** (00:22:28):
The days of very narrow, deep specialization feel more limited to me. I can come up with examples where we still need it, because there's an industry or technology expertise where there's only a few people in the world who really know how things work. We have examples of that on the team for encoding or how our playback systems work, and things that have been incredibly innovative and novel for Netflix. I still believe we need specialized practitioners in those spaces. But as a general rule, compared to five or 10 years ago, I would believe we have fewer specialists and more people who are generalists or adaptable in multiple directions. And that could be adaptable across functional expertise. It could be adaptable across flavors of engineering. So, can I navigate both backend and front end systems? Can I hook into infrastructure with a lot of expertise? I think the mindset now needs to be I can learn that quickly.

**Elizabeth Stone** (00:23:32):
And that goes back to the systems thinking. So, I think specialists can learn to have a broader array of tools more easily than was true in the past. So, we need fewer of them perhaps, because talent's able to grow in that direction. And there's something about sticking to a narrow specialty that maybe triggers for me a concern about, what about the mindset of growing in different directions and exploring? And I don't want to be too narrow even in my own assessment of that, but it's important that people who are specialists still have that sense of, I want to try a new way of solving these problems versus the way we have in the past.

**Lenny Rachitsky** (00:24:13):
And when you say specialists, are you thinking front end, I'm a front end engineer versus a backend or are there other versions of that?

**Elizabeth Stone** (00:24:18):
Yeah. Or it could be a domain set of knowledge of I'm a deep-

**Lenny Rachitsky** (00:24:22):
Like a payments expert?

**Elizabeth Stone** (00:24:23):
I'm a payments expert. I'm an ads marketplace design expert. I'm an expert in this very specific tooling that studio productions use. So, their specialist and subject matter expertise is an advantage, provided that person is willing to grow and extend into, is this really still the right tool or the right way to think about the problem? So, I think it's the layers of the stack from an engineering perspective that there's less specialty. And then tools that are unlikely to be static or to have a lot of inertia around them. I would think we would want people who are able to innovate and imagine what's the future version of this. And so, we want more talent like that.

**Lenny Rachitsky** (00:25:09):
Awesome. So, coming back to the systems thinking piece, people hearing this are like, "Okay, I got to work on my systems thinking skillset." How do people develop the skill? Is it just do it for a long time, work at a lot of complex projects? I think of this book that everyone always references with the slinky on the front, Thinking in Systems. Yeah. How do people learn this?

**Elizabeth Stone** (00:25:31):
Small trick. Each problem you're trying to solve, step out one click to the like, what am I assuming is true about the broader space in solving this problem? So, I was given a task to build some new feature for the Netflix member experience. Let me take one beat and think about, what is the bigger consumer problem we're trying to solve here? What's the type of content that this feature is going to be able to support? Do I think that the way I was planning to build this is going to make sense in a way that scales across multiple content types? Or it could be something that's a capability that then is contributed to a platform set of offerings from multiple areas. Is the consumer problem that I'm solving with this feature going to be one of the most important consumer problems that Netflix is going to need to solve, as we have an expanding world of entertainment and we want to make it more personalized and immersive?

**Elizabeth Stone** (00:26:34):
Those are all questions that you don't have to boil the whole ocean. You don't have to solve for Netflix's overall strategy and who are we relative to competition. But you take the thing you're responsible for and you just do one zoom out of the problem you're solving and question that. I wouldn't spend too long in the questioning state, because then you're stuck, then you're not making forward progress. But I think that helps people to think in terms of systems, and question that, are we solving the right problem in the right way that matters for the end consumer?

**Lenny Rachitsky** (00:27:07):
As you describe it, another way I'm thinking about it is think... if you were your manager, what's their broader perspective across not just your one team and problem and KPI, but the larger picture?

**Elizabeth Stone** (00:27:18):
I've got advice over years that is similar to that, which is are there ways that I can do my job that helps my manager do their job? And so, if I thought about all the things I'm directly responsible for, but I though about it from the perspective of my manager, so not just product and tech, but finance and content and other parts of the business. I would naturally zoom out and think about how all these component pieces need to come together, and how the whole could be greater than the sum of the parts. I think that's useful thinking. And for engineers to think about, how do I leave a better version of these systems? How do I think about the thing that's going to be high quality and scale for others? There's both a, how do I help my manager? And there's, how do I help my colleagues?

**Elizabeth Stone** (00:28:02):
Which is a core part of some of our engineering principles of do the thing that is right for the broader organization, instead of just what's right for you locally. That's systems thinking as well. So, it's not just seniority, but it's breadth of the way I solve this problem and I build this, is it going to be useful to my colleagues? And am I going to leave a stronger version of things for the future set of innovations that we want to make?

**Lenny Rachitsky** (00:28:24):
That is awesome tactical advice. Making your manager's life easier is always a good tactic career-wise.

**Elizabeth Stone** (00:28:31):
Several reasons. Yeah.

**Lenny Rachitsky** (00:28:34):
Following the thread a little bit, I know you all added career ladders and levels. Recently, it was a new thing. You used to not have these things. So, on that thread, what have you added to the career ladders within this AI world, if anything, that you find you want people to lean into more, you're looking to more or not? Did you not change your career ladders and performance criteria?

**Elizabeth Stone** (00:28:58):
So, the way we've approached this so far is, instead of trying to articulate at each level exactly how AI changes those expectations, to instead put an overlay across all of the talent at Netflix, people on the team and those who are hiring, to talk about an aspiration for AI fluency. And what that looks like is going to vary by function. It's going to vary based on where you are in your career. That could be what level you're in or what type of role or persona work you're doing. But the aspiration for AI fluency, which is a tough thing to define. So, does it mean that I have an experimentation mindset? Does it mean that I know where AI is useful and not useful? Does it mean that I've actually built things using AI? I feel like the way that has shown up in career ladders and how we talk about it evolves almost by the quarter, if not month or day, because the tech itself is advancing so much.

**Elizabeth Stone** (00:29:57):
So, the most useful thing is not to make it level specific or role specific, but to encourage everyone towards the expectation on AI fluency, which doesn't mean use it as a tech for the sake of tech. It's tech where it's useful, to have good judgment about that and to have the mindset to be open-minded to explore and try new things, that's the non-negotiable for all roles. And that's true at the senior most levels of Netflix, where we talk about we too need to have deep fluency in AI, even if we're not writing code as part of our day jobs. So, that's changed. And then that's showing up in our hiring practices as well, getting comfortable within interviews, exploring how are people thinking about AI or technology.

**Elizabeth Stone** (00:30:38):
What are they using in their day-to-day or their current job? How comfortable are they with change and exploration? And even for things like coding interviews, allowing candidates, of course, to use AI tools, because that's going to be part of what the work requires now. So, those have been shifts that we've made, but I doubt it's a shift that's done versus we're right in the middle of it.

**Lenny Rachitsky** (00:30:58):
I'm just going to keep following this thread. Obviously, AI is transformative for coding. It's a big unlock for prototyping. Are there other use cases of AI at Netflix that have been really impactful, that people may not think about or not realize?

**Elizabeth Stone** (00:31:16):
So, there's two that come to mind. So, the first is data analysis, distillation of information, modeling, which is using the tools to get our arms around all the insights we have, similar to what I mentioned before. What experiments have we run? What are the metrics that I should be looking at for a certain problem? What's the consumer research that we've done? And that is much higher velocity and much higher quality, contingent on you check that the results are valid, you work with your local data scientist on, am I using the source of truth data on this? But that's been a great one. And that's one personally that I would say I most use some of these tools for. So, that goes beyond prototyping and coding to general analytical thinking, and translating data to action and insight. The other one is on the content production creation part of the business, which has lots of applications.

**Elizabeth Stone** (00:32:14):
This was true before GenAI. So, ML and AI were deeply used in a lot of the production tools. We've used them to think about how to create promotional assets at scale, how to localize in subtitles and dubs. So, GenAI is a big step function in where the impact can be. In creative ideation, we call those things pre-visualization or basically bringing a creator's vision to life before you even get into the... You bring people to a set and start to actually go through the production itself. There's lots of use cases in post-production. So, we recently acquired a company, InterPositive, that was started by Ben Affleck, that built a set of models and capabilities. That allow you after you've shot something to relight, reframe, reshoot, change dialogue in ways that are very impactful to get higher quality content.

**Elizabeth Stone** (00:33:05):
Are still led by the filmmaker, creator saying, "You know what? I would like to try something else to bring this vision to life." But that impact is extremely promising and we're seeing lots of productions leverage different tools, some of them built in-house, some of them that we enable through other vendors for those content creation use cases. And then as we think about how content comes to the product, I mentioned localization, subtitles and dubs, but also how we create high quality trailers, images, artwork at scale that then we can use to help make sure that titles find their audiences around the world. Those all are huge levers when we think about the AI impact. So, that again, goes well beyond prototyping or coding to some of the creative use cases. And you can imagine that, just like they work for studio productions for film and TV, they work for advertising, they work for marketing, off-service campaigns. And so, those are all areas that we're exploring.

**Lenny Rachitsky** (00:34:01):
**Elizabeth Stone** (00:35:25):
The Netflix prize.

**Lenny Rachitsky** (00:35:26):
Yeah, the Netflix prize. Just show an example of how early you were to AI and ML. I think it was a million dollar prize to optimize the Netflix ranking algorithm a little bit, whoever could optimize it the most. And I think the winner optimized it by a few percentage points, something like that. And it was a huge deal. All these super smart people got around the world and it happened a few times, right?

**Elizabeth Stone** (00:35:49):
I mean, you said it on my behalf. Often, when there's questions about how is Netflix thinking about AI, it's great to remind people of exactly that point, that this is not new to us. That especially for personalization, it's been central to delivering a great experience to members. It's impossible to take the breadth of content that we have. There's ever more content, that's one of the challenges we face. And make discovery easier and easier and easier, which is one of the challenges that Netflix has. And using AI and ML has been a way to do that. You want to personalize right title for the right person at the right moment. That problem gets harder. The more exciting our catalog gets, the greater breadth of content we have, not just film and TV, but games and live and podcasts. Personalization becomes even more important and what that experience is.

**Elizabeth Stone** (00:36:40):
So, we can take a lot of that history and say, okay, well, now how do we solve this problem? Because the tech is even more powerful, but it gives us a running head start in being clear about the problem to solve, how important it is that Netflix solve that for our members. And then the same is true, as I was mentioning on the creative side of the house, AI and ML have been in things like visual effects or in localizing language for a long time. Now we say, what's the next era of that when the tech is more powerful? And in both cases, it ends up taking a strength that Netflix has, which is marrying entertainment, and technology, and making sure we stay ahead of the game to deliver things that are even better. So, I love that it's part of our history. It still continues to be a strength and it's going to have to be a strength, given the size of the challenges we're facing around the breadth of entertainment, while keeping a great experience.

**Lenny Rachitsky** (00:37:33):
Yeah. And I love that back then it was called machine learning and AI was like, no, no, it's not AI. AI is never going to happen. It's just machine learning.

**Elizabeth Stone** (00:37:41):
Well, then all of a sudden, we call everything AI and some of it's machine learning.

**Lenny Rachitsky** (00:37:45):
That's right. That's right.

**Elizabeth Stone** (00:37:48):
It depends, the thing that is of the moment to describe. So, I think we bucket all of it as AI now.

**Lenny Rachitsky** (00:37:54):
Yeah. And that's cool.

**Elizabeth Stone** (00:37:56):
And there's a lot of AI use cases that are not generative use cases. So, we could go down a deep dark hole of all the specific things. But in general, I don't think it would surprise anyone that Netflix is using a broad array with so much excitement about what's possible. The fun thing at Netflix for the people who work here is that if you're really passionate about the applications of tech for creative outlets, for consumer products, for infrastructure, we have all of those problems and AI is at the center of them. And it's good not to forget that that's true. Even if Netflix isn't branded as an AI company, AI is a tool that we're very comfortable using to get these great entertainment and technology outcomes.

**Lenny Rachitsky** (00:38:37):
The other really interesting thing, just to keep complimenting Netflix here, if you look at the early culture deck of Netflix and also our conversation last time, things that emerge from that are things like high agency. This was something core to Netflix in the beginning. High agency, autonomy, high talent density, very bottoms-up thinking, super quick experiments and launching, paying top of market. This is what I hear constantly now from how the top AI labs operate. So, we're all ending here and this is where Netflix has been forever.

**Elizabeth Stone** (00:39:13):
Yeah. It's a little prescient in understanding what makes talent incredible. I've thought about all those aspects of the culture at Netflix as, this is going to sound a little bit nerdy, but excellence as an operating system. So, the goal of all those cultural elements wasn't the end bone themselves. It wasn't, let's just make sure people have as much responsibility as possible. We don't like process, so let's make sure that we don't have any of that. It was instead a very strongly held opinion that you get to excellence by giving people a lot of agency and accountability, by pushing decisions as deep in the organization as possible, hiring great people who can be trusted to have good judgment and make good decisions. And that ends up driving incredible outcomes, plus a lot more motivation and sense of responsibility. It means every person on the team can feel like I'm being given a lot of keys and a lot of accountability for what happens here.

**Elizabeth Stone** (00:40:16):
And I myself feel like when you know you're carrying that level of trust and accountability, you want to do your best work. And so, there's something that feels very intuitive about Netflix's culture has always been aiming at excellence. And when you have great talent and you give them the ability to do their best work without micromanaging it or drowning it in process, you actually get much better outcomes. And so, I do think that the newer era companies are picking up on something that is feeling very familiar to us. And it's not something that comes easily. So, culture's not a static thing. Culture needs to grow and evolve as the company gets bigger, the types of problems you're solving, change. But the notion that we're going for excellence and trusting that exceptional talent needs to be able to do their best work, that's unchanged and something that I think continues to be a special sauce for us.

**Lenny Rachitsky** (00:41:11):
I love this concept. Excellence as an operating system. It's very systems thinking you might say for how to set up a company.

**Elizabeth Stone** (00:41:18):
Exactly, Lenny.

**Lenny Rachitsky** (00:41:20):
So, everyone listening to this will want excellence as an operating system. Who would not want this? It'd be helpful for people to hear what are the ingredients to make this happen. One is obviously high talent density, just hiring only the best. Two is accountability. There's the input and the output, essentially. Input, amazing people, the top people, make them accountable, give them autonomy. What would you say are the pillars of creating this excellence as an operating system, if founders are listening to this and like, I want them to do that?

**Elizabeth Stone** (00:41:51):
Well, the talent density is the non-negotiable. You have to start with that. If you don't have that, you can't get to a place where you have confidence in decision-making at all levels of the organization, allowing people to take risks and innovate quickly. That's a big part of excellence in the Netflix culture, which is being very comfortable with risk taking. We don't try to avoid failures. We try to recover quickly when we have them. I think there's been great examples of that. Our foray into live was a wonderful example of being comfortable taking a ton of risk, knowing it would be imperfect, knowing we would learn fast and we would be better for it. I've never been prouder of the team, seeing how we worked through that. So, you have to be talent density, comfortable that people are going to take the context that you give them, strong judgment, and risk-taking, and fight for the things that are the best outcomes for the business.

**Elizabeth Stone** (00:42:49):
You have to be very clear that what you're doing is driving outcomes for consumers and Netflix. So, Netflix matters, Netflix members' matter. It's not about my own personal success or what I prefer. So, there's a selflessness that is part of this excellence operating system. And then the other thing I would say is some of the things that are... they're really unnatural for humans to do. So, I could give a couple examples of things to get comfortable with, which is there are certainly days where I see decisions happening and I think I would make a different decision. Is that really going to be the best thing? But my job, especially in the Netflix culture, is not to step in, in every one of those cases and overrule or veto or question someone. Especially if it's not material, it's not going to burn the place down, let people make that decision and learn from it and ask for those reflections afterwards of how did it go.

**Elizabeth Stone** (00:43:52):
Maybe I was wrong. Maybe the decision was a great one. But that it's related to the risk taking. And help people learn how to feel comfortable making their own decisions, especially when they're not all going to be the right decisions and they're going to learn something tough from it. I felt that myself from my boss and my peers, saying, "This is your decision. I can provide input. I can help you brainstorm. It's yours in the end." And it just doesn't come naturally. When the stakes are high, when I feel responsible for what the org's doing to let people lean into risk, can be uncomfortable. And I think that also means in cases where things are not going well, as another example, to not assume that process is going to fix it.

**Elizabeth Stone** (00:44:36):
Something I've learned over the past few years, that when planning is difficult, I've never heard someone say like, "Oh, we figured out the perfect way to plan or the perfect way to go through feedback and leveling and compensation." But every time we saw that and we added more process, we spent more time without getting better outcomes. And so, it's another unnatural thing that I think everyone's inclination when things are hard and complicated, is you think you're simplifying the problem by putting a lot of constraints around it. But it actually goes against the, is there a more creative way to plan or to make people decisions or to make prioritization decisions that actually get us to better outcomes? And so, it's a resistance to do the thing that a lot of bigger companies would do and to feel comfortable in that discomfort very often. So, that's something I feel in my role and I would believe a lot of people at Netflix feel it, because you try not to do the thing that is standard.

**Lenny Rachitsky** (00:45:39):
It's easy to say that and hear that, but I so know what you mean, where somebody screws up and you're like, "Okay, what was the thing that went wrong? Let's put a process in place to avoid this from happening." And what you're saying is you need to resist that, because that slows things down. And the best people don't want to be working in a place with all these checklists and processing gates and things like that.

**Elizabeth Stone** (00:45:58):
No. I think the best people want to know there's going to be a blameless retro and they're going to feel so individually responsible that they're going to say, "How do I make sure this doesn't happen again?" Not with process, but with how could I share these learnings? How could I do work differently to make sure that I get to a better outcome next time? When you are trusting people to take those reflections and learn and grow, I think you get much better outcomes over time. And you get a much stronger team, which I think is part of our role as leaders, of you're trying to grow a team that is resilient and durable and knows how to have great impact. You're not trying to control everything.

**Lenny Rachitsky** (00:46:41):
Which is a key to building a team with high talent density. There's two sides of this that I want to chat about briefly. One is the hiring and the other is keeping the people. So, you're famous for the keeper's test. We talked about this last time. Another unnatural thing for people. People that want to understand what this is, they can listen to the first conversation, but how has that evolved over the last couple of years? That still a core part of the culture, this idea of the keeper's test?

**Elizabeth Stone** (00:47:05):
It's often cited in a way where you think of keeper's test as that moment where you decide to let someone go, that they're not the right fit for the role and the conversation about that. But it's equally commonly used to have a conversation about how extraordinary someone is, how well they're doing in a role. Because the entry point is for me to say to one of my direct reports or for them to say to me, "How am I doing on your keeper test?" And the lion's share of the time, my response is, "I would fight so hard to keep you. Let me go through a set of things that I think you're doing such a great job at, what your strengths are, where you're having a lot of impact. Here's how you could be even better." So, it's an entry into a conversation that is very positive and uplifting for people, but the framing is, do I pass the keeper test?

**Elizabeth Stone** (00:47:56):
And then, of course, there's the harder situations where I'm evaluating, does someone pass the keeper test or they're asking me? And this is the toughest thing to say, "To be honest, you're not passing that right now. I think you could get there in some cases." And that comes with feedback and what are those milestones. Or in some cases you're saying, "We've really tried and I don't see the path to success." So, it's an anchor and an entry point for a conversation that can go lots of different directions. And the thing I like about it is it's good hygiene on feedback and checking in on how things are going and forcing a tough conversation sometimes, instead of shying away from it.

**Elizabeth Stone** (00:48:37):
Or to keep great talent, you do need to say you're doing great. That's an important part of making people feel recognized and valued. So, I don't want it to come across that we just have this very negative view of it. I think there's this positive side of the coin as well.

**Lenny Rachitsky** (00:48:53):
Awesome. I guess just to explain to people what this is so they don't have to go listen to a whole other podcast, I'll try to briefly explain it. The idea here, a part of the Netflix culture is that when you have people reporting to you, you should always be thinking, would I hire this person today knowing what I know about them? And if not, then I should probably let them go. And the idea there is to keep the high bar, to not ever just settle. Okay, this person, they're here, I guess we'll keep them around. Is that roughly the way to understand it?

**Elizabeth Stone** (00:49:21):
Yeah. And the way it can... it's sort of a corollary to that. If that person came to me today to say they were leaving, would I fight to keep them or not? Or would I say, if my sense is relief of, oh, yeah, it probably would be better to have someone else in this role, I should've taken action and having that conversation sooner.

**Lenny Rachitsky** (00:49:41):
As you said, it's so many uncomfortable things you have to do to maintain this culture.

**Elizabeth Stone** (00:49:47):
Yeah. Well, the keeper test is one, maintaining talent density, context, not control among leaders. We talk about being highly aligned, but loosely coupled, which is where light process, the minimum to make sure we're clear on the priorities and we can execute them is what we're solving for. All of these things are not things that human beings or organizations at scale tend to do. So, it's constant diligence to try to maintain the thing that's made Netflix a special place. Because in the end, it's the work and the culture that attracts people and retains people. And we need that to be a successful business.

**Lenny Rachitsky** (00:50:22):
That's exactly where I was going to go. So, to make this work, you need to attract the best people. It's always been very hard to attract the best people. It feels insanely hard these days with the amount of dollars flying around, the fancy AI labs, so much competition. It's crazy. What have you found to be effective in convincing the top people to still come to Netflix and join versus all the other fancy places they can go?

**Elizabeth Stone** (00:50:49):
Yeah. We've always had a lot of competition for talent. It might feel more pronounced right now, but we have great talent on the team. Maybe that goes without saying, but I feel like I should say it out loud because I believe it. We have incredible talent at Netflix, recent hires, long tenured people. I'm always impressed by the work that the team is doing. So, I don't feel like we've suffered or other companies are vacuuming up all the good people, because so many of them I do think sit at Netflix. It does feel like we have to be more explicit about the types of people and talent that tend to thrive at Netflix versus other companies, like some of the Frontier Labs. So, people at Netflix have to be passionate about the application of technology and the application or building products to solve a certain set of problems.

**Elizabeth Stone** (00:51:45):
You have to love entertainment. You have to love consumer products at scale. You have to love the global nature of that. There are a lot of incredibly talented people who love that sweet spot, I am one of them, between tech and product and entertainment. And how do you make those things come together in a way that's remarkable? And you use AI to do it. You use other technologies and products to do it, but that has to be something that drives you to be really excited about a lot of the roles at Netflix. If instead you're inspired by some of the foundational work that the frontier model companies are doing, which is exciting in its own way, it's a different persona. It's a different... Here's the problem space that I want to work in. But I don't think there's a shortage of people who get really excited about the applications of the technology and see the connection to that, to things that they love and use every day, like Netflix.

**Elizabeth Stone** (00:52:39):
And so, that gets me up in the morning and I think it gets a lot of the team members up. And we have this conversation about that's something special that only talent at Netflix can do, or fill in the blank for another industry that's deep in the application of it. I think that's inspiring.

**Lenny Rachitsky** (00:52:54):
I want to touch on a couple things that I've been thinking about in this world of AI that we're approaching. One is junior people. It feels like everyone's just like... This is a good example. You're hiring a lot of awesome senior people that have proven they're awesome and high talent, density, high bars. Also, just AI makes it so easy to do stuff that people may not be learning how to do anything. Like junior engineers, I'm thinking, or junior PMs, junior designers. How do new people become these awesome senior people? Is there anything you think about? Are you hiring junior people? How do you think about this? What happens with junior people not necessarily learning or having a path to learn to become the senior person?

**Elizabeth Stone** (00:53:39):
We are still hiring junior people and they're really important to our talent strategy. So, we still have an intern program, we still have a new grad program, which was new for us as of a few years ago. So, prior to a few years ago, we were only hiring more experienced talent across all the functions. Now we do hire people straight from undergrad and graduate programs and we'll continue to do that. So, even in a world of AI where some things are easier, we were talking earlier about mindset, AI fluency. From my experience, younger folks are more open-minded. They tend to be more native in some of these new ways of working. For a company like Netflix, they're also very fluent in how entertainment is changing, how consumer behaviors are changing, how product and tech is influencing that in the products that they're using. That's really important to have on our team.

**Elizabeth Stone** (00:54:38):
So, there's the part of the persona, which is who are you as a new grad who's an engineer? But there's also, who are you as someone who's in their early twenties and has a perspective on the world that is highly valuable and a comfort with the way the world is changing? So, that's why I say it's a critical part of our talent strategy. To the, okay, so you step into the role and you have AI tools that didn't exist five or 10 years ago. I would say mastery of the craft is still very important. So, going back to, as the team member, I'm responsible for the quality of code that I am submitting for production. I'm responsible for the quality of products that I'm building, how they are designed, what that user-consumer experience is. None of that is going away. So, if I think about more junior or earlier career talent on the teams, we need to be investing just as much in the mentorship of this is what good looks like.

**Elizabeth Stone** (00:55:29):
This is how you use these tools, but you still take accountability for what the outcomes are, what the quality of the output is. And I think I mentioned this earlier, I find that mastery and that craft excellence scarce still. So, we want to make sure we're teaching that. I think it's a valid concern of, how do I get that if I'm not as hands-on as I would've had to be? But you still carry responsibility for reviewing code, testing code, being able to diagnose problems, knowing what a good product looks like. I think that's a very scarce skill to say, this is excellence in a product that solves a problem that matters and in how it's designed.

**Elizabeth Stone** (00:56:06):
So, I don't think that craft mastery, the importance of it is going away. Probably the way we train and grow talent has to change, because they're going to use different tools. And I can guarantee you that earlier career talent is going to be teaching older folks like me many new things, too. So, I think it goes in both directions.

**Lenny Rachitsky** (00:56:26):
Where do you think engineering goes in, I don't know, five, 10 years? Do you think people need to still understand code? Or do you think there's this abstraction layer that sits on top where you don't even have to learn C++, Java, Python, whatever?

**Elizabeth Stone** (00:56:42):
I think there's a difference between being able to write lines of code in a particular language, like Python or C++ and understanding how code, computer systems, products work. And I don't think the latter is going away, because if we trusted agents to know all the languages and write all the code, we're not going to know why is something... is it a good product? Is it a bad product? Is it working as we expected when it doesn't? Like I mentioned earlier, we take a lot of risk. We fail fast, we recover fast. That requires an understanding of how are these systems working.

**Elizabeth Stone** (00:57:21):
I might use an agent to help me understand those things, help me detect an anomaly or something that's broken faster and triage it, but I still need to have a fluency of what is this thing that we're building and how does it work, so I know if it's good and I know how to fix it. I don't know. I hope that doesn't go away, because that's like a, how do we make the world a better place through the stuff that we're building? I think requires some understanding of what we've built.

**Lenny Rachitsky** (00:57:46):
What I'm hearing, which it makes sense, is you may not have to write the code, but you have to understand it and what's happening. But it's so much harder to just... as a person not writing it to actually have that instilled in you.

**Elizabeth Stone** (00:57:59):
I think that's one of the things that the learning curve is very steep on right now. So, looking at some of the code that some of these models or agents are writing, they're very hard to follow. It's like, I know I'm getting better performance from this, but I have no idea why. And if this thing breaks, I'm going to have no idea how to fix it. That makes me uncomfortable. Maybe that's because I'm still on that learning curve of, how do we operate in that world? What's the set of tests or rationalization and understanding that we need to have to get comfortable with it? But at first glance, it looks very unfamiliar and very unsettling. So, I think engineering over time will evolve to be comfortable with that, and have fluency in it, and know how to guide new tech, and agents, and new capabilities to make sure that we feel really good about what the output is.

**Lenny Rachitsky** (00:58:48):
I wonder what the metaphor is for this where this... I continue to be astounded by how much engineering has transformed in two years. It's like a completely different dropdown. We used to sit there in NID and write code, and now you're just talking to agents and reviewing code and shipping 100 PRs a day.

**Elizabeth Stone** (00:59:05):
It feels like it's an acceleration of how much engineering has changed. But if you looked over the last 10 years or 20 years, you would say the same thing. So, there's just something that's moving faster. And it's hard to wrap our heads around how quickly it's moved in the past couple of years. But it's not totally unfamiliar that engineering or data science or product would have these big shifts, just like how filmmaking works. If you look over the last 100 years, it's unbelievably different because of technology and new tools that we've brought to it. Just feels like the cycle is speeding up.

**Lenny Rachitsky** (00:59:46):
Okay. I want to talk about entertainment for a brief moment. I'm curious just how entertainment will change over time in the next, I don't know, five, 10 years. Just today, we open up Netflix, check out some shows, watch some videos, it hasn't changed in a while. Just that idea of like, oh, I'm going to watch The Pitt and just watch it all. I'm going to watch a movie. I got TikTok, I got Instagram, feeds of stuff. How much different do you think this will be in, I don't know, five years, the way we entertain ourselves?

**Elizabeth Stone** (01:00:15):
I think it's already changing at Netflix, because entertainment is not going to be one thing in the future and it's already not one thing now. So, part of the reason that we are going beyond film and TV in our offering is because there's an expectation that consumers have of much greater variety across formats, devices, moments of the day, that Netflix needs to be able to serve well in order to meet consumer expectations and hopefully exceed them over time. So, when we think about the addition of mobile and TV or cloud games, live content, podcasts, working with a broader set of creators who are now on the Netflix service, all of those things create a greater breadth of what entertainment is. And Netflix is able to define and expand that. And it puts a higher bar or expectation on, how do we make sense of that for a Netflix member?

**Elizabeth Stone** (01:01:11):
So, how do we show you this very seamless journey from I listened to the Bill Simmons podcast to I watch Quarterback, because I love that as one of the Netflix offerings in the more, you could say traditional film or TV space to I play the most recent FIFA cloud game. And I want to be able to do that in both TV and on my mobile phone, because now I'm on the move and I want to be able to discover and engage with the content at different moments of the day. That's already a journey that we're building into Netflix, which I think will become stronger and stronger over time. So, the future of entertainment isn't going to be one thing. And it's going to have to be more personalized, more immersive, more interactive, with this sense of this is a world that I can explore in lots of different directions, depending on what I'm looking for in the moment.

**Elizabeth Stone** (01:02:00):
And the challenge Netflix has is we've got to make discovery and engagement much easier than it feels today. We have tons of content, it can feel very fragmented, especially when you consider all the services or offerings out there. And I think Netflix is very well-positioned to understand how to solve that problem across entertainment, product and tech.

**Lenny Rachitsky** (01:02:19):
The other element of this is AI, obviously. As an outside observer, it's so interesting to see how in tech it's like AI, I love it. It's the future, it's the best. In Hollywood it's like, no, shut it down.

**Elizabeth Stone** (01:02:33):
There's a mix. There's a very wide array. So, Netflix's role in this is to enable creators with whatever tools they want to use to bring their vision to life. There are going to be some creators or filmmakers who are on the end of the spectrum that says, "Absolutely not. No AI. That is not how I do production. It's not consistent with my vision." That's fine. We work with those creators. There's other creators, a growing number of them I would say, who are very interested in exploring, wait, can these GenAI tools make something possible that wasn't possible before? Can I tell a story in a new way? Can I make that story higher quality and more resonant for audiences? Can I do things that are extra creative in how I think about bringing a story to life? And we support them as well and we support all the folks who are in the in between.

**Elizabeth Stone** (01:03:24):
I think that's a really important position for us to be in, again, because entertainment is not going to be one thing. There's not going to be one format. I think there's going to be types of film and TV that feel traditional, and then there's going to be entirely new formats that unbelievable creators help to bring to life. And Netflix wants to participate in that, which means we need to have a flexibility in the tools that we provide, and the types of partnerships we have, and to really have a creator enablement view, rather than a prescriptive, we only do this one way.

**Lenny Rachitsky** (01:03:54):
I think people are going to be surprised by just how good AI content is. Spencer Pratt's videos are just like... everyone's like, wow, this is entertaining. Obviously, AI, but it's so interesting. Do you think we'll get to a place where just whole TV shows are AI and people love it?

**Elizabeth Stone** (01:04:09):
I have a hard time picturing entertainment that doesn't have humans at the heart of it. So, that's humans in the creation of the storytelling, which I think is a scarce and valuable skill. Storytelling is one and the same with humanity and knowing what connects with people. So, I think humans will always be a core part or a critical part of the story. And I think watching characters on screen who don't have that humanity feels less compelling to me. And what the power of storytelling really is, to see another human and to watch how they perform a role or bring an emotion to life, that's such a human element. Will AI help to bring that to life? Will it play a material part in some of those productions or how we get them to look and feel a certain way? Yeah, definitely. But I don't see the version of it that doesn't have the human as the backbone.

**Lenny Rachitsky** (01:05:13):
There's a quote that I think is misattributed to Salman Rushdie, which is, "When a child is born, they first ask for food and water and protection and then they ask for, tell me a story."

**Elizabeth Stone** (01:05:27):
It's a thing going back since the beginning of time, that storytelling has been a key part of community, and social networks, and human feeling and connection. So, I love the idea that technology can amplify that and can bring that to life in very new, novel, exciting ways. But to say storytelling wouldn't have that humanity at the center feels like something would be missing.

**Lenny Rachitsky** (01:05:57):
We're going to see some wild shit over the years coming out of all this.

**Elizabeth Stone** (01:06:00):
Oh, there's no question about that. And a lot of it could be very entertaining. I don't debate that either. But I think there's going to be a broad range and I think Netflix needs to be at the center of shaping that and bringing that to life, which is our plan.

**Lenny Rachitsky** (01:06:15):
Amazing. Well, we covered a lot of ground, Elizabeth. Before we get to our very exciting lightning round, is there anything else that you wanted to share, leave listeners with, maybe double down on some things we've talked about?

**Elizabeth Stone** (01:06:27):
It probably came across throughout, but I would underscore that this is a really exciting time to be building products in entertainment. Everything we talked about of what's changing in the tech and consumers and what is entertainment. We're at this unbelievable high velocity innovation period, so it's what keeps me at Netflix. I think it's a fun place to be. I would be missing something if I didn't reinforce that I think that's true. I also think that as an industry, we spend a lot of time sometimes talking about the pure tech or the capability and we sort of lose the forest for the trees. We're trying to build great consumer products that people love. We're trying to make great entertainment that people love and it's their favorite thing, that I don't want that to be lost in. Of course, there's amazing tech and product stuff that sits underneath, but in the end, the thing that's most inspirational is what do we bring to people around the world.

**Lenny Rachitsky** (01:07:23):
And along those lines, there's been such a... the opposite of glut and drought of a consumer, new consumer products, consumer experiences. There's very few success. Almost no consumer startup works and AI feels like an opportunity for something else to work. And I feel like Netflix is one of the rare companies and brands that continues to deliver an awesome consumer product and business. There's just not that many of them. So, good job.

**Elizabeth Stone** (01:07:48):
We're going to keep that up.

**Lenny Rachitsky** (01:07:49):
Well, with that, we've reached our very exciting lightning round. I've got five questions for you. Are you ready?

**Elizabeth Stone** (01:07:54):
Okay, I'm ready.

**Lenny Rachitsky** (01:07:56):
All right. What are two or three books that you find yourself recommending most to other people?

**Elizabeth Stone** (01:08:02):
I have to come up with different books than I said last time.

**Lenny Rachitsky** (01:08:04):
I don't remember what they were, but that sounds great.

**Elizabeth Stone** (01:08:06):
I still like a good throwback. So, two that are coming to my mind, Into Thin Air, Jon Krakauer and Liar's Poker, Michael Lewis. So, I worked on Wall Street and I like reminding people what it was like in the way back time.

**Lenny Rachitsky** (01:08:23):
Favorite recent movie or TV show you really enjoyed? Which is maybe too hard for someone working at Netflix, but just what comes up.

**Elizabeth Stone** (01:08:29):
The list is very long. The most recent I watched, Remarkably Bright Creatures, after a recommendation from my mom. It's a tear-jerker. Talk about the human part of storytelling.

**Lenny Rachitsky** (01:08:41):
Favorite product you've recently discovered that you really love?

**Elizabeth Stone** (01:08:44):
Critical for my health and wellbeing, Eight Sleep.

**Lenny Rachitsky** (01:08:48):
Do you have a favorite life motto that you often come back to in work or in life?

**Elizabeth Stone** (01:08:53):
I often go back to the things that my parents instilled in me in very early times. So, the risk of repeating, maybe. First, something good happens every day. Watch for it, even in the most stressful times. And second, that the last 5% of effort usually makes all the difference.

**Lenny Rachitsky** (01:09:17):
These are awesome. They hit me. Final question. I don't know anything about this, but you mentioned you're doing some kind of cycling event.

**Elizabeth Stone** (01:09:26):
Oh, yeah.

**Lenny Rachitsky** (01:09:28):
Tell us what's going on. What are you doing here?

**Elizabeth Stone** (01:09:30):
So, my husband and I are doing a trip where we ride alongside the Tour de France for the last week of the race. So, the tour is three weeks. The last week has a lot of mountain stages. So, we get to ride part of the route each morning and then watch the race in the afternoon. Not for the faint of heart, so I'm trying to train up so I can enjoy those rides. It's supposed to be a vacation after all.

**Lenny Rachitsky** (01:09:57):
My God, I love this vacation. We're just going to race. So, is it like a race?

**Elizabeth Stone** (01:10:02):
I love cycling. I love professional sports. It's fun to be able to participate in it.

**Lenny Rachitsky** (01:10:06):
So, is this like racing or you just kind of try to go as nonchalantly through the course?

**Elizabeth Stone** (01:10:11):
You go nonchalantly.

**Lenny Rachitsky** (01:10:12):
But still there [inaudible 01:10:13]?

**Elizabeth Stone** (01:10:12):
I think I mentioned... Yeah.

**Lenny Rachitsky** (01:10:12):
Other hills.

**Elizabeth Stone** (01:10:15):
It's physically and mentally challenging. And it's not a race, but I don't want to be at the back of the pack. So, I got to be comfortable enough to hold my own.

**Lenny Rachitsky** (01:10:25):
Wow. I love how different this is from your job. And it feels like someone [inaudible 01:10:29].

**Elizabeth Stone** (01:10:30):
It's a good balance and it gets me outdoors and gives me some nice perspective. So, I'm looking forward to it.

**Lenny Rachitsky** (01:10:36):
Elizabeth, you're awesome. Two final questions. Where can folks find you online if they want to follow you, reach out for maybe anything that came up? And how can listeners be useful to you?

**Elizabeth Stone** (01:10:45):
The best place to find me and some of the work we're doing or reach out is the Netflix tech blog, actually, where we're putting a lot of things that I've been talking about up there. We're trying to do a better job communicating about the fun stuff we're working on. So, that's a good first stop, usually. And then how listeners can be useful? Try all the new stuff that we're putting out there. Watch the live events, play the games, have fun with the new vertical video feed that we have on mobile called Clips. Send us feedback. So, we want to make it better. And a lot of these things are new zero to one efforts for us, so we're trying to get to great and excellent as quickly as possible.

**Lenny Rachitsky** (01:11:26):
I love that the homework is go watch Netflix.

**Elizabeth Stone** (01:11:28):
You can also watch other things. Tell us how we can be better, but I'm definitely interested in how can we be better at Netflix.

**Lenny Rachitsky** (01:11:36):
I love it. I'm going to go do that. Elizabeth, thank you so much for being here and being here again.

**Elizabeth Stone** (01:11:41):
Thank you for having me. Always fun.

**Lenny Rachitsky** (01:11:43):
Bye, everyone. Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify or your favorite podcast app. Also, please consider giving us a rating or leaving a review, as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
