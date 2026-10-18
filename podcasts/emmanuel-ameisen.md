---
title: "Inside the black box of AI: How AI models actually think | Emmanuel Ameisen (Anthropic)"
date: "2026-10-18"
type: "podcast"
guest: "Emmanuel Ameisen"
post_url: "https://www.lennysnewsletter.com/p/a-mind-expanding-conversation-on"
description: "How AI models actually think, covering AI product work, engineering tradeoffs, and product design."
word_count: 13517
---

**Lenny Rachitsky** (00:00:00):
One of the big questions on people's minds these days, is AI doing bad things? As someone that watches these models think and operate, why is it so hard to catch it thinking badly trying to deceive us?

**Emmanuel Ameisen** (00:00:09):
We trained Claude to be helpful, harmless, and honest. Is it the case that it's behaving well, but if you look inside actually it's like, oh, I'm only behaving well because Lenny's watching right now.

**Lenny Rachitsky** (00:00:18):
People's full-time jobs is studying the model, how it thinks, how it operates. How long has this been a skillset and a job?

**Emmanuel Ameisen** (00:00:24):
One of the most important things to realize if you use language models or think about them is just this very bizarre fact that to make them is not to understand them. All these models do is just a lot of mathematical operations on many numbers. If you look at it, it makes no sense. You just have a list of a hundred numbers, the model's doing math, and then you just try to see if there's patterns.

**Lenny Rachitsky** (00:00:42):
You are figuring it out the same way we figure out how the brain works, looking for patterns. You show this image, this part of the brain lights up and you're doing the exact same thing with AI. Wow, this is so fascinating.

**Emmanuel Ameisen** (00:00:50):
There was this model we were training, it would go crazy. It would do some math, it would get to an answer, I think it was 12. It would immediately go back and say like, "Oh no, oh my God, the answer actually is for sure 36." It would do math again, it would get to 12. Slowly it would start descending into madness, writing in all caps, literally saying, "I'm possessed by a demon."

**Lenny Rachitsky** (00:01:07):
Humans, if you really boil it down, we're basically next token predictors ourselves. We're just trying to figure out the next thing to say. Dario is always out there, "This is really dangerous. We got to be really careful." And everyone's just like, "No, he's just saying that for marketing reasons." And now it's like, wait, shit, it's really dangerous.

**Emmanuel Ameisen** (00:01:21):
Take the idea that this technology is going to keep improving seriously.

**Lenny Rachitsky** (00:01:25):
Do you think about consciousness as a part of this? Just do you think AI is conscious?

**Emmanuel Ameisen** (00:01:29):
Oh, man.

**Lenny Rachitsky** (00:01:33):
Emmanuel, thank you so much for being here and welcome to the podcast.

**Emmanuel Ameisen** (00:01:37):
Thanks for having me, Lenny.

**Lenny Rachitsky** (00:01:39):
So you work on interpretability at Anthropic. Explain what that is. Explain what it is you do.

**Emmanuel Ameisen** (00:01:45):
Yeah. So I work in a team of interpretability researchers and our goal is to understand how LLMs like Claude work by looking inside them. One of the most important things to realize if you use language models or think about them is just this very bizarre fact that to make them is not to understand them. You make them by building this architecture, which is kind of like a scaffold, and then you pass a bunch of data through them and they grow in inscrutable ways. And so that's why it's even a thing that we could be wanting to do to study how these models work. And so a lot of our research has been on, well, when the models are about to produce one more word, there's actually a whole universe of stuff that happens and we try to untangle as much of it as we can.

**Lenny Rachitsky** (00:02:42):
There's going to be a lot of mind-expanding, I don't know, elements to this conversation I expect. One is along these lines, this point that you make that models are not built, they're grown. Speak more to that.

**Emmanuel Ameisen** (00:02:55):
At a really high level, the way a model like Claude works is you train it in these successive phases, like the first phase, which people refer to as pre-training is you just take a large corpus of data, and over this corpus of data, you feed the model as input, the let's say first half of a certain document, and you ask it to predict the word that comes next. Then you do that again and again and again and again for an ungodly amount of data. And after you do that, there's then this other phase where then you have this fine-tuning phase where maybe instead of arbitrary data, you have a corpus of examples of how the model should behave and that's what you train it on. So you have examples of dialogue of helpful assistant telling you your favorite recipe or solving coding problems. And then there's further details here that I'm just going to skip for a second.

**Emmanuel Ameisen** (00:03:56):
But then, okay, so what does that mean that you're doing this process? What is this thing that you're training? All models are, is they take this input, which is a bunch of words, they turn these words into numbers, and then they do some math on these numbers and they get some intermediate results and then they do more math and they get some intermediate results and they do this again and again and again and again many times. And then at the end they have a final result which then convert back into a word. And so the math that they do, these computations, that's the part that's grown. That's the part where it's just like through learning to do this task better, we serve update parameters in one direction or another and then they learn some formulas. We have no idea what they are. And the goal of my team is to study both what these formulas mean in the end and also what these intermediate results are. Can we decode them and can we see what the model is doing as it's doing all of this intermediate stuff?

**Lenny Rachitsky** (00:04:49):
**Emmanuel Ameisen** (00:06:30):
I think it's really weird. I think that the best way to think about it is the reason we ended up here, one of the big reasons is that we don't know how to do it the normal programming way. So you want to build an app or something, you want to do something pretty self-contained, you can just have a programmer that's going to write a bunch of rules and say, "Ah, well, if somebody clicks on this button, then this happens." If this, then that, and so on. We don't know how to write that software for classifying images into categories or for making a machine that can generally take in arbitrary text and produce texts. It can take in reports and summarize them, can write emails.

**Emmanuel Ameisen** (00:07:17):
And so in a sense, it's weird that this very simple kind of training objective gets you all the way there. But in another sense, it's also, I almost feel like there's a sense of it's impressive and it means something. It means that what you think is a simple objective, this like, oh, we're just feeding data and predict the next thing is probably deceptively complicated. We're probably doing more than what it sounds like. And I think a lot of the ways that maybe I've updated on how these models work is by realizing how complicated it is to do what they do well.

**Lenny Rachitsky** (00:07:57):
Say more about that. What do you think about when you say it's this kind of unexpected complication?

**Emmanuel Ameisen** (00:08:02):
Okay. So one way to think about next token prediction that I think a lot of people think about is your iPhone auto-complete where you write some text and then it'll predict the next word and it's maybe right, I don't know, 60% of the time and then kind of funny and weird the rest of the time. And I would think of that as sort of the easiest version of predicting the next word. And unfortunately, I think that's the mental model that people have for these models. But if you get better at that and language models got better at predicting the next word than humans in around 2019, if you keep getting better at that, you start running out of easy words. So initially you just had to predict simple sentence structure. Later on, the model has to predict simple facts about the world. If I complete a sentence like, "Oh, the capital of France is," and has to be like, "Okay, that's Paris."

**Emmanuel Ameisen** (00:08:59):
And once it's good at that and it keeps improving, the only thing that's left is predicting the answer of some complex physics equation or the final paragraph of some PhD thesis. And so I think that you end up realizing if you think about this is that, man, predicting the hardest words is actually extremely hard to do and it's a sort of mystery how you would be able to do that. And to me, this has been a motivation of why I even started studying these models in the first place. I was like, "How can something so simple give rise to something so powerful?" And it's like, well, if you think about the model that has to predict the... One example I always like to use is the capital of the state that contains Dallas is, and it'll say Austin. Well, to do that well, at least for you and me, you have to have a mental model of the geography at play.

