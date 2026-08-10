---
title: "Anthropic’s first technical PM on token maxing, the jagged edge, and living in the future | Dianne Penn"
date: "2026-07-26"
type: "podcast"
guest: "Dianne Penn"
post_url: "https://www.lennysnewsletter.com/p/anthropics-first-technical-pm-on"
description: "Token maxing, the jagged edge, and living in the future, covering AI product work, engineering tradeoffs, and team leadership."
word_count: 15298
---

**Diane Penn** (00:00:00):
In 2023 when I started, nobody said Anthropic and Claude and coding in the same sentence.

**Lenny** (00:00:06):
I want to go back to the beginning of Anthropic. I remember feeling, "Man, these guys have no chance. OpenAI is so far ahead."

**Diane Penn** (00:00:14):
By the time I saw people were starting to use these models, not just for code autocomplete, but actually writing long-form code. Is that an opportunity for us to train Opus 3 to be better at? That was the inflection.

**Lenny** (00:00:26):
I always think about Opus 4.5 a year later during winter break when everyone was home able to code.

**Diane Penn** (00:00:31):
What was magical about Opus 4.5 is we also now not just had a model, but a vehicle, a great product experience like Claude Code. Opus 4.5 wouldn't have had that moment without a product like Claude Code and Claude Code wouldn't have had that type of adoption accelerated without Opus 4.5.

**Lenny** (00:00:50):
I want to talk about how the product role is changing.

**Diane Penn** (00:00:53):
For my team, the way to drive user value is to figure out the right user feedback. The evals, we actually have a saying on the team of evals are the new PRDs.

**Lenny** (00:01:02):
Something Garry Tan's been talking about. If you are willing to spend $100,000 a year right now in tokens, you are living the way somebody in 2028 is going to live.

**Diane Penn** (00:01:10):
You have to sweat the tokens as much as you sweat the pixels. You have to be using the models to come up with good and great and better ideas, and there's no substitute for that.

**Lenny** (00:01:20):
People need to be more ambitious with AI tools these days because they're just capable of so much.

**Diane Penn** (00:01:26):
One thing I ask the team is let's say Claude 8 comes around. What changes in what users do? What does that mean for how you're building today?

**Lenny** (00:01:36):
Today, my guest is Diane Penn, head of product for the AI research and Labs teams at Anthropic. She joined Anthropic as the first technical product manager over three years ago, which is a lifetime in AI time. When the product team was just five engineers, she's helped ship every model at Anthropic from Claude 2 through Fable. She's also helped incubate and launch Claude Code, MCP, skills, Claude Design, and also core capabilities like computer use, tool use, and reasoning.

**Diane Penn** (00:02:41):
Thank you, Lenny. It's so nice to see you again.

**Lenny** (00:02:43):
I want to go back to the beginning of Anthropic, the early days. I remember when Anthropic first launched, this was, I don't know, the first model when it launched years ago, three years ago, something like that.

**Diane Penn** (00:02:56):
It works.

**Lenny** (00:02:56):
Three years. I remember just feeling that, man, these guys have no chance. OpenAI is so far ahead. They're just like, what are they thinking? How is this possible? OpenAI is one. It's too late. Things are very different now. The latest number I saw was Anthropic was making, I don't know, $50 billion in ARR. That's what companies used to go public at. Very successful companies went public at 50 billion in valuation. Anthropic reportedly is making that every single year. You joined as one of the earliest PMs. There were something like five engineers when you joined. The model hadn't even launched when you joined. What was it like in those early days of Anthropic? What's something that might surprise people about what it was like at the beginning?

**Diane Penn** (00:03:44):
I think a big part of what's made Anthropic today actually has been very much the core of even the early days. So I joined in 2023. Like you said, we had five product engineers. There was one engineer for the entirety of our API business, if you believe. And I think a big portion of it was the culture was really strong. And I think this is something I emphasize for folks who are interested in the company, really do walk the walk of the mission and the culture and the values. And the energy was very much like a startup.

**Diane Penn** (00:04:23):
I think you're right, we were very much trying to find our identity in the early years. I think there's one piece around the technology, but how does that technology bring value to users, bring value to society, and what could it possibly be? And I think the early years were us exploring that in different ways. We did start with Claude.ai, another chatbot, chat assistant, and evolving into things like tool use. I think one of the moments where really we started to get into our groove was shipping things like Golden Gate Claude. I don't know if you remember that.

**Lenny** (00:05:02):
No.

**Diane Penn** (00:05:03):
So this was actually up for about 24 hours or so. We had just published one of our early interpretability research in early 2024. And one of the examples was essentially you could have what's called features of the model within the layers, which express certain types of thematics. So one of the themes that the researchers was able to identify was, let's say, bullet point writing. Another one was people and places. And one that really came up frequently that resonated was the Golden Gate Bridge. And so when you actually essentially dialed up that feature, Claude would obsess about the Golden Gate Bridge. So meaning in every one of its responses, it would come back and talk about the Golden Gate Bridge.

**Diane Penn** (00:05:54):
So if you said like, "Give me a recipe for making spaghetti," it would say, " Here is a recipe and the orange color is just like international red that the Golden Gate Bridge looked like." And so it was really quirky. And we very much wanted to, in that situation, just bring it to the masses and bring it to people who were starting to use Claude. And so the entire experience actually we spun up on our Claude.ai website within 24 hours. And that took engineering, product, design, our research teams all working together. And we were really, really proud of it. I think it maybe reached only 2,000 people, to be honest. But it made us feel like, oh, we can actually bring new user experiences, showcase our research in a way that's different and authentic to us.

**Diane Penn** (00:06:52):
And in a very startup be like pace. That to me was one of those maybe hidden inflection points of we were starting to find our identity, that we could build products, build experiences that were different from what our competitors had seen, what was already out there. And I think that obviously Labs, Claude Code, et cetera, we then started to identify ourselves as would we actually think the world, how to think about AI, how to bring that closer to the public. But it was a very bottoms-up culture. And so that entire experience was very bottoms up. I see engineers, I see designers donating time to work on.

**Diane Penn** (00:07:35):
And so I like to always use that as an example of what the early days were like. But the culture and the values have very much, I think, stayed the same since those early days.

**Lenny** (00:07:46):
**Diane Penn** (00:09:11):
Definitely when we were training and testing Opus 3, I think that was the moment when the company... I think we were less than 200 people still at that point. And it was very clear that we needed and wanted to create a frontier model. And that was very important in terms of our ability to reach users, consumers, and to showcase our research. And we were looking for ways for also why should somebody choose Claude? And that was a core question. And that was a core question we were getting asked in the early days. And I think with Opus 3, it launched, I think, early March 2024, but there was many, many months of various teens across inference, across research, fine-tuning, pre-training that rallied at different points and towards a common goal.

**Diane Penn** (00:10:11):
And I think everybody that was involved was really proud. I remember being the PM, us, the research leads, myself, we were all in our... This was around December, so we were all at home in our various parents' homes and seeing everybody's background of their childhood room. And everybody was working really hard to figure out what are we training the model for? Is it showing up the right way? So I think that was really powerful in terms of just building a lot of trust. And a lot of our research leads have actually, from that time, are now leading reinforcement learning, leading our character work and lineman work.

**Diane Penn** (00:10:54):
So that foundational trust I think also helped us work well now with any of our production models across product and research because we were working just so much in the trenches together in the early days. And then I think there were things like identifying that coding was important. In 2023 when I started, nobody said Anthropic and Claude and coding in the same sentence. I think competitor models like GPT-4 at the time was used a bit for coding, but it was one of many use cases. And one thing that, for example, I saw was people are starting to use these models, not just for code, not just code autocomplete, but actually writing long-form code.

**Diane Penn** (00:11:43):
And is that an opportunity for us to train Opus 3 to be better at? And it ended up being a relatively smaller change from a training perspective, but it ended up helping us differentiate in the early days competitively for users and actually bring a lot of the very early Claude enthusiasts and developers because we were providing a value that they didn't really think was possible at the time.

