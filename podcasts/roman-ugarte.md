---
title: "How we built Grok Bot in a month | Roman Ugarte (SpaceXAI)"
date: "2026-09-08"
type: "podcast"
guest: "Roman Ugarte"
post_url: "https://www.lennysnewsletter.com/p/how-we-built-grok-bot-in-a-month"
description: "How we built Grok Bot in a month, covering product design, AI product work, and team leadership."
word_count: 15333
---

**Roman Ugarte** (00:00:00):
The ultimate vision of Grok Bot is incredibly simple. You should have a team of AI bots that help you with your job and help you with your life.

**Lenny Rachitsky** (00:00:10):
Grok Bot is the hottest AI product in the world right now. That is a very high bar. There's a lot of competition for that slot.

**Roman Ugarte** (00:00:16):
We wanted to build something that wasn't just a great product for developers and engineers. We decided to create this very small team internally, to go off into a cave for about a month with the sole objective of build an amazing knowledge work product that brings agents to the rest of the company.

**Lenny Rachitsky** (00:00:33):
It's been only three weeks since launch. I went to a Grok Bot meetup. There were hundreds of people there, standing room only. It's very clear to me that you guys have built something very special.

**Roman Ugarte** (00:00:43):
Once you start breaking out of, this is AI chat with a set of connections instead to, this is a colleague with a computer, it just raises the ceiling of what you would think to give to AI.

**Lenny Rachitsky** (00:00:54):
You have this tweet, "An AI that does 100% of the job feels categorically different from one that gets you 90% there."

**Roman Ugarte** (00:01:00):
What made me so excited to work on Grok Bot is it was the first time for non-coding tasks that I felt like I could truly delegate work to AI, not have to think about it, and I would come back and it's done.

**Lenny Rachitsky** (00:01:15):
What is it that you think you did that is so different that made Grok Bot so successful?

**Roman Ugarte** (00:01:20):
It was two early decisions that at the time definitely did not feel obvious, but in hindsight I think are critical to what makes Grok Bot work.

**Lenny Rachitsky** (00:01:31):
**Roman Ugarte** (00:02:16):
Thank you. It is great to be here.

**Lenny Rachitsky** (00:02:18):
I am so excited to have you here. I am so hooked on Grok Bot. I have it over here in my window. I have like 15 bots that I use every day, all the time. I went to a meetup the other day, a Grok Bot meetup. There were hundreds of people there, standing room only, people sharing all the ways they're using Grok Bot. It's very clear to me that you guys have built something very special. It's very hard to break through the noise in the AI world. Grok Bot is the hottest AI product in the world right now. That is a very high bar. There's a lot of competition for that slot. I personally noticed I've moved a lot of my use cases from Cowork and Codex into Grok Bot just very quickly, which again, feels like a really big deal and a very special moment.

**Lenny Rachitsky** (00:03:07):
And so I'm excited to talk about so many things. I want to understand how you guys did this, where this came from, where this is going, what you've learned about the journey so far. First of all, just nice job. Nice work. This is very hard what you've done.

**Roman Ugarte** (00:03:21):
Thank you. I mean, I remember onboarding you by hand about a month ago and I think you were skeptical at first, but we're very glad that you've been using it and it's been great to see so many people really take advantage of Grok Bot.

**Lenny Rachitsky** (00:03:36):
I am going to talk about that onboarding. That was a very interesting element of how this worked. I actually remember in that onboarding, you asked me to do like a, let's try something and I was like, okay, try to come up with a tweet to promote my latest podcast episode. So I'm just like, come up with a tweet to promote my last episode. That's it. And it was actually very good. It figured out what the hell the last episode was, how to promote it. So I actually remember in the moment being like, wow, this is really good.

**Lenny Rachitsky** (00:04:03):
So let's actually start with the origin story. Where did this start? What was the original idea and when did the work on this begin?

**Roman Ugarte** (00:04:12):
Yeah, it started really as a blank page completely from scratch, build from zero exercise where I think we'd been feeling for a long time that we wanted to build something that wasn't just a great product for developers and engineers, which is really where we started. And I think we've gained a lot of intuition about how to build great agents and useful products that way. But what would that product look like for knowledge work?

**Roman Ugarte** (00:04:42):
And we decided to create this very small team internally. It was really just a handful of people to go off into a cave for about a month with the sole objective of build an amazing knowledge work product that brings agents to the rest of the company. And I think from the first line of code to when we released this prototype internally, it was only about a month. It was a very quick scrappy prototype that was pulled together. And I think in hindsight, this would not have been possible if it had been, I think, a much bigger group. I think it took a small focus group that was completely isolated from the rest of the company. And I mean that literally, it was like a separate part of the office where this team sat, private Slack channels.

**Roman Ugarte** (00:05:29):
And the goal, and I think in hindsight it was a lot of what allowed us to move so quickly on this, was we needed to make a lot of micro decisions every day, some things that maybe we'll talk about a bit later that were not obvious, were not really things that we'd done on other product surfaces before. And I think if it had been a very big group of people and we were thinking about this six to 12 month long vision, we just wouldn't have really gotten to the place that we ended up landing at. And so that was about a month from first line of code to here's a functional, useful product that the core team is excited about.

**Roman Ugarte** (00:06:05):
And so then there was a moment of rolling this out across the company, rolling this out across all of SpaceXAI. And so there was an all hands where we kind of shared the progress that had been made so far, there's this brand new product, we would love for you to use it. And I think what was most encouraging ... Because at that point we were excited about it. I think we were using it constantly, but it's easy to use the thing that you built and you kind of understand the mechanics and what it's good for. And so this was a real pressure test with reality. Are people actually going to switch from other internal tools, other external tools to use Grok Bot as their primary agent surface?

**Roman Ugarte** (00:06:44):
And in that first week after that all hands, I mean, I can't even tell you just the outpour of love for Grok Bot from people that maybe you wouldn't expect or from groups of the company that maybe you wouldn't expect, people who were daily driving ChatGPT or a chat interface, switching all of their day-to-day agentic tasks over to Grok Bot as their primary surface for doing work. And so the internal reception was really extraordinary. Can tell some funny stories from that week or two period. And then once we saw, I think the internal reception, we immediately switched into let's get this ready for the world. There's a lot of work to do to scale this out to millions of users. And then that led to the GA launch that we had a few weeks ago.

**Lenny Rachitsky** (00:07:31):
**Roman Ugarte** (00:09:20):
It was not obvious at all. I think you're completely right that that was one of those original decisions that at the time we had a lot of discussions about, and I'm very glad with where we landed. And I think to your point, it being a brand new product that you control every pixel of the experience and you have this consistent vision about where knowledge work is going and it's all contained in this new thing, I think has contributed a lot to the success. But there were a lot of discussions about Cursor, for example, and some of our coding products, people use it for non-coding tasks all the time. And these coding agents are really excellent at some of these things, but you run into small paper cuts. Sometimes the product itself is kind of intimidating to non-technical users. There's a brand association with these things.

**Roman Ugarte** (00:10:06):
And so I think we evaluated that path and I think we saw what maybe some of our competitors had been doing of this is all just one surface, you add new tabs for each new form factor and it feels a little cluttered. And I think for users, they can feel that, that this was not a single consistent vision of the way that work should work. And instead it's three different visions that all kind of share a screen and you can hop between, but it is kind of a shipping your org chart style thing that I think users are reacting negatively to. And so we decided let's just start completely from scratch. Let's see where we can get from there. There might be some really amazing opportunities to bring people from other surfaces into this more bot native experience, but it's really important for people to just have an amazingly simple and amazingly powerful experience.

**Lenny Rachitsky** (00:10:55):
That is a really valuable lesson for people to take away here, just that that might be the solution instead of adding in complicated and existing AI product. So interestingly, Codex went the other direction and it's like a different path than a different product, but it's interestingly, they're like, now we're going to make it one thing. So there's many ways to make it work and it also feels like the path you take there will kind of lead you, but maybe we'll look back and be like, that was not maybe the best idea.

