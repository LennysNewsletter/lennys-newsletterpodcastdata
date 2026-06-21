---
title: "Building the most AI-pilled engineering team in the world | Fiona Fung (Manager of the Claude Code and Cowork Teams)"
date: "2026-06-21"
type: "podcast"
guest: "Fiona Fung"
post_url: "https://www.lennysnewsletter.com/p/building-the-most-ai-pilled-engineering"
description: "Building the most AI-pilled engineering team in the world, covering engineering tradeoffs, team leadership, and AI product work."
word_count: 19294
---

**Lenny Rachitsky** (00:00:00):
Anthropic engineers on average have eight times as much code per quarter as they did compared to 2025.

**Fiona Fung** (00:00:05):
Coding is no longer the bottleneck. It's looked at the ceiling of what anyone is able to do.

**Lenny Rachitsky** (00:00:10):
Everything is now possible, in theory. Now it's about how ambitious can you be.

**Fiona Fung** (00:00:14):
It's always something we ask ourselves, what's better than me doing it? Having Claude do it.

**Lenny Rachitsky** (00:00:18):
The people that seem to be doing best are taking the most initiative, getting the most proactive, have the most agency.

**Fiona Fung** (00:00:22):
We say with high agency is also high accountability. So it's all about making sure folks have that freedom to cook. But then it's also like, okay, what's the accountability for it? What's the hypothesis of what you're trying to solve?

**Lenny Rachitsky** (00:00:33):
I'm curious what is lost in this new world of software engineering.

**Fiona Fung** (00:00:36):
It could start being a lonely experience because we all started just working with our agents so much. And on the Claude Code team recently we started a para-wise programming lunch.

**Lenny Rachitsky** (00:00:44):
Something you think about is this gap forming between people that are leaning into AI, killing it, and then people that are not, super frustrated, fighting, resisting.

**Fiona Fung** (00:00:52):
In terms of frustration, I think sometimes I also see a little bit of fear. For anything that there is a fear, my advice is lean in and ask, " What can I do about it? What is within my control?"

**Lenny Rachitsky** (00:01:05):
Today, my guest is Fiona Fung. Fiona leads the teams behind Claude Code and Cowork at Anthropic. She oversees both Boris Cherny and Kat Wu, both of whom who have been on the podcast and whose episodes are in the top 10 most listened to episodes of all time. Before Anthropic at Microsoft, Fiona ran the teams that built Typescript and Visual Studio. After that, she went to Facebook where she started the Facebook Marketplace team, which she took from idea to launch. 

**Lenny Rachitsky** (00:01:31):
Today, Facebook Marketplace generates over $100 billion in GMV every year. Also, while at Meta, she oversaw work on Meta's first smart glasses product and then she helped build Orion, their first AR glasses product. Then she went to Instagram where she led infrastructure, growth, integrity, and safety teams. While at Instagram and at Meta, she oversaw an org of over 500 people. Fiona has been an engineer for over 25 years and as a longtime engineering leader, especially now at Anthropic, she has such a unique lens into where things are heading, what's worth paying attention to, and what teams should be thinking about right now as AI transforms the world of building.

**Fiona Fung** (00:02:40):
Thanks so much for having me, Lenny.

**Lenny Rachitsky** (00:02:42):
So I was at the Code With Claude event, I don't know, a month ago at this point and I went to your talk and I was just like, "Holy shit, I got to get Fiona on this podcast. She's thinking so far ahead of where everybody else is going and where people are at with AI." So you've been an engineer for 25 years. I was browsing your LinkedIn. You started at IBM of all places, such a different place to be these days.

**Fiona Fung** (00:03:05):
Yes.

**Lenny Rachitsky** (00:03:06):
And it's just insane how much the job of an engineer has changed over the past just two years. It's like a completely different job. People may forget 100% of code was written by humans not long ago, and now it's getting to 100% of code written by AI. As Boris famously said, coding is solved. Along these lines, there's just this tweet that you guys put out yesterday where you showed, here's the tweet, "Anthropic engineers on average have eight times as much code per quarter as they did compared to '21 to 2025." We'll show this chart on the screen. It's just like stable, stable, stable, stable, shooting off into the moon.

**Lenny Rachitsky** (00:03:45):
So it's just insane how much this role has changed. I'm curious about your kind of path as an engineer living through this, having been an engineer for a long time, what have been kind of like the big moments along the way where it's shifted your way of thinking and operating that have led you to what you do now and how you operate now?

**Fiona Fung** (00:04:04):
Oh, I love this kind of love walk back in time. Yeah. IBM, working on DB2, the operating system services team. Back then I was thinking, "Oh, what's a hard area of the stack?" And I really thought the lower level you go closer to the OS, then it's more hardcore and you'll learn more. So I was really fortunate to gone into the IBM internship. But the funny thing was, I think there's even a big shift from IBM to Microsoft. So at IBM it was I think VIM. I didn't have an IDE that we used. I think there might have been an Eclipse license, but for some reasons, most of us didn't use it. 

**Fiona Fung** (00:04:40):
So I remembered it was mainly like VIM and kind of terminal debugging. And then when I joined Microsoft, I mean, this is how naive I was, I didn't even know about IDEs and such. And back then you didn't really get to pick teams. His was early 2000s. Actually, first off, I should say I was so grateful that I landed the internship and the role, because to take us all the way back in time, the dot com bubble burst in 2000. And so for my graduating class, a lot of the companies weren't hiring or were hiring freezes. So I was so fortunate when Microsoft extended me an offer.

**Fiona Fung** (00:05:14):
And so they're like, "You're going to work on Visual Studio." I did not even know what Visual Studio was because I came from a Unix school. So I remembered asking, because I was thinking, well, the name Visual Studio, I'm like, "Oh, is this a better Paint program?" And I could tell the look of my manager's face like, "What is going on?" But then it ended up becoming the love of my life for the first 11 years of my career. But that was the first time I used an IDE. So joining the Visual Studio team seeing, "Oh wow, here's an IDE with debuggers and you can set break points and do multi-threaded debugging." 

**Fiona Fung** (00:05:47):
That was also always mind-blowing for me to think about the stepwise change. So yeah, that was kind of the story going from IBM to Visual Studio. And then what I really loved actually about Visual Studio is I was on the Visual Studio editor team. So I used a VS editor to build the VS editor and that's where my whole love of dog fitting comes from. I remembered I wanted to first and foremost create a delightful experience, not only for myself, but for my teammates, because also if we go back in that time, if you remember, I mean, when did Twitter come out? Was it 2006 or so?

**Lenny Rachitsky** (00:06:22):
It feels like it's been around my whole life.

**Fiona Fung** (00:06:25):
But back then, before social media, it was also harder for most engineers to hear fast customer feedback. For sure, there you would be user research sessions or we would have customers visit us. But you didn't get the rapid feedback that you do nowadays. But back then I was so lucky because I was on VS. We ourselves gave each other so much rapid feedback because we were all heavy VS users on the team.

**Lenny Rachitsky** (00:06:50):
**Fiona Fung** (00:08:16):
Yeah. When I worked on Visual Studio, back then we also shipped software on CDs. 

**Lenny Rachitsky** (00:08:20):
I remember that.

**Fiona Fung** (00:08:22):
And that's why they were really hard deadlines because you had to make sure the software was ready for us to give to manufacturing, to then put on the CDs for us to then put on the shelves. And then so once that was another shift when we actually started to be able to ship software online. And I think that's the interesting thing, and I kind of mentioned this in my talk, it's engineering time was really precious resource, but you also have these really hard deadlines, for example, like printing software and CDs. And so back then you would do a lot more planning because you just wanted to make sure given the time you have, you make the best of it.

**Fiona Fung** (00:08:57):
And that's a shift that we're seeing with Claude Code and Cowork is coding is no longer the bottleneck. And so now you showed the tweet and that graphic, but now it's all about where has that shift happened. Now not only engineers, we also have designers, PMs, everybody on the Claude Code team checks in code. So when not only more people checking in code, but kind of different disciplines, but also the throughput is so high, how do we think about verification? That's kind of this other shift that I'm seeing.

**Lenny Rachitsky** (00:09:27):
Maybe just kind of set this theme that I want to have for this conversation. A lot of people are just wondering what is software engineering, managing software engineers, managing software and product teams look like in the future? And you are living through that right now. So you mentioned this point about a more focus on verification, making sure the quality of the code being 8X is actually high and something that will work. So just like let me ask this broad question, let's kind of see where this conversation goes. What does an AI pilled software team look like in 2026?

**Fiona Fung** (00:10:03):
Because the roles are blowing, it's shifting more to this builder. Everybody starts being a builder, I would say. The other shift that I've recently done is I actually have a Claude Code remote session that I enlist in all of our repos. And so this way I have full visibility into the work that everybody's doing. And this instance, it also has access to all our Slack channels and I'll have access to how are the metrics of everything we track. And so every month when I'd be like, "Hey, you know what's fun? Let's take a look back." 

**Fiona Fung** (00:10:36):
And so we'll actually do it together. I'll share my Claude Code, I've shared my screen, then we do our Claude Code session and it's just about, "Hey, what were the focus areas? What were some of the products that got shipped? How did it do? Oh, what were the feedback channels?" And so even though before I would've just used these sessions to generate PRs and bug fixes, I actually have these sessions to enable me to have conversations with folks that I support.

**Lenny Rachitsky** (00:11:03):
Say more about that. So this is a management technique, let's say, to help people not just ship but actually ship better, understand if they're shipping things that have impact. Is that kind of the idea here? Just use Claude to keep on top of all the things people are shipping and then make that a conversation with them?

**Fiona Fung** (00:11:20):
Exactly. So yeah, outside of just the action of shipping is how did it do in market or, hey, did we caught some bugs? And it's okay to, I have this saying, make new mistakes. It's okay to make mistakes, just make new ones so that we're always learning. Because if you aim to make zero mistakes, that probably means you're not moving fast enough or being a little bit too cautious. 

**Fiona Fung** (00:11:42):
And so by having Claude, so then it can also look at, for example, actually, I was just looking at, oh, given some of the incidents that we have, let's look across all of this. Can we generate a theme? What's a good area investment for us next, especially we think about quality. Are we seeing any hotspots of where there could be a gap? I think that used to be just a much more manual process, I would say. If I look back a year ago, I don't think I would've been able to have some of these insights with Claude.

**Lenny Rachitsky** (00:12:12):
Yeah. Well, partly it's because there's that and also people weren't shipping as much so you could just make a little bullet list. Here's the things I shipped last quarter, this feature, that feature, this feature, that feature. 