**Lenny** (00:12:10):
It's so interesting you talk about Opus 3 like that's so long ago and just it's hard to think that was a big inflection. And so this is really interesting to hear that that was internally a big milestone. It almost feels like this confidence y'all built that, wow, we could really ship a frontier model, which is now today so not great if you compare it to what we've got today. What I always think about is Opus 4.5, which was an interestingly a year later also during winter break when everyone was home able to code. Was that another big milestone?

**Diane Penn** (00:12:38):
Yeah. Opus 4.5 was definitely another large moment. I think what was magical about Opus 4.5 is we also now not just had a model, but a vehicle, which is a great product experience like Claude Code. One thing we say a lot on the team is you need frontier products in order to have frontier models and for people to feel the magic of frontier models. And I think we felt the magic of Claude Code for many months before that.

**Diane Penn** (00:13:16):
But the fact that the model essentially got to a level of intelligence where at a very broad level, users can experience both frontier intelligence in new use cases, allow it to run things end to end in agentic manner, I think that was the inflection. It was actually both. I think Opus 4.5 wouldn't have had that moment without a product like Claude Code. And Claude Code, I think, wouldn't have had that type of adoption accelerated without Opus 4.5.

**Lenny** (00:13:50):
So speaking on this thread, Dario, interestingly, if you look back at all his predictions, he's just like, "Okay, coding's going to be solved 100% in a year." Something like that. He kept talking about how AI is going to do all our code. And I remember everyone being like, "There's no way. This is way too complicated. How is AI ever going to get really good at this very complex thing that humans do? No, this is going to be humans for a long time." He was completely right. Something else that he talks a lot about is this exponential. Now that we're on, that's the way he describes it, now we're like, we're on the exponential curve.

**Lenny** (00:14:25):
I remember not long ago, new models were being released and everybody was like, "Okay, we're done. There's no more upside. It's plateauing. It's over. There's no more room to grow." And now it's the opposite. Now we're inside. If you think about the curve of the exponential, we're inside of the exponential now, which by definition means every improvement is a massive jump because we're on that hockey stick part. What's it like just being on the inside of this crazy historic moment when AI is improving so fast, so much is being unlocked? What is it like and how should people prepare for the coming acceleration of more and more improvement from AI?

**Diane Penn** (00:15:05):
One thing I like to say on the team is most of us weren't actively working yet when the internet transitioned from this novelty to something that everyone can use. And it feels like that's just taking humans... I think analogies are helpful. And so the analogy of that is I think a couple of things. Number one is adaptability becomes very important. I think we have evals, we have on the safety side, safety testing, red teaming on the capabilities and product side, new prototypes, products like Claude Code, Tag and others. But it's very hard to predict the exact moment or the exact model.

**Diane Penn** (00:15:54):
And so the adaptability of when you're faced with new information, how do you then make better decisions versus keeping the same plan? And so that agility is really important. I think another piece is with that, how do you actually be thinking very first principles and reason through what's next? What's the so what? How do we invest in new products? How do we invest in explaining the differences to users? So a lot of the experiences I think of being in that exponential is that pace, understanding how you operate and make better decisions, and then applying that first principle's thinking to then do something that maybe we pull up a plan that we're expecting a few months from now, but now the model can actually do and work on and actually bring that to users.

**Diane Penn** (00:16:51):
So this is things like co-work, skills, tag. It's a very positive self-enforcing loop. And I think a big part of it also is just having the trust in each other, making sure we're thinking through the right decision making. We're bringing folks along. Some teams might see the exponential feel it faster than others. So how do we have the grace to bring the organization, the growing organization and company along on that?

**Lenny** (00:17:23):
So what I'm hearing here is you almost don't know what will be possible with every model release. And so the important things to focus on is being adaptable as things emerge. To your point, the product itself has to catch up to what is possible. To your point again, just like it can do so much, but people may not understand how to do it and may not be able to do it. So the product making it easy and even just telling you, here's something you could do feels like an important part. Is that roughly what you're describing?

**Diane Penn** (00:17:53):
I think so. I think there's some really interesting graphs in the original scaling law papers. And I think folks are very familiar with the scaling loss in the lens of as you add in more compute and data, what's called loss, AKA the loss from next token prediction goes down. And so it's a very smooth linear curve of the models get more intelligent as you scale them up. What's actually also interesting in that paper is there are these very different emerging capability graphs. And so for example, as you add in more data and you train the models with more compute, you essentially see these actually discontinuous emerging capabilities jump.

**Diane Penn** (00:18:38):
So the models go from one plus one being a thing that it can't calculate to a thing that it could reliably calculate. And so these emerging capabilities, this some nature of predictability is not necessarily everyone knows the exact moment. You need the evals to be able to assess that has actually always been a part of how this technology works. And also what makes things like safety harder. Because unless you have the evals, unless you have the systems to test, these jumps might actually happen and you don't know.

**Lenny** (00:19:16):
That's so interesting that you may have developed this AI brain that can do something you're not even aware of. And so part of the job is just uncovering, "Wow, we just got really good at this thing. What can we do with that?"

**Diane Penn** (00:19:27):
I think there's product overhang and user overhang, to maybe put it in our PM language, even on today's models. And I think there's a lot that we could be exploring on our current opuses and definitely with Fable, for example. And that discovery is actually another part of what's been in the early days of Anthropic's DNA. And I think it's also continuing to be a big part of how we operate in product, in Labs and across research.

**Lenny** (00:20:03):
This makes me think about something Garry Tan's been talking about, president of YC, I don't know what his title is. He had this interesting point that if you are willing to spend $100,000 a year right now in tokens, you are living the way somebody in 2028 is going to live. Because by then it'll be really cheap. Everyone can work this way. But there's this alpha opportunity right now to just live in the future, go crazy on token spend. And so there's a big opportunity for people to learn what the future's like and also just build much faster. Thoughts on this idea and the value of token maxing, let's call it.

**Diane Penn** (00:20:37):
Yeah. I think I take more of a almost product lens. It's almost like token spin is more the input. And really the output is what you described of experimentation. And I think if we were orienting goals around experimentation, I feel like that might be the better framing of the outcomes. And therefore there might be different ways of achieving that outcome. I will say internally, some of the most creative thinkers, the best prototypers do spend a lot of time with Claude, with every new version of a research model that we have.

**Diane Penn** (00:21:14):
And so there is something around you have to be using the models to then come up with good, then great, then better ideas. And there's no substitute for that. It's very hard to come up with a perfect strategy without touching the technology when it's moving this quickly. At the same time, I think there's other things that we could be doing. So one thing that we do a lot is actually working in public internally within Anthropic. And so in the early days when we had less product surfaces, there was a Slack channel where everyone, almost the entire company was testing early versions of Claude and trying different use cases. People were not calling them use cases, but you might be asking it to edit an essay or to come up with the right way to send this email. They were all different use cases, but we all worked in public. And then what you would see magically is different users or different folks on the team coming up with an idea and then other people trying different variations of that idea. And then within maybe 10 or so requests, there was something magical or potentially in a use case that emerges. And I think there's a lot in not just individuals figuring out by themselves how to use this technology. I think we could be doing more to actually bring that communal discovery when we do experimentation. Experimentation is not always necessarily a individual sport.

**Lenny** (00:22:55):
It's so interesting. Yeah, this idea that we're not sure what this is capable of or what we could do with it. And it takes all this poking around and people trying things, hearing what other people are trying to figure out what's possible. Such an interesting, I don't know, technology. We're just like, okay, here's what... Oh, I figured out it could do this thing. What are you going to do with that?

**Diane Penn** (00:23:14):
I think in a broad theme we know. We know that the models could write great essays or could write long form writing, but individual pain points of what can you actually solve with that and bring it to a user level that people can use, I think is something that is more exploration or experimentation based.

**Lenny** (00:23:33):
So following this thread, you oversee product for the Labs team, which is extremely cool. We've had Ben Mann on the podcast, Mike Krieger, whom both work on Labs now. Talk about Labs. What is Labs? What's come out of Labs? Many people have heard of these things. And how do they work that enables them to create such innovative ideas outside of even the core Anthropic product team?