**Lenny Rachitsky** (00:11:21):
Something you mentioned that you did that is also really unique is this onboarding of early users. I heard you and your team onboarded two to 300 people manually, including me. Talk about why you thought that was necessary and what you learned from that experience and just how long that period was of this kind of manual onboarding.

**Roman Ugarte** (00:11:41):
I mean, you just learned so much and the first few onboardings were pretty painful. I'm glad you got a good one, Lenny, but there were some that were kind of rough and we learned a lot. And I think it was important for the core team to be in the room for those and to just sit on a call for 20 minutes when the computer isn't spinning up or when someone's in onboarding and they're just incredibly confused so that immediately after you're like, that can never happen again. We need to solve this tomorrow because tomorrow I'm onboarding this person and it needs to go better.

**Roman Ugarte** (00:12:13):
And so there was about a two-week period where we were in that mode and onboarded a couple hundred people. And not only did we learn a lot about the product, I think we didn't really know ... I think sometimes with these products there's some group think of ways to use them. And I think internally, because people inside of SpaceXAI were just constantly sharing tips and tricks for how to use Grok Bot, some patterns were starting to emerge that we thought would be useful to the world, but we weren't really sure and we definitely didn't want to bias the world.

**Lenny Rachitsky** (00:12:46):
Is there an example of that?

**Roman Ugarte** (00:12:48):
So when we rolled out Grok Bot internally, there was about a week or two where the common pattern of the way people would interact with the product was you would have five to 10 bots and each bot you would give a different scope, a different domain, and it was kind of shorthand for different lanes of work. And then at around the end of week two, we started to see these messages internally in Slack of people promoting one of their bots who is a bit of a standout performer, and it was like their kind of primary personal assistant promoting that to their chief of staff. And then they would actually mostly talk to their chief of staff and the chief of staff would fan out all of these tasks to the other bots and would kind of manage the team. And there are some funny screenshots of people actually telling the bot they're promoting that they're promoted and the bot is asking if they get a raise and is their token budget higher, all of these things.

**Roman Ugarte** (00:13:42):
And we kind of took note of that and I think more of the companies started to slightly shift in that direction, but it was not the majority of the company. People use this product in very different ways. And so in some of the onboarding sessions and just from the early access program in general, we really did not want to lead the witness and say, create a chief of staff bot, here's exactly the way that that chief of staff should manage all of the other bots and see if early access users would get there themselves. And we actually did see that many of them did. And so then we had a bit more of an opinionated take in the product of this feels like a pattern that's working, this feels like a pattern that we should slightly encourage, but it shouldn't be a one-way door. And there were a few other examples of internal thesis that we really wanted to make sure would bear out in actual external usage without us imposing that in the product.

**Lenny Rachitsky** (00:14:30):
Is there anything else there? Any examples come to mind?

**Roman Ugarte** (00:14:32):
Yeah, I think another thing we really tried to pay attention to in the early onboardings was just how much users wanted to see. And I think it is something a bit shocking or just different about Grok Bot when you first start using it versus some of the other products that you mentioned, where a lot of the internal mechanics of how Grok Bot works are not shown to the user. And the reason for that is we think as these models get smarter, the same way that your teammate, you wouldn't ask for second by second updates of exactly all the buttons they're pressing and websites they're going to. I think it's too much to ask your bots to do that too.

**Roman Ugarte** (00:15:16):
And I think it's honestly just overwhelming and can create more harm than good. And so we moved completely in the other direction of you send a message, you tell your bot to do something, it just starts doing it. It sends you progressive updates as it sees fit, and you just see that typing indicator in the little green active circle kind of Slack-like that it's active, it's doing work, it'll get back to you soon. But you don't see the internal mechanics, you don't see the tool calls, you don't see exactly every little click it's making on its own computer. And we really wanted to take a strong stance that users did not need to see all of those mechanics, and so that's where we started. And we did get some feedback that's like, I would love to see my bot's to-do list. I would love to see roughly how it's prioritizing tasks and what it's doing. And that's great feedback, but it was useful to hear that nobody wanted the long stream of just text streaming out and chain of though sequences. So that also gave us more confirmation that that was the right direction.

**Lenny Rachitsky** (00:16:17):
The fact that you did two to 300 onboarding calls with a small team, I know the team grew over time, but just that is a huge time commitment and you could argue a distraction from the building, clearly not a distraction, clearly a core part of the success. Do you feel like that's the volume people need to do to figure out what actually needs to happen?

**Roman Ugarte** (00:16:41):
Well, one thing to emphasize is the early access group is not necessarily just people that are highly influential taste makers.You're in this category, Lenny, and we certainly wanted to get a lot of your feedback just from being very close to many other products on the market and just being a power user of these things. But we also wanted to get early access to more unconventional profiles that we as a company had never really interacted with.

**Roman Ugarte** (00:17:10):
So one example is there's a coffee shop owner that was a friend of a friend through the company who had heard about Grok Bot, and one day somebody on the core team had shown them a demo of the test flight and got very excited. And this coffee shop owner ended up being not only amazingly an amazing power user of Grok Bot, but also a rich source of feedback for us. We have a very lively thread with many, many bugs that get identified or feature requests, and it's a completely different use case of running a small business. And so for example, if the Shopify integration was a bit flaky or if it wasn't writing copy for products in a particular way, we would get really rich feedback on that, which is pretty different from the type of feedback we'd get from dog feeding this internally.

**Roman Ugarte** (00:18:00):
And so I think it was an important exercise for us to check our blind spots and say, A, this is going to be a very general product that is not just a thing that developers use. In fact, it is likely that this is most powerful for non-developers. We need to understand that group much better. And then B, is we absolutely live in this kind of Silicon Valley AI bubble, which I think is a useful place to be to kind of push the frontier and push the future of how these products are evolving. But we need to actively get out of that because I think a product like this has the chance of really being the way that the mainstream user and the mainstream business customer can interact with AI in a way that's useful.

**Lenny Rachitsky** (00:18:41):
Let's go back to the timelines real quick just to kind of understand that. So it was a month from first line of code to internal beta, and then what happened after that?

**Roman Ugarte** (00:18:50):
It was about three weeks from internal beta to public launch, and then I think we're about three weeks out from public launch as of recording this.

**Lenny Rachitsky** (00:19:00):
Wow. Okay. So a month of building the first thing, three weeks only of iterating, and then it's been only three weeks since launch. It feels like it's changed the world from my vantage point. So wow, okay. What most changed in those, I don't know, in those three weeks of internal beta, let's say?

**Roman Ugarte** (00:19:21):
We unshipped a lot. I wish I could have shown you what things looked like maybe two weeks out from launch where I think we'd realized that the core team, we had a lot of experimental features that we wanted to get internal feedback on, which was useful. We also were kind of putting pseudo developery visibility tools into Grok Bot instead of having a separate observability pane for those things. So for example, we actually did expose sometimes a lot of the internal thinking of the models and the specific memories it would store and all of these things, which was useful to debug issues. And if you're building the product, you didn't want to go somewhere else to maybe pull that context, but we had to really aggressively trim what we think the user absolutely needs to see in the surface versus what they don't. I think there's even more room there to run, which is something the team's focused on right now is how can we just ruthlessly simplify this product and abstract away anything the user doesn't need to actively be thinking about? So that was one big push was unship, a lot of jank.

**Roman Ugarte** (00:20:34):
And then I think the second big push those few weeks was making it just work. And I think a lot of what people want from AI is not this thing with lots of dropdown menus and bells and whistles, but just a thing that you describe a task, a task that's meaningful to you, and it goes and it does it and it comes back with complete work or it comes back with something for you to react to and then steer it in its kind of next cycle. And so in order to actually deliver on that promise, it's actually not a lot of feature product roadmap style stuff. It's like hill climbing five really important problems in the backend that many users don't directly experience, but you totally feel when your bot is going off and doing something and can't click the right button, or your bot is off and doing something and can't log into a website and it just completely stalls your ability to make progress on that task.