**Fiona Fung** (00:12:22):
That's right. 

**Lenny Rachitsky** (00:12:22):
So, I think what I'm hearing here is this is one of the only ways to stay on top of all the things a teammate is shipping. So this is a really cool thread of just how you found ways to stay on top of this 8X increase in code. What else has worked in helping you and your team stay on top of and maintain quality of all the stuff that y'all are shipping because that's obviously a challenge, a bigger challenge.

**Fiona Fung** (00:12:42):
Yeah. And so definitely the feedback channels are really important to us, but then we also get a lot of feedback. And for example, even I myself, usually my morning ritual would be I get my morning cup of coffee and then I look at the feedback channels and then I try to pick, oh, if I have some maker time, what's something that maybe I would be able to help out or what I could see some gaps like that. It just used to be something I would do every morning. And yeah, I think maybe a month or two ago we launched Routines and that's also completely changed. 

**Fiona Fung** (00:13:11):
Now I just have a routine that automates all this for me. And then there's also, it's almost like before I would be able to generate some prompts, but now with Routines, it's almost like I'm having an agent help me generate the prompts and the PR. So for example, one is, "Hey, keep a look on this feedback channel, what are some of the themes?" And then when I wake up, then I have a really good summary of that and then even some PRs that I'll be able to take a look and review.

**Lenny Rachitsky** (00:13:38):
And the feedback channel, where's that feedback coming from? Is that like emails, Twitter, or a combo of everything?

**Fiona Fung** (00:13:46):
Our feedback channels are definitely like we have a lot from internal ends, but also emails, channels. Actually everybody when we all get feedback on either when friend's ping us or on LinkedIn or socials, we'll all actually post all of that in Slack as well. And we also have of course partnerships and so we have different channels for all the various sources, but that's what I mean. I need Claude's help to help me stay on top because there is so much incoming feedback.

**Lenny Rachitsky** (00:14:14):
Got it. Okay. So this is cool. So this is a way of working that you've built to stay on top of all the stuff shipping, which is this kind of daily ritual/routine where you as a manager look at what people are saying about the current state of Claude Code and Cowork and used to just like, "Okay, someone go fix this, go fix that." Now it's like, "Here's the PR that'll fix this thing. Check it out. We're ready to ship it if you want." Awesome.

**Fiona Fung** (00:14:15):
That's right.

**Lenny Rachitsky** (00:14:41):
Okay. Obviously a big challenge for people is also just code review. I imagine Claude is also doing a lot of its own code review. Is there anything there you've recently figured out that allows your teams to ship faster stuff that they are confident is great?

**Fiona Fung** (00:14:55):
Yeah. And honestly, it's crazy when you think we didn't even have Claude Code reviews last year. And so speak of bottlenecks, that was a really, really big bottleneck of the human reviewers. So we definitely, for the important areas that need deep subject matter expertise, we definitely want to make sure we have the proper humans still reviewing. I would say what helps us though is the more that we can automate to almost check in the framework for what good looks like. Claude is very good when you give it a framework to validate against those frameworks. 

**Fiona Fung** (00:15:25):
So I had mentioned recently we just updated the content design to have a skill in it. And this is why I think if you have specs or check those into the repo and then make sure the spec also keeps up to date with the code frequently. But that's what I found works really well of anytime you have a statement of what good looks like, get the end to the repo and then Claude Code review can make sure it's still matching what you set up to do.

**Lenny Rachitsky** (00:15:53):
And basically it's like the evolution of test driven development.

**Fiona Fung** (00:15:56):
Yes. For TDD, because I remember that was a big thing, my gosh, maybe like in the 2000s of the test first and then you can make sure the test fails, then you do actually the code. In principle is really good. But I know I remembered, I myself struggling a bit because it was almost like you have to eat the broccoli first because I was like, "Oh, you have to write this test first." And I just get so much thrill out of shipping and building product. So it's funny, actually the first bug I fixed on Claude Code, I remember asking Claude, "Hey, I want to do test-driven development. Help me write the test first, make sure it's fails and then we'll actually do the fix and then now the test passed."

**Fiona Fung** (00:16:32):
And the fact that used to be that test generation used to just be this tax that I remember having to pay, the fact that that's now automated and you can even revisit all these principles that have been around for a while. But now they actually might be even more efficient just because you have the models that can do more of the work for you.

**Lenny Rachitsky** (00:16:51):
Yeah, that's so unfair. It just writes the test for you first. So on this point of builders, one of my favorite slides from your talk that I want to ask about is who you are hiring and what you look for in people. And so I'll read what you said there and I want to hear more here. So the two profiles that you now look for when you're hiring are creative builders with product sense and deep systems experts for the hard parts.

**Fiona Fung** (00:17:18):
Yeah. The deep subject matter expertise, for example, when I first joined Claude Code, we had really great product generalists and then I realized, oh, we were missing folks with systems background. And so that was definitely an area that we needed more folks with systems and distribute systems expertise. And so I would say it's all about trust but verify. The models are really good, but there are definitely a lot of areas that still need the verification. And so wherever you need the deep subject matter expertise, I would say that's an area to definitely still invest in. 

And the other one is kind of like the product [inaudible 00:17:57], almost like the dreamers. These are folks that usually will be like, "My gosh, you're really passionate about a product." And they have an idea, they build it, and then it's always like looking at the feedback and then iterating and polishing and making sure that the product is a delightful experience. Owning that product end to end, that's another skillset that served us really well on Claude Code.

**Lenny Rachitsky** (00:18:20):
This super resonates. There's this word ambition. I don't know if you used it, but that's what I thought of as you were talking. That's been coming up a bunch recently in the podcast and other work I've been doing. There's this 10xC engineer I was talking to the other day and he was just like, "I heard about a feature idea." Someone's like, "Hey, we should build this. " And I was like, "No, that's really hard and complicated." And he's like, "But now I'm like, no, no, that's so possible. I just ask Claude Code to do it and he just does it."

**Fiona Fung** (00:18:20):
Yes.

**Lenny Rachitsky** (00:18:48):
And it's this whole mindset shift and he's just realizing now it's about how ambitious can you be. Everything is now possible in theory. Now it's about how ambitious and how big can you think versus just like, okay, it's all these stupid little features and things they have to unblock. Does that resonate? Is that something that you think about?

**Fiona Fung** (00:19:06):
Yes. Actually, I was just catching up with an engineer yesterday and he actually is not a mobile engineer by trade, but we really needed to update this feature to also have a mobile footprint. And it was just amazing. He's like, "You know what?" And it's common because you might think, wait, but I'm not like an Android expert. But now, thanks to Claude, actually I can actually have a partner and actually also do this on the mobile surfaces. And so that definitely resonates. It's lifted the ceiling of what anyone is able to do.

**Lenny Rachitsky** (00:19:39):
So let me follow that thread, as the role has transformed in such a crazy way, some people are thriving, some people super frustrated, unhappy, fighting, resisting. What do you see common across the people that are doing really well, the engineers that have adapted and are thriving versus the engineers and even outside engineering that are just frustrated and having a bad time?

**Fiona Fung** (00:20:04):
I would say a growth mindset really, really helps. Actually, even before AI tooling, I found that has been just so valuable. And I learned that a lot. Actually, it was the shift from Microsoft to Meta. That first year I'm like, "Oh, this is what having a growth mindset really means." It's really this concept of always be learning, also what served you to get you to this point may not serve you no longer. But it's really hard because of course everybody, we've all gotten to the state by acting or operating in a certain way. And so sometimes it is a little bit scary to think, "Wait, but I've been successful so far. You're asking me to change what has made me successful." 

**Fiona Fung** (00:20:48):
And so I would say the growth mindset has really served me well and I think it's also served others well that I noticed like always leaning in with curiosity and always being able to learn. And then in terms of the frustration, I think sometimes I also see a little bit of fear. And so my advice there is, at least this is how just in life, because we all have... And fear is of course an evolutionary, I didn't study anthropology, but I think it makes sense, right? It helps us make sure we were able to survive and not get eaten by larger predators.

**Fiona Fung** (00:21:27):
But for anything that there is a fear, my advice is kind of lean in and ask, "Okay, what can I do about it? What is within my control?" Because sometimes the frustration comes from fear and feeling like everything is outside of my control and so it's happening to me. And so if you think about, "Okay, what is in your control instead of happening to you, is it happening for you? And then what's something that you might be able to do and change?" I felt that's been helpful, because if not, it is super frustrating to have the fear and then feeling like everything's outside of your control. 

**Fiona Fung** (00:22:04):
I actually remembered when I was in, actually when I was in high, it's funny when we were going back to IBM, when I was in high school, I actually didn't go into computer science or engineering. I really wanted to be a visual artist and this is how far back we go. Back then, computers were really expensive. So I actually didn't even have access to a computer. My first access to computer was grade nine, I think in high school. I don't even know if this happens in high school anymore. My high school had a typing class where you went to class just to learn how to type on a keyboard and learn to be really proficient and that was my first time and then the next class was maybe like some HTML programming.

**Fiona Fung** (00:22:45):
So anyways, but the reason why I fell in love with it was what I love about art is creating and being able, if you have an idea, you can go ahead and create and tell a story. And then I realized, oh, computers and programming, that enables me to do that. So anyways, I tried to really fast try to make up for all the science classes for me to get into university, but I had this fear of, "Oh, but how will I afford to get into an engineering school?" And it was this big unknown. I grew up in Ontario, so I was very grateful. I knew there was an Ontario School Assistance Program, OSAP, I think, which I'm very grateful for. But I didn't know how much of that would cover my tuition or expenses and it was just this unknown and it would be like a year out.

**Fiona Fung** (00:23:29):
And I remember thinking, "Okay, what can I do about it?" And then as luck would have it, the National Bank of Canada just posted this flyer in our high school saying, "Hey, we're hiring high school interns to be a bank teller." And I remember, and of course it was going to be minimum wage, but I thought that could be a lifeline. But it was funny because the class I hated the most in high school was accounting, so I don't know if it would be any good at it at all. But I signed up to be a bank teller and that ended up being such a great decision because I worked all summer, saved up. 

**Fiona Fung** (00:24:00):
And then actually I was able to work as a bank teller on the weekends. So I would go to school Monday through Friday and then on Saturdays be a bank teller. And that ended up being this lifeline that enabled me to pay for all my school expenses. And we talked about the year 2000 dot com crash that when folks weren't hiring as much interns actually, I continued being a bank teller for two years. But that was the one action I felt I could take that was within my control to try to counter this fear I have of, "If I'm really going to go down this path, I don't even know if I could have afford to go to school."