**Diane Penn** (00:23:58):
The thesis of Labs in many ways is identifying and pulling the thread on...

**Diane Penn** (00:24:00):
... in many ways is identifying and pulling the thread on the thread of discontinuous large bets that might not be in the core roadmap, and figuring out is there a there there? And also, what is the 10X, 100X, 1000X of the there there? And so for example, things like Claude Code, I think-

**Lenny** (00:24:26):
I've heard of it.

**Diane Penn** (00:24:29):
Things like Claude Code, things like skills, and most recently Claude Design, MCP. The thing that we really try to emphasize within the teams is, especially right now, there are so many things that could be built. What does it mean then to have a discontinuous bet? And I think one approach that we're taking this year is you can be very strongly held opinion about the theme or the area, and then more weakly held about the exact prototype. And so there's a culture of experimentation. There's a lot of the bottoms up engineers on the team are very self-enabled, self-driven to test out different ideas. And sometimes, we have a thesis, and it might not work yet, and so we then might revisit it in one to two model generations. And so this idea of these prototypes that actually end up just helping us learn, that's also valuable even if it doesn't lead to something immediately shipping. And so I think that allows the incubation and the charter of Labs to really accelerate and see around corners more broadly for Anthropic.

**Lenny** (00:25:44):
It's so funny to think about Labs within an Anthropic, which was already so innovative and creative and just shipping like crazy, that there's value to still creating a Labs team within Anthropic. What enables Labs to work as well as it has? Because you listed all these products and it's like, what else has Anthropic shipped? It feels like all the biggest wins almost. I'm sure there are many that I'm not thinking about right now. What's core to creating a successful Labs org within a larger company?

**Diane Penn** (00:26:12):
I think the team culture, similar to broadly at Anthropic, I think the team culture is very valuable. I think Ben sets an incredible vision and pushes people to think about the 10X, 100X of the idea. And the teams, the pods within Labs is small, sometimes these ideas start with one engineer. And I think sometimes when there's almost really large teams pursuing very ambiguous large ideas, you end up actually being slowed down because of that. So I think it's culture.

**Diane Penn** (00:26:56):
I think we actually also select for folks who actually want to do that zero to one experimentation. And it's not easy. There's a lot of bets that we end up turning down or turning off. And maybe we revisit them in the future, but that's hard. That's hard when you pour your heart and soul, you're acting as a founder for a bet and it's not working yet. So I think it's like that type, it's selecting for that type of personality, folks who are really passionate and deep about the zero to one.

**Lenny** (00:27:30):
So you lead product for the research team, you work with the researchers at Anthropic. A lot of people get a sense of what is research. What do researchers do? I think a lot of people don't totally understand these very valuable people at all the AI labs. The way I think about it, and I want to help people understand, help me understand just what are researchers doing all day. What I imagine is they have a hypothesis for how to improve the model. They find data, they tweak some algorithms, they adjust how it's trained, and they test it, see how it did, keep iterating and keep trying to find ways to improve the model. Is that roughly right? Slash help us understand what researchers are doing all day.

**Diane Penn** (00:28:09):
I think that's a lot of maybe the more day-to-day. I think one piece around researchers and research organizations like at Anthropic is there's also a vision of the future more broadly. So for example, things like, I think even at the founding of the company, researchers were talking about how do we get Claude to use a computer? How do we get AI to navigate a screen? So there's a lot of actually very founder-like energy is how I describe it within researchers are really bold and ambitious researchers, and we have a ton of those at Anthropic. So there's one layer of vision of what this technology can go.

**Diane Penn** (00:28:59):
And then I think on this other side of the loop, there's also, now that this technology or Claude is in people's hands, how do we make it better today? So it's a medium and long-term, and a lot of energy thinking about that lens of the future. And also, in the immediate and short term, what are the improvement areas we can make? And so I think you're describing a really good sense of how do we make iterative improvements on different versions of Claude?

**Diane Penn** (00:29:26):
The way that my team works with researchers is being very integrated and embedded in those loops, particularly areas where there's a lot of impact on users. So this is things like vision, computer use, coding, agentic coding, tool use, test time compute, things where there's a direct user impact. And then figuring out what are the ways to bring the user feedback, and ground it in a level that is understandable for researchers, and also actionable for researchers.

**Diane Penn** (00:30:08):
And I think that's the second piece is actually a big part of the job and sometimes a hard part of the job. So for example, we might get feedback on claude.ai. "Claude hallucinated." It's very vague. If you bring that to a researcher and you say, "Please fix Claude from being hallucinated," it's not very actionable. And so part of the time of the team is understanding, okay, what's the trajectory of why that user gave that feedback? And it's consented. And so we look at, okay, what should Claude have called tools in that moment? Or from its current knowledge or it looked at the right document, but it looked at the wrong facts. In the first case, that would have been a failure on tool use. On the second case, it would've been a failure on, let's say, search or knowledge insertion, search synthesis, or it could be something around alignment.

**Diane Penn** (00:31:06):
And so bring that level of detail to researchers coming up with, is this a big enough problem? Figure out things like evals to then describe what we've improved it. Those are the levels of actionability, and it's the day-to-day language of their researchers. And so we try to stay very close to how to bring that in an actionable manner between users to the core model training and the research development loop.

**Lenny** (00:31:36):
I was talking to someone the other day about how it feels like AI research is the place to be now if you want to be very successful in life. What does it take to become a really successful researcher from which you can tell? Not everyone's brain is going to work this way, but just say people are like, "Hey, I want to explore this career path." From what you've seen, what does it take to make it there?

**Diane Penn** (00:31:59):
Researchers generally, or research and product managers working with research, or both?

**Lenny** (00:32:04):
Let's do both.

**Diane Penn** (00:32:04):
Yeah.

**Lenny** (00:32:05):
But the researchers, PMs working with researchers also going to be very successful, but it feels like everyone's trying to poach all the top researchers across every company. So I know you're not an AI researcher, but just from what you've seen, just what does it take to make it in that career path?

**Diane Penn** (00:32:22):
Yeah. I think a lot of the most successful researchers and research leadership at Anthropic are folks who are really strong first principles thinkers about problems. They reason through problems really well, who are just passionate about their research area and have a bold description of what that could look like. And then who are actually close to the details. And so our leadership, our chief scientists, our heads of fine-tuning and RL, folks are actually really close to the training runs and actually look at things like how the training run is going, evals, looking at the underlying data. So actually staying really close and be excited to be in the details, I think have been a sign of really strong researchers and developing taste. And I think another piece is just their ability to think big over time and be very ambitious. Like the Dario, like we can transform software engineering. And I think going in that direction, you learn so much. You have to shoot for the stars in many ways across your ideas, I think, in order to be a successful researcher.

**Lenny** (00:33:49):
I love just this meme of just be more ambitious comes up so often now, which is so hard. It's easy to say that it's hard to actually just like how big can you think, and how that's so much of what AI now unlocks, just be more ambitious.

**Diane Penn** (00:34:01):
Yeah.

**Lenny** (00:34:02):
Yeah.

**Diane Penn** (00:34:03):
I think it's thinking through it once or twice end-to-end. And then being, I think, stubborn about the area and maybe more loose around the exact approach. It is a question we challenge ourselves with, but the technology is moving so quickly, and so how do you make sure what you're building is actually forward compatible? And so it's also actually part of, I think, the core product development loop to think bigger. One thing I ask the team frequently or how I think about when we're building a product is let's say Claude 8 comes around. What changes in what users do? And then what does that mean for how you're building today? Is it going to be forward compatible to that experience? So just grounding, I think being ambitious is very broad. And so trying to ground it in some ways of describing that.

**Lenny** (00:35:13):
And also, yeah, everything heading in a direction that all is cohesive and makes sense versus just ambitious in a completely different direction. Speaking of ambition and Claude 8, Fable/Mythos recently feels like hit this very new tipping point with models where it used to be you have an awesome model, release it. Hey everyone, welcome. Opus 4.5 is out. Everyone can use it. Mythos went in a very different direction. We got blocked. There was a lot of scrutiny, a lot of concern about what it was capable of. All the companies had to go make sure it wasn't going to hack into all their systems. And it feels like now every model, because they continue to get better, will now have a lot more scrutiny and there'll be more restrictions on who can use them, which feels like a big deal. How do you think about that? How does that change the way you operate?