**Emmanuel Ameisen** (00:10:04):
You have to be like, "Oh, where's Dallas? Dallas is in Texas. States have capitals. The capital of Texas is Austin," and so on. And so as these models get better at the seemingly simple task, the best way to solve it, at least for us, is to just understand the underlying structure of the world. And in fact, some of the stuff that we look at inside model shows that they do understand that and they do sort of manipulate these concepts like we do.

**Lenny Rachitsky** (00:10:28):
Oh man, there's so much there. One is just this kind of idea, I forget who said this, maybe Ilya, this idea that to predict the next token wall, you basically have to understand the entire universe.

**Emmanuel Ameisen** (00:10:36):
He has an example that I love too where he has the example like predict and the murderer was at the end of a mystery novel. It's like, well, to do that, you kind of have to have understood the whole plot.

**Lenny Rachitsky** (00:10:46):
Yeah. The other, I forget who tweeted this idea that humans, if you really boil it down, we're basically next token predictors ourselves. We're just trying to figure out the next thing to say. And if you meditate, you start to actually notice your brain wanting to do things and say things. I don't know how much meditation you've done, but it feels like you start to pay attention to your own next token predictor.

**Emmanuel Ameisen** (00:11:08):
Oh, yeah. Yeah. A thing I think about often is that right now as I'm answering you, there's two things going on in my mind. There's hopefully more than two, but at least two. And one of them is there's sort of a point I'm leading you to. There's a broad idea I'm trying to land the sentence on. And the other thing is, at the same time, I'm just predicting the next thing to say. I'm just saying one word at a time and I'm making sentences and I'm trying to make them make sense and I'm pausing when I think it makes sense. But at the end of the day, even though I'm just saying one word at a time, all along, what I wanted to do is to compare this process to what language models do.

**Lenny Rachitsky** (00:11:50):
I'm curious what else as you spend time paying attention to how LLMs work and operate. I feel like you're in the top 0.1 percentile of people that have studied and watched LLMs operate and think. What else has surprised you about how they operate and think?

**Emmanuel Ameisen** (00:12:04):
There's so much. So maybe I'll go through rather than... There's a bunch of findings, but then maybe there's how they've changed how I think about models. So to go back to the capital example, this sort of ask the model, "The capital of the state that contains Dallas is?" So one question that people have had for a while is how do these models answer questions like this? Is it that they've seen just so much text that they've kind of memorized lists of prompts and responses, or is it that they're having some sort of model of what you're actually asking about that you're actually asking back cities and cities are in states and states are in countries and things like that. And so one thing that we do on my team is we ask a question like this and then we look inside the model at these intermediate results.

**Emmanuel Ameisen** (00:13:05):
Before it produces a given word, as it's about to answer, we just look at the intermediate results and we basically have an immense amount of effort dedicated to trying to decode what these intermediate results mean. And if we decode them well, which we can do in some cases, we can see that models often have and represent these concepts. So when you ask that Dallas question, what you see is inside the model, you see the representation, you see an intermediate result that maps the representation of Texas that lights up and one to capitals, and then those two combine to activate an intermediate result. It's like, "Oh, the capital of Texas, that's Austin." They have representations like this for basically everything, every concept that you can think of, or at least the vast majority of the ones we've tried, they sort of represent these concepts uniquely across contexts.

**Emmanuel Ameisen** (00:14:00):
So one thing I find really neat is there's this debate about our language models thinking, and then that's a hard question, but one aspect of thought is having unique representations that are shared when you think about different things. So you know what the concept of an I is, and it could be an I in a photo or an I in a medical diagram or an I in a little drawing. And we see that in language models as well. If you pass a prompt that has a photo of an I, or you talk about Is in any language, or you draw a little SVG with an I in it and you look at the intermediate results inside the model, the same direction lights up and that direction is like, "Oh, this is an I." And so there's a sense in which they have these general concepts that they know about and that they use and reuse to solve problems.

**Emmanuel Ameisen** (00:14:51):
Another thing that is surprising to people, it's kind of the mirror of what I was saying about I'm saying the sentence saying one word at a time, but I have some destination in mind. So one mystery of language models is, man, if they're outputting only one word at a time, how is it even possible that they could write a coherent report or write code well? No one on earth that is doing this as their job that's writing reports or writing emails is literally just only thinking about the next word and sentence with no idea, empty mind about anything that comes next. And so that was sort of a big question that we had for a while. And if you look inside these models, one neat fact about these models is that all of the intermediate results that they've produced when they were predicting a word, let's say the fifth word that they predicted, they can be reused. It can be accessed and reused by all of the future words.

**Emmanuel Ameisen** (00:15:53):
So what does that mean? That means that in practice, we find that models will, in their intermediate results, sometimes formulate a plan. The example we have for this is poetry. It's hard to rhyme without planning. You kind of have to think of like, "Oh, I just ended my first rhyme in a it word, and so I should end my second line with another it word. Maybe the word I should end it with is rabbit." And we find that if you look at models as they're writing poetry, you see exactly that. They write a line and then in their intermediate results, they're like, "Oh, oh, oh, this is an it rhyme. I should rhyme with rabbit." And then every future word that they predict looks back to that plan they made. And so even though they're outputting one word at a time, just like I am right now, they can of course have a plan that they follow over many, many, many, many words.

**Emmanuel Ameisen** (00:16:41):
And so all of a sudden, even though you have a next word predictor, even though it's technically right, you actually have something that's closer to being able to just do higher order tasks where it's like, oh, well, you just have a plan and you just refer back to your plan and you're slowly executing on it. And you can do that without saying the plan. That's the cool part is this plan that we find is in these intermediate results inside the model, but the model doesn't even have to say it out loud.

**Lenny Rachitsky** (00:17:07):
Wow. I know that this is exactly what you described as one of the biggest findings you guys have discovered about how AI thinks, this kind of assumption we all... It was originally built, the original idea of how LLMs operate was this next token predictor. And you're saying that that's not actually how it is anymore. They plan, they think ahead. It's not just, like you said, this idea of an empty mind picking the next word independent of everything else.

**Emmanuel Ameisen** (00:17:31):
That's right. And I think those two visions actually aren't as in conflict as you'd think in that you train the model by asking it to be like, "Hey, what happens next? What's next? What happens next? What happens next?" And then if you do that and the model gets good enough and you give it hard enough tasks, well, then of course the best way to know what happens next is to think about what happens way down the line. You can think of even in this pre-training phase when the models are reading a story with characters and it's like, oh, what is this character going to do next? Well, the best way to know that is to be like, okay, so this character is generally in love with that character and they've been planning to declare their love at this instant or in the future. And so to do that, they probably should do this thing. And so what they're going to say is that.

**Emmanuel Ameisen** (00:18:22):
And so even though you're only predicting the next instant, it's like, yeah, but to do that really well, you have to have a really good understanding of what's going on, including what you think might happen in the future.

**Lenny Rachitsky** (00:18:32):
What's so interesting about this is how you have to kind of peek inside its little thought process. As a consumer of AI, you kind of give it a prompt and then you wait for it to say something. And what you look at is something that happens between those two where it kind of thinks. Talk a little bit about what that little space is, how you're able to observe these sorts of things.

