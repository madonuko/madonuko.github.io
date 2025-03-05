---
layout: posts
title: Will AI Replace Me?
date: 2024-03-05 18:00:00 +0800
author:
- madonuko
categories:
- en
tags:
- irl
---

[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fmadonuko.github.io%2F2025%2F03%2F05%2Fwill-ai-replace-me.html&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)

## 1. A Talk about AI

2025-04-28 (Friday). I went to attend a talk about AI. Before you ask, I was forced to attend the event because it's a college assembly.

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

Conclusion:
1. **AI will replace programmers that are not real programmers (i.e. if you just copy and paste)**.
2. **People that heavily relies on AI to write code are just performing a modern version of [Copy-and-paste programming](https://en.wikipedia.org/wiki/Copy-and-paste_programming)**.

## 2. 