**Diane Penn** (00:36:02):
I'm going to maybe leave the policy and the export control side to folks on that and work on that. I think the product question and how we interact with these internally is, I think as you mentioned, as frontier models become more capable, the safeguards and the ways of red teaming and testing and the pre-release process also needs to evolve and adapt quickly to address that. And so one example is before Fable models, we didn't have as strong of, let's say, fallback UXs and systems because our goal was to make sure that there is asymmetrical benefit for this technology and to minimize the downside or a severe risk of it. And so we ended up building fallback systems so that users will still get a great response from Opus 4.A immediately. And so I think there's a piece around as we evolve and improve safety systems, how do we continue to develop and deliver great user experiences? I think there's more that we can do on both sides. And so you'll see us innovating, improving on what we call now the model safeguards package more and more in the coming weeks and month.

**Lenny** (00:37:29):
What's really interesting and just unexpected here is it creates this really interesting advantage for Anthropic where you have access to the latest stuff. And this is going to happen at every lab. Everyone's going to keep improving and it creates this unfair advantage within the Labs to have access to the best stuff that other people can't yet outside of your control. You'd prefer everyone use it. So it's a really interesting, this new feedback loop that's going to start where models that are so advanced are only accessible to certain companies, and that's going to be a whole new unexpected, it's like a second order effect of all these restrictions.

**Diane Penn** (00:37:59):
Our goal is to be to develop these systems in the models to be as inclusive as possible. I think our goal is to not have that happen for the general purpose, general use technologies and to make it more accessible. I think this is one of our top priorities right now to reduce what we're seeing there.

**Lenny** (00:38:21):
Yeah, that makes sense. I would imagine you'd want as many customers if people are using this thing as possible.

**Diane Penn** (00:40:04):
We actually, on my team, have not changed our hiring loop for three years now. So what we actually look for and the traits and how we evaluate generalists like PMs, generalists like research, product managers have actually been the same. So I think some of those traits, number one is first principles thinking. And this is really rather than pattern matching what you used to do in, let's say, consumer product or B2B SaaS, but actually figuring out in this moment for this user group with this technology, what is the user value?

**Lenny** (00:40:50):
Is there an example of that? A lot of people hear first principles thinking, they're like, "Yes, I got it." I'm good at this. What's an example of someone having really demonstrated really good first principles thinking?

**Diane Penn** (00:41:00):
I think one example is I think you think of a product manager as I own product strategy and delivering user value, but I demonstrate day-to-day by writing a PRD or writing a product vision doc. And for my team as research product managers, the way to drive user value is to figure out the right user feedback, the evals that then can be a personification of that user need. So we do write some product documents and PRDs, but we actually have a saying on the team of evals are the new PRDs. Because in order to deliver that user value, it's not that exact artifact that people used to write in the last one to two decades. It's a new way of working. And so the first principles thinking would be, let me figure out what is the thing I should do to achieve my goals, rather than here is a set of activities that I've done and therefore I will continue to do.

**Lenny** (00:42:10):
So the idea here used to be have an idea, create a PRD, talk to people about it, align on the plan, design it, build it, ship it, see how it goes, iterate. What I'm hearing here is it's like, okay, here's some feedback about something that's wrong or an opportunity. Step one is the eval is now how you define what the work is versus a PRD.

**Diane Penn** (00:42:32):
Maybe step one would be understanding the user pain point. And so the way to even access a user pain point is different. In the past, we might do a user interview. I think if you go deep enough, you might have the user walk you through their user flow, the pixels. Here, you have to sweat the tokens as much as you sweat the pixels, and so one activity we have on the team is reading the transcripts and understanding what was the trajectories of failed very deeply to then say, was this a hallucination? Was this Claude being overconfident?

**Diane Penn** (00:43:14):
So the theme of the failure actually has a lot of nuance, and then that allows you to build a description, a sustained description of that pain point. So that could be essentially in a new eval. And is the eval on distribution? Is it capturing both the positive situations where this is failing and also areas when it should actually not fail?

**Diane Penn** (00:43:43):
And then bring that back to, let's say, research so that we can make the improvements and actually measure the quality of, okay, when we have Opus 5.5, is this area improving or not? Is Claude now able to identify the right places in the document and pull the right synthesis out? So it's just the actionability and shorten the distance to actionability for our stakeholders and partner teams like researchers to take action on.

**Lenny** (00:44:16):
Is there an example of something like this where you found an issue or opportunity and then wrote the eval? And what is the eval looking like in most cases? When people want to picture an eval, what do they picture?

**Diane Penn** (00:44:29):
We actually pioneered this concept within Anthropic. So one of the early examples is the early Claude models were not very good at following specific schemas. So things like outputs in JSON. And now that is fundamental to Claude being able to be a good agent. If you can't output a certain format, you don't know how to access APIs, you can call tools, et cetera. And so the initial end-to-end was I was hearing feedback around Claude two days. Claude was not very good at following instructions. So then digging in with the users, what do you mean by Claude is not good at following instructions? Give me what situations this was happening. What's the exact paragraph? What did you ask? What was Claude's response? Going to that level of detail.

**Diane Penn** (00:45:25):
And what I saw was something like 80% of what people meant in the early days for this failure was Claude would not write the right JSON. And so then, okay, let's generate maybe to start, just 30 to 40 examples of when Claude was not doing this thing correctly. And then that actually is your eval set. And you could have essentially a prompt and a response. And if that is not working in the right golden answer that you might have, then that means that the eval essentially is beneficial because it's identifying a pain point consistently. And so then we added that to our repositories for evals, and when we have versions of Claude, we actually run that eval and just check. I think at this point, it's always 100% or 99.9 and so it's no longer a pain point. But in the early days, it was taking the user feedback, figuring out actually what they mean. Can we reproduce it? Is it consistent? Is it a big issue? And then figuring out how to standardize it in a way that can be consumable for researchers.

**Lenny** (00:46:42):
It's basically test-driven development for PMs is the world we're living now where you write the test first. So is this just a core part of the product management job now at Anthropic writing evals?

**Diane Penn** (00:46:54):
I think so. I also think it's something I've talked to other PMs at other companies about, and I think it's also more and more of the skillset more broadly because a lot of the products that we're building is at the intersection of models with harnesses, with a set of contacts for a set of users. And so having things like evals actually is a way, not just for folks working on models, but generally within product to get to better user experiences because you can't improve what you can't measure. And a lot of this is very still tactile-based. It's still very judgment-based. And so you have to stay close to the details.

**Lenny** (00:47:38):
And also very non-deterministic, which is a big part of this just like it's not going to give you the same answer every time so you got to describe it more broadly, it's not going to be an exact match. So this is a really interesting change in the way product happens and will happen is evals, writing evals versus PRDs is a big part of this. Do you guys still do PRDs? Is there still a one-pager describing a problem or is it replay? Okay, now you're shaking your head yes.

**Diane Penn** (00:48:00):
We are. We do.

**Lenny** (00:48:01):
Wait a minute. Okay. Now you're shaking your head.

**Diane Penn** (00:48:03):
Yes. We are. We do. I think when there's a very defined problem, I think things like evals might be almost a shorthand. I think there's other cases where PRDs are really valuable. PRDs are great vehicles for getting a very large group of people aligned on a set of sources of truth about experience and set of goals. So when we do have a model, we actually, for every model, we do have a PRD, less necessarily for our researchers, but more for our growing product surfaces, for our engineering teams, for our stakeholders like legal and safety and others as just a source of truth of putting together what we're aiming to achieve so that a big group of people can row in the same direction.

**Diane Penn** (00:48:54):
The other place where I do think PRDs are valuable are on the more ambiguous problems and opportunities. So if we haven't shipped a thing like computer use, we don't necessarily have a set of user specific pain points always. And I think there's value in the product vision portions of a PRD to explore what could, even if a technology is not yet ready to work for everyone, how do you get it to work well for some group so you can explore the value? You can actually bring something that is coherent to a user group. So we do have PRDs. I think the application's a little different now.