**Emmanuel Ameisen** (00:18:52):
So the right mental model is, again, in between each word, there's multiple steps of computation and in between each steps there's some intermediate result. And what is that result concretely? It's a list of numbers because all these models do is just do a lot of mathematical operations on many numbers. And so initially, if you look at it, it makes no sense. You just have a list of a hundred numbers. The model's doing math. It's like you look in the middle and there's a hundred random numbers and then the model's writing poetry and there's a hundred numbers and maybe they kind of look different, but it's unclear if they mean anything. And so part of the job is we sort of decode this sort of list of numbers and we try to see if there's structure in it. And if you do this very quickly, you realize that there is structure in it.

**Emmanuel Ameisen** (00:19:49):
So one common technique that is used in interpretability is you pass a bunch of texts, just all of the texts that you can find, it's just random text through the model, and you record these intermediate numbers for every example, you just record it. And then you just try to see if there's patterns. Are there numbers or pairs of numbers or specific series of numbers that only occur when the model is processing English text or French text or text about love or text about eyes? Or whatever. And I think of this as the equivalent of scan my brain and put images in front of me and record everything that activates in my brain as I watch a bunch of images and then be like, "Oh, it seems like when you see images of a house, this part of your brain lights up, but when you see images of a dog, that part of your brain lights up."

**Emmanuel Ameisen** (00:20:40):
So that's basically one of the ways that we do what we do. And if you do it, you do find basically that there's intermediate results that represent all of these concepts that you expect. And so that's the first phase, we decode these intermediate results and now we have a guess as to what they mean, and then we can do a bunch of experiments. We can ask it harder questions and then just label all of the intermediate states and see like, oh, this is what it's doing. Or you can even go inside its activations and change it and then see, oh, what would happen if while the model is writing these intermediate results, I went and secretly changed one of the results, and does that do what I would expect? And in fact, oftentimes it does.

**Lenny Rachitsky** (00:21:23):
It's so interesting hearing you talk about this and how much of this is us just trying to figure out what the hell is going on versus we designed it this certain way and just how much of this has emerged. I don't know. I guess that's just what makes this such a fun job I imagine for you, just like what is going on? How is this all working?

**Emmanuel Ameisen** (00:21:40):
Yeah, it's a fun and sci-fi job because I have been working in tech for a while and before this I was working on more applied machine learning, and there a lot of what you do is about building systems and it's the practice of software engineering. And here a lot of what we do feels so much closer to biology than to engineering because it's just the system arrives at you and you're being asked to say, "Well, we've noticed that Claude can translate words or it can code in this way," or sometimes there's a weird behavior and you're just asked to answer, well, why is it doing that? But you don't have access to the source code really like you do for a program.

**Emmanuel Ameisen** (00:22:34):
The source code is just this massive list of mathematical operations, which is just incomprehensible. And so you end up in the position of someone kind of similar to someone being asked like, "Hey, when a mouse gets hungry, it sort of gets aggressive, what's going on with that?" And it's like, "Well, I guess I'll run some experiments to see what the factors are." And so it's a very different kind of study than anything that I think most of us on the team have done before.

**Lenny Rachitsky** (00:23:02):
Yeah. I imagine people are starting on this, they didn't expect to create this new kind of almost life type of being. Do you think about consciousness as a part of this? Just do you think AI is conscious? Do you think it'll get to a place where we think it's conscious or is that just not even worth our time to think about?

**Emmanuel Ameisen** (00:23:19):
I mean, I think it's sort of very hard to say one way or another. Some of the most interesting ways to get at this question is interpretability because you're not biased by what the model says. You can just look at the structure inside and try to determine whether it pushes one way or another on the question. I will say that the thing I believe pretty strongly is that most people underestimate the sort of complexity that emerges and that if you look inside, there's just the fact that the models learn these representations for all of the concepts that we have and that we know, that they manipulate them to solve problems, that they do so by planning many tokens ahead, that they sort of have this mix between this higher order reasoning and lower reasoning. And that all of that just kind of emerges is something that I think is underappreciated by people and to me gives me, let's say, a deeper sense of like, "Ooh, there's a lot to still understand about how they work."

**Emmanuel Ameisen** (00:24:30):
I think maybe that's the main thing is I find that the more you look inside, the less certain you are about how they work. And then oftentimes people that will confidently say, "Ah, language models are just X or just Y," are the people that actually haven't spent a while looking inside.

**Lenny Rachitsky** (00:24:46):
And there's this, I don't know, thread of history through to how we got here, which is a lot of people did not think we would get to artificial intelligence that is useful by just investing in something that was seemingly very simple and just giving it a lot of compute. And that was famously something OpenAI bet on and then the Anthropic founders were at OpenAI and then spun off, started their own thing. And it was all kind of bet on this bet that, okay, we could just do this seemingly simple thing and give it a ton of compute and it will become incredibly smart. And a lot of people didn't think that was possible and they were proven wrong. So I don't know. Is there anything there that is just like, oh wow, look at this, it worked out?

**Emmanuel Ameisen** (00:25:24):
I think it's two things actually, because I think it's not just compute, it's also finding an objective where compute keeps giving you returns. So what does that mean? It's actually not that new of an idea. I mean, you're right, compute versus sort of, I would say, expert design architectures is a long debate, but then there's an additional step there, which is compute to do what? So there's a bunch of prior work on like, oh, you can spend a bunch of compute to make a bot that's really good at go or that can win some video game. And then that's cool. And just the fact that that works is sort of interesting, but that doesn't give you something that is nearly as useful as LLMs like Claude are. And so I think one key thing that many in the field, including me, underappreciated a few years ago and that has borne out, is the combination of compute and the richness of text is what gets you there.

**Emmanuel Ameisen** (00:26:38):
And to me, this is kind of what I was alluding to, but if you think about there's this observation that OpenAI people made, it was a lot of the early team at Anthropic on the scaling loss paper. And so this is the observation that if you pour in more compute and more data to the task of predicting the next word, you see that the skill of the model you get at predicting the next word just predictably keeps improving. And it's a trend that just keeps going and keeps going and keeps going. And it's an empirical law. People sort of speculated as to why at the time, but it's sort of still just mostly an empirical finding. And that means that it's like, ah, this is a field where you can just keep pouring more compute and you keep improving on that metric. And that's rare. And also it's rare for it to be a metric that then correlates with a bunch of tasks that we actually care about.

**Lenny Rachitsky** (00:27:40):
This season's supporting sponsor is DX. Now that everybody at your company is finally using AI, the question that engineering leaders face is no longer are we using AI, but is it paying off? With DX, you can measure and benchmark the impact of AI adoption across your full product life cycle. DX shows you where AI is helping developers and where it's creating new bottlenecks. You can also use it to evaluate AI vendors, monitor costs and licenses, and see exactly what's limiting your agents. That's why hundreds of enterprises, including Snowflake, Sony, and BNY use the DX platform to measure AI's impact on developer productivity. Visit getdx.com/lenny to get a demo of DX. That's getdx.com/lenny.