**Roman Ugarte** (00:21:32):
And so those few weeks we collected a really rich set of what are tasks that people actually are giving bot, how can we quantify these things and how can we see week over week that across those categories of tasks that we're hill climbing on very important dimensions to making that just work behind the scenes?

**Lenny Rachitsky** (00:21:48):
Is there an example, one of those hills you were climbing that was kind of a technical breakthrough or technical challenge you overcame that really helped it just work?

**Roman Ugarte** (00:21:56):
Yeah. One example was from rolling out Grok Bot, one group inside of the company that was actually incredibly bot pilled, so to speak, was our go-to-market team was sales. And there are a bunch of tools that sales uses that do not have well-supported MCPs or APIs. And I think that's a lot of what made bot so before and after powerful for this group was these were things that they just could not give another AI tool reliably. We would get stuck at some part in the process. And then Bot kind of felt like they had an assistant or kind of felt like they onboarded someone to their personal team, they gave it a laptop and it could just run.

**Roman Ugarte** (00:22:39):
And so there were a bunch of small things and probably a list of 10 or 20 of them of places where for whatever reason, the mouse would just not have fine enough control to click on exactly that part of the Salesforce dashboard or something like that, that we would have to take back to the core team working on really the infrastructure to say, "Here's a very concrete case of where the agent not having this visibility into the browser or this visibility into the pixels on the screen is making it impossible for this task to be done." And that was just a lot more tangible than seeing a number on a dashboard slowly creep up.

**Roman Ugarte** (00:23:20):
It was kind of like new chunks of work getting unlocked and you would immediately feel the feedback where you would ship an improvement that was kind of behind the scenes, kind of infrastructure-y. And then the next day you would just get this outpour of love and appreciation from the sales team that now this workflow that was failing the last seven days finally works. And it's just a constant exercise of finding those next tasks to unlock and then solving them.

**Lenny Rachitsky** (00:23:45):
So computer use basically improvements seems like a big unlock. I heard also I had Adam Ward on the podcast who's head of recruiting, head of hiring, basically head of talent. I heard that his team was one of the top users of Grok Bot.

**Roman Ugarte** (00:24:01):
Yes. The recruiting team gave us a lot of great feedback. Anytime the product, especially in the early days, if there was a little bug, we'd get a ping from some folks on the recruiting team. Yeah, I think the main use cases for recruiting that were particularly interesting was first, it was incredibly valuable as a sourcing tool. And I think one thing Adam talked about on the podcast with you, and it's a big part of our hiring philosophy internally, is looking for a job, being on the market is not a precondition for us trying to hire you. And in a lot of ways, the best way to hire is really just look at the biggest problems at the company that need someone to own it or take it to the next level, find out of the total universe of people in the world who would be best and then ruthlessly go after them and try to convince them to join.

**Roman Ugarte** (00:24:57):
And this is a lot of the philosophy from the very beginning of the company. And so if that's your mindset, really the best recruiting work stream or workflows to automate are not here are a bunch of resumes, read through them, help sort them. The most useful thing is here's an entire universe of potential people, help match that to this very concrete business problem or this very concrete role that we're recruiting for and help me get in touch with them, help me get coffee with them. Let's just throw everything at it. And so there have been some cases of really kind of unexpected ways of finding top talent that is beyond even just looking on LinkedIn and trying to find interesting people. But who are the co-authors of this paper and the PDF doesn't exist on Google Scholar. It just exists on this conference website. I want you every morning to go to the conference website, download the PDFs.

**Roman Ugarte** (00:25:54):
If there are any new ones, you should find every new name that we've not yet tracked. You should add that name to a spreadsheet, you should do research, you should look at everybody at SpaceXAI, see if there's anyone directly connected. If so, you should send them a Slack message asking for an introduction. It's those types of always on sourcing use cases that I think in the past were incredibly manual and now it's the type of thing AI is superhuman at and our team can focus on closing great candidates and getting conversations with great candidates and not pulling these huge lists.

**Lenny Rachitsky** (00:26:28):
Wow, that is such a cool example. First of all, someone's about to take the transcript of what you just said, put it into a bot and create their version of this, which is great. On the other hand, I think you guys could sell a template of this bot for a billion dollars. I think could basically use Adam's team strategy for finding the best people and just turn it into a bot, holy moly, democratizing hiring.

**Lenny Rachitsky** (00:26:50):
I want to come back to a few things. Okay. So one is you made this point about unshipping, such a important point I think that people can overlook because AI is not good at telling you what to take out. It's very good at, okay, here's more ideas, here's more stuff. And something that's come up a number of times in the podcast is that's a big space for humans to continue to be very important and valuable is knowing what not to ship and what to cut and what not to do. And so it's so interesting to hear that that's been a big part of the internal evolution from prototype to launches deciding, okay, we need to cut a bunch of stuff. Anything more there?

**Roman Ugarte** (00:27:34):
Yeah. So one thing we talk about internally is for anything that we're working on for Grok Bot, what is the launch post? What is the thing that we would actually tell users? And if it's not-

**Lenny Rachitsky** (00:27:47):
A launch tweet, I imagine.

**Roman Ugarte** (00:27:48):
Launch tweet. And if it's not compelling, maybe we shouldn't be working on it if it's not something that users will directly feel in the product. And to take that even one step further, I think there's this old school software tendency to say things like Grok Bot now has, and when you think of completing that sentence, it would be like a new button to press or it'd be a new dropdown or it'd be a new integration that you can press plus and add. And instead to reframe it as Grok Bot can now, which is I think a much more human way of describing these capabilities. And I think it's forced us to think more in the frame of what are tools and what are capabilities that we can give Grok Bot, not what are new things we can add to the product? Adding things to the product is not the goal, that's not the thing that's going to push this product forward and make it more useful to more people.

**Roman Ugarte** (00:28:43):
Making your bots reliably do really impactful work for you behind the scenes in a way that just works and giving them the capabilities to do that, that's what users actually care about. And so I think in the context of unshipping, there have been a lot of Grok Bot now has things that we've realized are actually just capabilities that don't need pixels. Let's kill as many pixels as we can. Those can just be things that your bot manipulates behind the scenes for you and you don't need to directly control. And I think one example of this is the way that many of our competitors, you set up automations or routines is you go into a sidebar, you press plus, you select what the trigger event is, you then select what action it should take after that, and you might describe it in natural language and it's just really clunky.

And it means that people don't set up many automations for many things. We certainly have seen this in the coding realm. And so I think what Grok Bot did in response to that was actually you should just define automations in natural language and you should tell your bot, "Remind me that at 8:00 AM every day, please." And then it should just do it and you should never ever have to see that interface of creating an automation. And so that's kind of the decision that we've made and now that's how 99% of automations on the platform built. And I think there are a bunch of other places where we can do things like that.

**Lenny Rachitsky** (00:30:03):
So I tweeted about how much I love Grok Bot when it launched and a lot of people replied, they're like, "Wait, can't you just do all this with Codex and Cowork?" And you can. Technically everything, as far as I know, you can do with Grok Bot you can do with the other foundational models, the coding assistants. So let me just ask you this big question. What is it that you think you did that is so different, that made Grok Bot so successful?

**Roman Ugarte** (00:30:28):
I think it was two early decisions that at the time definitely did not feel obvious, but in hindsight, I think are critical to what makes Grok Bot work for people. And the first is you should never have to think about local and cloud and where are these workflows running? Does my computer have to be awake? If I kick it off from my phone, does it need to be tethered to my computer back at home? There's so much jank happening right now when people are trying to conceptualize where this runtime lives.