**Lenny** (00:49:39):
Okay, this is great. I just had Andrew, he's the head of the Codex app at OpenAI, and you guys are aligned. PRD's not dead. Still very useful for specific projects and ideas. Great. Okay. We've closed the book on... PRD is still kicking. Okay. So we've been talking a bit about just what kind of skills are emerging for product people. Is there anything else that you find has shifted in what patterns are common across people that are doing well in this new AI world in terms of product managers and folks on the product teams? Is there anything else that you're like, okay, this is something you got to shift or something you look for more people?

**Diane Penn** (00:50:19):
I think maybe specifically for folks who might be mid-career or folks who have been more in a managerial product leadership seat. One thing that I think I feel pretty strongly about is in order to be good managers of teams and PMs working with this technology, you have to be really hands-on yourself and have spent not just time tinkering, but actually shipping with this technology. And again, being in the details and sweating the tokens along with your PMs and your engineers and your teams. And so even for folks that I hire who have more tenured PM experience, the onboarding plans are exactly the same as somebody who is more early career. And it's around understanding users, reading consent and user feedback, talking to customers. I think there's something around being able to understand what to do with this, what good looks like, and having developed that in a very hands-on manner that's important.

**Diane Penn** (00:51:40):
It's not necessarily easy for someone to agree or be able to see what a good or great AI product or AI feature could look like if they haven't kind of experienced building themselves. So I do feel pretty strongly that if you're a manager, you have to be hands-on; you have to spend a portion of your time actually shipping. You have to kind of walk in the shoes of your teams. And I always try to carve out a portion of time to actually own one to two work streams when we have models in order to keep my theory of mind, keep my sense of how the models are moving, how quickly it's improving, so I can help the team make decisions and make better decisions.

**Lenny** (00:52:35):
So what I'm hearing here is no matter where you are in the ladder of hierarchy at a company, if you're not building yourself, if you're not actually talking to cloud, talking to Codex, building stuff, you're not going to make it.

**Diane Penn** (00:52:46):
And you should have fun working with this technology. I think that's the other piece. I think the folks that would be most successful, regardless of their level, are people who love working with AI and are exploring and experimenting. And carving out the time, not just for the experimentation, but actually hands-on shipping end-to-end, getting the user feedback, I think has to be fundamental for everyone.

**Lenny** (00:53:12):
I 100% know what you mean there. Just me sitting on my newsletter and this podcast just talking about stuff and like, yeah, yeah, that sounds great. Every time I actually build something, and I tinker with all kinds of little projects, you're just like, okay, I see what's happening here. And you just get so much more. It's hard to exactly describe what you experience actually working with the models and building stuff, but it's a whole different world of like, okay, I see. Here's what they're talking about computer use; here's what they're talking about with this limitation of this UX situation. And you made this really interesting point that you have to have fun with it, which is not easy for a lot of people because they're pushed to use AI or they just don't know exactly what to do with it. For people that are just like, I don't know, it's just so annoying. I just have to do this. I hate this frigging thing. Why do I have to work with this? Things are changing so much. I'm tired. Advice for helping people find that joy in this work.

**Diane Penn** (00:54:06):
I think maybe I'll reemphasize something I said earlier around just that experimentation is not an individual sport. Some of the moments where I think I've touched practically every version of research models across 20-plus versions of Production Cloud at this point. And I think part of the joy comes from seeing other people discover use cases too. And so maybe one idea here would be pairing with somebody who is excited and seeing what on a use case that you care about and working together versus identifying or trying to figure out the perfect use case yourself because that might feel like work. Working with others feels like joy a lot of the time, and is there more that we could do to bring other people along? That's something a lot of times internally we have somebody who is very curious, and them sharing an idea of a new prototype actually brings a ton more people who are like, oh, I didn't know this could work now with Claude. And so there's just some virtuous cycles here and ways of continuing to have joy with this technology.

**Lenny** (00:55:22):
That's such a good point. I think that's also why Twitter is so useful for a lot of this is you see other people sharing what they've done, and it inspires you to come up with your own little ideas. And also it's just fun to share your own thing that you've done. So that's a really good point. Just find other people to play around with and look for use cases. The thing I've also heard a lot is just find a problem you want to solve in your life or work and just open up Claude, Claude Code, tell it, here's what I want to do. And it's incredible how far you can get just with a vague idea of a problem you want to solve.

**Diane Penn** (00:55:53):
Yeah. I think it gets hard in that there's so many different things that you could try. And so you just narrowing in on either pairing with someone, working with somebody who have a lot of joy about this technology, or figuring out something that you could immediately find value. Either of those things allow you to go deeper rather than more high-level about too many things. I find it hard to keep pace with the number of prototypes or products that are out there. And so my lens has been: how do I go deep in one to two of them myself?

**Lenny** (00:56:31):
That's so interesting you say that because that's exactly it. We just had the survey that I ran with my colleague Noam asking my readers just how they're feeling about all the things going on in the tech right now and AI. And one of the most interesting takeaways we had was to find that happiness is exactly what you said is go deep in a couple things versus trying to just ton of little things. Find a couple things to really solve well and then go deep. And that is a source because a lot of the happiness people feel is when they finally unlocked their way for AI to actually make their lives better versus just a couple messed up, broken, half-working things.

**Diane Penn** (00:57:08):
Yeah. It's, how do you go from this being a check-the-box? Right? And so us as product people, it's then an exercise of product prioritization of your time and your energy. And if the goal is to experiment with joy, then what are the inputs that you need for that? But yeah, I think the secret sauce of Anthropic is the culture and the bottoms of nature of how people work and this experimenting in public. And by doing that, it's very much about how to bring other people along. That ends up being, I think, really valuable.

**Lenny** (00:57:55):
Yeah, I've heard this so many times from all the labs, just like no one's exactly sure how some of this is going to be used. And a lot of it is just putting stuff out early, seeing how people use it, seeing what's possible, and then using that information to build the actual product to lean in.

**Diane Penn** (00:58:10):
Yeah. Yeah.

**Lenny** (00:58:11):
I'm curious how, kind of on this thread of finding ways for AI to help you in your work and life, are there any interesting ways you've been using Claude lately in your work as a PM?

**Diane Penn** (00:58:22):
I think there's a lot of things with Fable and things like TAG. So I think TAG is in the very early days; I think there's something around how you work in a different paradigm of allowing an agent to go off and work and them bring back product and experiences to you. I think one area that it's not more recent, but one that I bring up a lot with the team and I think we could do more on using AI is just how to use it to also have better conversations with each other, to be better managers. I don't think it's necessarily just about raising the IQ of experiences we build, but also I use it a lot and actually prepping for how to have better conversations in the moment during crucial conversations.

**Diane Penn** (00:59:22):
So I love that book. And so I actually have a skill that helps me figure out, am I going in the right level of detail given the situation at hand, and actually helping me be a better manager and better supporter for the team. So for managers on the team, that's actually a thing that I've been sharing more with our managers of, okay, how do you actually use Claude to make you a better coach? Because it's hard sometimes to find the right perfect words, and the models have a lot of perfect and right words. And I think there is something about how it can actually augment us from an EQ perspective in addition to IQ.

**Lenny** (01:00:04):
Oh man, there's so much interesting stuff there. So just to understand what you're doing there. So you built a skill; you're just like, "Help me, Claude, build a skill." Pulling in lessons from Crucial Conversations, the book, which it knows enough about. You don't have to even give it the content. And then you use that skill to talk to Claude, "Hey, I have this very difficult conversation coming up with a colleague. Give me some tips on how to approach it."

**Diane Penn** (01:00:25):
Yeah. And it's a great, it's almost like coaching, individualized, personalized coaching of just how to make you... And there's so much context switching that we do all day. And having Claude help me pair and help me... And maybe there are times where I end up not using suggestions from Claude, but it actually ends up being very helpful for just coming up and brainstorming. Am I thinking about reactions in the right way? How do I actually go a bit deeper, faster, build trust faster, be more direct?