**Fiona Fung** (00:24:38):
So that's probably my other advice of growth mindset and the source of frustration or anxiety. If it's coming from the like, see, is there one action that's within your control that you can take. There was a saying do some things. What would you do if you're not afraid actually? Those were my two favorite things before like, "What would you do if you're not afraid and do something scary once in a while?" Because-

**Fiona Fung** (00:25:00):
... Are my two favorite things before, like what would you do if you're not afraid and do something scary once in a while? Because that's also usually how we grow. I found that when you're really good and professional at what you do, you're kind of at peak maximum efficiency. But then how do you keep growing is you then do something scary that you might not have done before and yeah, you will have a dip because you need to learn, but that's kind of how you keep pushing yourself to learn.

**Lenny Rachitsky** (00:25:23):
The quote that I have probably used the most on this podcast of all quotes is, "The cave you fear contains the treasure you seek."

**Fiona Fung** (00:25:32):
Oh, I love that.

**Lenny Rachitsky** (00:25:32):
Yeah. And it's so true. I forget who put this, but just the thing that is scariest is like, that's a compass towards that's what you should be doing. In terms of career.

**Fiona Fung** (00:25:42):
I'm going to steal your quote.

**Lenny Rachitsky** (00:25:46):
Yeah, please do. Don't do all the scary things. Maybe don't jump off a cliff, but maybe in career moves, it's probably a good choice. So kind of following this path, something that I know that is important to you, something you think about that I also think about is this kind of gap that is forming between people that are just leaning into AI, killing it, doing super well, and then people that are just not. And this is a scary time for people that may be left behind in this new world that is emerging. I know you spent a lot of time with small businesses; that's a big passion of yours, to help people learn how to use AI in their work. Talk about just how you think about that and what maybe we should be thinking about to help folks stay, not fall behind basically.

**Fiona Fung** (00:26:31):
Oh, I love this. Yeah, it's one of my passion topics because I kind of mentioned growing up in Canada and I moved there when I was a kid. I was born in Hong Kong so I didn't speak any English and my parents had to work all the time. So my grandma who is the best grandmother anyone could have ever asked for. I know everybody thinks their grandma's the best, but I really was so lucky I had the best grandma. She moved with us just to take care of me while my parents were working, but neither of us spoke English, but I was able to learn how to speak English by going to school and speaking with classmates. And when I think about my grandma, it was very alienating for her to be in a new country where, and back then it wasn't as walkable.

**Fiona Fung** (00:27:12):
But one summer I remembered we just happened to find this little yarn shop that was owned by a lady that also spoke Cantonese. And so that became every week we would go to this yarn shop the summer. My grandma found her knitting circle and then I think I learned how to do macrame, which I think is having a comeback by the way. It's always funny to see what's-

**Lenny Rachitsky** (00:27:32):
Macrame coming back.

**Fiona Fung** (00:27:33):
Macrame. I think, yeah. Heard it here first on Lenny's podcast. I think macrame's coming back.

**Lenny Rachitsky** (00:27:38):
All right.

**Fiona Fung** (00:27:40):
But that was probably where my love came from. I'm like, oh wow, this little small business created this wonderful sense of community. And I've been really fortunate to become friends with all of the small businesses that I love. So that's kind of like where the passion comes from. And then how it happened was I was using Cowork for my own business expensing travel. I don't know what it is. I really don't like doing business expensing. And when I was using Cowork, it was magic. I'm like, "All these things that I don't like to do, like Cowork is doing for me." And I'm like, "Wait a minute, all my friends," and honestly, small business owners, they really bust their butt. They work incredibly hard and sometimes might be operating on really small margins.

**Fiona Fung** (00:28:20):
And so I thought if Claude Cowork is so good at helping me do my little business travel expense, this would be huge for it. Because I see my friends sometimes sitting at the bar with stacks of bills and all they're doing is invoicing and expensing and I think nobody actually really likes to do it. So that's kind of where it came from. And then so yeah, I remembered helping a couple of them onboard and it was also very humbling to see them go through our onboarding flow. Actually, they found some really good bugs. So it was really like a win-win, but it was also delightful for me because they also use Cowork in ways that I wouldn't have thought about because I was all fixated on, look at how it is amazing with PDFs and invoice.

**Fiona Fung** (00:29:02):
And then one of my friends who runs two restaurants, she's like, "Oh my gosh, this folder I have is like a junk drawer of, like it's basically our documents folder. It just becomes this junk drawer of every, or downloads, just like the kitchen junk drawer." And she's like, "I know I have a few menus in here and I can't find it." And I'm like, "Well, let's ask Cowork." So we gave Cowork access to directory, found the menus. And then she use in a really unique way. She goes, "I want to make sure I keep my prices reasonable for locals and tourists." So she goes, "Hey, Claude, look across my style of cuisine in this area. Is it comparable?" And it came back with really cool, almost like market analysis. And she goes, "Hey, I actually just went to that restaurant in Seattle and that was pretty good." So I learned something every time. And yeah, they've been giving me great feedback as well.

**Lenny Rachitsky** (00:29:48):
So the question then is just like, how do we spread this to everybody? Because a lot of people are just like, "I don't have time for this" or "I hate AI." It's just like, I want to ignore it. Is it like talking, is it just talking about these, sharing examples? What do you think? What's a way to make a dent in this problem?

**Fiona Fung** (00:30:07):
For all of us, especially to your listeners, are probably very AI-pilled. If there's anyone either in their community or their family that has like... I would start with what has something that you really have felt has made a meaningful life change for you with the AI tools and then seeing if that is a conversation starter for... Because for me, AI is a tool. Again, it's the whole light in the dark. I totally understand the frustrating part as well. But for me, I'm also felt like knowledge is power. Have to learn how to use the tools because it could actually be the light part of that light and dark equation. So I think that's something that I would love everybody's help with, whether it's a community member or even if there's a business you really like and you think, "Hey, have you ever..." It's a little awkward to start.

**Fiona Fung** (00:30:56):
I remember when I first reached out to my friends, I'm like, because I don't talk about what I do with them a lot, but I'm like, "Hey, I kind of work in AI. Can I..." It's even unnatural for me to do it because I'm like, "Hey, can I show you what Cowork is possible?" But we ended up having a lot of fun. So yeah, I would love for, like that conversation starter would be great of, yeah, because I just want to make sure we keep sharing the knowledge and making the tool equitable because if not, I'm concerned that the divide grows larger and larger.

**Lenny Rachitsky** (00:31:29):
Me too. I find that sharing use cases, as you said, is so powerful. I was just using Cowork the other day to fill out my son's camp forms and just sharing that on Twitter, just like a lot of people are like, "Oh wow, I didn't think about that." Yeah. It's just like these little things you don't think about that Cowork and Claude Code can do.

**Lenny Rachitsky** (00:31:47):
Kind of along those lines, speaking of Cowork, if you think about it, Anthropic has been super early on uncovering these really big opportunities ahead of everyone else. For example, coding. So far ahead, like realizing this is a huge market. Whether it was intentional or not, it was just like, whoa, that's maybe the biggest new business opportunity in history. And then Cowork is a great example, just leaning into knowledge work. Let's just solve all knowledge work. Why not? So far ahead of everyone else. Another element is it feels like a focus on the personality of the model, something you all were very early on, just how important that is, not just for the experience, but just also the intelligence and success of the model. What is it that you think Anthropic and the teams do differently that allows you to uncover these opportunities and then just go big on them before other labs, let's say?

**Fiona Fung** (00:32:43):
Well, I haven't worked in any other labs, so I'm not sure how labs operate, but I will share like, yeah, with... And actually on the Claude Code team as well and Cowork, we also keep an eye on latent demand. Now, we're very fortunate with coding as a use case because so many ads that we were like our own first customers and we're able to do really rapid feedback. But latent demand has been like a, for example, like Cowork we noticing a lot of folks that were not necessarily coders were using Claude Code. Can we make that experience better?

**Fiona Fung** (00:33:15):
I think that's actually even outside of Anthropic, that served me well in all the different products I've worked on. And actually it's funny you mentioned the Claude for my passion with small business. After I had a few of those visits, we ended up now launching Claude for Small Business, which is really cool because I, and it totally didn't come from me, so I'm not taking credit, but I noticed it too of like when I was working because they were asking me, "Oh, does it have this plugin or at this plugin?" I'm like, "I think it does." And then we have to go and search for it.

**Fiona Fung** (00:33:45):
So actually now Claude for Small Business bundles it all up. So inside Cowork, you just have this little toggle and there was a wonderful team that's been doing Cowork sessions with small businesses that probably found, "Hey, we could have an efficiency gain here or make the experience better." And so I would say always, not only for products that you're on, like making sure you're always listening to feedback and always iterating, trying to make a delightful, reliable, high quality experience, but then also keeping an eye out for, "Oh, what are these other use cases that are popping up? And can we also make that experience better?" It's interesting. In software, I've learned that customers will use your product in ways that you did not intend for good or for bad. And so the best way is really, it's all about the iteration, learn and keep close to the feedback.

**Lenny Rachitsky** (00:34:40):
Weight and demand. That term's come up a bunch on this podcast. There's some there. Might be some there. So essentially, it's just watching closely for behavior that you may not have expected or that it's just kind of emerging and then just going big on that essentially, exploring it, building something awesome.

**Fiona Fung** (00:34:57):
Yeah. And having a hypothesis for, hey, because actually when you see people jumping through hoops to make something work, can you actually make that an even like, a smoother and better experience?

**Lenny Rachitsky** (00:35:08):
Yeah. Coming back to the way that your teams operate, you guys are so at the edge of what's possible and the role of just engineering has changed so much. I'm curious what you think is the next kind of frontier of how engineering in particular is going to change. Is it like fleets of agents? Is it something else? Just what's the next big shift to how engineers operate that either you're already working on or implementing or just is starting to happen?

**Fiona Fung** (00:35:36):
I would say we're shifting more towards async, like asynchronous. And so to your point, the fleets of agent, like that's why routines is so interesting because it's almost like I used to be doing a prompt and synchronously and then I would maybe kick off different props asynchronously, but now I can actually have a routine that actually generates these prompts for me. So it's almost like the level of abstraction keeps pulling up a little bit. And so yeah, I wish I have a crystal ball to see what this is going to look like. It'd be fun actually for you and me to revisit a year from now.