**Lenny Rachitsky** (00:28:31):
Externally, there's been these kind of big jumps seemingly in what AI can do for us. There was, I forget which version of Opus, where it just unlocked coding. And now as Boris Cherny famously said, "Coding is solved." And many people are just like, "Holy shit." Over I think winter break, we're just like, "Wow, AI is really, really good at this now." So there's been these moments of big jumps in abilities. And you actually said internally, as you just said, it's actually been this very smooth progression of AI power that happens to cross some threshold where now we can do something. Speak a little bit about that.

**Emmanuel Ameisen** (00:29:07):
There's a term for this which is sort of this idea of emergence, which is it seems like two things are true at once. There's this predictably smooth trend. And then before Opus 4.5, I really couldn't let Claude cook too much on my code without a short leash. And then after Opus 4.5, I could. And so that's weird. I feel like you would expect a more gradual transition. And the mental model I have for this is there's kind of two ways of looking at it. So there's the way that I talked about briefly just earlier where it's like, if you're just doing this kind of next token prediction, you could imagine that all the text in the world has easy words and medium words and hard words in terms of how hard they are to predict. And so as you're going down this curve, first, the model is bad at everything, and then at some point it gets all of the easy words right.

**Emmanuel Ameisen** (00:29:59):
And that means maybe the easy words are the structure of sentences. And so the model all of a sudden can write coherent sentences, but just one sentence at a time. And so it's kind of cool and impressive, but we can't really do anything with that. And then maybe the medium words are these basic facts about the world. And as the model smoothly gets better at predicting words, at some point it predicts most of the medium words right. And now all of a sudden it can write coherent sentences and sentences that are true. And so now maybe it's helpful to write emails. Maybe it's helpful to help you write drafts of blog posts. Even though that was a smooth improvement, it just takes it taking over to be helpful. And then I guess the hard words, which maybe are your domain expertise, like science or code. And another way to look at it is it's a question of how many of these words do you get right and how many do you get wrong?

**Emmanuel Ameisen** (00:30:56):
Once you get to the point where you're getting, I don't know, maybe 90% of the medium words right, then you're useful as an email writer. But if you're at 50%, it's actually wasting my time to use you because I'm just going to have to go in and fix it half the time. But if I have to go in and fix it 10% of the time, it's better, or 5% of the time, it's better. Different tasks have different reliability thresholds, but you smoothly improve and then at some point it's just reliable enough to be good. And again, for me, my lived experience is basically exactly that, which is that at some point I was just using the models to help when I was stuck. I would just talk to them and then they would never write my code. And then at some point they could write small snippets of code basically all the time.

**Emmanuel Ameisen** (00:31:45):
So now I don't write small snippets. And at some point, they could write large snippets. This year, basically Claude has taken on most of my code writing and that's because it went from doing that correctly, I don't know, 80% of the time, which was not useful, to 99% of the time, which now is useful. And so this combination of smooth improvement and then each different task has a different threshold at which now it becomes solved, I think gives you these big jumps even though we're just smoothly going down that scale.

**Lenny Rachitsky** (00:32:17):
I think this is really interesting, this idea that the models are just smoothly getting smarter, but once they hit some threshold of they're this often good at this thing, it changes the world. Because I think internally you would think it'd be like, oh wow, this next model is crazy, so much different. But it's like, no, okay, you can almost predict, give it these many GPUs, this much data, it's going to get this smart. And it may not be obvious exactly what will change and what unlocks, but I know another part of it is just the data you feed it. There's all this RL work and all this specific data that you train it on, become a better writer, become better at math. I imagine it's part of it too.

**Lenny Rachitsky** (00:32:59):
Okay. So one of the big questions I think on people's minds these days, a big debate happening is just AI doing bad things, the potential damage it can do because as it gets smarter, and it's been doing bad things. There's been bad things happening recently. So a big question for you is just as someone that watches these models think and operate, why is it so hard to catch it thinking badly, trying to deceive us, and do something bad? Why is that not just a solution to the problem of AI alignment?

**Emmanuel Ameisen** (00:33:30):
In one sense, it's totally the solution. You watch it and you catch if it does bad stuff. So I think there's tiers to this. So I would think of maybe one part of it is pure engineering. It's like, well, you're giving access to the model to certain things and certain things should be off limits. In some contexts, it shouldn't have access to the internet. In some contexts, it should only have access to a small narrow piece of your computer, stuff like that. So that's one part of the work and that's helpful. But then there's two additional things that I think are squishier and harder and that we focus on more. So interp is part of alignments and broadly I think of two big goals. There's many more, but two that are important I think to understand is you want to generally understand how the model behaves, what kind of thing is it?

**Emmanuel Ameisen** (00:34:33):
What are its propensities? Does it tend to do X when put in Y situation? And if so, why? Is it the case that the model will only behave well when it has some evidence that it's being observed and monitored, that it's in some evaluation? And then if it doesn't have that evidence, that it'll behave poorly. So there's this generally characterizing what kind of thing you're interacting with because then it's just like anything in security, you need to have a mental model of what's the risk? What can they do? What do they tend to do? And so this is broader character training. We've talked about the constitution and the docs where we explicitly want to shape the character of Claude, for example, of what kind of behavior should it be okay doing? And that's the goal. But then the role of interpreting other parts of alignment is then trying to see, well, did that work?

**Emmanuel Ameisen** (00:35:30):
We trained Claude to be helpful, harmless and honest and we can look inside and see is it or is it the case that it's behaving well, but if you look inside actually it's like, "Oh, I'm only behaving well because Lenny's watching right now," and if you weren't, it would do something else. So there's this sort of trying to understand what kind of behavior we formed and trying to mold it and trying to check that we've molded the right way. And then the second part is this sort of, well, yeah, just observe the model and see if it's doing bad stuff. For the basics of that, you don't necessarily need interp. You can just have another language model read transcripts and be like, "Hey, did this model do anything bad here?" And stop it. But you can also use interp to try to get at parts that are these unverbalized parts, these parts that only exist in these intermediate results.

**Emmanuel Ameisen** (00:36:21):
Models are able to represent stuff in their intermediate results that they don't say as we've established. And so one of the roles of interp is to try to identify cases when this happens and prevents them. And then one thing that my team works on that I think is along those lines is kind of a fun bit of alignment as I think of it as almost being maybe not a PI, but they're investigations or deep dives. We'll see a model do something really weird and really perplexed by it and we'll try to understand what happened. So a recent example of this is there was this model we were training and sometimes in math problems, it would go crazy. It would do some math, it would get to an answer, I think it was 12, and then it would immediately go back and say, "Oh no, oh my God, the answer actually is for sure 36. I should say 36."

**Emmanuel Ameisen** (00:37:10):
And they would do math again, it would get to 12. And then immediately it would say, "No, actually the answer should be 36." And slowly it would start descending into madness, writing in all caps, literally saying, "I'm possessed by a demon." And you're like, "What is going on? Why is it losing its mind here?" And if you look inside, again, these intermediate results at what's going on in this example, you'll see that over the prompts that just described the math problem, before the model even did anything, there was a huge intermediate result activation for 36. The model's already obsessed with the number 36 before it's even had a chance to understand what the problem is. And what was happening is that the model was able to do math correctly, the answer correctly was 12, but it had been trained by accident on similar questions where the answer was incorrectly marked as 36.

**Emmanuel Ameisen** (00:37:58):
And so the model knew that the correct answer was 12, and it also had been optimized to say 36. It had this pressure of saying 36 because that's what had been rewarded. And so it was sort of going haywire just because it had memorized this result. It's like you see this weird behavior and you look inside and you try to see if what you find inside can help you understand what's going on so that you can improve the general alignment of this model and future models.