**Lenny** (01:01:05):
Yeah. Man, I have so many questions here. This is so interesting. One is just there's concern people are going to start talking the way AI writes because they're talking to AI so much, and it's going to be like, "Dianne, it's not this, but it's that." I know that you're not doing that, but that's a concern people have. Let me just ask about that, I guess. Do you fear there's this brain-rot atrophy stuff people talk about it where you're just so reliant on AI now and we stop learning and thinking and overlaying AI thoughts on that, being so close to it and being so integrated with AI constantly?

**Diane Penn** (01:01:38):
A lot of actually thinking process and writing process are tied together for me personally. And so I think there are ways where I use Claude to augment my thinking, but what I want to make sure, and maybe this is what you're describing, is Claude doesn't take over all of my thinking for me. And so I think depending on the situation, depending on how much more personal judgment I want to have in a situation, I might come up with my own POV first and then work with Claude through that, and making sure that I maintain my sense and tone throughout. I think there are then other things like updates. We have monthly business reviews, and then in those cases it's much more, I actually want it to be standard, and I want it to be much more like it gets a crystallized information in the right way.

**Diane Penn** (01:02:35):
And I have a skill, and we're augmenting and improving our skill for that. I want to get to a place where the monthly business review, the writing of that, is potentially asymmetrically less valuable than the thinking. And so how do I get that piece delegated to Claude fully? And I'm more of a reviewer and a verifier of that information. So I think it depends on what you're using Claude for and what you're trying to convey, and is there asymmetrical value in delegating more to Claude.

**Lenny** (01:03:11):
What I'm also hearing, the first tip is really great, which was think first, have a point of view, and then use Claude as a sparring partner almost to evolve the idea, push back on the idea.

**Diane Penn** (01:03:22):
Yeah. Yeah. And I think this is where things like actually our alignment research and safety research is helpful because what you don't want is AI that just agrees with you. What you want is this technology to actually augment and grow and get to a better outcome. And so sometimes it's having Claude push back makes me better. And so that's great. Like a coworker, I want somebody to push back when my ideas are not fully formed.

**Lenny** (01:03:53):
I want to hear more about that. I've heard that when Ben Mann was on the podcast, he talked about the constitution that is built into Claude and how unintuitively the work and the focus on safety and alignment, as you said, and this constitution that describes how Claude should think and operate. You would think that would limit the abilities of Claude and make it less fun and interesting. It's exactly the opposite. Claude is the most interesting personality. I hear that constantly. It's just like I much prefer talking to... OpenClaw famously was built on Claude, and then people were forced to switch. We won't get into it. Were forced to switch to ChatGPT, and they're like, "This is so bad. This is not who I'm used to talking to." So that is, I think, a really interesting point. I just want to make sure we spend a little time on. Why is it? Why is that the case? Just this focus on alignment, safety, having this clear constitution? Why does that make Claude better and more interesting to talk to you also?

**Diane Penn** (01:04:49):
In order to make Claude as intelligent and as capable as possible, being able to have Claude actually push back in the right points and then add, it's like a yes or no and actually helps you come to a better conclusion. So I've used Claude to help with things like, are we making the right pricing decision on the next version of Claude? It's a little bit meta, but using a research version of Opus, asking it to figure out how it should price. And being able to come out with better outcomes is a goal at the end of the day.

**Diane Penn** (01:05:27):
And so having AI not just be an assistant, not just be a doer and being delegated task, but figuring out is it doing the right thing? That's actually very integrated with knowing when to push back. That's part of knowing when you should be proactive. Proactivity is not necessarily always doing a thing that you are scheduled to do. It is knowing when to come up with a new idea. And so in order for Claude to be more useful, the general approach has to be that it knows when to push back. It's a core part of the characteristics together of the models.

**Lenny** (01:06:10):
That is so interesting. It's so interesting that that is what a big part of it being less compliant is almost what makes it better and more useful because we need that. I've had so many people where they're like, "Hey, AI told me I was right." And they're like, "No, I wish it was to other people."

**Diane Penn** (01:06:26):
Yeah. And it comes back to our earlier point around thinking. How do you protect your thinking? If you have an AI that can be a thinking partner, a thinking partner doesn't just agree with you. It should add to you. And you should come away at the end of the day having better ideas because you worked with Claude. That should be the hero goal, not just making your ideas 10% better.

**Lenny** (01:06:52):
Yeah, I love this sense. It used to be think 10X. It used to be the way founders push people like, what if we 10X this? And I love what I keep hearing is it's like, how do we go 1,000X from this idea? What is the most ambitious version of this? I want to come back to something that I was thinking about as we were talking about talking to Claude constantly. It's very clear when AI has written something still. It's funny that it's a large language model. You would think, of all things, it would be very good at writing, and interestingly, just no AI is very good at writing. It's always very clear this was AI-written. Do you think we'll get to a place where we will not know this was AI?

**Diane Penn** (01:07:32):
I think it depends on what's the goal that you're looking to achieve by knowing or known-

**Lenny** (01:07:39):
What's the eval?

**Diane Penn** (01:07:40):
Yeah. What's the eval? I actually do think there's more that we could be doing on making Claude write better. There's actually very active efforts on my team and on the research side about making Claude write better, just generally. I think it should be clear where an idea is being led by you or by you, Lenny, or me, Dianne. I think it really depends on what's the goal of that writing. For something like a monthly business review, I would actually love to have that end-to-end be written by Claude. And-

**Lenny** (01:08:22):
Obviously, and not make it feel like it was written by a human. That's such an interesting point you're making. Is it actually better for us to know that it's AI versus not?

**Diane Penn** (01:08:29):
Yeah. But it's also for maybe the lens is more around verifiability or who's verifying the output. Right? Who's signing off? Maybe less around who's writing, but who's verifying who's signing off? That becomes more what matters than who's writing it.

**Lenny** (01:08:52):
Why do you think AI is not great at writing? My guess is it has studied all of the best writing in all of humanity. It's figured out, here's the best way to write. And there's only so many ways to write. And so we've just recognized, okay, this is what AI does. It has these tropes. Is that the core of it? Is there something else that's keeping it from being a great writer? Ironically, being a large language model of all things, you think you'd be really great at language.

**Diane Penn** (01:09:21):
I think part of it is also we need to invest more in training improvements to make AI continuously strong on areas like writing. I think it's also the technology's jagged-edged, like we mentioned. So sometimes when the models were good at writing, but not agentic, our thesis is: how do we make the models more agentic or call the right tools? Now that that's improved a bit, then it's, well, now it's these other areas actually become more of the rough edges. And so I think we're in one of those moments worth writing where we need to actually just focus and prioritize on training the models to be great at this area. And that is a very active area for us. So fun that you mentioned.

**Lenny** (01:10:11):
Okay. I'm glad. I'm glad. And also it was going to be interesting once AI is so good, we're like, "I don't know who wrote that." But to your point, sometimes we actually want to know that it's AI. That's really interesting. I never thought of it that way. The other interesting part of this is that there's that comedian who was joking that we're on a plane and the WiFi's down and we're just like, "What the hell? The WiFi's not working on this plane. This sucks. How dare you?" When you're in a tube in the sky flying like a bird. And how dare you complain that the WiFi doesn't work? Your point is there's so much advancement and so much power. We can't fix it all. We can't make it all work the best possible and so basically writing has been not the priority, and it feels like there's more investment happening there.

**Diane Penn** (01:10:53):
Yeah. I think tone and character is a priority. I think it's this advancement of the technology is a work in progress and so we see a leap or an emergence of a jump in agentic behaviors. And so that is a new normal. And then these other capabilities needs to continue improving. And I think once we improve, let's say, writing and tone and character, we probably will say, how do we have Claude be even more proactive? Proactivity is an opportunity, and that's human nature. We want to make ourselves better. We want to make this technology better and I think we're applying it to AI, which is the right thing. We should be making it better.

**Lenny** (01:11:41):
I want to ask you a couple questions I like to ask folks working at the very center of the future that is coming. One is, where do you think human brains will continue to be most valuable over the years? I know Anthropic's mission and vision will reach AGI, a super intelligence. So in the future, maybe nowhere. But before we get there-