**Roman Ugarte** (00:31:04):
And we made a really early decision that this should just all be in the cloud. And if it's in the cloud and it's this persistent colleague that has its own computer, it can do its own work, it has the same state everywhere you interact with it opens up a lot of really amazing opportunities to text your bot, kick it off from your phone. In the future, you should be able to call your bot from anywhere and it should be able to do real work.This is its own entity and it lives separately from your device. And I think that was a very important decision that current products I think haven't made that same decision. And I think it has a bunch of paper cuts as a result of it that users feel every day.

**Roman Ugarte** (00:31:44):
I think the second decision was to take that one step further of not only should this be an agent loop that kind of runs in the cloud and you can interact with in various ways, it's actually really important that these bots have their own computer. And part of it is what I described earlier of there are a bunch of tasks that don't have well-supported MCPs and APIs. We as humans don't do our jobs via MCPs and APIs. We use a computer and we click on pixels and we kind of type things and input boxes and it's very important that your bot has those baseline capabilities as well. But even to go one step further, I think we're in a really weird moment right now that I think we're going to look back on and be like, I'm surprised that this is the way that a lot of people worked with AI, where you're onboarding these super intelligent new colleagues, these AI bots, and you're asking them to share the same computer that you have. It's crazy.

**Roman Ugarte** (00:32:39):
If you were onboarding someone to your team and you said, "It's your first day, I'm going to onboard you. You don't have your own laptop, you're going to sit next to me, we're going to share this laptop forever and constantly trip over each other. You're going to have access to my credentials, I'm going to have access to your credentials." There's a good reason why that's not the way people operate. And I think bots and these kind of AI colleagues of the future will also need a way to onboard them that's somewhat similar and we've tried to push the product in that direction.

**Lenny Rachitsky** (00:33:10):
That is so funny. Why do you think the other companies didn't do this? My guess is they were building off of their existing coding assistant platform and approach, and this was a pretty big shift.

**Roman Ugarte** (00:33:24):
I think a lot of it comes down to starting from scratch and how freeing that is. And we felt that ourselves where a lot of the primitives in Grok Bot we had attempted or we had built in other ways, cloud infrastructure we built for coding agents. The way that you could maybe name agents and talk to them as discrete entities, it's a pattern that we're also seeing for developers bringing specific named agents into Slack. But instead of trying to retrofit those concepts into some new surface or into an existing surface, which I think would've been the strong default I think for many companies, we decided to start from scratch and we decided to just try to get these things really right for general knowledge work, which is a new audience. And then second, for the point in time that we're at now where the models are very capable and if you give them the right tools and the right infrastructure, they can do a lot.

**Roman Ugarte** (00:34:23):
But a lot of these ideas, these aren't strokes of genius on our part and I think for good reason. I think these are primitives that had already been getting attention and product market fit by other products, the open claws of the world. And I think we took a lot of inspiration from that and tried to productize it into a bit of a tighter surface, something that required a little bit less setup and I think it was more accessible to more people. And so I think our competitors and other tools that have been trying to solve these types of problems, I think we're all seeing the same opportunity. I think we're seeing a lot of the feedback from the market, but I think it's just been hard to act on if you're stuck in the existing paradigm. And if you have a lot of sunk cost in that existing paradigm, it's very painful to create a new thing from scratch. And I think a lot of that is what allowed the product to just work and click for so many people.

**Lenny Rachitsky** (00:35:17):
So what I'm hearing here is the keys to success of what made this breakout a cloud-based computer for every bot instead of locally, a name kind of specific bot. And by the way, there's this, we're all moving from agents to bots now. Nice job. It feels like you guys have pushed it over and now, okay, we're all bots now. So a bot per kind of task use case, very unique versus a thread conversation or something or a one-off job. And then it feels like it just works, was a core part of this. And you talked about how long it took to get to that place of like, okay, now it actually works really well. You mentioned OpenClaw. Obviously this is inspired by that, which to me, when I first used OpenClaw, like, holy, this is the future. How could we not have this? And then Hermes came out and everyone's been trying to build the OpenClaw that works very easily for everybody.

**Lenny Rachitsky** (00:36:14):
Can you say more about just how OpenClaw and that story informed the way you guys thought about it?

**Roman Ugarte** (00:36:20):
Yeah, so I think OpenClaw got two major things right that when we were seeing the way the market was reacting to OpenClaw and ourselves using the product, we found quite exciting. I think the first thing was the models are really smart and they're going to continue to get smarter, but even at current capability levels, if you can just give your bot access to the tools that you use to do your job, it can get a lot of the way there. In a lot of the places where people think AI is dumb or maybe not as impactful as it's been promised, a lot of that I think is downstream of it just being harnessed in the wrong way. And so if you give access to a much larger set of things, if it has access to its own computer, how far can you go? And I think OpenClaw really forced that question for many people.

**Roman Ugarte** (00:37:13):
And then I think the second way OpenClaw changed the mental model of AI was really viewing these things much more as colleagues and teammates and people and personifying it a bit more and it being this helper entity that has access to your life and can extend you even further. And so we took a lot of that and I think what Grok Bot maybe extended was, A, it needs to be really easy to set up and the hacky, you have a VPN at home and a Mac mini set up, clearly it was not going to scale to millions of users. Clearly it's not going to be the way importantly that businesses take advantage of this technology. And so we really wanted to build an amazing product with that in mind.

**Roman Ugarte** (00:38:01):
And then second is I think there are a lot of places, a lot of rough edges to stand down and just make a delightful product experience and make these things just work and try to remove some of the abstractions that power users of AI are very familiar with, things like skills, for example. How can we make a Grok Bot user not even have to know what a skill is? They should never have to type a slash command. These things should be created in the background as a useful primitive that the bots have access to, but something that users, it's not incumbent on them to always be on the cutting edge of AI. And so that's really where we tried to innovate and I think there's still more room to go there.

**Lenny Rachitsky** (00:38:40):
As you say that, I have my Mac mini with my formerly live OpenClaw on there and that was an era and it's so awesome the work that it has inspired. I know it continues. I know there's still a lot of value to OpenClaw, but when I saw Claire Vo, who's been the biggest proponent of Open Claw and it's become a core part of the way she lives and works with her kids and does all her work, she just switched all over OpenClaws. She shut them all down and switched to Grok Bot. It sounds funny, but that's actually a huge milestone of just how much things have shifted.

**Lenny Rachitsky** (00:39:21):
What's the vision for Grok Bot? Where does this go? What does this look like in the future? What's the ideal platonic version of Grok Bot?

**Roman Ugarte** (00:39:31):
The ultimate vision of Grok Bot is incredibly simple, which is you should have a team of AI bots that help you with your job and help you with your life. And it should really feel like a team. It should really feel like teammates that are autonomous are helping you. You can steer them in various ways. You don't have to micromanage them. They have access to the tools necessary to do great ambitious work. And one thing we really use as a north star on the product side in building this is as we kind of get closer to this teammate future, how can we, in every product decision we make, think about this less from the perspective of a SaaS product and more from the perspective of we're trying to build useful AI teammates. And so there have been a bunch of examples where we kind of have to push ourselves to be more like colleague pilled in a way.

**Roman Ugarte** (00:40:29):
We sometimes use that term where we're having a product debate about something, there are good arguments on one side, there are good arguments on another side, both paths feel sensible. In product land, this maybe doesn't feel like there's a clear cut answer. And then you zoom out a little bit and you remove yourself from the tech company-ness of it all and you start thinking, how would a human do this? What would you want from your teammate in this exact situation? And oftentimes the answer is really clarifying and pretty unanimous. There's oftentimes not a lot of disagreement among the room of how a human teammate you would prefer to work with in a certain way. And then once that answer is there, well then we just need to build it and there are product implications, there are model implications, there's a lot of things that need to go right to actually deliver on that experience.