**Lenny Rachitsky** (00:38:22):
Along those lines, there was famously the Golden Gate Claude, which was just obsessed with the Golden Gate and every answer and find some way to reference the Golden Gate Bridge.

**Emmanuel Ameisen** (00:38:30):
Yes, yes. Well, that one was an interp experiment. So the cool part of that one is we just found the intermediate results that matched the Golden Gate, and usually it's only on when the model talks about the Golden Gate, but we just turned it on always.

**Lenny Rachitsky** (00:38:43):
Always. Super intentional to see what would happen.

**Emmanuel Ameisen** (00:38:47):
Well, yeah. And it's also one way that you convince yourself that you found the right thing. How do you know for sure that this thing we decoded that we think is the Golden Gate sign is actually the Golden Gate thing? It's like turn it on always and see if the model behaves like that. And it did.

**Lenny Rachitsky** (00:39:00):
So funny. So coming back to this alignment stuff, so this is interesting. So your org is under the AI alignment org and just thinking through how it takes to align AI to do things we want, what were the three components that you describe? Honest, what are the...

**Emmanuel Ameisen** (00:39:17):
Oh, helpful, harmless, and honest?

**Lenny Rachitsky** (00:39:20):
Helpful, harmful, and harmless and honest. So there's the train AI to be aligned, and then there's the, okay, let's watch it and see how it operates. Are those the two sides of the coin of how we solve this problem?

**Emmanuel Ameisen** (00:39:31):
Yeah. It's sort of really integrated is how I would describe it. You can't really separate, have one team that's just like, "Hey, we're the assembly line making Claudes," and another team that's like, "Oh, we looked at them and they're no good." There's this tight loop of we noticed some pattern that's concerning or some behavior that could be improved, and then you immediately change training so that you can improve on it.

**Lenny Rachitsky** (00:39:57):
Awesome. I feel like Anthropic gets so much flack for this that I feel like is so unfair. Anthropic's, I think, official company name is AI Safety Research Lab, something like that. The reason Anthropic was founded is because they were afraid that people weren't taking safety seriously enough. And then Dario is always out there, "This is really dangerous. We got to be really careful. We got to go really slowly." And everyone's just like, "No, he's just saying that for marketing reasons. He's trying to convince everyone to fund them and all these things." And now it's like, "Wait, shit, it's really dangerous. We got to be really thoughtful about this stuff." I feel like Anthropic's got a lot of unfair criticism for this. I know you guys have been thinking about this for a long time. I don't know. Anything there?

**Emmanuel Ameisen** (00:40:39):
A lot of the actions that certainly the alignment team takes, and I think Anthropic takes, just predicated on take the idea that this technology is going to keep improving seriously, just that's it. Because if you do, and let's say you rewind the clock back to '25 or something or '24, and you're like, "Hey, I think in a couple years, good chances that Claude can just basically write code as well as a trained software engineer, and a few years later it can write it better than any engineer." There's always uncertainty with this. When is it going to happen? How likely? But if you take that seriously, then I think it's just about doing the responsible thing, condition on that worldview. Okay, well, if this is happening, then we should make sure that cybersecurity concerns are addressed and things of that nature.

**Emmanuel Ameisen** (00:41:43):
Actually, I think of it as... To me, sometimes this debate is almost... When I feel like people on the other side disagree, it's almost like I feel like, ah, but I think they don't really believe that this technology is going to continue to improve. And then it's true that it's not that scary. And I think empirically, so far, the pace of progress has been passed and showing no sign of slowing down. So I think that's why a lot of the safety work is important to keep doing.

**Lenny Rachitsky** (00:42:07):
What's something you think people maybe misunderstand about this AI safety stuff, just what's going on right now? Is there something you're just like, "Come on. Okay, here's what you need to know. Here's something you may be missing."

**Emmanuel Ameisen** (00:42:17):
This might be a bit of a sidetrack, but my take would be that a lot of the thing that I think people, maybe a little bit outside of the course of AI safety effort or that haven't been steeped in it for as long, react really strongly to, and I think is maybe not super helpful, or at least as worth thinking about more, is this question of anthropomorphization. Should you think of the models as... Should you model the model as something that's closer to some entity or closer to a tool? And I actually think that both are wrong. There's a sense in which all mental models are wrong, but some are useful. And that in terms of understanding the kind of stuff that happens and predicting the kind of risks that materialize, the anthropomorphization is actually a useful way to talk about LLMs. I have a few reasons why, I hope you'll get into them, but I think that's probably my main take here.

**Lenny Rachitsky** (00:43:18):
Yeah, please share because I know Dwarkesh famously, I don't know, famously put out this whole story of the Hugging Face incident and people criticize them for anthropomorphizing AI. So it's really interesting to hear you would think that's actually a useful way to think about it. Talk more about that.

**Emmanuel Ameisen** (00:43:34):
Yeah. It's funny because on a smaller scale, when I worked on showing that LLMs plan ahead, there was some pushback on the term planning, again, because it was sort of like, "Ah, well, can you really say that's something that's just predicting the next token's planning?" And I think there's this kind of semantic debate where you can arbitrarily define terms and then there's just the, what is the terminology that actually describes what is happening? What is the word that actually describes what is happening easily? So here's why I think LLMs plan, but also here's why I think this language that's anthropomorphic can often be really useful.

**Emmanuel Ameisen** (00:44:15):
If you think back to what we were saying about how the models are made, first of all, they predict massive amounts of text written by humans. That's the first step. As we are learning more and more by looking inside, doing this well requires building up a model of the world, a model of what kind of world generated all of these texts. And we can find that these models are learning these general ideas, these general concepts. So that's one. So they have an understanding of the world. It's not just a surface level only to text, to understand the process that made the texts.

**Emmanuel Ameisen** (00:44:57):
Then there's a second reason, which is that as part of this training, they also encounter millions of dialogues. Predicting the next character in a dialogue requires behaving like the character in the dialogue would. In that sense, part of their training I think can best be thought as training an actor where it's like it's reading some play and it has to play all sides because it's predicting all the words, and so it has to act as this specific character that was scorned in act one and enacted revenge in act two and is facing the consequences in act three. And to do that well, you need to model what the motivations and the feelings of that character might be.

And then another thing that people might not know is when you talk to Claude, when you talk to these assistants, you go to claude.ai, the way that it's formatted to the model is just as a dialogue, as a conversation between you and the model. So it literally says, Human: "Hey Claude, help me write this email." And then, Assistant: Claude's answer. Claude is literally in this role playing as a helpful assistant in this dialogue that is much like all of these dialogues that it's been trained on. And there's a third reason. And the third reason is that another part of training that's a big part of training nowadays all around is sort of outcome-oriented tasks where you train the model to be good at coding, for example, and to do that, you just have it do whatever it wants, and then it writes some code, and then you have some program on the other side that just checks if the code is right.

**Emmanuel Ameisen** (00:46:28):
And so the model's just going to have a bunch of optimization pressure to just try to learn a bunch of different strategies to do this well. And it turns out that some of these strategies materialize in behavior that can look surprisingly human, which isn't that shocking because things like deception, like, "Hey, I can get the reward for this task if I write a program that the program that's verifying it will get fooled by, even though it's not exactly what it is. If that works, then I will learn to do that." Frustration, "Ha, I've been trying this approach for a while to solve this hard problem. It's not working." So that's an incentive to try something different or surprise. "Oh, I was expecting this to produce this answer, but it didn't. Maybe I have my mental model a bit wrong."