**Lenny Rachitsky** (00:36:09):
No, I want to hear more about this. So help us understand what is routines and then when you say synchronous, you're writing a prompt and it just kind of goes off and is it writing it immediately? Talk about what this actually looks like.

**Fiona Fung** (00:36:21):
Ah. Yeah. So routines is like how you can... So if you remember, I was chatting about my... What I used to do is always wake up with my morning cup of coffee and, "Hey, look through this Slack channel for me." But then now I have a routine that I set to run every morning at a certain time.

**Lenny Rachitsky** (00:36:21):
It's like a chronic job.

**Fiona Fung** (00:36:37):
To say hey. That's right. But then it's able to actually go and kick off agents on your behalf because even before it would be, oh, you could, yeah, do a chronic job to automate, but now it's, "Hey, look at these feedback." And then if you're seeing some of these bugs, that what are some polish fixes that you might be able to knock out? And then it would go kickoff and then I wake up and I end up having PRs that I could review versus before, which is still more of AI can have different agents.

**Fiona Fung** (00:37:05):
And then I'm still thinking about, okay, now what do I do with this information? So it's like that higher level abstraction of, okay, now how can I actually write a routine that also basically does prompts for me for spawning different agents? So I think we'll move more towards that kind of asynchronous style of working.

**Lenny Rachitsky** (00:37:23):
So interesting. So in a sense as a manager, you have these kind of things you do daily and what you're saying here is you can set up these prompts that kind of check in every day on the things you would be doing. Like how are the projects going? What's falling behind? What should I unblock? Who's struggling? And how do I improve some polish? And so the idea here, what you're describing here is write these things that you almost do as a manager daily and have Claude essentially do them for you and then show you, here's what I'm doing, here's what there is to review.

**Fiona Fung** (00:37:54):
And then it's even like, then giving even more autonomy at some point of, you know what, go for it. For example, a verification-

**Lenny Rachitsky** (00:38:01):
[inaudible 00:38:01].

**Fiona Fung** (00:38:00):
Is really good.

**Lenny Rachitsky** (00:38:01):
Yeah.

**Fiona Fung** (00:38:02):
Go for it.

**Lenny Rachitsky** (00:38:03):
I see. So you give it a little bit of freedom to do more of this?

**Fiona Fung** (00:38:05):
Yeah.

**Lenny Rachitsky** (00:38:06):
Okay. That is so interesting. It reminds me, speaking on this idea of go for it, like I wasn't planning to talk about this, but I just watched Tyler Cowen had this awesome talk about just like what's happening. I don't know if you know Tyler Cowen, this really smart dude, economist, has a podcast. There's so much talk of the people that are doing best in this world. His term is initiative. They have initiative. Another term people use, agency. Is that something just like, people hear this a lot, just like the people that seem to be doing best are taking the most initiative, getting the most proactive, have the most agency. Does that kind of spark any thoughts to you, just what people may need to, I don't know, think about or improve on?

**Fiona Fung** (00:38:47):
Actually, I love that word: agency. That's what we really hold important on the Claud Code and Cowork team. But it's interesting, I say along with high, because we really, it's about like, "Hey, here's a problem." And then it's really everybody on the team has ideas for how to address the problem. So it's really high agency. And then we say with high agency, it's also high accountability. So it's all about making sure folks have that freedom to cook, but then it's also like, okay, what's the accountability for it as well? And again, it goes back to what's a hypothesis of what you're trying to solve. So I think, yeah, the balance like are almost like two sides are the same kind of agency and then accountability I think has served our team really well.

**Lenny Rachitsky** (00:39:29):
Such an important element of agency. Okay, cool. Everyone's off doing stuff, but okay, what have you busted it up? What have you done? So kind of along those lines, it feels like there's this vibe shift recently from token maxing, just go crazy, spend as much as possible, just see what's possible to like, wait, what are we actually getting out of this? How much is it costing? What's the ROI? Interestingly, Boris was actually head of eng productivity at Meta. That was his job, is measuring eng productivity. And then also just this tweet of lines per code, like code shift. There's this interesting discussion of just how do you actually measure productivity increase and ROI of AI tools in spend? You guys have the unfair advantage of getting free tokens working in Anthropic. With that in mind, what have you learned about just how to measure say ROI of engineers in today's world?

**Fiona Fung** (00:40:27):
This eng productivity is such a fascinating topic. Yeah, because I remember even Boris mentioned like, "We'll first start with lines of code." And then I remembered once then there was a debate of, "Well, lines of code, this engineer had this crazy lines of code, but they just took some library and then just was porting it." So they checked it in and then I was like, "Well, maybe it's significant lines of code." And then it's, "Well, but what if we're updating our frameworks and now we're generating less code, but the output's still the same?" So now I was like, "Okay, maybe it's time to land PR." But it's very interesting of it's always been whichever metric, like if you're really focused on the out... My advice here is one is output, like is the output really going towards the outcome? Because yeah, the token maxing, it's almost like the lines that we code that we used to have, but I'm really much more about a, what is it that we're trying to do?

**Fiona Fung** (00:41:26):
All of this... There was another saying I really like, "Don't forsake motion for progress." Because if you're measuring tool user usage, then you're measuring the action, but is it really making whatever the end outcome of yours important? And so I really try to zoom out and focus on what is the problem we're trying to solve, what's a good way to measure that. And then that's what we focus mostly on versus the productivity measurement. I would say though, outside of metrics, especially on teams as you're having more people adopt AI tooling, I would say definitely go on a listening tour for the leaders listening to a podcast. Especially, I love to focus on the senior engineers as well, like hear from them on what's working, what's not, how can we actually make it better because they will also help you multiply and scale that up across a full engineering team.

**Fiona Fung** (00:42:21):
And sometimes it's those conversations where you might spark an idea that comes up and also really good shared learning versus metric dashboards. It's very interesting. I've learned some good lessons from metrics. I'm all about, like it's really great when you have a metric that you can actually help climb on, but always keep in mind of is, kind of my whole growth mindset of, is it still serving you? Always keep in mind like, is that metric really still serving the outcome that you were aiming for?

**Fiona Fung** (00:42:50):
A fun example I have of this is in the early Facebook Marketplace days, we were kind of launching by region and we really wanted to make sure we're building a delightful product before we expand. And I remember in the early days, one thing we would keep an eye on is number of sellers. And I remembered after launching to our first region, I'm like, "Oh, in this area the number of sellers is low, but actually people are finding items that they're looking for," which is what we're aiming for or like helping people find items that they need.

**Fiona Fung** (00:43:19):
And then I realized in that region it wasn't a large number of sellers, but there were power sellers. But our first gate before we expand would've just been factoring heavily number of sellers. And I remember that quick conversation of, hey, and this goes back to that whole people will use things in ways you may not expect and shift, iterate, learn. And so then we updated the metric to go, oh, it's not a number of seller because it didn't factor in power sellers. And so that's the advice I have too. Whatever metric, whether for productivity or even for product, always keep an eye and make sure that you're not just having blinders on that's blindly following a metric that used to make sense because sometimes the landscape can change so fast, even the metrics themselves might need to be adjusted.

**Lenny Rachitsky** (00:44:01):
And this comes back to your process that you shared of having Claude watch all the PRs shipping per engineer, let's say, and then not focusing on the metrics, but focusing on that leading to a conversation about what impact does this have, what was maybe some bugs that happened and that being a really powerful way of understanding what's going on with this engineer. Awesome.

**Fiona Fung** (00:44:24):
That's right.

**Lenny Rachitsky** (00:44:25):
Let me come back to this, just this question of speed and quality and just impact. Is there anything else you've learned about just how to balance those things, just like this crazy velocity of code that's being generated and just staying on top of quality and impact. Is there anything else there that might be helpful to other teams that are trying to wrangle all these PRs being shipped every day?

**Fiona Fung** (00:44:47):
I would say, and this is what honestly we want to keep doing more of and being better at it too. The proactive quality, so especially for quality, making sure that what are the experiences that are key and making sure you actually is, actually speaking of metrics, those are really good things that make sure you can see trends over time. And so on the quality front we found, and this is like the more proactive we can be of making sure we can get an earlier detection into quality. And so that's been one thing that we've been paying a lot of attention to. So I started this, "Hey, let's have a concept of what's bad versus what's sad." And bad is like a very bad irrecoverable error and sad is something that's kind of like a pain point, recoverable, but it's interesting when you stack up sads, it could generally go to bad.

**Fiona Fung** (00:45:39):
But even starting with a high level framework like that and because if not, I think sometimes with dashboards you can have time to load or all these other, but when you're dealing with a lot of different product surfaces, it's harder to go, "Wait, is that a good number or not a good number?" And so one thing that's helped us is versus just raw performance or reliability numbers, also having some framework of what we think is a bad experience and making sure we're focused on addressing those and then also keeping an eye on where we're seeing in terms of the sad.

**Lenny Rachitsky** (00:46:12):
I like that.

**Fiona Fung** (00:46:12):
That helped us a little bit.

**Lenny Rachitsky** (00:46:14):
Yeah, I like the bad and sad. So these are like thresholds of this is bad. Okay, this is serious. And this is in terms of performance or failures or what sort of things are you measuring here?

**Fiona Fung** (00:46:24):
So for example, we allow each team, like speaking of agency, so knowing that bad is like a really bad irrecoverable error, we enable each team of further surface areas or it could be services that they lead. So for example, on CLI could be crash rates, like a crash is pretty bad, you lost work. And for example, sad might be, "Hey, is it flickering?" It might be recoverable. But we have each team, and that's why it's been interesting because surface areas are different, we would have all these dashboards, but it's harder to zoom out and go, "Okay, what's the overall theme of the experience?" So to your point, we give high agency to each team of what we think constitutes a bad and what's a sad, and then what's the goal that each team wants to take.

**Lenny Rachitsky** (00:47:07):
The main takeaway I'm hearing here is one of the best tools for staying on top of quality is just monitoring and tests versus spending more time reviewing, which makes sense because the speed is just impossible to stay on top of. And it almost speaks to this idea of closing the loop for agents to be able to figure things out themselves. They know what success looks like, cool, we'll fix it ourselves. So that's a really interesting takeaway, is just invest more in the tests. Evals I imagine is part of this and then just monitoring failures and speed and things like that.

**Fiona Fung** (00:47:38):
That's right.

**Lenny Rachitsky** (00:47:39):
Something, I think this is public. I know that you guys have this dashboard that tracks just like F-words, how often people are like, because they're so and frustrated. There's like a funny term for it, I think. I forget what it's called.