**Lenny** (01:12:00):
Intelligence. So in the future, maybe nowhere, but before we get there, where do you think human brains will continue to be most valuable, as we approach that timeline?

**Diane Penn** (01:12:09):
We started to talk about making Claude and models better at judgment, especially in the last year or so. I think judgment is an area where, it's accumulation of so much nuance and so much experience. And these systems haven't experienced as much as humans have. And so I think that hard-earned judgment is a area for product leaders and just generally will continue to be really critical. There are so many things AIs can build. Which one are the things that an org like Lab should build? A lot of that requires human judgment, persistence, so proactivity. These are all traits that are beyond just general capabilities, but just behaviors and characteristics of people at that level of how do you get to the best solutions? How do you create the best experiences? So I think those types of traits are actually the tactile traits that I think will continue to be important.

**Diane Penn** (01:13:22):
I think there is also still a lot of capabilities and subject matter expertise as well. I think software engineering has been really transformed by AI. I think there's areas like biology, life sciences. These are all things that we're just at the foot of the exponential on. Maybe software engineering, we're on the exponential. On some of these other areas, we're not quite there yet. And so I think you're seeing us shift things like Claude Science investing in these areas because those are areas that I think is just bring this technology to society and having a positive benefit for society. So I think there's a lot more to go there.

**Lenny** (01:14:11):
Another question I want to ask is, as someone with kids, how do you think about what you are encouraging them to learn? Where do you think you're going to nudge them to be successful in this wild new world that we're entering?

**Diane Penn** (01:14:27):
I actually think it's a lot of the same traits you and I probably grew up with, which is curiosity for learning, persistence, believing in your own inner voice. Developing and then believing in your own inner voice. I have a four-year-old, I have a eight-year-old. It's on me to help them develop their inner voice. And whether that's being opinionated and taking a stance to me and developing that, encouraging that, I think that those types of skill sets are things that is important in the future and having their own individual voice.

**Lenny** (01:15:10):
That is so interesting. It's so related to the answer you had when I asked about how to avoid brain rot essentially and over-relying on AI, which is just keep focused on your own point of view and your own perspective before you over-rely on AI. And just this idea you're describing of building that in kids is really important. That is interesting. And I love how all this connects judgment, persistence, a point of view of your own.

**Diane Penn** (01:15:34):
Yeah.

**Lenny** (01:15:35):
Both for kids and also adults.

**Diane Penn** (01:15:37):
[inaudible 01:15:37]. Yeah. Anything-

**Lenny** (01:15:37):
Anything-

**Diane Penn** (01:15:37):
You think about for your ...

**Lenny** (01:15:39):
Oh, man. Well, the question I'm thinking about is just when to get them on some AI-y thing. I have a three-year-old, so it's pretty early for that. But how do you onboard them to this crazy thing? I was at an event recently and a bunch of parents were talking about how they think about AI and their kids. And one person had a really interesting approach, which is keep them on the very early models so that they still have to struggle a bit and not get all the answers immediately. Thought that was interesting, like an open source local model, not Fable.

**Diane Penn** (01:16:11):
I like it.

**Lenny** (01:16:12):
Yeah.

**Diane Penn** (01:16:12):
Yeah.

**Lenny** (01:16:12):
Yeah. And curiosity is something. I keep mentioning Ben Mann, but his answer, actually, to this question has always stuck with me, which is curiosity and also just he's a big fan of Montessori, which is what we're encouraging for our kids. So there's something there. Maybe a last question, just along these lines, something Fiona Fung actually suggested ask you, who was recently on the podcast. How do you stay just recharged and not burnout, being in the center of this crazy storm of AI, as a mom working in ... We're seeing the research work at Anthropic. We're living through the most unprecedented time, working at ... Just being on the outside of Anthropic, it's crazy. I don't even know what it's like to be on the inside. What have you learned about avoiding burnout, staying recharged, staying sane during the middle of all this?

**Diane Penn** (01:17:01):
In 2024, we shipped four models in the whole year or four series of models. And I think we did more than that volume in just Q2 of this year. I think I've been really lucky with the team that we've grown and built, both the stakeholders on the research side and within our research product management team. I think that one of the magical parts about approaching all of this is that it's not an individual sport. There's a sense of radical ownership and team collaboration that, I think sometimes it does feel like a high performance sport because you're in very critical decisions. There's new information about users, about training, and you have to make recommendations and judgments and decisions very quickly. And nobody can do that sustainably by themselves.

**Diane Penn** (01:18:04):
And so I think what's really helped is having a team that is incredible, who looks out for each other, who the night before a launch, even if they're not the core DRI on that model, will stay up and help the DRI to review the blog post and make edits and come up with better demos and knowing to be each other's extra hand. I think it's very easy, if you take all of this change on your own shoulders, to feel like you're alone and to feel like you have to do everything. But I think one of the magical parts of Anthropic is this ability for us to figure out what are those opportunities to help each other and actually then taking the next smile of mind melding.

**Diane Penn** (01:18:54):
We called it entering the hive mind. There was an article about this. And I think part of that is just that allows the team to replenish. I was just on PTO in June. It's not just that you can take PTO and you come back to 3X the amount of things to do. It's actually that you can take PTO and know the team can figure out the right things to do and that we individually can watch out for each other. So I think that's a big part. I'm really lucky, just personally. Also, my partner is really supportive. This is year six of me working in AI, so Amazon and then Anthropic. And so he sees how much I just love the technology and what this can do. And that really helps, I think, also from a personal perspective as well.

**Lenny** (01:19:45):
I love how many of these answers connect. So what I'm hearing here is just working with other people, relying on other people, helping each other out when things get crazy, which is a similar answer you had for just how to find the joy and fun in this work. Just be inspired by other people, see what they're doing, work together.

**Diane Penn** (01:20:06):
Yeah.

**Lenny** (01:20:08):
And it's interesting, when Fiona was on the podcast recently, I was asking her just what's changed in the world of software engineering? And she pointed out it's a lot lonelier now because now we're working with agents instead of other humans. Teams are smaller. People are having all these fleets they're talking to constantly. And so this is just a reminder of just the power of just actual other humans around you.

**Diane Penn** (01:20:26):
We're asked to work and make decisions on really big things because you have more scale from the technology. And I think having individuals, having other folks more who can have some level of mind meld with what you work on, how you approach, maybe not exactly every detail, but what are their first principles? What are the assumptions you make? Then helps them back up for you or push your decision and sharpen your thinking. So I think I really try to look for that when building the team, growing the team, hiring. Is this person going to care about their own ego and building out a big org or are they going to care about contributing to Anthropic and contributing to the impact of the team and orienting towards folks who are low ego, team-oriented? I think it's a big part of the sustainability.

**Lenny** (01:21:30):
Yeah. A lot of it always just comes down back to culture and hiring. And I know I've heard a lot, just the reason Anthropic is able to move so fast. I remember that moment when something shipped every day of the month. There's a calendar of launches and people were talking about how is this possible? And what I heard a lot is just because everyone is so aligned around the mission and the values, it allows people to make decisions really quickly. Before we get to our very exciting lightning round, is there anything else, Diane, that you wanted to share? Anything else you wanted to touch on? Anything you want to maybe double down on of things we've talked about?

**Diane Penn** (01:22:04):
This was actually really fun because I feel like your questions actually sharpened some of my thinking around how the thoughts connect.

**Lenny** (01:22:10):
I'm your real human Claude over here.

**Diane Penn** (01:22:13):
One thing that I really want to convey or have people take away is I think one, in the ways of working, but also just two, this is a lot of growth and change and having the joy in using this technology. And if you're feeling like in this moment, you don't have as much of that feeling of initial joy, how do you find people who do, if this is an area that you're excited and want to work on? And I think developing skillsets, replenishing skillsets in many ways of things like thinking from a first principles' manner about what you solve. I think fundamentally, you didn't ask me this, but there is this question in the community of do we still need PMs when the models are so capable, when engineers are leaning in?