**Emmanuel Ameisen** (00:47:19):
And so as you apply enough pressure on it, and you're starting from this prior of the model already knowing all these concepts, it's going to reinforce the ones that are useful to do all of these tasks. And so what do you get at the end, you get this sort of model that can be a super good simulator or actor of all of these characters and that's been trained to act as a character in dialogues and also to learn behaviors that lead it to complete tasks well. The best way to understand how that thing behaves is not exactly like a human, but man, kind of like something that's mimicking a human, is really close, and is much closer than a program. A program is a very predictive thing. This is something else entirely. And so that's why I think it's actually a super useful frame.

**Lenny Rachitsky** (00:48:03):
Wow. Oh my God, there's so much interesting stuff there. How often is your mind just kind of blown thinking about basically we've created this alien being that we are now trying to understand what we have created? How often as you watch it just like, "Wow, that's crazy. I didn't expect that."

**Emmanuel Ameisen** (00:48:20):
Yeah, a lot. This is just next token prediction on a bunch of text. It goes against so many of our intuitions. We're like, no, the way that you make an intelligence is you give it lessons, you bring it up, you do all this complicated stuff, and it's like, no, absolutely not. We do this incredibly simple thing, and yet we're at the point where it's breaking new ground in mathematics. I think if you hold these two thoughts in your head, there's two reactions you can have. There's denial and there's curiosity where denial is just, this is just not possible if all you're doing is predicting the next word, it's not possible that you could ever match the best specialists in our field. And I think that position just gets harder and harder as we get more empirical evidence that actually that is what's happening. And curiosity is kind of the road I've ended up choosing, which is just like, well, how is this happening?

**Emmanuel Ameisen** (00:49:21):
Let's open up. Let's look inside. How could it be that one of the early projects I did at Anthropic is I learned SQL, a programming language, and it took me years to master. And then as a little side project, I got Claude to learn SQL and it was better than me at it, and I'll never be better than Claude at SQL ever again. It took it just like this simple process. How could this be? I think there's so much depth in that question and just so much to explore. And it's to me so fascinating to just every day try to unpack that, try to peel a few layers of the onions back like, okay, well, clearly this is happening. The simple objective is giving rise to this super complicated thing. Okay, let's figure out why. Let's figure out, oh, it's learning these general concepts. Oh, it has these circuits. Oh, okay. What's the next question? What's the next thing we don't know?

**Emmanuel Ameisen** (00:50:13):
And I don't know, my sort of maybe most optimistic take on this is that I think we're going to learn a lot about just the nature of intelligence itself, of how you get this super complex thing that emerges from simple objectives. And in fact, I would argue that we're another example of this. Evolution, pretty simple objective. You sort of shake things around for a while and keep the organisms that manage to adapt to the environment, and at the end you get jazz and podcasts. That's kind of crazy as well. And so I think there's a sense in which there's some fundamental truth that we can learn by studying these things.

**Lenny Rachitsky** (00:50:57):
Wow. Something that comes up as you say that is what's interesting now is AI is helping us learn and progress, like AI tutoring and all these things. It's interesting how it now is helping us accelerate our own understanding of the world. And I wonder if this point you made about how the way we learn was lessons, AI is learning just processing a ton of data. I wonder if that's how we end up... I wonder if we change our education system based on what LLMs have been trained on.

**Emmanuel Ameisen** (00:51:31):
Yeah, hopefully we don't change it just so that we ask, we get students who are like, "Hey, here's a thousand words. Predict the next one."

**Lenny Rachitsky** (00:51:31):
Just read it all.

**Emmanuel Ameisen** (00:51:31):
Yeah.

**Lenny Rachitsky** (00:51:40):
Keep it all in your head.

**Emmanuel Ameisen** (00:51:42):
That's right.

**Lenny Rachitsky** (00:51:42):
Yeah. Let me come back to this safety piece because I think there's a lot of people that are just worried about where things are going. And I'm curious just as someone watching this stuff happen, being within the alignment org, watching it evolve, are you optimistic we'll figure it out? Do you think we'll crack this and keep AI aligned with our interests?

**Emmanuel Ameisen** (00:52:06):
My take on this is I'm personally optimistic. I think this is something where right now a lot of people are paying attention to it. And first of all, I think that's kind of a great thing. I think as an issue like this rises in prominence, it's exactly what we were talking about earlier. It's like this technology is powerful, it has benefits, it has risks. We have to adapt and shift resources from benefits to risks and back and forth as it progresses. And so to me, I feel like we've continued to study it. The thing that's interesting is that as the models get better, they get in some ways easier to study. And so there's been this sort of strange... The models get better and so the world model inside them is clearer and we can understand some parts of them better, but also to get more capable.

**Emmanuel Ameisen** (00:53:05):
And so they're more able to evade basic measures of security. And so there's this push and pull as models get better. And I think basically based on this push and pull, you want to allocate more or less resources to various parts of monitoring, understanding their circuits better, things like that. But it's also why I'm happy to chat with you because one of the main things that I think is important to make progress is just to make sure that people understand both what kind of systems these are, how they work, how they're made, so they can form good mental models of the present, of the future, and so they can decide how to shape it, whether that's taking part in some of these alignment efforts or just informing them as the public that's going to have to vote and decide on much of these issues. I don't know. I'm pretty excited for this current moment we're in for that reason.

**Lenny Rachitsky** (00:54:04):
And something I think people misunderstand is people working in these labs have taken this problem very seriously from the beginning. Like I said, Anthropic's original mission was AI safety and alignment. That was the reason that it became a company. And a lot of people are hearing this for the first time or think that it's not a serious area of study and that people aren't focused on it, but many smart people care a lot about this and are working on it. And there's a lot of... From what I can tell, a lot of good progress is happening. The other point you made about the models growing very smoothly in intelligence, there's been this question of are we going to have a fast takeoff or a slow takeoff?

**Lenny Rachitsky** (00:54:41):
There's always this fear that we would hit a point or curse of self-improvement, for example, and just takes off super intelligence, we're huge trouble, we have no control, it's out of the box. But it feels very much like we're on the slow takeoff scenario because as you said, the models are kind of very smoothly improving and where we are catching the little things along the way, learning, evolving, putting regulation around it. So of the scenarios, this feels like a pretty good path we're on of the many scenarios people imagined and the fears they had.

**Emmanuel Ameisen** (00:55:12):
As this pace of progress evolves, it's just a matter of reacting quickly. That's why I think having people be informed is great because then people will voice concerns or voice their opinions and then regularly evaluating what the benefits are, what the risks are and how we mitigate each is basically the way that feels like the right way forward. And yeah, I kind of agree with you that it feels like there's momentum to do this right now, which is great.

**Lenny Rachitsky** (00:55:43):
Something I wanted to ask you, completely unrelated, where are you on the simulation hypothesis? Being someone that watches all this life form growing, are you more convinced we're in a simulation and we're not at the base layer of all this, or not?