**Fiona Fung** (00:47:51):
Yes. Actually, I remember. Yeah, that was last September because we were all seeing some frustrations and yeah, that was an engineer on the team of, "Hey, we should maybe track swear words." I'm like, "Oh, that's a great idea." I remember it. I had just joined when we were having that really fun conversation. Yeah. So it's again, like it's very interesting to look at... And that's why evals is hard too because it's going back to that user experience and how we can make sure it's a delightful experience and less frustrating. But yeah, the swear word dashboard is a fun one.

**Lenny Rachitsky** (00:48:22):
**Fiona Fung** (00:50:01):
I love it. It's funny, when I first join...

**Fiona Fung** (00:50:01):
I love it. It's funny when I first joined, and I have amazing recruiting partners and I noticed this whole theme of growth mindset, it's just because the landscape is changing so fast. What worked well before may not make sense and even what makes sense today may need to change tomorrow. That's what I have to keep reminding myself. So yeah, when I first joined recruiters like, okay, yeah, we have these couple of manager postings and because actually how it came from a listening tour I did with all the members on the team, and I heard a lot of these, "Hey, I really appreciate the agency, but how can I make sure prioritization?" And so through that, and then there was some really good feedback too of making sure that it's not too many layers of reviews. There was good feedback. Some folks might have joined from other companies.

**Fiona Fung** (00:50:51):
And I actually think as a leader, if you actually start as IC first without the worry of supporting people, because that's a very heavy responsibility, but before you have to take on that full responsibility, give yourself that maker time to actually dive deep into the code and learn the code base or the product, whatever it is. Honestly, the PRs I do, but it's more about for me, it's important because it keeps me in the flow because we're making so many changes to Cowork and code. So even me doing PRs, it's less about what it is I'm fixing. It's more about me using the product every day just to keep that touch, because as amazing as metrics and everything are, and I do look at those dashboards, as a leader, if you're not living and breathing your product every day, you sometimes lose the touch and feel of the product.

**Fiona Fung** (00:51:48):
But anyways, on the manager front, I think giving time for managers that join to be able to go deep into do that before supporting people, and then they actually end up building really great rapport with the team, because if not, I think sometimes as managers, you might come and join a new team and you instantly think, "I have to manage. Let me dig into my manager toolbox and do manager-y things." But if you actually give yourself time to not have to worry about that first and actually learn what it's like to be an engineer and teammate on the team, that also goes really far to building rapport. In terms of using the product, I think that's important. It's interesting, every team I've joined, one of the first actually across all the different products, it could be VR, it could be smart glasses, it was like Instagram.

**Fiona Fung** (00:52:34):
Usually when I first joined, one comment that comes back to me is, "Hey, you know what? I really love how you're actually using what we build." It's refreshing to see you giving user feedback, and so I think as leaders too, it's also a way for us to experience the work personally that the team does.

**Lenny Rachitsky** (00:52:50):
Something that people may not realize you were overseeing an organization of like 500 people at Meta before you moved to Anthropic and you moved to IC engineer basically and Anthropic from that.

**Fiona Fung** (00:53:02):
I started out, it was for a very short amount of time, but actually this was my journey between Microsoft and Meta. So at Meta, I interviewed as a manager, but I think at least for the first quarter, I was also an IC because I really wanted to learn what it's like to be a Meta engineer, because before then I was at Microsoft, cut my teeth on engineering at Microsoft. So I knew all the code bases, the tools, the languages, but it was so valuable to have those first months actually learn what it's like to ship as a Meta engineer. Plus it was also fun. I think sometimes we forget, but that's by the way, what I love about Claude Code because the last time I shipped production software at Meta was probably 2017, and every year, I do a lot of dogfooding and I also use dogfooding to help me vet the quality of product as well.

**Fiona Fung** (00:53:58):
But it's been a very long time since I shipped production software, it's because part of it is I don't want to screw something up. I'm always so scared of what if I do something and then I cause a bug and then am I verifying everything properly, or am I wasting someone's time? Because also the tool flows would change, but I remember that first week on Claude, at first I almost again did my usual, let me go meet all the engineers and treat them to coffee, and then I'm like, "Oh wait, let me ask Claude." And so Claude was this really good onboarding buddy of mine because I was curious about the copays asking questions, and then it also really helped me do the automated test, but I also want to still do some manual testing, and I asked Claude, "Hey, help me come up with what's the way for me to manually test this to make sure I cover all the case." But all that then gives me confidence that okay, I can ship here again.

**Fiona Fung** (00:54:50):
And then I got kind of more comfortable with it again, and so I've actually had a lot of friends reach out to me that have been managed for a while that's like, "Hey, I'm shipping code again, thanks to Claude." But in general, it's just important to me as leaders to make sure you're using the product that your team builds.

**Lenny Rachitsky** (00:55:09):
It's so interesting that you are overseeing the team as an engine leader that is most changing the role of an engineer. It's such a meta role. The work of an engineer is transforming because of the software that you're building. One question along these lines is just do you worry about engineers' skills to code atrophying from not actually writing code anymore and does it even matter? Is this something you think about? Is it a big deal?

**Fiona Fung** (00:55:39):
It's interesting because we actually have this discussion on the team a bit. Are there things that we miss? Or actually to your point, I'm always thinking about when someone's onboarding and ramping, you have Boris who handrolled the code in the early days and of course now doesn't anymore, but he gained that knowledge from before because he was in the code base. So for especially all the engineers that join, I'm also like, make sure you're taking the time too to all the work that you do, still get the understanding of the architecture or the change because it goes back to that trust but verify. Maybe one day it won't matter anymore, but at the pace that we're going, I actually still think, it's always double clicking on that layer that you depend on. Maybe that to me is a meta. It's always take that time to learn about your dependencies because this way when your dependencies change, you're kind of more aware, or you might not be taking advantage of changes to dependencies.

**Fiona Fung** (00:56:31):
So I think it's always about doing that double click, but the other thing that we found interesting on the Claude Code team is after a while we felt it could start being a lonely experience because we all started just working with our agents so much. So recently we started maybe a pairwise programming lunch because what we also learned was on Claude Code, everybody uses Claude Code Cowork. Everybody uses a flow so differently, and so we found that wow, when we do pairwise programming, we actually learn so much from each other, and then the other thing too is we make sure that we also have the maker time together too. So for example, hackathons is another thing we really like to do just to make sure we're kind of interacting together as a team.

**Lenny Rachitsky** (00:57:16):
That is such a good point, just like the loneliness that emerges because used to be engineer teams building code together. Someone's doing backend, someone's doing front end, someone's doing iOS app, probably a bunch of people on the backend and it's like, " Well, if 10 Claudes running in parallel doing all these things," that is such a good idea of just finding ways to connect engineers. So the idea here is almost parallel programming but not. It's like parallel play when kids are grown up. You're kind of working next to each other but building your own things, but even just watching how other people build, your finding is really valuable.

**Fiona Fung** (00:57:51):
Yeah, and it's because our own tool chain is changing so fast as well, but yeah, it's very interesting to me. Everybody on our team just uses Claude Code and Cowork in different ways, and so every time I watch someone work, then I learn something myself as well.

**Lenny Rachitsky** (00:58:06):
How do you manage people getting over obsessed with their optimizing their workflows? Is there anything you're just like, "Okay, it's fine, just keep going."

**Fiona Fung** (00:58:15):
I haven't seen too many folks on our team. I think as everybody is just really excited about either an architecture update that we think will be higher reliability or some product experience. So most folks, that's what we talk about a lot. It's fun lunchtime conversations, but I don't think we over optimize because there's no perfect answer actually.

**Lenny Rachitsky** (00:58:39):
There's too much to do. These are really interesting insights. Just like as the role transformed, things come, things go. So I'm curious what else has kind of lost in this new world of software engineering. I used to be an engineer. I don't know if you know this. I was an engineer for 10 years, and it was like so fun just to sit there inflow coding, this feeling just like, "Oh wow, it's working. Look at it compiled. It's amazing. I'm making progress." And now you don't do that anymore. You just sit there and kind of wait for agents to build the thing. What else is kind of lost in this new world for engineers?

**Fiona Fung** (00:59:12):
It's so funny. I just had that conversation with the engineer and the team of talking about flow. Remember the old days you have this really gnarly problem and you pop that music soundtrack in, and then you're just in the zone? So yeah, and then there was always that big aha moment at the end I would remember. You remember being like, "You finally cracked it. Yay." So we do, but I think now we get a lot of joy from the product, but I do think because I hear from other engineers as well of well, some of the hardest parts is what I used to enjoy. Yeah, I heard that from another engineer as well, and so I think we're all just kind of shifting, but I do see the thing and that's why I was talking about the pairwise programming and the hackathon, that did recently come up more. Folks were starting to feel like it started to be a lonely experience.

**Lenny Rachitsky** (01:00:07):
So interesting. Within Anthropic, I'm curious, so engineering the most transformed I think of any role right now, what's the second most transformed role so far would you say within Anthropic that's most different from how was like a couple years ago, let's say?

**Fiona Fung** (01:00:23):
It's all the coding adjacent roles are shifting. I know you were chatting with Kat, I think PM is also transformed quite a bit because PM are no longer bottlenecked if they have an idea waiting on engineering bandwidth. So that's kind of like the next role that I saw on shift. Actually, our PMs have also helped us roll up sleeves and help shift some features when there was something we wanted to do, and an engineer wasn't able to. So I think it's all the coding adjacent roles are starting to shift, but I think that's where again, the verification is important because when you have more different disciplines checking in, how do we make sure everybody has higher confidence? I also think we need to do more to keep automating these other portions of the workflows. For sure, we focus a lot on coding, but next when you think about design or data science, those are starting to be the next areas that I think are good opportunities for us to see how we can start improving the experiences there as well.

**Lenny Rachitsky** (01:01:26):
Yeah, speaking of data science, I have a data science friend and he was just saying how data science is so different now where now most of their job is people doing their own not amazing data science work using AI, and then just showing it to the data scientists, "Here, here's the analysis I did. Can you just make sure it's right?" And half the time it's not right, and so the job is just a whole different job now instead of doing the work that they thought they wanted to do. Now it's like, "All right, I'm just reviewing all this AI data science all the time. What the hell?" Along the lines, coming back to just how your team operates and how things are changing, let me see if something comes with this question. What should an engineering manager expect from their team now versus a couple of years ago, what's a normal, I don't know, baseline expectation of how things should work other than just we're shipping faster, is there anything else?

