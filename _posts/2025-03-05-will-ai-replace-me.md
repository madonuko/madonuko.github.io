---
layout: posts
title: Will AI Replace Me?
date: 2025-03-05 18:00:00 +0800
author:
- madonuko
categories:
- en
tags:
- irl
---

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fmadonuko.github.io%2F2025%2F03%2F05%2Fwill-ai-replace-me.html&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

## README

This post is a mix of my opinions and my real life experiences.

## 1. A Talk about AI

2025-04-28 (Fri). I went to attend a talk about AI. Before you ask, I was forced to attend the event because it's a college assembly.

Anyway this time around they invited a speaker who is the [...] of [...], "an AI solution provider to financial institutions and the Managing Partner of [...], a fintech asset management platform."

This person basically claimed that AI will replace jobs and even programmers in the near future. They said that one of their friends (or colleague) who knew nothing about programming,
asked ChatGPT (or maybe another chatbot) for help with creating a website for finding partners, and that was a success and they made a lot of profit.

Whether that's true is, well, up to you to think about it. It's possible, since websites are pretty easy to make anyway in general.
But the part about AI replacing programmers is a bit more complicated.

I've tried using numerous AI tools to assist programming but none actually helped much significantly in general other than just pressing tabs to complete simple
and short code snippets, as opposed to writing a full fledged program or function. If they ever try to generate anything larger it just doesn't work. I've no idea why.

Well honestly that's not really the reason why AI will not replace programmers though.

### Why AI Won't Replace Programmers

First, in order to have AI replace programmers, they need to have the **capability to write code that has never been written before**. This is basically **impossible**
since you know, the *training data comes from existing codebases that humans have written*. If you ask in LKML how many of them think that AI is going to replace
their maintainer position, most of them will probably say no.

Second, AI needs to have the **ability to reason logic**. This again, is not possible for LLMs, due to a number of reasons:
- When we reason, we do so **recursively**. We break down the problem into smaller parts, and then solve each part individually; and to solve each part, we further break them down into even smaller parts until we reach a point where we can solve them directly with intuition (basically [System 1](https://en.wikipedia.org/wiki/Thinking%2C_Fast_and_Slow)).
  - To achieve this, we activate our neural system recursively, where we basically put the output of the neural system back into the input of the neural system and try again until we reach the answer.
  - However, LLMs do not think recursively. They output each word one at a time (which is `O(n)`), and they do not have the ability to reason recursively. Does this count as real reasoning?
  - The reason why LLMs seem to exhibit some form of reasoning is because they are trained on large amounts of text data, which allows them to learn patterns and relationships between words and concepts. However, this is not the same as true reasoning, which requires the ability to break down complex problems into smaller parts and solve them step-by-step.
  - When LLMs are trained enough, they have a really strong "System 1" intuition, but they basically don't have "System 2" reasoning at all. Everything (including what seems to be reasoning) is purely their "intuition" and there is no reasoning involved.
- We put **background information and context into part of our neural networks** (brains) in order to reason.
  - There is no such equivalent for LLMs. The background information and context (i.e. prompts) are not part of the neural network, but rather are inputs to the model.

### Then The Problem Becomes: Why Do So Many People Think That AI Will Replace Programmers?

- There are a lot of people that think they understand AI, but they don't.
- There are a lot of people that think they understand programming, but they don't.
- There are a lot of people that write code by just copying and pasting from Stack Overflow before AI, and after AI was invented they just switch to AI and goes
  "wow this is so much better" because they never understood programming at all.
  - this is also shown in https://stackoverflow.blog/2021/12/30/how-often-do-people-actually-copy-and-paste-from-stack-overflow-now-we-know/#h3-62be7933c6450.

### Conclusion

Again, these are my opinions, but:

1. **AI will replace programmers that are not real programmers (i.e. if you just copy and paste)**.
2. **People that heavily rely on AI to write code are just performing a modern version of [Copy-and-paste programming](https://en.wikipedia.org/wiki/Copy-and-paste_programming)**.

## 2. Chatting with Mum during Lunch

2025-03-04 (Tue).

"[…] which is why I don't think AI will replace *real* programmers."

"Yeah, like… I agree that AIs don't actually have the ability to think or reason.
They just 'copy and paste' from existing texts that were once written by humans,
and their knowledge is built upon what humans have written before.
As you've said about the [Strawberry Test](https://www.benluong.com/testing-llms-on-the-strawberry-challenge/),
there needs to be a random person out there that stated that the word 'strawberry' has 3 'r's in order for
LLMs to know that 'strawberry' has 3 'r's."

"They never understood and reasoned that they actually do not have the
ability to count letters due to the limitations [within the designs of LLM tokenizations]."

"If humans didn't exist, then AI wouldn't exist either, because they have nothing to learn from / train on."

"Yeah, exactly."

"This reminds me of your classmate X [actual name redacted].
X's parents said on Facebook that X went to [Hong Kong University of Science and Technology](https://en.wikipedia.org/wiki/HKUST) for an interview.
The interviewer asked '**[do] you think that AIs should have human rights?**'.
Guess how X answered."

"How…?"

"Guess."

"Oh come on, just tell me already. Maybe yes only if AI has feelings or stuff like that?"

"Well, he answered '[no] because animals also don't have human rights, then why should AIs have human rights?'"

"Uhhhhhh…"

"Yeah and they [as in the parents] didn't mentioned that X got an offer from HKUST, so X most likely didn't. So they [as in the interviewers] probably didn't like X's answer too."

## 3. AI → AI?

2025-03-04 (Tue). During dinner.

Bro "I need to attend a talk about AI this Saturday"\
Mum "What's it about?"\
Bro "About AIs and random junk talks and idk"\
Mum "You know your brother also had to attend an AI talk?"\
Bro "Oh, how did that go?"\
Mum "Ask your brother"\
Bro "(to me) How was it?"\
Me "Yeah it was trash and the person claimed that AI would replace programmers which I don't think is possib-"\
Bro "They claimed that ***AI will replace AI?????***"

<small>なんのオチやねんこれ</small>

---

Mum "So yeah but without an offer X still got into UST."\
Dad "Interesting. How would you answer that question then?"\
Me "I… don't know?"\
Dad "Well obviously that depends on **whether we should treat AIs as humans**."\
Me "Obviously. Well now the problem is **how do we define 'humans'**."\
Dad "Yup. How then?"\
Me "Maybe… language?"\
Dad "Animals do have languages too? Like elephants, dolph-"\
Me "Yeah yeah yeah true. How about… emotions?"\
Dad "Nah anim-"\
Me "Ah wait yeah nah like I remembered there was news that there was like a dog and it could press buttons to reply to humans and stuff like that."[^1]\
Dad "What?"\
Me "Yeah it was like… They place a bunch of buttons on the ground that maps to different vocabs, and the dog just presses them to form partial sentences."\
Dad "That's probably fake…?"\
Me "Ok whatever but yeah animals do have some sort of languages. And they have emotions yeah."\
Dad "Yeah I think there were news about apes getting emotional when they lost their loved ones."\
Me "Yeah so… no clue then."\
Dad "… Well, the answer is **認知 (_cognition_)**. If they can start thinking about their own questions and create their own knowledge, they are basically human."\
Me "… what about aliens?"\
Dad "Are there aliens?"\
Me "We have one at home (*points to my brother*)"

[...]

"… Back to the topic, **if they can start thinking about things like 'why am I here?', 'what is the meaning of life', etc., then we can probably regard them as humans**."

"I see…"

"So basically, **philosophy**."

---

## Footnotes

[^1]: <https://www.youtube.com/shorts/pbqp-FnOfGs>