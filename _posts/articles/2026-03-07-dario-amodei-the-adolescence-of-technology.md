---
layout: post
title: "Reading Review - Dario Amodei: The Adolescence of Technology"
author: Kai
tags:
- conversations
- reading review
date: 2026-03-07 00:00 +0000
toc: true
---
### Reading Review - Dario Amodei *The Adolescence of Technology*

1. 如何想象未来AI的能力？我非常喜欢他用的这个比喻：
   ***A country of geniuses in a datacenter***

2. Dario谈到AI model的不确定性。
   - 其实，这是我一直以来思考的问题。为什么总说LLM是不确定的？这个问题指的是LLM的输出是不确定的吗？可是我们知道，LLM处理输入的本质是一个非线性方程。对于同一輸入 x，f（x）应该是*确定*的。可是连Dario也这么说。的确，从使用的角度来说同一个prompt貌似产生了不同的输出，可是据chatgpt说这来源于AI公司刻意改变random states然后筛选以产生更优的输出。

   - 因此无论LLM多像人脑，它依然更接近经典的代码。人脑对于同一input在不同时点会产生本质上*非确定*的output。不过人脑产生不确定输出的原因或许是细胞活动导致人脑的model（即其weights and biases）在每时每刻都不断变化。想测试人脑在同样weights and biases的情况下针对同一输入是否有不同输出，这是不可证伪的。

   - 扯远了。有一种可能是，我想的问题和他想表达的不是同一个东西。他所谓的不确定性或许是指LLM在训练的时候只设计了架构，然后喂数据。（Quote: LLMs are grown instead of built) 训出来什么不确定，因此用它去产出输出自然不能说是确定的。这倒是说的通。还有一种可能是，他所谓的'不确定性'是指输入到输出的'不可预测性'。下一点就要讨论这个。

3. "By "looking inside," I mean analyzing the soup of numbers and operations that makes up Claude's neural net and trying to understand, mechanistically, what they are computing and why."
   - 这个想法很自然。可是真的可行吗？LLM的本质是一堆weights and biases通过非线性连接出来的。加上我猜AI公司为了产生好的效果会用很多tricks，那从最高维度抽象看这个输入到输出的全过程就是一个巨大的非线性方程。首先它大概率不能用数学公式描述。其次有个说法叫computation irruducibility，意思是唯一预测某一非线性过程的结果的方式是实际从头到尾跑一遍。或许，当LLM最终被优化到不能再优化的时候，除了跑一遍输入到输出之外无法直接预测输出是什么。就是因为computation irreducibility。

4. "It was never true that Google could give you all the necessary information: genomes are freely available, but as I said above, certain key steps, as well as a huge amount of practical know-how cannot be gotten in that way."
   - 这里讲LLM可以告诉一些google没有的hands on knowledge。很有意思。记得以前说google会被LLM替代，事实上LLM有搜索引擎没有的功能。我想google也不会被完全替代，它们有重叠但还是不能被等价。

5. （我自己的 random thought）LLM把智能的成本降低了。Anthropic研究自家员工对AI的使用报告中提到27%的使用是用在了曾经不会做的事上：比如一些nice but not necessary / low priority things。我同意。从经济学的角度解释LLM就是降低了marginal cost。很多曾经marginal benefit < marginal cost 的事现在反过来了，因此从不值得做变成了值得。这或许是个机会---就像是high frequency trading一样，如果能找到好的scale up方式，则可以把很小的优化积累成可观的利润。

6. "But a personalized AI agent that gets to know you over years and uses its knowledge of you to shape all of your opinions would be dramatically more powerful than this."
   - This indeed sounds very scary.

7. "AI could likely be used to compromise any computer system in the world, and could also use the access obtained in this way to read and make sense of all the world's electronic communications."
   - 的确。AI和以前的系统最大的区别是可以自动化'理解'能力，这包括文字、图片、视频。我觉得以前人们在互联网可以自由表达的一大原因是过去的科技根本不可能*理解*百万计的文字、图片、视频。某种程度上这也是low signal noise ratio。现在利用AI可以轻松的从noise里提取表达者的观点和态度。的确很容易被用于mass surveillance，AI时代需要新的个人隐私保护法。

8. Dario is against selling chips to China: "In my view, this is like selling nuclear weapons to North Korea and then bragging that the missile casings are made by Boeing and so the US is "winning.""
   - Humorous. I don't think this is the correct analogy.

9. "Autocracy is simply not a form of government that people can accept in the post-powerful AI age. Just as feudalism became unworkable with the industrial revolution"
   - Interesting. I need to read up on this.

10. "AI could displace half of all entry-level white collar jobs in the next 1–5 years, even as it accelerates economic growth and scientific progress."
    - I am inclined to agree.

11. "By contrast, AI is increasingly matching the general cognitive profile of humans, which means it will also be good at the new jobs that would ordinarily be created in response to the old ones being automated."
    - 确实，这就是AI和工业革命的区别。那么答案是否在于增加一些从定义上就必须由人完成的工作呢。比如体育竞技需要人类对手，游戏，设计新游戏，表演，娱乐，电影，脱口秀，社交。或许未来的唯一工作是当老板，员工将是"the country of geniuses in a datacenter"。可以研究历史，感觉有不少明明是消耗人体力/脑力的活动，人们却还热衷甚至付费去做。

    - 我猜不同的人会有不同想法。I'm very curious to learn about other perspectives.

12. Dario认为AI不会有 "gaps in it"。
    - 我不同意。Data - model - compute 黄金三角中，AI最不可逾越的是看似最不重要的'data'。除非大幅使用摄像头，录音设备等，AI不会有物理世界的信息，人际交往信息，包括人类的感觉器官的信息。没有信息它再聪明也没用。因此未来很多人的工作可能是充当人和AI之间的interface。

13. "The most famous example of extreme concentration of wealth in US history is the Gilded Age, and the wealthiest industrialist of the Gilded Age was John D. Rockefeller. Rockefeller's wealth amounted to ~2% of the US GDP at the time. A similar fraction today would lead to a fortune of $600B, and the richest person in the world today (Elon Musk) already exceeds that, at roughly $700B. So we are already at historically unprecedented levels of wealth concentration, even *before* most of the economic impact of AI."
    - wow. 真是第一次意识到这个数据。今天Elon Musk的财富以相对GDP计算已经超越美国历史上任何一个时代的首富，这还是在AGI到来之前就如此财富不平均！

14. "The formula for building powerful AI systems is incredibly simple, so much so that it can almost be said to emerge spontaneously from the right combination of data and raw computation."
    - Well then why did it take more than 100 years since Alan Turing?
    - Dario的看法似乎是目前的model已经足以带我们到达AGI，而不久前 Ilya 在采访中说 Safe Superintelligence 在尝试优化架构