**Roman Ugarte** (00:41:21):
But in some ways it's not a rocket science, doesn't require you being a genius. You just need to ask the question of what would you want from a human teammate and can we push AI to behave in a similar way? And so to give some examples of that, we've been thinking about what the right voice experience with these bots should be. And I think in the context of a human, for example, we have a really good analog of a lot of times I'm slacking back and forth with a teammate, we're sharing context, and a lot of times it's just much simpler to get on a five-minute huddle with them and just press huddle, talk back and forth. I share my screen, I show exactly what's on my mind, they share their screen, we hop off, and then we continue async from there.

**Roman Ugarte** (00:42:01):
And that's not really an experience that any AI product has gotten right right now, and it is deeply integral to the way that I think humans collaborate. And so we want to build something like that. And there are a bunch of other examples of these very clear patterns that just work that I think you should also feel when working with AI.

**Lenny Rachitsky** (00:42:19):
I love this term colleague build, and it's come up so many times over the course of this chat already how that is kind of a through line to making these decisions. For example, the computer example you gave is so good. Obviously people would have their own computer. The naming piece is also very important part of that. A big question on my mind in this space, and I'm so curious to get your take, is the separation between work and personal. Do you think people will have two different assistants, a work and a personal, or do you think it'll be one?

**Roman Ugarte** (00:42:49):
When people think about a work product versus a consumer product, I think there's just a lot of baggage that comes from the last decade or two of horrible B2B software that leads to people seeing a product that is very simple. In some ways ChatGPT was like this. I think Grok Bot has many of these properties. And assuming that it's not a work product or assuming that it's not a power tool. And when you think of a power tool in this kind of last generation, I, in my head, picture something a bit like Photoshop, for example, where there are all of these different dials to turn very precisely. The user of the tool is this kind of ultimate cockpit flyer who knows exactly what all the knobs do and can use them perfectly. And I think power tools of the future will actually be very different from that, where it is mostly just intent being expressed and good steering on the part of the human and these AI tools abstract away all of the knobs.

**Roman Ugarte** (00:44:01):
You should never see them unless you need to directly manipulate it, which might happen and there should be a great affordance for that. But ultimately, it really is just working with a teammate. And so the interface for that is quite conversational. And so in a lot of ways, Grok Bot, when you look at it, when I walk by someone's desk and I see Grok Bot up on their computer, for me for a split second, I'm like, "Oh, are they on a messaging app?" And it's like, no, this is actually the primary tool that they're using to do much of their work.

**Roman Ugarte** (00:44:28):
And so I think to your question of are you going to have a different set of bots for your personal life and a different set of bots for your work life. I do think there will be a separation for many people. They want a separation between personal and work life, and I think that's great. I think that's important. And I think there are a lot of common sense reasons why those things should be separate, even from the perspective of an enterprise.

**Roman Ugarte** (00:44:53):
But I think our goal and the thing we're trying to build towards is Grok Bot should be the way that a large portion of the things you do day-to-day in your work, you should be able to delegate a lot of that to Grok Bot and focus on the higher leverage things. And then it should similarly be the way that you delegate a lot of the low leverage parts of your personal life. And those two things actually are not different problem sets. In a lot of ways, the product form factor and the ways of solving those problems is pretty much the same. And so my instinct is that I think one product will be the best form factor for both of those things, and that's really what we want to build.

**Lenny Rachitsky** (00:45:30):
Bam, that's a big TAM right there. I love to hear. It makes so much sense. Obviously the question is how do you avoid cross-contamination, personal stuff somehow infiltrating, ex-filtrating stuff from work, but it feels like that's kind of okay. So what I'm hearing is that's the direction. The question is just how to do that and make people feel super safe, have the SOC 2 stuff in place and also just feel really fun.

**Roman Ugarte** (00:47:33):
Yeah, I think to go back to the teammate frame of the product, to extend the analogy even further, if we were on a team together, you and me, I think the number of times that you would have to manually take over my computer and start clicking on things and you're doing this wrong, you should go here instead and type in manually, hopefully it's pretty close to zero. Hopefully that is not something you have to really do with a colleague or a teammate. And so similarly, I think right now we're in a place where computer use is good, it's getting much better, and in very short order, I think the computer concept will be completely abstracted away from the user. You should never be clicking into a remote virtual machine. You should never have to take control if there's a wasteful path and you have to steer it into the correct path.

**Roman Ugarte** (00:48:30):
So in the medium term, I think the computer concept will be an important concept for users to have, but will not actually be something that they're interacting with. So I think the right way of thinking about Grok Bot is it's a team of bots, it's a team of agents that do work for you. And in terms of what they have access to, they have access to a very long memory set of your past interactions with them. And so I think there's a current paradigm if you create a new chat for each discrete unit of work, I think there are a lot of problems with that. I find myself copying and pasting between chats all the time. I think it's just not a great way of grouping categories of work. Instead, the same way on a team, you have a good way of grouping categories of work of roles.

**Roman Ugarte** (00:49:15):
You should have roles of different swim lanes of work that you do, and it should learn from you and it should get smarter over time. So I think that's one very critical thing is these are long-lived agents. These are not individual one-off sessions, and these agents get smarter over time. And then the second thing is those agents have access to all of the tools that you would expect a human colleague to have, which is the APIs, the MCPs, that's great, but then access to its own computer, which it can freely manipulate the way that you would.

**Lenny Rachitsky** (00:49:44):
At this meetup that I went to, Shab, who's on the, I think, go to market team, demoed something that blew everyone's mind. Because you have a computer within each agent, you can run a lot of different things on the computer. He was running Grok Bot within Grok Bot. The bot can run its own Grok Bots, and I know he was using it for testing and watching regressions and things like that, but that's just a mind-expanding idea. And I'm curious how many levels you can go before the universe collapses on itself.

**Roman Ugarte** (00:50:14):
I do that one too. That one's actually a very useful thing to do is you download Grok Bot for one of your bots, mine is like a QA tester bot. And that way if there's ever bug report or if we're testing out a new build, for example, of the desktop app, I can just say, "Hey, here are 10 workflows that we need to make sure are getting better release after release. I want you to test it. I want you to write it to this notion document that has an extensive list of all of the past tests that we've done of past client versions and compare them."

**Roman Ugarte** (00:50:45):
And so I think once you start breaking out of this is AI chat with a set of connections, which is I think where most people are conceptually now, instead to this is a colleague with a computer and anything I would ask a colleague to do on a computer, I can ask Grok Bot to do. It just raises the ceiling, I think, of what you would think to give to AI.

**Lenny Rachitsky** (00:51:05):
Are there any other mind-expanding use cases or ways to use Grok Bot that you've seen or you use?

**Roman Ugarte** (00:51:13):
One pattern that I've seen from many users that is simple, but I think there's a lot of depth if you keep investing in making it better, and this is where I can get kind of nerdy about optimizing my setup, is Grok Bot as an infovore in some ways of just consuming huge quantities of information, removing that from your own cognitive load, giving you peace, and then coming to you with the stuff that's important. And I think the V1 implementation of that, which many people do, is Grok Bot sits on top of Slack and it sits on top of email, and I tell it high level, "Here's my role at the company, here's kind of what I care about. I want you to notify me in these cases. In these cases, you don't need to ping me directly, but you should include this in your daily roundup that I read every day." I think that's the V1 implementation.

**Roman Ugarte** (00:52:11):
I'm not sure what the V10 implementation is, but maybe I'm at V3 or four, which is you can give these bots a complete fire hose of information. So I have mine hooked up to every mention of Grok Bot ever on X, and it's interacting with our internal context. It's interacting with the QA tester to see if it can repro any bugs or feedback that we're getting. I'm hooked up to my own messaging services to quickly act on feedback and reach out to people. And I think there's this just always on chief of staff entity that can preserve your focus on the things that actually matter, but is always kind of surveilling to see if there's anything that should get your attention.

