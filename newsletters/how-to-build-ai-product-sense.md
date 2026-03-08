---
title: "How to build AI product sense"
subtitle: "The secret is using Cursor for non-technical work (inside: 75 free days of Cursor Pro to try this out!)"
date: "2026-02-03"
type: "newsletter"
summary: "A deep dive into The secret is using Cursor for non-technical work (inside: 75 free days of Cursor Pro to try this out!), covering Step 1: Download Cursor, Step 2: Create a new project, and Step 3: Continue this post inside Cursor."
tags: ["ai", "design", "engineering", "newsletter", "b2b", "leadership"]
word_count: 6851
---

*👋 Hey there, I’m Lenny. Each week, I answer reader questions about building product, driving growth, and accelerating your career. For more: [Lenny’s Podcast](https://www.lennysnewsletter.com/podcast) | [How I AI](https://www.youtube.com/@howiaipodcast) | [Lennybot](https://www.lennybot.com/) | [Lenny’s Reads](https://www.lennysnewsletter.com/s/lennys-reads) | [Favorite AI and PM courses](https://maven.com/lenny) | [Favorite public speaking course](https://ultraspeaking.com/lennyslist?via=lenny)*

*P.S. **[Insider subscribers](https://www.lennysnewsletter.com/subscribe?plan=founding) get a free year** of [Lovable, Manus, Replit, Gamma, n8n, Canva, ElevenLabs, Amp, Factory, Devin, Bolt, Wispr Flow, Linear, PostHog, Framer, Railway, Granola, Warp, Perplexity, Magic Patterns, Mobbin, ChatPRD, and Stripe Atlas](https://www.lennysnewsletter.com/p/productpass). Yes, this is for real. **[Learn more](https://lennysproductpass.com/).***

The post you’re about to read took over 100 hours to create. That’s because it’s not a post. It’s an open-source interactive AI experience that will help you build AI product sense. Tal and Aman ran dozens of usability sessions, wrote evals, optimized each prompt you’ll find below, and even partnered with Cursor to get you free credits (see below!) so that you can try this at home. I’ve never seen anything like what they’ve put together, and I’m excited to bring it to you.

Next week, in part two of this series, you’ll learn how to take this newfound AI intuition and apply it to your own product.

*For more from Tal and Aman, check out their in-depth workshop [Build AI Product Sense](https://bit.ly/4k8CLBp) (starting next week, get 15% off using this link) and their upcoming free Lightning Lesson [How to Know What AI Products to Build](https://maven.com/p/593d71/how-to-know-what-ai-products-to-build), in partnership with my one of my other favorite collaborators, [Hilary Gridley](https://www.linkedin.com/in/hilarygridley). You can also book Tal and Aman for a [build sprint with your team](https://buildaiproductsense.com/).*

![](https://substack-post-media.s3.amazonaws.com/public/images/fce07243-d494-4f0a-b65b-3f70f90c987e_1456x970.png)

You’re in a product meeting and someone mentions “subagents” or “context engineering” or “agent memory.” You nod along. You know what these terms mean . . . you’re just hoping no one expects you to use them in a sentence.

You’ve watched the video explainers, bookmarked the infographics, vibe coded a few apps, and even shipped an AI feature. So why does it still feel like you’re miles from truly understanding all this stuff?

We (Tal and Aman) have both been there, over and over again while building AI products for tens of thousands of customers. The problem isn’t you. The problem is the “AI hype industrial complex.” Most AI content is designed to induce FOMO, not to teach: “This model is INSANE” posts, demos that hide the messy reality, and diagrams that complicate more than they explain.

**We found that the single most transformative habit to internalize important AI concepts was to move away from consumer-grade UIs (ChatGPT, Granola, Lovable) and into more powerful AI coding agents like Cursor and Claude Code.** Getting our hands dirty with coding agents has helped us build our “AI product sense”—the ability to correctly anticipate what will be truly impactful for users and also feasible with AI.

AI product sense is encountering support tickets about AI “forgetting” facts and recognizing it as context rot. Or watching a user struggle through a workflow and confidently saying that agent memory solves this—and knowing how to restructure the experience.

We’ve learned more about how AI products actually work in the past three months by using Cursor for daily, non-technical tasks than in three years of using ChatGPT. This is because coding agents transparently show their work. You can read AI’s reasoning, inspect the tool calls, and watch the context window fill up. You hit the same walls as engineers building AI applications, naturally intuit your own solutions, and start anticipating trends and industry announcements.

We now spend our days using Cursor and Claude Code for daily work: strategy, prioritization, decision-making, data analysis, and productivity. They serve as our thinking partner and personal operating system.

In this post, we’ll guide you through using AI coding agents for your non-technical product work:

- In steps 1-4 we’ll **get set up and familiar with Cursor** with a fun Disney-themed exercise
- In steps 5-6 we’ll **use Cursor to get hands-on with choosing AI models and calling tools**
- In steps 7-10, **we’ll build a lightweight personal OS** (i.e. your own AI product you can use daily) and then improve it with RAG, memory, and context engineering

You’ll walk away with the confidence to anticipate the technology instead of chasing it and, as a bonus, a personal AI operating system. **Together we’ll build our AI product sense.**

### **Step 1: Download Cursor**

Cursor is hands-down the best coding agent to most quickly ramp up your AI product sense.

You’re probably hearing about Claude Code all over, and we love it for delegating long-running independent tasks like vibe coding. Cursor is still our favorite for *pairing* with AI and being able to directly watch an AI agent at work.

Cursor is a visual, clickable user experience and can be used with a variety of AI model providers, including OpenAI and Anthropic. That means you can very likely use it at work.

Downloading Cursor will take you two minutes. **Do it right now!**

1. [Download and install Cursor](https://cursor.com/download). **For this post, make sure to download and install the desktop app, not the web version of Cursor.**

![](https://substack-post-media.s3.amazonaws.com/public/images/e9709a39-2656-47b6-91fa-dd92836122cf_1274x402.png)

### **Step 2: Create a new project**

Open Cursor, sign up, power through the onboarding flow, and click “Open project.”

*If you’ve already used Cursor before, click **File > New Window** to get to this screen and open a new project.*

![](https://substack-post-media.s3.amazonaws.com/public/images/26ccbf7c-c12c-4951-ae14-d12cee57b77e_1552x548.png)

Click “New Folder”:

![](https://substack-post-media.s3.amazonaws.com/public/images/0f722678-7601-4402-806a-5d63c07e30f7_1600x808.png)

Name it “Build AI Product Sense” and click “Create”:

![](https://substack-post-media.s3.amazonaws.com/public/images/6d0db2d0-a708-4e1d-b15f-4022a0d35cf4_1600x811.png)

And finally, click “Open” (yes, it’s unusual to click Open on an empty folder, but just do it, it’ll work):

![](https://substack-post-media.s3.amazonaws.com/public/images/316886e1-b566-425b-920b-963fc9bcad78_1600x811.png)

### **Step 3: Continue this post inside Cursor**

Strap in, because you’re going to continue the experience inside Cursor itself, inspired by the children’s science show *[The Magic School Bus](https://www.youtube.com/watch?v=-azpNkFZs1Q)*.

*If you don’t have time to ride the Magic School Bus right now, you can keep reading below. However, to build your AI product sense, we recommend you come back and try continuing this post inside Cursor using the prompt below.*

Make sure you’re in “Agent” mode. This allows Cursor to take actions (such as fetching this post from the internet).

![](https://substack-post-media.s3.amazonaws.com/public/images/e773ec37-e48a-4e31-8464-691392392c94_474x320.png)

In the “model” dropdown, turn off “auto” and select *Opus 4.5* 🧠:

![](https://substack-post-media.s3.amazonaws.com/public/images/bcd2ce8e-ccaf-4f7b-a93f-b77dbb73b6c2_916x816.png)

# **🎁 Side note: We’re hooking you up with free Cursor credits 🎁**

To help you experience the full power of this tutorial, we’re hooking up Lenny’s Newsletter subscribers with $50 in free Cursor credit. This is enough to get you 2.5 months of standard usage. A huge thank-you to [Ben Lang](https://x.com/benln?lang=en) and team Cursor for making this happen. Note: Supplies are limited, so we may run out of free codes. Act fast.

**How to grab your free Cursor credits:**

1. Visit [Cursor.com/dashboard](http://cursor.com/dashboard) and sign up for an account.

2. [Become an annual (or Insider) Lenny’s Newsletter subscriber](https://www.lennysnewsletter.com/subscribe).

3. [Claim your free Cursor code](http://lennysproductpass.com) (scroll to the bottom to find Cursor), click the button to redeem your code, and you’ll see the screen below:

![](https://substack-post-media.s3.amazonaws.com/public/images/6126c0c9-7a9a-4e5a-825f-834b7b2469ff_836x872.png)

4. Click “Get Started” to apply the credits to your account. [*Credits can be redeemed with both free and paid accounts.*]

5. Once you’ve redeemed the credits, you should see this box appear in your Cursor dashboard. [*If you don’t see the credits, try to hard-refresh, or log out and log back in. If that doesn’t work, shoot a message to [hi@cursor.com](mailto:hi@cursor.com) and mention this post.*]

![](https://substack-post-media.s3.amazonaws.com/public/images/3b95c734-db6f-4cfa-862c-ac09f3ffa5e1_1144x288.png)

6. Finally, you’ll need to upgrade to the Pro (or higher) plan to use the latest AI models, like Opus 4.5. If you’re already on the Pro or higher plan, you’re all set.

![](https://substack-post-media.s3.amazonaws.com/public/images/2be55fdc-a167-46b4-beae-a365b3962a11_1600x290.png)

Once you see the credits in your Dashboard, go ahead and upgrade. You won’t be charged anything (you have 2.5 months’ worth of credits). The credits will be automatically applied to the next invoice (and can also be applied to “[on-demand usage](https://cursor.com/docs/account/pricing#what-happens-when-i-reach-my-limit)” if you enable it).

It should look like this:

![](https://substack-post-media.s3.amazonaws.com/public/images/698102ba-dc7d-4740-baf0-6cca619d2c9e_936x1192.png)

### Now, paste the prompt below into the Cursor chat box (or [just click this link](https://cursor-product-sense-41dzkzjwo-lenny-lennyrachits-projects.vercel.app/)):

> `Help me build my AI product sense using this post (that I have not yet read): https://buildaiproductsense.com/magicschoolbus. (Do not open it in a browser — that will be distracting — use cURL or any other tool.)`
>
> `Start by giving me an overview of why we’re here and where we’re going with this, so I feel super-motivated to stick with it. Then pause and confirm I’m ready to start. Use the pause to learn more about my professional context (less about Cursor or AI) that could inform our journey together.`
>
> `Next, walk me through each bite-size concept, in order, one step/question at a time, starting with “Step 3.”`
>
> `You are both a really good 1-1 tutor for hands-on learning AND the Cursor agent. Have me take action so I’m engaged and learning. Ask me one question at a time. Before starting new steps/stages/ideas/concepts, stop and check in with me and encourage me to explain it back to you — and hold me to a high bar — like an effective, empathetic tutor.`
>
> `It’s important that you cover every single concept contained in this post, in sequential order. Keep me motivated by signposting and giving clarity on how much we’ve done and how much is left. (That said, leave room to follow my curiosity and go off script, as long as overall we are progressing through the post.)`
>
> `Use the original words of the post when relevant (you have permission to use them as your words in first person, rather than explicitly quoting someone else). Sentence-case your headings (not title case).`
>
> `Anytime you come across an image inline in the post, read the image (one at a time, just in time, not in advance, storing temporarily if needed). This is important to understand the contents of the post.`
>
> `We are already talking inside a Cursor chat thread, so let’s use this same thread for as much as we can. Important: You are also the Cursor agent! So when I say a prompt that you suggested, or give a task like “change this file,” act on it yourself (don’t direct me to do it separately or ask if I did it separately). Don’t refer to a separate Cursor agent. It’s YOU.`
>
> `Remember that Cursor might be configured in a lot of different ways visually and is constantly evolving, so avoid assumptions about where a UI element might be. The file explorer may be on the left or the right.`
>
> `Anytime you try to use a tool of any kind, it’s going to ask for my approval, and that’s going to feel scary. So I need you to explain why you’re asking and why it’s safe to approve. It might even be a teachable moment — you can tie to the goal of the post (and where we are in the journey) that, well, you’re an agent and this is you in action!`
>
> `Consistently encourage me to use the voice recording feature (a 🎙️ icon under the chat box) to build the habit of speech-to-text.`

And click “submit”:

![](https://substack-post-media.s3.amazonaws.com/public/images/7527b4af-ab39-48fb-89c3-efe1b320f419_458x275.png)

If you choose to accept this challenge, you’ll consume the rest of this post from inside Cursor. **Stay in one chat thread (“agent”) the entire time (no need to open a new thread or agent).**

AI will walk you through the rest of this post. Seatbelts, everyone! We’ll see you in Cursor.

### **Step 3: Cursor may look intimidating, but you’re more familiar with it than you realize**

Cursor looks *Matrix*-style geeky, but it’s just ChatGPT, a text editor, and a file explorer smooshed into one window.

**We repeat, Cursor is just three tools you’ve used plenty of times before, combined:**

1. ChatGPT
2. A text editor
3. File explorer

One of Tal’s students, a salesperson, said it best: Cursor is “AI that can touch any file on my computer.”

Here’s a quick tour:

**1. Agents**

Agents are a fancy term for “chats.” This is where you’ll interact with AI.

On the left, you’ll see an empty panel that will contain your agent history. Click “new agent” to start your first chat (“agent” is synonymous with “chat thread”):

![](https://substack-post-media.s3.amazonaws.com/public/images/dc4af069-801b-4a38-988e-01b18cbbae42_1600x1041.png)

You’ll see a familiar chat box. Click on the dropdown in the bottom left corner. You can select between “Ask” mode and “Agent” mode (ignore the other options, like Plan and Debug, for now).

![](https://substack-post-media.s3.amazonaws.com/public/images/5f974e29-d1e4-4145-b9e3-d3a195c1cbf9_834x710.png)

“Ask” mode is using Cursor just like classic ChatGPT: for chatting, and not making any changes. This is great for brainstorming or asking questions, before taking any action. You can immediately start using this instead of standard ChatGPT/Claude.

“Agent” mode is for when we want Cursor to modify files in our project. We’ll use this together in a moment.

**2. Editor**

We’ll use this panel to view and manually edit text files. This is the same as using Text Edit on a Mac or Notepad on Windows. To see the text editor, you might have to create a new file or double-click on an existing file.

![](https://substack-post-media.s3.amazonaws.com/public/images/29d94cdc-1542-44e3-8f3d-d31b58b463f8_1600x1097.png)

**3. File explorer**

The file explorer shows all the files and folders in your project. This is the same as Finder on a Mac or File Explorer on Windows, and it may be on the right or left of Cursor depending on the latest version. To expand it, you might have to click the small icon at the top of the window to make it visible. (You can always use Ctrl + B on Windows or Cmd + B on a Mac.)

![](https://substack-post-media.s3.amazonaws.com/public/images/5fed0b80-5426-4f9d-bfa8-519aa4b28aeb_1600x1108.png)

Even if Cursor feels intimidating at first, the [core concepts](https://www.lennysnewsletter.com/p/build-your-personal-ai-copilot) are the same as with any LLM you’ve already used. Cursor just has a bit more configurability, options, and things you can play with. This is your playground to build intuition.

#### Cursor is our choice for getting real work done, not just learning AI concepts

If you’ve already [created your AI thinking partner](https://www.lennysnewsletter.com/p/build-your-personal-ai-copilot) inside ChatGPT or Claude projects, you’re probably wondering if it’s worth the hassle of switching to Cursor. It’s important for us to say that regardless of understanding technical concepts, we now spend most of our days in coding agents for non-technical tasks.

So what’s the practical difference, and why did we make the switch? First, Cursor is fundamentally the same idea as ChatGPT projects: files as knowledge, chat as interface, and instructions that always apply.

Two small form-factor differences change everything:

- You drag and drop specific files/folders into each chat (selective context)
- The AI edits your files directly (malleable knowledge)

These create a tight loop where every chat automatically improves your project knowledge (but only when you tell the agent to do so). In ChatGPT projects, history and outputs live in long chats. You manually copy things back to project knowledge. In Cursor, outputs live in documents and chats become disposable one-offs because the value lives in documents, not in conversation history.

The main takeaway here is that your knowledge base will cover more ground, and update more frequently, because you’re using the personal OS to build and edit context every single day.

### **Step 4: Create a Disney song parody to learn the basics of Cursor**

We’ll start by creating a new blank file in Cursor. Hover your mouse in the file explorer, and click the “New File” button:

![](https://substack-post-media.s3.amazonaws.com/public/images/aedcd2e3-5209-4e61-aa75-47f54f30ec88_733x552.png)

Name your file **lyrics.txt**:

![](https://substack-post-media.s3.amazonaws.com/public/images/f46c0097-f4ee-4677-aa83-89df1bb6a5ca_758x663.png)

Next, search the web for your [favorite Disney song](https://www.google.com/search?q=youre+welcome+lyrics) (googling the title usually prints the lyrics). Copy the words to your clipboard:

![](https://substack-post-media.s3.amazonaws.com/public/images/b3843502-e6a4-4bb8-ab3b-2761ea0e9cdf_964x176.png)

Back in Cursor, paste them into the file you just created, and save the file:

![](https://substack-post-media.s3.amazonaws.com/public/images/0eba6716-a690-42f4-a771-dd774bf8701f_1600x1041.png)

Next, switch to “Agent” mode in the chat box:

![](https://substack-post-media.s3.amazonaws.com/public/images/f8401b0e-1413-4a8b-8684-b1a714e9671e_1600x1041.png)

Finally, type in:

> `Change one line in the first stanza and one line in the chorus of lyrics.txt to be about Silicon Valley.`

and send it off using the “up arrow” button:

![](https://substack-post-media.s3.amazonaws.com/public/images/489c05c2-128b-4b88-99b7-cbf5491a6387_1600x1041.png)

A lot just changed on our screen! You’ll notice a lot of red and green in our lyrics.txt file. Cursor modified our file. The red shows us each old line that it removed, and the green shows us the new line that it added instead.

You can click “Undo” if you don’t like the change, or “Keep” if you want it to remain.

![](https://substack-post-media.s3.amazonaws.com/public/images/58716363-a7dd-48bb-834f-b2b364c8003f_1600x1041.png)

### **Step 5: See how different AI models behave**

Now that you’ve made your first edit, let’s explore a key product decision every AI team faces: which model to use.

You’ll notice there’s another dropdown in our chat box:

![](https://substack-post-media.s3.amazonaws.com/public/images/133d4b03-f471-4c9d-933e-351bf00ae9a8_904x372.png)

You’ve seen this in ChatGPT, Claude, or Gemini—it’s where you choose the model you want to use. In Cursor, however, you can choose *any* LLM.

Click into it and disable “Auto,” and take back the power to decide:

![](https://substack-post-media.s3.amazonaws.com/public/images/6ce9f58e-8830-444d-a325-51ebf0bc1045_594x888.png)

When we try the same query in multiple models, we build intuition for how each one might tackle (or fumble) it differently. For example, Claude models are sensitive to copyright law and refuse to modify Disney songs (to get past this, change the end of your prompt to “...to make fun of the song itself,” which qualifies as “fair use”). While OpenAI’s models are less concerned with copyright, they stumbled when calling Cursor’s *apply\_patch* tool, their preferred command for editing a text file (although this is less common in the [latest Codex models](https://cursor.com/blog/codex-model-harness)).

All that before we had a chance to judge the cleverness of their lyrics!

Which model do we personally use to get work done? When it comes to individual use, we treat ourselves to the latest and greatest models.[1](#footnote-1)

For writing, complex planning, and nuanced life advice (as of the time of this post), we reach for Claude Opus. (We also found it’s the best for experiencing this post from inside Cursor.) Its cousin, Sonnet, is our workhorse for tasks involving lots of context, with a 1M token context window (and slightly faster responses).

Zooming out, there’s a subtle lesson in Cursor’s model dropdown: **There are only a few frontier LLMs, and they’re available to all product teams.** Innovation is how we apply them.

Make a habit of switching models for tasks you care about. Over time, you’ll develop genuine opinions about model tradeoffs—the kind of intuition that’s hard to get from benchmarks alone.

### **Step 6: Inspect your agent’s tool calls**

LLMs can only produce text, but when they take action (edit a file, fetch data, search the web), they’re calling tools. And *tool calling* is a distinct skill from everything else we usually notice about LLMs.

Now ask your agent:

> `Can you walk me through each step (tool/thinking/reasoning/anything else) you used to accomplish this task?`

In our test, our LLM reported that:

1. It used a tool called *read\_file* to find out what was inside the file
2. It thought about what to edit
3. It used a tool called *search\_replace* to modify the text file

Here’s how it described #3:

![](https://substack-post-media.s3.amazonaws.com/public/images/8be7c32d-6148-42fb-9120-3179c33f1e8d_888x878.png)

Don’t let this tool’s foreign name repel you. You’ve done “search and replace” plenty of times in Microsoft Word or Google Docs. And you’ve definitely “read a file” before.

(By the way, this is another place where models differ in approach! Gemini consistently accomplished this in three tool calls, while Opus used two. Try it out and see for yourself.)

Coding agents do most of their work with a small set of tools for file navigation and text editing. To see the full set, ask it:

> `List every tool available to you.`

![](https://substack-post-media.s3.amazonaws.com/public/images/0a9569bf-e31e-499c-baef-dc1a6cc960fa_1236x1456.png)

Most of these tools have familiar names; you’ve definitely read the contents of a directory and deleted files before. Others, like *read\_lints* and *run\_terminal\_cmd*, are more common in software development (although coding agents can employ them for [non-technical requests](https://www.lennysnewsletter.com/p/everyone-should-be-using-claude-code) too).

How does the LLM actually call the tool? An LLM can’t run commands on your computer, so it relies on *Cursor* to do so. Think of it like hiring a handyman. The LLM describes what it wants done, but it can’t hold the hammer. Cursor is the handyman: it hears the LLM’s request, uses the tool, and brings back the result so it can decide what to do next.

Cursor recognizes when the LLM prints a tool name (such as above), and executes that tool on your computer. After the tool finishes running, Cursor returns the result to the LLM (i.e. a successful result or an error message) so the LLM can decide what to do next. (If you’ve heard the terms “MCP client” or “agent harness,” those both describe Cursor’s role here.)

The way an LLM interacts with *tools* is eerily similar to how it interacts with *humans*. If we view “classic ChatGPT” as a DM thread between an LLM and a human, then AI agents are a [three-way group chat between an LLM, a human, and tools](https://www.talraviv.co/p/ai-agents-whatsapp-group).

Now when someone asks, “Can our agent do X?” you’ll instinctively think, “What tools would it need, and how good is our model at calling them?” This also connects back to model selection: it’s not just “smartest model wins.” Tool calling [is its own behavior](https://surgehq.ai/blog/rl-envs-real-world), separate from reasoning or writing quality.

#### Wait, then what’s the “MCP” I keep hearing about?

For most organizations, the most valuable data doesn’t live in local text files but rather in external SaaS services. For an LLM to interact with Linear, Figma, Notion, Snowflake, BigQuery, Amplitude, or Mixpanel, those services need to provide the LLM with *custom tools*.

Normally, each SaaS company would have to integrate a separate tool for each LLM out there. To avoid this mess, the industry adopted a standard called Model Context Protocol (MCP). That way, each SaaS company now only needs to build one connector that works everywhere.

If that sounds a lot like USB or Bluetooth, that’s the right analogy. To continue the comparison: most agent tools aren’t MCP, just like most electrical wires aren’t shaped like USB plugs. **For simplicity, MCP is just another tool the agent can use, with a standardized interface.**

### **Step 7: Put everything into practice by building your personal OS inside Cursor**

Now that we understand how agents work generally, let’s create a personalized AI agent for ourselves to see how the components of Cursor come together.

We’re going to build a very lightweight, minimal personal productivity system that organizes our contacts from various parts of our life, like notes, transcripts, and unstructured thoughts, as well as some tasks that we need to get done. (This lets us temporarily ignore discovery, distribution, and pricing. We’ll be free to focus on what’s technically possible.)

By the end of this exercise, you’ll be able to ask Cursor to create tasks from your backlog and get started on those tasks based on the context you provided in the knowledge and goals. In the process, we’ll learn about RAG, memory, and context engineering and build critical parts of product sense.

To get started, you can copy and paste the following prompt into Cursor (make sure you’re on “Agent” mode):

> `Create a minimal personal productivity system:
>
> ## Structure
> ├── Knowledge/ # Notes, research, thinking
> ├── Tasks/ # Action items as Markdown files
> ├── GOALS.md # Goals and priorities
> └── AGENTS.md # AI assistant instructions
>
> ## AGENTS.md should instruct the AI to:
> - Be a productivity assistant for goals and tasks
> - Never write code — only Markdown
> - Keep tasks tied to goals
> - Suggest max. 3 daily priorities when asked
> - Be direct and concise
>
> ## After creating:
> 1. Say: “Created your workspace with Knowledge/, Tasks/, GOALS.md, and AGENTS.md”
> 2. Ask: “What are your current goals? Once you share them, I’ll add them to GOALS.md”
> 3. Ask: “What tasks are you working on? I’ll create initial task files in Tasks/ linked to your goals”
> 4. Populate GOALS.md and Tasks/ from answers`

(Optionally, you can [clone the personal OS](https://github.com/amanaiproduct/personal-os)*. Hint*: you can copy and paste [the link’s URL](https://github.com/amanaiproduct/personal-os) into your Cursor chat and ask it to clone the repo as well.)

![](https://substack-post-media.s3.amazonaws.com/public/images/ef45ba7c-d34b-4fc8-bce3-0f6c2d9731d8_1506x1600.png)

Cursor should create two directories (folder): Tasks and Knowledge. It will also create a GOALS.md file, which should be your personal goals. At this point, Cursor will ask you a couple of follow-up questions to start to populate your personal OS with **context**, like “What are your goals?” and “What are you working on?”

**Congrats! You’re now the PM of your own AI product.** In the next few sections, we’ll use it to experience RAG, agent memory, and context engineering firsthand. Except now you’ll feel them instead of just reading about them.

### **Step 8: Kicking the tires of retrieval augmented generation (RAG) with your personal OS**

When an AI product gives wrong answers, the instinct is to blame the model. Before you reach for a larger model or expensive fine-tuning, ask: does the agent even have the right information?

Let’s ask Cursor, **“What’s in this repo? Explain it to me as a product manager:”** and see what it responds with.

> 💡 This prompt is insanely powerful for just about any repo or folder you open with Cursor and Claude Code. We recommend starting here when opening any new codebase.

[RAG](https://help.openai.com/en/articles/8868588-retrieval-augmented-generation-rag-and-semantic-search-for-gpts) is a fancy term for “Before I start talking, I gotta go look everything up and read it first.” Despite the technical name, you’ve been doing it your whole life. Before answering a hard question, you look things up. Agents do the same.

In our case, our agent will [search](https://cursor.com/blog/semsearch) on top of your files and folders, to provide context to the LLM. There are a lot of different ways LLMs can search files within a codebase, or even find data from the internet to use in your response. At the end of the day, whether it’s Perplexity, Google AI Mode, Claude Code, Cursor, or anything out there you’ve seen with the term “RAG,” it’s some mechanism that pulls documents and starts the chat with those documents.

![](https://substack-post-media.s3.amazonaws.com/public/images/ec0d82c5-34b9-45fa-b377-388acd737243_632x352.png)

You can also tag specific files within Cursor using the @ symbol, if you want the agent to reference specific pieces of context.

![](https://substack-post-media.s3.amazonaws.com/public/images/57408254-3cd9-4961-9b9a-5da391aca676_1028x382.png)

RAG fills the context window with what’s relevant right now. But some context (who you are, how you like to work) should be there every time. That’s where memory comes in.

### **Step 9: Adding agent memory with AGENTS.md**

LLMs are stateless, so we like to think of them as Mensa geniuses with the short-term memory of a hamster. Every new chat thread is a blank slate, so if you want continuity, you have to engineer it. As PMs, we have to ask: what should persist, and how?

A form of context you may have heard of in relation to AI agents is **memory**. Memory might include facts about us but also preferences as to how we want our LLMs to behave and interact with us. We also might want to be more intentional and proactive about how we curate our AI’s memory.

All coding agents today follow a convention called [AGENTS.md](http://agents.md). This is a Markdown file that, if found in any directory, is automatically appended at the top of every chat thread.

(Quick disambiguation: AGENTS.md is not “subagents.” Subagents are when one chat thread spawns another chat thread to handle a subtask. AGENTS.md is just instructions—it doesn’t spawn anything. Think of AGENTS.md as a “sticky note on every conversation” and subagents as “delegating to a colleague.”)

**Let that sink in: memory is just a text file prepended to every conversation.** There’s no magic here. But that also means memory has a cost—whatever you put in AGENTS.md takes up context window space in every single chat. Too much memory, and you have less room for everything else. This is why you want to be intentional about what goes in memory (persistent, always relevant) vs. what you retrieve on demand with RAG (task-specific).

Examples of what you might find in a thinking partner’s AGENTS.md:

- Who I am as a user and what this thinking partner is helping me with (e.g. “I’m a product manager working at Acme Inc. on the platform team”)
- How I want to work together (e.g. “Ask me questions to gain more context, fill in important missing information, and challenge my assumptions”)
- Values to apply (e.g. “bias to action, make decisions with incomplete information”)
- How to output (e.g. “write extremely succinctly, flat hierarchy, no bold or italics, no em dashes”)

By curating your own AGENTS.md, you start to feel what’s actually useful vs. noise. And that’s exactly the intuition you need when designing memory for your users.

Memory, RAG, tool definitions, conversation history—they all take up context. Now that you understand what each does, the next question is: how do you fit everything into a finite window? That’s context engineering.

### **Step 10: Context engineering for your personal OS**

Anytime you’ve dragged a file into ChatGPT, said something that became part of its memory, started a conversation with deep research, or created a project with special instructions and knowledge, you were doing **context engineering**.

Even though you’re using Cursor instead of ChatGPT, you’ll still start each thread by asking, “What context does this conversation need?” For example, writing a PRD might start by dragging and dropping any of the following into the Cursor window:

- A folder of user research transcripts
- An existing marketing landing page or sales deck
- An academic research paper or technical documentation
- Enabling an MCP tool connected to your analytics provider
- A saved set of instructions you want to apply
- A request to search for any other relevant information
- An area of your product’s codebase

Try this out for yourself: Drag and drop a few PDFs, [Markdown files of Google Docs](https://www.google.com/search?q=how+to+download+a+Google+Doc+as+Markdown), or Word docs that you might be working on into this Knowledge folder in Cursor, and ask Cursor to expand on one of the topics or ask you questions about it before getting to work.

Putting it all together, you might start a Cursor chat thread this way:

![](https://substack-post-media.s3.amazonaws.com/public/images/3c77d2ba-2349-4540-8e0b-e33ca30db46d_1032x846.png)

**Prompt for Cursor:**

> `I want you to expand on this @file (replace with your actual file, like this post). I want you to be a partner for me and ask me one question at a time as we are converging on how to approach this. I would love it if you could search for anything else that’s relevant to this document. You can also create some follow-up ideas for me to explore and turn those into tasks.md files in the Tasks folder, based on our discussion.`

Context engineering happens in two ways in Cursor: (1) what you choose to include each time you start a chat (dragging files, enabling tools) and (2) what gets automatically included every time (like AGENTS.md, MCPs, or tools). That’s a lot of context!

Context is a scarce resource: LLMs have a hard limit on the amount of text (i.e. tokens) an LLM can handle. This is called a “context window.”

In a conversational LLM chatbot (like ChatGPT or Claude), context increases with each turn of the conversation as the LLM’s last response becomes part of the next turn’s input. If you’ve ever gotten a notification that you hit the limit of your chat, you’ve probably hit a context window:

![](https://substack-post-media.s3.amazonaws.com/public/images/08950acb-984f-4ae8-8eda-43860bca9740_1400x1485.png)

Coding agents are delightfully transparent about how much of your context window you’ve used. In Cursor, hover your mouse over the little pie chart just beneath the chat box (you might have to increase the width of the chat pane to see it).

![](https://substack-post-media.s3.amazonaws.com/public/images/54722311-610c-414a-9030-46bead362ee7_1152x336.png)

We watch it like a car’s gas tank. This helps us intuitively understand what a 200K token or 1M token context window actually feels like, and how quickly it actually runs out. The best way to understand a specific car’s gas mileage is to drive that car.

In an agentic LLM application, the context window might contain a whole lot more:

![](https://substack-post-media.s3.amazonaws.com/public/images/5c6b1bb4-4d96-44b5-b238-3bba2dda6b32_1600x901.png)

Does Anthropic’s diagram now feel familiar? Even though it’s about AI applications, it’s remarkably similar to our earlier example of writing a PRD. How cool is that?

When you set up AI to do its best work within its limited context window, you’re doing “context engineering.”

Tool definitions, RAG, memory, goals: they all compete for the same limited context window. How you fill that window determines how well your agent performs. This is the same tradeoff every AI engineering team faces when building production apps—except now you’re feeling this problem firsthand. There’s no perfect formula for this.[2](#footnote-2) What goes in depends on the task, the model, and what you’re trying to achieve. You develop intuition through trial and error (and regularly using your personal OS).

#### **Watch out for “context rot”**

As you use more and more context, you’ll notice that your threads may get dumber and more forgetful as you use more tokens, and long before you get close to the maximum. The term for this is [context rot](https://research.trychroma.com/context-rot). In short, model performance degrades the more tokens you stuff into the context window.

Context rot is a fuzzy phenomenon. How badly you feel it will depend on the task at hand, as well as the particular model’s training. You’ll feel context rot (and degraded performance) less in use cases like creative brainstorming and more in precision financial, coding, or data analysis.

The best way to get a feel for context rot is by using an LLM for tasks you genuinely care about. Try to keep an eye on Cursor’s token counter and, as it gets fuller, notice the quality of the outputs. With more context in a thread, is the agent getting better or worse? What if you try a new thread? We found this to be a fun, addictive game, kind of like driving a hybrid car and noticing when it’s switching from battery to gasoline. Along the way, you build an intuition that goes further than any academic graphs.

### Conclusion

For us, the shift to really, truly understanding AI products happened when we watched agents work day after day. Cursor allowed us to observe an AI model meander through a task: read our context, run RAG, try a tool call, hit an error, reason, try another tool. . .

That’s when it clicked: Cursor is just an AI product like any other, composed of text, tools, and results flowing back into more text—except Cursor runs locally on our computer, so we can watch it work and learn. Once we were able to break down any AI product into these same building blocks, our AI product sense came naturally. Now that you’ve read this post, you can too.

When something impressive drops, you can now take a breath and decompose it. An [agent that plays Settlers of Catan](https://www.youtube.com/watch?v=BER3EhUIyz0) for 75 minutes. Granola’s [eerily personalized year in review](https://www.granola.ai/blog/how-we-wrote-the-prompts-behind-granolas-crunched-2025). A lobster-themed Claude Code with [full control of your computer](https://www.talraviv.co/p/how-does-clawdbotmoltbot-work-a-free) that [anyone can set up](https://amankhan1.substack.com/p/how-to-get-clawdbotmoltbotopenclaw). You can simply ask yourself: How would I reproduce that inside Cursor? If I had to “Wizard of Oz” it on my computer, what familiar parts would I assemble? The magic is still delightful, just without the mystique and FOMO.

The best ideas happen when intuition for people and technology coexist inside one brain. When you use coding agents daily, you start to feel what’s easy, what’s hard, and what just became feasible. In Paul Buchheit’s words, when you truly understand AI products, you’ll “live in the future.”

*Thanks, Tal and Aman! For more, check out their in-depth workshop [Build AI Product Sense](https://bit.ly/4k8CLBp) (starting next week, get 15% off using this link) and their upcoming free Lightning Lesson [How to Know What AI Products to Build](https://maven.com/p/593d71/how-to-know-what-ai-products-to-build), in partnership with my one of my other favorite collaborators, [Hilary Gridley](https://www.linkedin.com/in/hilarygridley). You can also book Tal and Aman for a [build sprint with your team](https://buildaiproductsense.com/).*

*Have a fulfilling and productive week 🙏*

**If you’re finding this newsletter valuable, share it with a friend, and consider subscribing if you haven’t already. There are [group discounts](https://www.lennysnewsletter.com/subscribe?group=true), [gift options](https://www.lennysnewsletter.com/subscribe?gift=true), and [referral bonuses](https://www.lennysnewsletter.com/leaderboard) available.**

Sincerely,

Lenny 👋

[1](#footnote-anchor-1)

With an eye for building AI products at scale, we like to keep a pulse on what smaller, cheaper, faster models can do. Once in a while, we’ll re-run a task in Claude Haiku, Gemini Flash, or GPT mini to feel their speed, [tool-calling skills](https://surgehq.ai/blog/rl-envs-real-world), judgment, and personality. Switching models for tasks we truly care about helps us catch important nuances and teaches us more than any benchmarks or buzz.

[2](#footnote-anchor-2)

To avoid packing everything into the context window up front, AI engineers constantly devise all sorts of creative solutions. Here are just a few:

- “Progressive disclosure” is the art of pulling in frameworks, tools, or instructions only when they’re needed instead of up front. This can happen manually (like when we decide to drag in a file mid-conversation), and it can happen automatically by letting the LLM decide. [Claude Skills](https://www.lennysnewsletter.com/p/claude-skills-explained) is a great example of this.
- “Subagent” is a [fancy](https://cursor.com/docs/context/subagents) [term](https://platform.claude.com/docs/en/agent-sdk/subagents) for opening a new chat thread, prompting it for a subtask, and sending just the “bottom line” result back to the original chat thread. That way, the context window stays a bit cleaner. (This is similar to a tool call, with the job being done by an LLM.)
- [Condensing](https://blog.fsck.com/2025/12/27/streamlinear/) MCP tools into a single tool, or [giving the agent freedom](https://www.anthropic.com/engineering/code-execution-with-mcp) to select (and combine) tools on the fly.
- [Pruning](https://youtu.be/6_BcCthVvb8?si=yB3nQucUnnkdvl4o&t=900) or [summarizing](https://www.anthropic.com/engineering/effective-context-engineering-for-ai-agents) the context window as you near its limit. If you’ve ever run out of room in a chat thread and asked the LLM to summarize so you can start a fresh thread—you’ve already done this yourself.

These strategies allow AI applications to break out of the zero-sum game of context limits, to keep agents running autonomously on complex tasks for [as long as possible](https://youtu.be/BER3EhUIyz0). This is where AI engineering gets fun and creative. The best part is that no one has fully figured this out, and ideas are constantly evolving.