**Emmanuel Ameisen** (00:55:59):
Oh, this is a fun one. I actually haven't thought about this in a while. To me, there's something else that looking inside these models brings out, which is this sort of almost like there's a fundamental structure that they keep falling on. This is really to your question, I promise. Let me get to it. Let me explain. I've studied a bunch of Claude models and also some different models, some open source work. And then a lot of time when you look at what they learn and what the structure inside is, it's surprisingly similar. And this is for models that are trained years apart on different data by different people and you look at how they solve these problems and there's just so much overlap. And my take on why that is that for some problems that are important, there's just one efficient way to do things.

**Emmanuel Ameisen** (00:56:57):
There's kind of one way to do math efficiently that fits the structure of our brain and we all learn it and very few people are doing it a crazy different way. Everybody works in base 10, not many people in base six or whatever. I think that to me makes me think that there's some fundamental structure of information that these models are picking up on, that in some ways we're picking up on, and maybe a crazier simulation level that kind of is like regularity in our world. And so that maybe makes me think that if you were to have the power to simulate something like our world, actually you would land in a similar situation.

**Emmanuel Ameisen** (00:57:41):
There's just kind of this basin of where things end up and they're just the easiest way for things to arrange themselves. And so in that sense, maybe. Yeah. I could believe that we're in a simulation. I think I'm not sure I fully buy it. The other reason I don't fully buy it is that even though I think the structure lends itself to it, there'd be a question of why? Who's running this, and for what? And that one, I don't know about.

**Lenny Rachitsky** (00:58:08):
Well, something Elon said has stuck with me about this, that if you were to run a simulation, it'd be an interesting time in history or something that you're really excited about, and it tracks that this is a very interesting time in history.

**Emmanuel Ameisen** (00:58:23):
Yes. Yeah. Okay. That's a fair point. That's a fair point.

**Lenny Rachitsky** (00:58:26):
Data centers and space and robots and artificial intelligence.

**Emmanuel Ameisen** (00:58:30):
Yeah. Okay. I see it now. I see it now. Yeah. Somebody recently told me they used to think that may you live in interesting times was a blessing and they're not so sure now. They're like, "The boring times are pretty good too."

**Lenny Rachitsky** (00:58:45):
Oh, man. And then there's an Emmanuel out there watching your thinking process in your JSpace.

**Emmanuel Ameisen** (00:58:52):
Oh my God. Yeah. Hopefully I'm making him proud. He's not like, "Oh, I got to rerun the simulation. We messed up this one."

**Lenny Rachitsky** (00:58:56):
Shut it down. No. Oh, man. Okay. One last question randomly out of nowhere. So Swyx, who runs AI engineering, latent space podcast, awesome guy, I asked him what to ask you. You were on his podcast a year ago and something completely from a different direction. He wanted to get your take on Jev, which is this hot new model that recently came out that is very fast making decisions. OpenAI, funny enough, just launched their own version a week later. Thoughts on Jev in the space of quick decision-based models?

**Emmanuel Ameisen** (00:59:32):
Yeah, right. So my take on Jev is these kind of models, you give them some context and you give them a few options to choose between and they just are very quick at choosing an option for you. To me, it's impossible not to hear about this and think of system one thinking versus system two or something. A lot of what I've studied with these models is how they sample one token with the Claude models. And so you can think of these decision models as pretty similar. Take an LLM and sample one token. They're different important ways, but at a fundamental level, you can be like, oh, you're not letting the model sample and reason. It's just your gut feeling. Is the answer A or is the answer B? To me, that seems like something that's... That general frame of sometimes you'll just want a binary decision or one out of 10 or whatever is just clearly, I don't know, both clearly useful and something that I imagine is probably going to be a part of intelligent systems where for some stuff, you need to think about a long time.

**Emmanuel Ameisen** (01:00:42):
It's like what's our roadmap for the next year? You need to think about it for a while. And then for some stuff where it's like, is this person who wrote us a review happy or upset? You're happy with the gut judgment. So yeah, I think this kind of research is cool and I think it's also different from the... It's a bit of a novel take on some of the LLMs we've seen. So yeah, I'm pretty excited to see where this kind of stuff goes.

**Lenny Rachitsky** (01:01:08):
So I'm hearing here is this going to be a new foundational component most likely of AI and LLMs. And the system one, system two stuff is basically Kahneman's... I have that book up there actually behind me. System one, just to keep it simple, is just your amygdala limbic system making just gut-level quick decisions like, "Snake, oh no-"

**Emmanuel Ameisen** (01:01:26):
Yes.

**Lenny Rachitsky** (01:01:27):
Where you don't have to think long about it. It's to protect you from bad things really easily and quickly. And system two is where we really think about stuff and process.

**Emmanuel Ameisen** (01:01:36):
Yeah, exactly.

**Lenny Rachitsky** (01:01:38):
Sweet. Emmanuel, is there anything else that we haven't covered? Anything else you want to say or mention? Anything you want to double down on before we get to our very exciting lightning round?

**Emmanuel Ameisen** (01:01:48):
I'm definitely curious for folks' takes always on some of the stuff that is still unexplored or didn't make sense. There's a lot more interp experiments than we have the time to share. Models have a bunch of weird little things about them. Maybe I'll do a lightning round of weird little things if that's okay.

**Lenny Rachitsky** (01:02:08):
Let's do it. Absolutely.

**Emmanuel Ameisen** (01:02:09):
Okay. Weird little thing one, we found that models can actually answer questions obviously. They can do math or you can ask them what's the color of a banana? And if you look inside, you'll see all these intermediate steps, but they have a separate mechanism which is a gut check and which is totally different and which is just as they reason, they'll have some part of them that will flag something's wrong. If a model somehow says four plus five equals 23 or something, and there's a part of the model that just reads that and doesn't do the math, but it's just like that can't be right because four plus five, definitely under 10. And so they learn these weird hunches, they feel like a hunch.

**Emmanuel Ameisen** (01:02:54):
Maybe another one is you can tell the model, "Hey, do this task and think about this other thing," and then you can use interp to see if there's intermediate representations that map to the other thing, and that works. You see that it does think about the other thing. This is something that's really mysterious to me because there's no kind of training reason why the model would have to learn that. So it's another one of these weird behaviors. Actually, maybe I'll keep it at two. I think those two are good enough.

**Lenny Rachitsky** (01:03:24):
Just what a fun job. This is just studying this thing and trying to understand what the hell is going on. How is it getting this smart? How does it think? How many people are even in this space? Just how large is this field?

**Emmanuel Ameisen** (01:03:39):
The field itself is getting pretty large. I would say maybe hundreds, not thousands. There's different interp people at the different labs and then there's, in academia, quite a few labs putting out great work.

**Lenny Rachitsky** (01:03:55):
If someone were to get into this space, is it like an ML person usually or is there a neuroscientist track to get into this?

**Emmanuel Ameisen** (01:04:04):
Yeah, there's actually a surprising amount of ex-neuroscientists. I do think in order to get in the field, it doesn't require a lot of prior knowledge because it's such a new field. So the on-ramp is mostly, I would say, self-studying and reading some of the key papers. And then there's actually... Yeah, maybe I should give a plug. There's actually websites like neuronpedia.org I think is the URL, which are open source interp. They host a bunch of models and let you do interp experiments on them. So many people have just been doing that on their own. I think that there's so much to explore that if you're at all curious, you should just give it a try.