**Fiona Fung** (01:02:20):
Oh, interesting. Well, definitely I think most commits are Claude assisted, and so that was a shift. I think I kind of mentioned we have Slack channels with all the feedback and also our dashboards that we have gave to Claude. I think having engineers keep building that stronger product sense muscle is I think also another, and I think that in general helps with these really strong-minded product engineers. I would say more of these roles that were traditionally non-engineering, you do now see engineers, and sometimes you're just blocked by waiting for a cross-functional partner. I think there's less of those blocks now just because the models are able to augment additional capabilities that you may not have as an engineer.

**Lenny Rachitsky** (01:03:12):
So it's kind of interesting. It's both directions. Engineers becoming more product-minded and responsible for the quality and success of a product, and then everybody becoming an engineer more and more.

**Fiona Fung** (01:03:23):
Yeah, that's right. Yeah, it's all blurring.

**Lenny Rachitsky** (01:03:26):
Yeah, I forget who said this, but there's this like, " What is a role anymore?" And this guy said that it's like, "What's the average of what you do? What's the highest percentage of what you do, and that's kind of your role now," whatever it is to be.

**Fiona Fung** (01:03:40):
Yeah.

**Lenny Rachitsky** (01:03:41):
Oh, man. I want to come back to your point about obsession with the product. Living, breathing, the product, dogfooding. I talked to a bunch of people that work with you about you, and that's the thing that came up most, just your obsession with living and breathing the product, using the product constantly, whatever it is you're building, this idea of dogfooding. Talk about just why that is so important, why that's something you instill within your teams and reports.

**Fiona Fung** (01:04:06):
Oh, love it. Yeah, I think it's really and this has worked for me. It's just been a really good way for me to keep a pulse. Anytime you build product, there's a dream. You're really hoping to enable an experience or making an experience better. So I think that helps me keep really close to the pulse. I also think, and maybe for sure on Visual Studio, that was where I got this love of it, but it's interesting because even Marketplace, I remembered once in a while, even after I left the team actually, one time I had a MacBook Air I wanted to sell. I'm like, "Oh, I haven't sold anything on Marketplace." And I could not believe it the minute I put it up for sale, a seller or buyer tried to scam me, and it was an interesting new scam vector I didn't detect, but that goes to, again, people will use your products in ways that you may not expect.

**Fiona Fung** (01:05:04):
And so especially as leaders or even anyone on the team, we all have different life, actually, it's funny when I was supporting the VR and AR teams, somehow how I used VR, the setup, I would always be able to find these really weird floor height issues. So that ended up being a, "Oh, I'm going to help us," because somehow I got a good repro environment, and so I think it's number one, that's how you keep your pulse on the product that you're building and don't get too lost in metrics and dashboards only, or presentations.

**Lenny Rachitsky** (01:05:40):
I think that's such an important point you're saying there that I just want to make sure people here is just like there's always this idea of anecdotal evidence and just examples versus the data, and what you're saying here is as a product leader, as an engineer leader, you've found a lot of success in the anecdotes, the specific little one-offs that you experience as a user versus obsessing with the data only.

**Fiona Fung** (01:06:02):
Yeah, and actually sometimes it's also how I've been able to most effectively help the team. So for example, the last team I was on, I was leading a VR team and because back then I have not checked in any code into that code base just because I was really worried about messing up the operating system, but what was a gap? We were doing a lot of polish fixes and I'm like, "Hey, you know what? I'll use my job fitting time to actually vet how the experience looks." And so that was also probably a way that I felt I could still meaningfully contribute to help hold the quality bar for the team, and then like I say, every team member usually always really appreciates because I think as a lead leader, you're supporting folks on team that outside of metrics and everything, everybody really wants to make sure their work matters and just making sure that leaders use your product. I think folks feel the leaders, and then remain really engaged and not too distanced.

**Lenny Rachitsky** (01:07:06):
And this connects a lot with your point that engineers need to become more product minded, that engineers need to become more PM-y, but this is like as an engineer, this is one way to do it. Use the product constantly and that'll help you understand what is missing in the product as a user because you're just using it.

**Fiona Fung** (01:07:21):
That's right, and I would say if you're leading a team where it's really hard for you to use a product, then meet with customers. Whatever that other avenue is, I think that's also been really important too. Every time I've done customer visits, I always learn something new. Actually, I remember that was Facebook Marketplace, we're trying to launch to Latin America and so we were testing in Chile, and I remembered it just wasn't doing as well as the other regions. Everything else, we've tried it and then I remember, I'm like, oh yeah, and we had a really small research trip where I went to Chile and I remember getting us a whole bunch of Android phones for us. It was very small crew, like just three of us, and upon landing and upon me opening up these Android phones and I'm like, ah, the LTE connection was much slower than what we were used to in the US.

**Fiona Fung** (01:08:09):
So I'm like, "Oh, the Marketplace feed didn't even load very well on these low LTE situations." What a growth block that you can't even load, but again, that's why it's so important to always listen to customer feedback and get that fast feedback loop.

**Lenny Rachitsky** (01:08:25):
I think it was Jeff Bezos that said if you have data and you have an anecdote, trust anecdote over the data, surprisingly and that's a great example. Okay, just a couple more questions. One is in your talk, you had this really interesting slide at the end of what questions you're kind of thinking about right now that you haven't figured out how to solve with how much it's changing. I'm going to read the three. I'm curious just like if it's still these three, if there's anything else like current problems we need to figure out that we haven't solved in how we operate. What you shared in your talk was do we still need separate iOS and Android organizations? How far do you push fully on automated reviews, and with role blurring, how do you ensure everyone's equally productive? Still problems, is there anything else that you're thinking about like, "Okay, we need to crack this. We haven't figured this out."

**Fiona Fung** (01:09:15):
You know the iOS Android one, I think and actually it's funny because speaking of the deep expertise, we definitely feel that it's really important to still bring on folks with those expertise, but we probably don't need as large because people are flexing. So it's again, making sure we have the Android and iOS experts, but then less of the larger kind of like mobile art one per, but again, that's still a balance that we're trying to figure out, do we have the right and enough expertise? Sorry, what was the second one?

**Lenny Rachitsky** (01:09:52):
Oh yeah, it is how far do you push fully, automated review?

**Fiona Fung** (01:09:57):
Yes. Actually, well, this is a fun one with the content design check. I think we're looking for across all of it, how do you actually get what good looks like? And so actually the verification is still one that I think, and that's kind of like the second and the third that I think there's a lot more opportunities there for us, but the how far to push, I think looking at where we think experts still matters and then also again, have to keep asking ourselves, okay, is there a way to leverage that expertise to also automate? I think looking across the whole end-to-end experience, making sure we're not missing, I think we come at it from an engineering standpoint, but making sure on experiences how we think about those other areas. I think there's definitely still more that we can do there.

**Lenny Rachitsky** (01:10:44):
Basically, how do you set up a verification that the experience is what you wanted it to be?

**Fiona Fung** (01:10:51):
Exactly, and I think that one is still a hard one to crack because you kind of mentioned evaluations because some of it for sure is accuracy, but it's also that experience. So that's something that we're still kind of thinking through.

**Lenny Rachitsky** (01:11:03):
Awesome. Is there anything else that's like, "Oh, this has changed recently. We got to figure out how to rethink the way we operate," or is this kind of the big ones?

**Fiona Fung** (01:11:11):
I think because with routines and everything being more async, I think there is starting to be a high load on our context switching because I even remember myself, I was like oh, I kicked off, and so I think that's probably another thing we have to think about whether for team members or users, how can we actually make the experience better to reduce that load? Because I do see the context switching load increasing.

**Lenny Rachitsky** (01:11:39):
If you have 20 agents running, there's just endless checking in and reviewing and you have to remember what you were doing there. It's like such an interesting world where the idea flow we talked about before, like engineers and most people, there's less of the just hours of flow, but now the agents can kind of just remind you, "Here's where you're at." The reset to switch almost is easier because you don't have to relearn everything. You don't have to reunderstand the code base and the architecture. You can kind of just like, "Okay, but here's what we're trying to do." It's kind of like both, got better, got worse.

**Fiona Fung** (01:12:12):
Well, it's interesting because I used to book out focus time, the focus time for coding because you want that dedicated, and then the whole context switching, and then it's interesting now that because I can context switch more with more async agents, I'm noticing I do actually have to go back and block a focus time for me to catch up on all the different async work that I've kicked off.

**Lenny Rachitsky** (01:12:32):
Yeah, do you have any thoughts on the solution there? Because that's hard just like people just want to do more and more, and just how do you do that without constantly context switching? It's really hard and annoying.

**Fiona Fung** (01:12:43):
Yes, I agree.

**Lenny Rachitsky** (01:12:45):
Open question.

**Fiona Fung** (01:12:45):
Definitely I haven't cracked it yet.

**Lenny Rachitsky** (01:12:48):
So interesting. Okay, there's a question I thought of as we were talking that I'm so excited to hear your answer on that. I wasn't even planning to ask this, but it's so important these days, which is just like engineering jobs and hiring. So interesting that you would think AI would make engineers less necessary. On the other hand, it feels like you guys are hiring engineers like crazy, OpenAI's hiring engineers like crazy, just there's so much demand for engineers. Where do you think this goes? What do you think about just the future of the end role? And this big question, but just thoughts?

**Fiona Fung** (01:13:21):
Actually, I'll share some vulnerability here. Speaking of big open questions, I really do think how we grow the next generation just because how you and me got to our engineering path is just so different. It's almost like okay, now when you graduate from school, it's like, "How do you fast-forward?" But the important thing to me, but still understand that double click I talked about to the layer of a need, but that is a big question I have, and I wish I have the answers, but I wonder if it's for software engineering, it's almost like you go more towards a fellowship or apprenticeship program. I know it's odd because technically we have internships that would, but those were kind of like three months and little projects, but I do wonder, and I wish I have a crystal ball here, but it's like how do you almost cram, and maybe it won't matter, but some of the life experiences that we all got, how do you actually enable us to teach that to the next generation of builders?

**Lenny Rachitsky** (01:14:28):
Right, if you don't have to ever look at code, what's the incentive for a new software engineer to truly understand how infrastructure works and memory allocation, all these things that are kind of foundational?

**Fiona Fung** (01:14:42):
And it's interesting, maybe the models will get good enough that it doesn't matter.

**Lenny Rachitsky** (01:14:46):
You don't have to worry about it.

**Fiona Fung** (01:14:48):
But I do think there's something about that double click because I think that's where there might be an opportunity to improve the product or the system, but figuring out how to learn that not necessarily by years of-

**Lenny Rachitsky** (01:15:01):
Of typing code.

**Fiona Fung** (01:15:03):
Yeah.