**Roman Ugarte** (00:52:56):
And we've seen some funny cases of people actually giving their Grok Bots, which I have not done this yet, but maybe soon, giving their Grok Bots access, the ability to page them. And so if something super urgent happens and they're at a coffee or whatever, they get paged by Grok Bot, which is the type of thing that you only want to do if it's urgent and you really want to trust that Grok Bot does not have false positives. So far, those people have reported that it's been very helpful and successful. But I think we're going to see more of that type of stuff where the agent or the bot should actually be more proactive to you than you reaching out to it. And I think that will be the next shift in AI.

**Lenny Rachitsky** (00:53:36):
There's a number of things that I've been very impressed with watching your team operate. One is speed, which I want to talk about, but the other is how you are. There's awareness that this is a moment in time to capture a lot of market share and really take as much of the market as you can before somebody comes around and they're like, okay, now we got something awesome, especially one of the foundation labs. So watching just how many free accounts you guys are giving out. Also, the focus on use case is so smart because it's such a novel thing and you open it up and it's like, what do I do with this? And there's such a focus on, okay, here's a bunch of things people do with it. And then there's all this talk on Twitter and just all the ways people are using a template.

**Lenny Rachitsky** (00:54:20):
It makes so much sense. Just these two kind of focuses, from what I can tell, get as many people on as possible, as fast as possible until somebody's like, okay, because someone's going to come around and be like, all right, here's the next thing. Super smart and also the use case focus. I know you were a go-to-market person at Cursor before this. Anything you want to share there about just the approach to go-to-market right now for getting this out there?

**Roman Ugarte** (00:54:43):
I think the pattern we saw for coding will be somewhat similar to what we see for general knowledge work. And I think we've learned a lot from that on the go-to-market side and more generally just building practical AI that people use. And I think we as a company have culturally really cared about not building demoware, building actually useful stuff in the world and kind of obsessing over that. And there are so many shiny objects and fun prototypes to build, but ultimately that's a very different problem than getting this in the hands of millions of people and having it transform companies. So that's really, I think, culturally where we've always been focused.

**Roman Ugarte** (00:55:32):
And so I think on the go-to-market side, what we saw for coding was a very simple pattern, which was there was an early adopter crowd. The early adopter crowd would use these coding tools and really push them to the limits, and they would mostly push them to the limits on individual projects. On nights and weekends, I'm thinking 2023 earlier, people would go home from work. At work, they were using a basic IDE, this is pre-AI, and then at home they'd work on a side project and they'd be using Cursor or they'd be using the latest and greatest AI coding tool. And that would give them an extreme amount of acceleration. It would feel like they were experiencing the future, and then they would come back to work and they would demand it. And they would say, "I cannot picture working any other way than this. I feel like I'm completely walking through molasses right now. This needs to change." And I think for knowledge work, we're going to see a similar pattern of people really feeling the aha moment, sometimes in a personal capacity.

**Roman Ugarte** (00:56:38):
And I think we're certainly seeing a lot of this on X right now. You see all these examples of Grok Bot controlling their home robot computer, home robot vacuum cleaner or Grok Bot helping them save money on their Tesla charger negotiation, all of these fun use cases. But I think the next step is going to be, this is not a consumer product. We think this is going to transform businesses, we think this is going to transform teams, and it will be bots coming into teams and contributing really economically valuable work, especially as they get much smarter.

**Roman Ugarte** (00:57:14):
And so on the go-to-market side, we're certainly making a big push on prioritizing businesses and thinking about not just the single player use case of working with a single bot, but how does a bot work inside of a broader team? How does a bot work inside of real company systems that are complicated and there's a lot of context and a lot of history to understand? What does memory look like in a broader organization versus a single individual you're catering to? And I think there are a lot of unanswered questions there, but I do think Grok Bot is the right primitive to create this switch to agents for the rest of the company outside of coding, and that's a place where we're quite focused right now.

**Lenny Rachitsky** (00:57:56):
And along those lines, it's very clear you all understand the power of distribution and how you need to find both an amazing product and get distribution right because Grok Bot's amazing, but the combination of how smart you guys have been with getting it out there in all these different ways is really impressive. And I think that shows you what it takes these days to build something that's really successful. I want to ask about the brand of the different brands around this product and the company, just so people can try to understand, because I know you're going through a transition, acquisition, SpaceX, all these things. So there's Grok Bot, there's Cursors. So talk about the products and the way to think about these different brands today, and I know it'll probably continue to evolve just so we could communicate about it correctly.

**Roman Ugarte** (00:58:42):
Definitely. Yeah. I think there are three big pillars right now of SpaceXAI. So the first pillar is the coding product instead of products, and right now that's Cursor and Grok Build. And I think we're big believers that having a professional work surface for developers and for the engineering part of the organization is going to be really critical. And right now people use Grok Bot sometimes to kick off cloud agents or to merge PRs or to do QA, a bunch of engineering adjacent tasks. But ultimately when you're shipping production software, we're big believers that is going to require a product where every pixel is optimized for that end user. So we're making big investments there.

**Roman Ugarte** (00:59:28):
The second category is general knowledge work, and we think bot is a really exciting step in that direction. I think there's a lot more work to do of making it more useful, extending it to new surfaces, it really feeling like an AI teammate that you can delegate work to, especially inside of companies and businesses. So that's kind of the second pillar. And then third is the general model effort. We want to train the smartest models in the world that are really capable.

**Roman Ugarte** (00:59:54):
And I think one thing that somewhat distinguishes SpaceXAI from other AI labs is I think our goal is less to build, chase super intelligence or some kind of vague aspirational ideal. And the goal is actually very practical, which is to build useful AI. And we do that on the product side, we do that on the model side. And I think part of that is also just cultural of the group of people contributing to these models are engineers and people who came into the model training effort from a very applied mindset. And I think that's what gets this company going and I think is actually a slightly different direction from some of the other competitors out there.

**Lenny Rachitsky** (01:00:43):
Super interesting. Okay, there's a couple directions I want to go. One is you have this tweet that is, I think you pinned it or maybe it's your last tweet. It's up there in your timeline if people check you out. So the tweet is, "An AI that does 100% of the job feels categorically different from one that gets you 90% there. I've significantly updated what I think AI is capable of." Say more about that.

**Roman Ugarte** (01:01:06):
I think for me, what made me so excited to work on Grok Bot and contribute to it is it was the first time for non-coding tasks that I felt like I could truly delegate work to AI and not have to think about it and I would come back and it's done. And I think engineers have been feeling this for quite some time, for maybe a year, a year and a half, things have been like that. I mean, the job of a developer has completely transformed. It is unrecognizable from what it was two years ago and many, many words have been said on that topic. But I think it's underrated how different that experience is from what most people are feeling about AI right now and the way that AI has changed their lives. And it looks quite similar to the way that people would use AI two years ago where you create a new thread for a task, you type it into an input box, you hit enter, you watch all of these steps happen, you get an output, it's not quite right, you keep working on it.

**Roman Ugarte** (01:02:13):
And Grok Bot, I think short circuits a lot of that. When you first lay eyes on the first screen, you're like, "Whoa, this is clearly different. Let's see if it actually works, but this is different." And then you give it something and it kind of works to a surprising extent. And I think we're going to do a lot to make it work much better. And so I think what I was expressing in that was when you have a teammate that you only 90% trust and you give something to, which luckily I do not have the experience of here because I work with great people, but if you delegate something to someone and you're like, "I know I'm going to have to be thinking about this while you're doing it, and I know it probably is not going to be quite there and I'm going to have to intervene and steer it slightly," that's not 90% task completion.