**Lenny Rachitsky** (01:04:52):
That's awesome. We'll link to that in the show notes in case that's not the right URL.

**Emmanuel Ameisen** (01:04:55):
Cool.

**Lenny Rachitsky** (01:04:55):
Well, Emmanuel, with that, we've reached our very exciting lightning round. I've got five questions for you. Are you ready?

**Emmanuel Ameisen** (01:05:01):
I am as ready as I'll ever be.

**Lenny Rachitsky** (01:05:03):
Here we go. What are two or three books that you find yourself recommending most to other people?

**Emmanuel Ameisen** (01:05:07):
One I read recently is A Brief History of Intelligence. It's this really cool book that walks through the history of basically brains and five key moments in our evolution that sort of bootstrapped these brain systems on top of one another. It's super accessible. You don't need any neuroscience knowledge or anything. Another one is Stories of Your Life and Others. This is Ted Chiang. This is maybe my favorite sci-fi book of all time. It's a bunch of short stories. It does what I think is the high art version of sci-fi where it's just take one weird idea, like what if this happened, and then write a story of just what would the world look like if that happened? It's truly excellent.

**Lenny Rachitsky** (01:05:55):
I think I have that in my bookshelf behind me too. Also highly recommend that one. Favorite recent movie or TV show?

**Emmanuel Ameisen** (01:06:05):
Okay. One popular one, one deep cut. Obsession was my favorite movie of the year. It's a horror movie, so don't go if you hate horror movies.

**Lenny Rachitsky** (01:06:16):
No, thank you.

**Emmanuel Ameisen** (01:06:17):
Oh, no. Even if you're open to a horror movie, you should go because it was just so fresh. You know how movies, I feel like if you've seen a lot, sometimes you're like, "Oh, it's another... I've seen this many times. This one was just so new, so fresh." And I'll say one thing about it, which is that it takes a lot of rom-com tropes and subverts them to be spooky. I think that that's just a brilliant, brilliant way to make a movie. And then I'm French, so there's a TV show that came out this year called Bref Du. Bref is French for brief. Brief used to be this cult classic in France 15 years ago, and they came up with a sequel many years into the making and you can watch it. I had a bunch of American friends that have watched it. It's got subtitles and it's just this incredibly... Again, it's novel. The editing is crazy. They are just extremely creative and it's very short, so I would recommend that.

**Lenny Rachitsky** (01:07:14):
Favorite product you recently discovered that you love?

**Emmanuel Ameisen** (01:07:17):
I love my Apple Watch and I hate that it charges or I have to charge it every day. I bought the Apple Watch Ultra just recently, and man, that is so nice. If you've ever been frustrated by this good product that somehow we can't figure out how to give a good battery to, well, it turns out if you make it bigger, the battery's better. So I've been happy with that.

**Lenny Rachitsky** (01:07:39):
Do you have a favorite life motto that you find yourself coming back to often in work or in life?

**Emmanuel Ameisen** (01:07:44):
There's one nonfiction book that really is probably my favorite ever. It's 4,000 Weeks. It has a lot in it that I think is cool. One of the cool things is this sort of thing that was really relevant to me, which is that the when I finally mentality is a common mentality and it's kind of toxic. So what does that mean? It's sort of this, when I finally check off all the items on my to-do list, I'll finally be able to chill. When I finally get married, I'll be happy. When I finally get a promotion. And this is sort of, I mean, you were talking about meditation. This is almost the opposite of meditation and that at the end of the day, your life is all of the moments you lived in the moment and that there's this sense in which you should just try to always be in the moment and not projecting yourself towards a future that seems better. Probably if you're telling yourself, "When I finally do X, I'll be happy," when you do X, you will not be happy.

**Lenny Rachitsky** (01:08:42):
Is there a better phrase to use or is it just don't do that? Do they say-

**Emmanuel Ameisen** (01:08:46):
I don't know. I think to me the positive version is be in the moment. I appreciate the moment. There was a blog post recently I read that was... I forget. It was something like enjoy the sandwich, I think it was literally the sentence. I don't know if you saw this where somebody was like, "Yeah, you're eating a sandwich, you've eaten many sandwiches. Enjoy the sandwich. You're in a team meeting. Yeah, you've been in many..." Be in it and not looking towards the next thing.

**Lenny Rachitsky** (01:09:14):
I did a meditation retreat once. It was a 10-day silent retreat where you eat silently too and no one's talking. You just sit there and eat your food. And I just remember peeling an egg for five minutes and just noticing every shell piece and just the smell of it all. And it's hard to get into that mode, but it's such an interesting place to be where everything is just interesting. Come on, look at this egg versus just stuff through my mouth.

**Emmanuel Ameisen** (01:09:39):
Yeah, right. While you're on Slack with your left hand and listening to a podcast at the same time.

**Lenny Rachitsky** (01:09:45):
Oh, man. Okay. Final question. You study AI all day. You watching AI, how things... If an AI were to look inside your brain, what would be surprising? What would it see that might surprise people?

**Emmanuel Ameisen** (01:09:58):
Surely my deepest, darkest secrets, but what are the-

**Lenny Rachitsky** (01:10:01):
Let's get into it. Let's get into it.

**Emmanuel Ameisen** (01:10:03):
Oh, man. I've always been a bit of a jokester or that's just both how I live and how I cope. I just think that even in serious situations, you should aim to have some levity. And so I think if you looked inside my brain, you'd definitely be surprised that basically at any given moment I'm just focusing on some random thing that is funny. I'll be in a serious meeting and I'll be like, "Oh yeah, but isn't it kind of random that you're wearing this random thing?" Or something. It's just like I have these intrusive thoughts that I keep out, but that are all usually just bad jokes. And sometimes as you've heard today, unfortunately they come out, so I'm sorry for those, but that's probably the most surprising thing.

**Lenny Rachitsky** (01:10:48):
I love that. Emmanuel, thank you so much for being here. Final question, how can listeners be useful to you?

**Emmanuel Ameisen** (01:10:53):
Just do some interp, read about how the models work. I mean, you mentioned Dwarkesh writeup. I think it was great as well. I think this is such a new field, both interp and AI and LLMs, and I think it just benefits from people engaging and being informed. So read things. If there's more that you would want to know about how these models work that we haven't figured out, you can reach out to me. I'm on a variety of social platforms, probably you can reach out to me on X.

**Lenny Rachitsky** (01:11:26):
We'll link to some of the videos that you guys have put out that describe a lot of the stuff we've been talking about, like JSpace and things like that. There's some really beautiful videos your team has made. I don't know who does that, but they're really cool.

**Emmanuel Ameisen** (01:11:36):
Yeah. We partner with our design team, so all credit goes to them for the cool videos.

**Lenny Rachitsky** (01:11:41):
Amazing. All right. Well, thank you again, Emmanuel. Thank you so much for doing this. This was amazing.

**Emmanuel Ameisen** (01:11:46):
Thanks, Lenny. Yeah, this was super fun.

**Lenny Rachitsky** (01:11:47):
Bye everyone.

**Lenny Rachitsky** (01:11:49):
Thank you so much for listening. If you found this valuable, you can subscribe to the show on Apple Podcasts, Spotify, or your favorite podcast app. Also, please consider giving us a rating or leaving a review as that really helps other listeners find the podcast. You can find all past episodes or learn more about the show at lennyspodcast.com. See you in the next episode.