**Fiona Fung** (01:15:00):
Like years of-

**Lenny Rachitsky** (01:15:01):
Of typing code.

**Fiona Fung** (01:15:03):
Yeah.

**Lenny Rachitsky** (01:15:04):
Yeah. Somebody's got to have to understand code at some level. It's like some Cobalt engineer they have to pull out of that retirement one day. Do you remember how to write Python?

**Fiona Fung** (01:15:13):
You know actually what's really fun, one of my previous managers, he started software engineer when it was punch cards and it's so fabulous. He's been messaging me everything he's been building with Claude Code and I'm like, wow, what a career that you go from. He's really seeing this whole change. So maybe I think for us to think about is when I think about his career, how he got started with punch cards was also totally, totally different than now. I think it'll be interesting for us to see what remains important and then what changes in terms of importance and then it's like how do you gain... I have a theory, maybe that's what is important will shift over time. And then how do you build the proficiency in doing that?

**Lenny Rachitsky** (01:16:03):
Yeah, just learn the things that really matter. The argument that I constantly hear is just like it's a new level of abstraction, just like assembly and binary. It just keeps going up and up. And now, okay, we don't need to actually look at the code. It's like a new layer of traction, prompts and Claude's thinking messages.

**Fiona Fung** (01:16:20):
Yeah. And it's maybe like, okay, what is an interesting problem and what's the prioritization for experience to build? It's interesting. Yeah. And then when you build things, how do you know it's actually resonating and it's doing what you intended?

**Lenny Rachitsky** (01:16:34):
And it's good. Yeah. Are we just building a bunch of slop here or is this actually this architecture that will work? I think the advantage though for young people is it's so much easier to just lean in and work in this new way versus being stuck in the way that things used to be. It's rare. It's amazing how many longtime engineers like yourself have adapted and embraced this. It's like so hard to just change everything. Okay, let's do it. Everything.

**Fiona Fung** (01:17:06):
Well, because the rate of change is also so fast. Actually, that was the one thing of, I remember the first time it was probably Sonnet 35 or 36 and I remembered it was still making some mistakes when I was doing things on the side. I'm like, "What are you doing?" And then what I noticed was some of the engineers that were resisting AI tooling, they're like, "Ah, but see, look at all of these." But then I think it was hard to understand of how the exponential rate of improvements. And maybe that's another interesting thing that I, myself, I'm learning too. There might've been something I tried to automate that Claude wasn't quite good enough. And then actually in the next model, oh, well, now it is good enough. So it's always also thinking about what may have not worked. It might be worth the time to revisit because that now might be a new capability.

**Lenny Rachitsky** (01:17:50):
Yeah. That comes up a lot on this podcast. Just build something that is almost working that is at the edge because once the model gets there, you'll be so far ahead of everybody else. Okay. Final question. You may have already answered this with what you just said, but what keeps you up at night?

**Fiona Fung** (01:18:07):
The thing that keeps me up at night is probably... It's how we... So we talked about Claude Code and Cowork team culture and the team culture is really important to me. It's the one team mentality and I share with folks. And by the way, culture is like a living, breathing thing. It's not just a poster you slap on a wall and it changes over time and it shows up in how we treat each other, how we're there for each other. And so the culture of the team is important to me because we are growing and since the culture shifts, making sure that maintaining the things are important, that we still really... It's really important for me to have diverse perspectives so then we can have good, healthy, open, honest, debates out in the open and we welcome those and what I call that one team mentality that when you get close to the finish line, look behind you and see is there some teams to help because we finish as a team.

**Fiona Fung** (01:19:02):
That's probably the thing that keeps me up at night. There's so many other hard problems, right? But I think maybe a lot of the other ones are product or engineering challenges that yes, we have dashboards or theories or hypothesis, but the culture is like a human aspect that is... I think that's the one that I always want to make sure that we're as we grow, we're still maintaining that culture because it is the fiber of the team. And when it starts drifting... I'm always worried if it drifts, are we catching it and having conversations as a team together to make sure we're all wanting the culture to grow in the right direction?

**Lenny Rachitsky** (01:19:49):
Yeah. I imagine everybody is struggling with this considering the pace of change and the phase of hiring, just like... Especially at a company like Anthropic that's in this crazy, the most unprecedented growth trajectory in history. I could see how that could be a challenge with so much change. So it makes sense. Even at Airbnb when I was there, that was quite a growth trajectory and that was nothing like what you guys are going through and that was a constant topic of conversation. How do we maintain the culture?

**Fiona Fung** (01:20:19):
Actually, I'm curious, what was your experience at BAB to maintain the culture as we're growing?

**Lenny Rachitsky** (01:20:24):
There's a couple of things. One is just what worked well is the founders being obsessed with it. Every all hands, every big meeting is just reminding of the culture and the value of the culture and what the values are. Just the founders top down being obsessed with it was a big part of it. You just couldn't have a meeting without that coming up as a thing. The other is a memory I always come back to is we had Cheryl Sandberg's PKMETA come do a fireside chat and somebody asked her just, how do you maintain culture as you scale? Because we're just growing so fast and it's so hard to deal with all this change and culture and all these new people. And her advice was, "This is actually a problem you want to have because this means you're growing and doing well and this is normal versus nothing will change if you're doing badly."

**Lenny Rachitsky** (01:21:18):
That's a much worse situation when you're not growing and you're not hiring like crazy. That's a much worse situation that will cause even more pain and suffering. So this is a good problem you're dealing with is her advice, which has always stuck with me.

**Fiona Fung** (01:21:32):
Oh, that's great. It's interesting hearing you talk, I think one of the important things to Claude Code and Cowork team is whether ICs or managers, but this is a thing I especially as for managers on the team is really important that we all talk about for sure what's going out, but also just be open about what's not going well because then if we can actually have a conversation of what's not going well, that's how we can actually go ahead and address it. Speaking of what keeps me up in that, my nightmare is, especially if someone's in a manager position and I'm like, "Hey, how are things going? Everything's fine." I'm like, "Oh, my gosh, I'm not doing fine. I know this thing's..." You know how there was this meme of the dog drinking a cup of coffee in a room that's on fire? That is my nightmare.

**Fiona Fung** (01:22:17):
So that's actually a discussion I have with a lot of folks on the team by special managers, especially when they first join up, "Hey, let's always have these open conversations so that we can solve problems together."

**Lenny Rachitsky** (01:22:28):
I imagine this is something a lot of people struggle with seeing so many people around them doing super well, at least seemingly doing well, everything's going great, I'm growing, this awesome company or just like everything, it's like hard to actually be honest and say, "It's not going great. I'm struggling here. I'm falling behind," because everyone around you is just like on the surface feeling like they're killing it.

**Lenny Rachitsky** (01:22:53):
Before we get to our very exciting lightning round, is there anything else that you either want to leave listeners with, anything else that we didn't cover? Anything else that's important that you wanted to share?

**Fiona Fung** (01:23:03):
Maybe one thing is just a suggestion because we talked about how can Claude do automate. One other thing that's really big on Claude Code and Cowork team culture is explicit permission to kill processes that no longer serve us. And so maybe a suggestion is for anyone working on a team or leading teams, what's one process that you either dread doing or is really highly noisy or is really expensive in terms of just a lot of... Or something that's just very manual, pick one thing and first ask is it still having its purpose? For example, when even our planning... Actually, that was my own big first learning when I first joined Claude Code. I'm like, "Hey, maybe we should do a six-month roadmap doc, but we're going to do it super lightweight because I don't want to waste a lot of time planning." And I felt we did a really lightweight process, but that was such a good learning for me because the exercise was good to kickstart conversations and enter aligned, but three months into it, I'm like, "Wait, have we still referenced stuff?" Because so much has changed.

**Fiona Fung** (01:24:10):
So that was also something I... And so that was also something I changed that I myself brought in thinking, "Hey, maybe this will help." So always be open to learning and always ask yourself whatever process you have, is it still serving its purpose just because the field is changing so fast?

**Lenny Rachitsky** (01:24:26):
I love that advice. I got to follow up on this real quick. How do you think about planning now? Do you do any planning? Is it just a month long roadmap? What's the simple way to explain where you're at with that?

**Fiona Fung** (01:24:37):
Yeah, I call it JIT planning now, just in time planning. So it is around, because yeah, I think six months was too long. So now for sure some projects will take more than a month, but we try to do a month planning, really lightweight. Actually, there's not even dogs. It's really just us aligning on a little spreadsheet of what we think is important. But even that one, I'm thinking through, hey, every week we should probably still keep what we're trying is here are the month's priorities and we're going to try it out, but I have a feeling like every week we'll probably want to do really quick like, "Hey, just to check, yep, this is still this month's priorities, good." But now we've shrunk it to JIT monthly planning.

**Lenny Rachitsky** (01:25:17):
So it's monthly meaning for the next month, here's a little sheet/Excel spreadsheet of what we're planning to do for the next month and then every week check-in is this still what we're planning to do for the next month?

**Fiona Fung** (01:25:29):
Yeah.

**Lenny Rachitsky** (01:25:29):
So cool.

**Fiona Fung** (01:25:30):
Very, very weird. But even that one, I'm also still feeling, how can we even automate this more? Because I never want it to be feeling like attacked when someone has to update the spreadsheet. So this is actually, just yesterday we're chatting, "Hey, how can we actually automate this?" Speaking to that question, always ask yourselves, "Can we actually automate this better?"

**Lenny Rachitsky** (01:25:50):
My PM brain is like, "How could you not do something like that? Okay, here's what we're thinking for the next month. Let's just check it once a week, make sure this is..." It's hard to imagine that not happening and you don't have a lot of item on this spreadsheet is what I'm hearing also.

**Fiona Fung** (01:26:05):
Yeah, we really try focus. So we'll share, here's what we think are the highest priorities. And again, for that agency, given the priorities, then everybody's their kind of item for how they think addresses those priorities.

**Lenny Rachitsky** (01:26:19):
Is there anything that's like, here's for the next six months bigger bet kind of stuff or is it just let's just think one month ahead?

**Fiona Fung** (01:26:26):
So usually definitely there's themes of where we think the work. And actually the whole team will bring everyone together every six months. So there will usually kick off some themes, but then it's really the making sure we keep the pulse of what... Because again, even those themes change so fast when the landscape changes.

**Lenny Rachitsky** (01:26:49):
All right, let's pull out the spreadsheet. Let's take a look. Oh, man, man, this whole podcast could have been just talking about this planning stuff that you do. Okay. I'm going to have to find someone else to talk about this because this is so interesting just how you all plan. Yeah. Okay. Well, Fiona, with that, we reached our very exciting lightning round. I've got five questions for you. Are you ready?