**Roman Ugarte** (01:02:59):
You're still doing the thing and it feels that way and it's weighing on you in the same way versus truly throwing a no look pass to a colleague and being like, "You got this, here's the context, go off and run. I'm excited to see what you do." That's a different category. And I think that's the type of thing that people feel with Grok Bot every day are these no look passes and you just trust that it can get it done and then it does and it's just a very magical experience.

**Lenny Rachitsky** (01:03:26):
Yeah, I've had that experience consistently. Okay, so another element of how y'all operate that has really impressed me and I've not seen this before is how fast y'all move. So I got added to this Slack as I was giving feedback with some folks and it's just like, okay, how about, okay, tomorrow we're going to give you some free codes to give out. You could do it tomorrow. We'll do this tomorrow. Or we're going to launch a marketplace with templates, we're going to launch this in two days. It's just like, what? I don't have time for this. How do you guys, with all the things going on, all these things constantly shipping and also staying consistent and high quality and feeling clear that it's towards a specific vision.

**Lenny Rachitsky** (01:04:05):
So there's kind of two parts of this question, just what's the secret to how fast you all have been moving and how do you stay aligned moving that fast towards a vision that you all believe in and where you want it to go versus just band-aiding it along the way?

**Roman Ugarte** (01:04:25):
Yeah. One thing I've been really happy has never changed is that startup feeling inside of the company. And for context, when I joined Cursor originally, we were about 15 people. We scaled to over a thousand. And then now we're a part of SpaceXAI, which is kind of an even bigger organization. And it's something that is just so fun to be a part of when you're around this group of incredibly talented people. Everyone's moving a hundred miles an hour. You trust, you deeply trust everybody to execute on their part of the equation. And there's a clear vision that everyone is fired up about and knows that they need to execute on.

**Roman Ugarte** (01:05:06):
And as companies grow, and we've had the fortune of hiring really great people from other companies that have gone through hyper growth, things slow down and you kind of keep telling yourself, we're still a startup, we still move quickly, but you really don't and everyone knows that you don't and it's easier to say than to actually be. And fingers crossed, this continues to be true. I think it's really critical for our success if this continues to be true. But even as we scaled, it has always felt like that startup that I first joined. And I think if you define a startup by number of people or by the funding round, none of those things really make any sense.

**Roman Ugarte** (01:05:50):
The core thing that defines a startup is exactly what you're describing, which is this kind of scramble energy of things are kind of chaotic and kind of disorganized. And for a lot of people, that's not a pleasant working environment to be in, but it has these amazing properties of you can make extreme impact in a particular direction in a short amount of time and you really do get out of the system what you put in. And so I think as a culture, I think as an organization and the way we construct ourselves, it's really been to enable that property in a way that I think some of our competitors and other AI labs have gotten much bigger and you can feel it. And I think us, even as we scale, there is that start-upy impulse that is quite important to move quickly on these things.

**Lenny Rachitsky** (01:06:35):
Let me pull on this thread and let me ask you this big question that I've been looking forward to asking you. If you were to look at Cursor from the outside, it shouldn't have worked. It shouldn't have lasted because, one, it's in the most competitive market in the world competing against the fastest growing companies in history, OpenAI and Anthropic. So that's one. It's like the competition is unlike anything anyone's ever experienced. Two, it sits on top of those platforms to power it. And what I've seen as an outsider is what has allowed Cursor to win and have this massive exit and continue to succeed is how quickly you all adjust to the reality of the market. Started as auto complete and then things moved on to just talking to agents and then into the cloud and now Grok Bot.

**Lenny Rachitsky** (01:07:30):
To me, that feels like a core part of the success is quickly adjusting to reality and also building the best in class experience for a thing that also exists other places. Grok Bot's a great example. You could do this other places, but it's the best in class experience, Cursor, the ID, the best way to code. So that's my question. Maybe I answered it, but what do you think has been core to Cursor's ability to not just survive in this crazy competitive market, but do so incredibly well consistently for so long?

**Roman Ugarte** (01:08:01):
I mean, a lot of this, and it's a fuzzy answer, a lot of this I think is downstream from culture and the culture that you set and the people that you bring in and the way that they approach these problems. And I think for us, exactly as you said, we have never been complacent. We've never felt like we've won, and it's always been about the next thing. And I think there's been a really deep belief across the company that AI is moving incredibly quickly. Our goal is to translate those capabilities into amazing products for customers, but those products are going to change and they need to meet the moment as the capabilities get stronger. And what met the moment two years ago is completely different than what's meeting the moment today. And if we as a company can't completely reinvent ourselves every six months, which recently it's felt even shorter than that, of complete very significant reinventions of our priorities, the core product, what users feel, we're going to lose.

**Roman Ugarte** (01:09:06):
And I think it's that spirit of always pushing to be on the frontier, never thinking it's over or that we've won or that we've gotten it right and just constantly updating our beliefs that has gotten us to where we are now. And to your point on the competitiveness of this space, one thing that I think is important to point out is AI coding has always been competitive from when Cursor first came to be. And at the time the competitors were Microsoft and others and a handful of maybe 10 or 20 companies. And I think it's notable that none of those competitors are at the forefront of AI coding right now in large part, not because of any incorrect decisions that they made or any lack of resources on their part, but this cultural inability to move quickly and to change to meet the moment as the moment's changing. And so I think that's exactly what has led us to invest in things like Grok Bot, for example.

**Lenny Rachitsky** (01:10:04):
Are there any core values, just specific ways you phrase this to kind of remind everyone of this is how we work?

**Roman Ugarte** (01:10:10):
Yeah, two values that I find myself coming back to quite a bit. The first one is this idea of deleting the product. And I think it exactly ties back to what you're saying right now where when you look at every past iteration of Cursor, for example, but even I think when you look at every past iteration of Grok Bot, I think we will feel the same thing, is things going away, not new things getting added, but these scaffolding product overhang style things that get built in because the models have not yet gotten smart enough to just do it themselves, those things will get moved away over time and we need to feel comfortable making kind of hard decisions that might upset a small set of users or a small set of us internally to do the bigger thing of make the product simple, make the product powerful and adapt to where the future is going.

**Roman Ugarte** (01:11:02):
So I think that's been very core. And then the second thing, which ties back to the pace of execution is just do the thing, which I find myself kind of repeating a lot even as we've kind of grown as a company is it's on you. We're all in this boat together, we want to win. And if you see something that you think needs to happen, this is not an ask for permission culture, you go out and you fix the thing and you pull in the resources that you need to make it happen. And I think that has made many people very successful here before, and I think it's something we really share with SpaceXAI as well.

**Lenny Rachitsky** (01:11:39):
Agency, as you may have heard. So interesting. One of the big questions that comes up, and this might be my final question, is around moats. And a lot of people look at Cursor as a really interesting example of they're in a market with technically maybe no moats, but they've continued to win and succeed. The two moats you think about with Cursor is the data feedback loop of people auto completing, learning what they're doing and training models based on that. So that's unique. The other is just best in class experience and being a high daily active user product and finding over time what works and what people need.

**Lenny Rachitsky** (01:12:19):
What have you just learned? And I guess any thoughts on moats in this space that might be helpful for folks that are trying to figure this out for themselves?

**Roman Ugarte** (01:12:28):
Yeah, there's a lot of talk about moats and it is a pretty interesting moment in time to be starting a company. So I can understand why so many founders are kind of asking themselves that and trying to project out 12 months from now, 24 months from now, it just feels like an eternity. I will say that I think if Cursor and many other successful companies of this kind of vintage, I think if they had thought about moats/kind of tried to work backwards from some strategy diagram or a maybe more abstract notion of how a company should work, I don't think that would've created this outcome or this product. I think what really created the magic of Cursor was an obsession with building a useful thing today. And I think it was constantly this exercise of you can kind of see where the world is going three months from now, six months from now, models are going to get smarter, a thing that isn't solvable now is finally going to be solvable.