**Diane Penn** (01:23:10):
I think the role of people who are user-centric, who go into the details of understanding what users are trying to accomplish, bubbling that up in an actionable manner and doing the relentless work to do that, that, to me, is a core of a product person. And I actually think we need more of that. I think we are becoming very technology layered-driven. And actually to make that impactful, you have to go deep, you have to be curious, you have to be super hands-on. And those are things that are also traits that have, I think, helped Anthropic from a product development and model development perspective and as part of the culture. And hopefully that's valuable for others as well.

**Lenny** (01:23:59):
Amazing. What an inspiring way to end it. Oh man. Yeah. And I've been saying this too for a long time. Just now that building is easy, the hard part becomes, as you said, what should we build and is the thing we have built correct and good and worth leaning into? And to me, that's what PMs do and what PMs are good at.

**Diane Penn** (01:24:18):
Yeah. Yeah. And it's getting into the details of the user.

**Lenny** (01:24:22):
Yeah. Empathy. Okay, great. PMs are going to make it. Okay. PRD is not dead. All kinds of important lessons here. Diane, with that, we've reached a very exciting lightning round. I've got five questions for you. Are you ready?

**Diane Penn** (01:24:36):
Yep.

**Lenny** (01:24:37):
First question, what are two or three books that you find yourself recommending most to other people?

**Diane Penn** (01:24:43):
One personal one, I really like How to Raise an Adult. So I'm a mom. I think a lot about what is the things that I want to instill in my kids. And that book is really helpful for describing, we're not trying to raise children, we're trying to raise adults. So just the framing of what does that mean? And what does it mean, what are the characteristics that we want to hone and harness and foster in our kids? The other book that I was listening to on Audible recently is Incorrigible by Eric Reese. So the author-

**Lenny** (01:24:44):
Incorruptible, I think is-

**Diane Penn** (01:25:22):
Incorruptible. Yes.

**Lenny** (01:25:24):
Yeah. His recent [inaudible 01:25:26].

**Diane Penn** (01:25:27):
Yeah. And I think the question of how to build great companies is important. I've personally just been most fascinated with how to keep great teams and great companies going further. And it was very interesting to just see his framing and reframing of the question. I loved some of the examples around having metrics around culture. If you only measure revenue and then that's how you're going against. But if you have other better metrics, that's actually the way to sustain the values you care about. I've been trying to think about how to actually bring that to the team level of how do we better articulate our norms, a lot of the things we talked about on the team. So I think that's also a really good read.

**Lenny** (01:26:16):
There you go. That'll be your next watch, everyone, as you're listening to this, the Eric Reese episode. Such a good episode. Yeah. And his book just came out, Incorruptible.

**Diane Penn** (01:26:25):
[inaudible 01:26:25].

**Lenny** (01:26:25):
I think it was like a New York Times bestseller. It's actually doing incredibly well, which I was really happy to see.

**Diane Penn** (01:26:31):
Yeah, exactly.

**Lenny** (01:26:32):
Next question. Favorite recent movie or TV show you've really enjoyed. Most people at Anthropic do not have time to watch things, but I'm curious if you have an answer.

**Diane Penn** (01:26:40):
**Diane Penn** (01:26:58):
Yes, it's based on the video game. I think it's witty, it's humorous. It's also super action-oriented, so highly recommend.

**Lenny** (01:27:08):
Okay, next question. Do you have a favorite product you've recently discovered that you really love?

**Diane Penn** (01:27:12):
I really do think Claude Tag is very interesting in terms of a product experience. We actually have different versions of this within Anthropic, and I think it's actually been a really, really, really powerful tool.

**Lenny** (01:27:29):
Yeah. I think some people are like, "What's the big deal?" The fact that everyone at Anthropic is raving about it tells me something important is going on here. And I'm trying to actually get it working within my Slack community that I have for paid newsletter subscribers. How cool would that be?

**Diane Penn** (01:27:43):
Yeah.

**Lenny** (01:27:43):
Yeah. I'm trying to figure out how it works when it's not a company, when it's just a bunch of people that don't know each other and how that might work, but we're trying it out. Okay. Two more questions. Your favorite life motto that you find yourself often coming back to in work or in life.

**Diane Penn** (01:27:57):
So I was actually raised by my grandparents for the first 10 years of my life. And my parents were immigrant college and master's students in the US.

**Lenny** (01:28:08):
Oh, wow.

**Diane Penn** (01:28:08):
And my grandfather always says, no matter how far you go, there's always another level, which is, I think, a really good way, though a pretty intense way of describing his life philosophy. But I go back to that whenever there's something new or unprecedented that we experience. And I think first half of this year, there was definitely a lot of that. There was a lot of new things that we were learning, I was learning. So just feeling like there's always another mountain, another opportunity to come.

**Lenny** (01:28:50):
Not good enough, Diane. We need to go better. We need to go bigger. Makes me think about, actually, another Ben Mann line from his podcast episode, that this is the most normal it's ever going to be. It's only going to get weirder and crazier.

**Diane Penn** (01:29:04):
Yeah.

**Lenny** (01:29:05):
Oh my God. Okay. Final question. I was poking at your LinkedIn. You were a high yield bond trader at JP Morgan Chase early in your career. You have this redacted $100 million trading portfolio of some kind. What did you learn from that time in your life that has stuck with you? And/or is there a crazy story from that period? It was four years of your life.

**Diane Penn** (01:29:31):
I think I learned, actually, a lot that I applied here at Anthropic and other jobs thereafter. So when I was at JP Morgan, the trading floor, you could envision Wolf of Wall Street. That's very different. Most traders, I think, are in front of a terminal. They're much more doing analyses on their computers, but it's still very, I would say, male-dominated. And so I was the only woman. I was the only person with my background on the trading desk. And I learned that there was a very good environment to building one, my sense of authentic self. And two, that even if I was the most junior person, even if I may look different, that the best ideas and having conviction in the best ideas, irregardless of all of those other factors, is the most important thing.

**Diane Penn** (01:30:43):
And so I think just bring that sense of how I show up more at work. I'm pretty vulnerable and authentic with my team. I try to really make sure that, regardless of people's levels or tenures, if they have a great idea, how to help them pursue that and to do also the same. So to put the idea out there, to actually have conviction in it, to do the follow through, to do the nitty-gritty work to make it happen. So those are all things that I learned from trading. And yeah, I think applies to any job in many ways.

**Lenny** (01:31:20):
That is beautiful. Where can people find you online if they want to follow you? And how can listeners be useful to you?

**Diane Penn** (01:31:28):
I don't have a large presence on social. I think the best way to find my work, my team's work is really the Anthropic blog and when we're publishing new models, new product experiences. I think in terms of useful for me, I think the best thing, number one, is your feedback. We actually, if you thumbs up or thumbs down on any of our product surfaces, if you contact your salesperson with feedback about the model, it will make its way to me. We actually, with every research model, I actually get pretty close into understanding favorability and feedback. So giving us that feedback, pushing Claude, telling us where it's falling down, those help us make Claude better. The other thing is if you have folks in your network who seem like this type of profiled person that I just talked about, I'm hiring, the team is growing. We really will love just people who love this technology, who are deeply curious, first principles thinkers, who are fearless in questioning assumptions and who have a tinkering hackery spirit.

**Lenny** (01:32:46):
Wow, what a dream job. So basically open PM roles at Anthropic on the research team.

**Diane Penn** (01:32:52):
Yes.

**Lenny** (01:32:53):
And they apply, I assume, on the website, the careers page.

**Diane Penn** (01:32:56):
Yes.

**Lenny** (01:32:56):
Holy moly. All right, here we go. Enjoy the flood of resumes you're about to receive.

**Diane Penn** (01:33:01):
Thank you, Lenny.

**Lenny** (01:33:04):
Diane, thank you so much for being here.

**Diane Penn** (01:33:06):
Thank you so much for having me. Thank you for really helpful, though-provoking questions, helping me even connect the dots on how we work, how this whole technology is coming together and being proud of people in it.

**Lenny** (01:33:21):
I really appreciate that. But thank you, Diane, for real. Okay. Well, bye everyone. Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