**Fiona Fung** (01:27:10):
Ready.

**Lenny Rachitsky** (01:27:11):
Okay. First question, what are two or three books that you find yourself recommending most to other people?

**Fiona Fung** (01:27:17):
Ooh, I will say for fiction, actually two authors I recommend to everyone, Margaret Atwood and Haruki Murakami. I mean, I grew up in Canada, so I read a lot of that when growing up, but her books are fascinating because it's almost like speculative fiction of you can squint and say, "Okay, could this actually happen to a society?" So I love her take on speculative fiction and Murakami, I love his magical realism style. But then the one book, so there are authors, but the one book I always recommend to everyone to read at least once a year, The Little Prince, I'm sure we probably all read it at some point in our lives, but I think I read it at least once a year just to remind me to think about what's truly important.

**Lenny Rachitsky** (01:28:17):
Wow, that hasn't come up a bunch. Okay. I love it. Favorite recent movie or TV show you have really enjoyed?

**Fiona Fung** (01:28:25):
I haven't watched TV shows.

**Lenny Rachitsky** (01:28:27):
That's very common across Anthropic people I have on the podcast. Tell me theme.

**Fiona Fung** (01:28:32):
But I will share with you what I always have downloaded on my phone so that if I'm on the airplane... So there's three movies that I'll always have on my phone because I think they're just so fun to watch if I have time. One is Emily. It's this French movie that, oh, my gosh, all of these movies are going to be very old, by the way. It's going to be like vintage movies, but I loved Emily, super whimsical. So really highly recommend it to anyone that haven't seen it. If you remember, I told you I was going on a... I thought I was going to be a visual artist. So when I was 16, my high school, we took a trip, a high school trip to Paris and I have so many memories of that and Emily really captures the magic I felt at Paris.

**Fiona Fung** (01:29:18):
And the other two are Ghibli films. I love Spirited Away. I just love that story. I just love everything about Spirited Away. It's probably one of my favorite Ghibli films. And then the third one is another Ghibli film, Nausicaä Valley of the Wind. And I think about this one quite a bit because if anyone asks me, "Hey, how did you think about all these leadership traits?" I think I watched that movie probably when I was eight or nine and the heroin Nausicaä and seeing how she leads just left such a thumbprint in my heart, I guess you could say, that probably Nausicaä has inspired me to a lot in a lot of my different leadership principles.

**Lenny Rachitsky** (01:30:08):
Wow. What is that book called again?

**Fiona Fung** (01:30:11):
The movie's called Nausicaä Valley of the Wind, but it was actually based on a manga.

**Lenny Rachitsky** (01:30:15):
Valley of the Wind. So it's like high output management and you grow Valley of the Wind, Nausicaä.

**Fiona Fung** (01:30:21):
That's right.

**Lenny Rachitsky** (01:30:21):
Two top management books. So cool. Okay. Do you have a favorite product you've recently discovered that you really love? Could be an app, could be clothing, could be a gadget, could be kitchen equipment.

**Fiona Fung** (01:30:33):
I'll share the product that I'm reminded of how much has made a difference in my life recently because I've been just traveling a little bit and I like to travel really light so I use whatever shampoo and conditioner the hotel gives and I forgot that... So the product that I actually have one of their hand, I promise is it's not an infomercial, but Sweet Sisters Body Care, it's a local business on Whidbey Island, but the reason why their product has made such a big difference in my life, it's a full line of organic, hair, body, skincare. But a few years ago, I started getting this rash on my nose right here that was really painful, actually bleeding. And I could not for the life of me figure out how to stop it. I tried not using any lotions. I cut everything on my face and it was still really hurting. And then somebody says, "What's the shampoo you're using?" I'm like, "It's the same shampoo I've used since I was a teenager." And they're like, "Maybe your body has now..." And it's like generic brand shampoo they get anywhere.

**Fiona Fung** (01:31:39):
And they said, "May your bodies just start developing an allergy to it because of the chemicals in it that..." I'm like, "What?" And so anyways, this was an organic shampoo that I found. Lo and behold, I use our shampoo because you don't think that when you wash your hair, it actually then goes over to the rest of your body. So since then, I've switched everything that I used to be Sweet Sisters, but I'm recently reminded of how important this is because after a week of hotel shampoo, I actually started having some skin reactions again. I'm like, "Ah, maybe I should get travel size bottles that I could bring with me."

**Lenny Rachitsky** (01:32:18):
This is an awesome pick. I love local business picks, even big bonus points for that. And by the way, this travel you're doing, just for folks that may not know this, there's these Code with Claude events that are happening all over the world. I went to the one in SF, there's one in London, you're going to one in Tokyo. Is that the end of it or is there more after that?

**Fiona Fung** (01:32:36):
Tokyo is... So yeah, that's next week and that's the last leg of the trip.

**Lenny Rachitsky** (01:32:42):
Okay. And then probably more in the future. So cool. I love that that's happening. Okay, two more questions. Do you have a favorite life motto that you find yourself coming back to often in work or in life?

**Fiona Fung** (01:32:51):
Ooh. So in work, I really love to remind folks, keep it simple. What is the thing that you're really trying to do well and focus on that? Keep it simple because I think sometimes we could overthink. So it's always a good mantra to think about that. And then in life, probably in a world where you can be anything, be kind.

**Lenny Rachitsky** (01:33:14):
I love that one. We were at a Montessori school tour and that's what the teacher had up on the wall.

**Fiona Fung** (01:33:21):
We have so many things going on that you never know what's going on in someone else's life and that one small act of kindness can make the biggest difference. For me actually that was when... Do you remember COVID? We were all working from home during the COVID-

**Lenny Rachitsky** (01:33:37):
How could I forget?

**Fiona Fung** (01:33:40):
It's just always really struck with me because I was in these back to back meetings and one-on-ones are really important to me because actually that time is usually also really important for the other person. It's something that they've been looking to. They might have things discussed. I always really prioritize one-on-ones, but during that time, my grandmother wasn't doing well and she was in a home in Canada because of COVID I couldn't go visit and actually even my aunt and mom couldn't go visit and it was just very rare of if they have a helper that can help, we could do FaceTime, but you never know what time that is going to be because there's so many people that take care and all of a sudden I get a message from my aunt going, "Grandma can FaceTime at 12:00 PM today." I'm like, "Oh, no, there's this one-on-one that I've been mean to have." And I just messaged my report to say, "I'm really, really sorry. It's the last minute. Is it okay to..."

**Fiona Fung** (01:34:36):
And I know now when I say it doesn't seem like it's a big thing because it's like... But to me, it's always really important to keep. But he was like, "Yeah, totally. No problem at all." And for me, that was just a small after kindness and he totally didn't make it into big deal, but that made the biggest difference to me that I got to say hi to my grandmother on FaceTime.

**Lenny Rachitsky** (01:34:56):
I love that. Okay, final question. So Boris Chernyy, when I asked him about you, when he had this interesting insight where he said in very important meetings, you can often hear Fiona, you can hear the click-clack of Fiona knitting in the background. Maybe talk about just what's going on there and what are a couple of things you knitted recently.

**Fiona Fung** (01:35:18):
Oh, my gosh. Well, I knitted this top recently.

**Lenny Rachitsky** (01:35:22):
You make your own clothing. Unreal. This is very meta for Claude Code building itself.

**Fiona Fung** (01:35:31):
Actually, there's this whole fun thing I think between knitting and programming because it's like two stitches knit and a pearl. So zero and one. And anyway, so many concepts of stacks and queues you actually could... I'm kind of a compiler. I'm kind of generating an executable when I knit. Yeah, actually it was my grandma that taught me to knit when I was eight. I mentioned her and I going to that yarn shop. And so every time I knit, I think of her, but I always like to multitask as you could see like, yeah, kick off multiple agents. And so anytime I'm sitting and because I practice enough and got proficient at it, I don't have to look at what I'm doing. So it's almost like how you know sometimes people have like fidget spinners and such. Knitting is just... So anytime I'm sitting still, I'm like, "Oh, this is time to generate more knitting executable." Because I got so much yarn that if I don't do this, I might have a slight yarn addiction problem.

**Lenny Rachitsky** (01:36:28):
I love this. When I asked Boris what he would do when AGI hits, when we don't have to work, he said he's going to make me so... I'm guessing your answer would be just knit and make beautiful clothing.

**Fiona Fung** (01:36:38):
Oh, my gosh. My dream is to actually open up a yarn store in my grandmother's name-

**Lenny Rachitsky** (01:36:42):
There we go.

**Fiona Fung** (01:36:43):
...and create that community.

**Lenny Rachitsky** (01:36:44):
Oh, wow. And then Cowork would help out you automate everything.

**Fiona Fung** (01:36:47):
That's great. Especially invoicing.

**Lenny Rachitsky** (01:36:50):
Oh, my God. Fiona, you're awesome. It's just incredible the work that you and your team are doing, just changing the world in such profound ways and it's clear why it's growing so fast. So good job. Good job over there.

**Lenny Rachitsky** (01:37:04):
Thank you for making time for this.

**Fiona Fung** (01:37:07):
Well, I'm just really honestly lucky and humble that I get to work with such an amazing team. I know how lucky I am and I'm so grateful. But thanks a lot for having me on the podcast as well. This was a lot of fun.

**Lenny Rachitsky** (01:37:20):
Two final questions. Where can folks find you online if you are online if they want to follow up on anything and how can listeners be useful to you?

**Fiona Fung** (01:37:26):
Ooh, so definitely I'm on LinkedIn and I'm sure most people have shared this already, but would love feedback of what's going well, what's not going well, also any latent demand that you are all using that might be interesting use cases. I had a friend message me recently to go, "Oh, I'm using Claude to help me generate a building plan for my shed." And he actually showed me his whole shed, which was cool. So would love to hear about that. And then yeah, maybe also we talked about reaching out across. So there's someone, whether a small business that you love or someone that you feel like hasn't... As all the listeners are super AI pilled, maybe take a time to hold somebody's hand to show what AI might be able to help them with.

**Lenny Rachitsky** (01:38:11):
Such a good one. That is such a good answer to this question, especially coming from you. Fiona, this was awesome. Thank you so much for being here.

**Fiona Fung** (01:38:19):
Thanks so much for having me, Lenny.

**Lenny Rachitsky** (01:38:20):
Bye everyone.

**Lenny Rachitsky** (01:38:22):
Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