**Roman Ugarte** (01:13:34):
And I think Cursor was a little bit this recurring prompt of how could we pull that stuff to today, even if it requires a little bit of engineering on top to make it work or a lot of engineering on top to make it work, even it requires changing the product in a specific way so a user can interact with this new capability. How can we bring that forward? And then three months from now, we should delete all that stuff because it'll just be good and basic common bare minimum of the product and then we'll build the thing for three months from then. And then it was constantly just doing that over and over again that I think led to users really trusting us and placing their time inside of our product and trusting that we were kind of bringing things to this next frontier and to the next future.

**Roman Ugarte** (01:14:21):
And so I would really encourage many founders or people starting out today to be more grounded in that perspective of how can I make something that is not possible now possible? Users are going to come to me to use that thing. I'm going to pull them to the next impossible frontier. And then through all of that, I'm going to gain a lot of distribution advantages. I'm going to gain data advantages. There will be value there, but I think that's really the place to play.

**Lenny Rachitsky** (01:14:49):
I love that answer. Essentially, the way I'm thinking about it is just build something people are obsessed with, don't overthink the moats piece. And if you can continue to do that, you'll find something which in Cursor case ended up being a few things completely. And that came up actually recently on another podcast I did, I don't know if it'll come out before or after this, this idea that moats are discovered, not planned ahead of time a lot of times.

**Lenny Rachitsky** (01:15:11):
Okay, let me actually ask you for Grok Bot tips as an actual last question. Some people are going to be like, "Oh, shit. I got to try this thing. What's all this excitement all about?" What would be some advice for folks that are trying out, let's say for people that are new to it, just like here's some keys to success and maybe some power tip for someone that's already with it and just like, "Oh wow, I didn't know that"?

**Roman Ugarte** (01:15:31):
Yeah, I want to stay away from the super hacky pro tip stuff because I think our philosophy as a team and as a company is that those things really shouldn't exist. There shouldn't be all these crazy knobs. You should be able to delegate something to Grok Bot and they should do it. And so what I would encourage for someone new who's just downloading the app, you're looking at the screen, I think the first thing is give Grok Bot the context it needs to be successful. So in a similar way as if you were onboarding someone to your team, it'd be really helpful for them to have access to Slack and your email and the company records that you use every single day. So I'd give it access to the tools and then I would actually ask Grok Bot what it can do for you and let it kind of go through those connections that you've initially set up.

**Roman Ugarte** (01:16:28):
In my case, it might be I give it my email, I give it Slack. And I was really surprised when I was first onboarding. We didn't have any onboarding screens at this time, so this was kind of the first task I gave it, was go through my Slack, go through my email and suggest five things that you can take off of my plate and what it would take for you to do that. And it suggested five and two of them were actually really helpful and I just immediately spun off two bots to solve those two. And that was my big wow moment of feeling like no other AI tool in the past could have done those two things. It was not like draft an email, it was like do a chunk of work. And so I'd encourage people who are brand new to do it that way.

**Roman Ugarte** (01:17:06):
And then for people who are not brand new, I kind of am constantly finding new patterns for ways that my bots can interact with each other and can collaborate with each other. And so I've been creating a bit more of a scaffold of where these artifacts that Grok Bots create should live and how it can write to a place that's very legible to me. So I have these frequent digests that I read every day and it kind of pushes to a database and I can just read it very easily. And so I would encourage power users to think about ways that Grok Bot can actually write to a single store where you can organize a lot of its outputs much easier.

**Lenny Rachitsky** (01:17:49):
Damn. We need another episode of going deep on Roman's Grok Bot setup, which probably has way too much private sensitive information we can show it. Okay. That's an amazing tip. Roman, is there anything that you wanted to share or anything else you wanted to touch on before we get to our very exciting lightning round?

**Roman Ugarte** (01:18:09):
Nothing else on my side.

**Lenny Rachitsky** (01:18:10):
We covered so much ground. I can't believe that was only an hour and a half-ish. I felt like we've been talking for ages and covered everything I was hoping to cover. With that, we've reached our very exciting lightning round. I've got four questions for you. Are you ready?

**Roman Ugarte** (01:18:22):
I am ready.

**Lenny Rachitsky** (01:18:24):
What are two or three books that you find yourself recommending most to other people?

**Roman Ugarte** (01:18:28):
Yeah, so two books for you. One is I love Kurt Vonnegut. So Cat's Cradle has been a fun recommendation and a copy that I bought many friends before. And then second is The War of Art by Steven Pressfield that I find myself frequently coming back to even if it's just a page or two at a time and I'd recommend for anybody.

**Lenny Rachitsky** (01:18:51):
War of Art, incredible. It's such a short book and it's like once you read it ... And it's not The Art of War, which is what people might think they're hearing.

**Roman Ugarte** (01:18:58):
Yes.

**Lenny Rachitsky** (01:18:58):
But it's the War of Arts to play on that and it's about the challenge of being creative and creating something new and how to overcome the resistance. I love that recommendation. Next question. Favorite recent movie or TV show if you've had any time to watch any of these things?

**Roman Ugarte** (01:19:14):
Yes. Recently, so every year I do a watch of Casablanca, which is one of my favorite movies. And it incidentally also has a character with my last name, Ugarte, which is the only example of I think a Ugarte in the media. So Casablanca, always a great re-watch. And then on the TV side, I sometimes sneak in an episode of Monk, the detective show, which was one that I watched as a kid with my family and I've come back to now that I live in San Francisco. And it's just a great moment in time snapshot of San Francisco in the late '90s, early 2000s when it was shot that I really enjoy.

**Lenny Rachitsky** (01:19:57):
First Monk reference on the podcast. Okay. Favorite or most interesting AI product right now? You can say Grok Bot if you want, but if there's anything else, you get bonus points.

**Roman Ugarte** (01:20:08):
I've always been a big AI semantic search nerd. I love any SEM search product, especially the kind of out of the ordinary ones. So I was a very early user of Metaphor at the time, which became Exa, and I love using Exa to do all of these maybe more strange queries over the internet. But I see a lot of examples of people building semantically search over an embedded image store of the MoMA or things like that. And I always have so much fun playing with those. So anything semantic search engine over a weird data set, I love.

**Lenny Rachitsky** (01:20:47):
And Exa in particular is one you'd recommend?

**Roman Ugarte** (01:20:49):
I love Exa, yeah.

**Lenny Rachitsky** (01:20:51):
Very cool. Okay. Favorite life motto that you often come back to in work or in life?

**Roman Ugarte** (01:20:56):
Not as short as a single motto, but I love the Desiderata, which I don't know if you've read, but I have it on my door and I've had it since I was a teenager and everywhere I move, I kind of paste it there and it's a very short poem, but each line, I find myself finding something new in it every time I read it and I find it really grounding.

**Lenny Rachitsky** (01:21:20):
Roman, this was amazing. What a point in time we're here right now at this moment in time of Grok Bot, of AI in general. It's going to be really fun to revisit this in a year and be like, wow, we were so right and so wrong about so much. Thank you so much for doing this. I know it's a very busy time on your team right now, so I really appreciate you carving out a couple hours to chat. Is there any place you want to point people to? Anything you want to plug other than check out Grok Bot? Is that ...

**Roman Ugarte** (01:21:47):
Check out Grok Bot, of course. And yeah, main thing would be please send feedback. I think we're in the very early innings of this still. I mean, we released a beta three weeks ago and a lot of the feedback that we've been getting from this early set of users is directly translating to what we built and how we build it. And so really appreciate all the input that people are giving.

**Lenny Rachitsky** (01:22:10):
Nice job, Roman and team. I know there's a whole team behind all this. Roman, thank you so much for being here.

**Roman Ugarte** (01:22:17):
Awesome. Thanks, Lenny.

**Lenny Rachitsky** (01:22:18):
Bye everyone.

**Lenny Rachitsky** (01:22:20):
Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
