---
layout: post
title: Why AI is Harder Than We Think?
summary: "Melanie Mitchell published the paper 'Why AI is Harder Than We Think?' in 2021 and mentions the misinterpretation of AI."
cover: "/assets/img/why_ai_is_harder_than_we_think/ai.webp"
img: "/assets/img/why_ai_is_harder_than_we_think/png/ai.png"
tags: ["paper review"]
categories:
  - paper review

published: true
---

> First of all, this blog post is inspired by the paper “Why AI is Harder Than We Think?” whose author is [Melanie Mitchell](https://www.santafe.edu/people/profile/melanie-mitchell) who is a Professor at the Santa Fe University and has numerous pieces of research on artificial intelligence and cognitive science. Mitchell has pointed out four fallacies while interpreting the AI and I really encourage you to read the [original paper](https://arxiv.org/abs/2104.12871).

Today, we all know that Artificial Intelligence is a popular topic in both academic research and society. This popularity is affecting expectations of AI and its future of it and with the improvements in the field, it is expected that rapid progress towards "General AI" by first the researchers and then the society. Theoretically, General AI, in other terms [Artificial General Intelligence (AGI)](https://en.wikipedia.org/wiki/Artificial_general_intelligence), is the use of artificial intelligence in any domain to solve any challenge that calls for intelligence by behaving like a person.

However, Mitchell states that *"Even with today’s seemingly fast pace of AI breakthroughs, the development of long-promised technologies such as self-driving cars, housekeeping robots, and conversational companions has turned out to be much harder than many people expected."* and these situations occur because of people's over-confidence about AI, terminological fallacies while interpreting it, and our perception of intelligence.

Related to those fallacies and misinterpretations, AI expert Drew McDermott talks about a **cyclical pattern** in the field of AI. As we can see in the history of AI, it means that the technology and new initiatives hyped the field of AI and the following investments by governments and startups supported that. But the expectations are stuck in two cycling periods, "AI Spring" and "AI Winter".

![Spring and Winter period of AI](/assets/img/why_ai_is_harder_than_we_think/ai_winter.webp)

## AI Spring and AI Winter

The AI Spring can be described as the hoping period of AI, new approaches have come up and ideas of where the AI can go and which problems it can solve are debated with a positive attitude. Conversely, the AI Winter follows the spring when all the pretentious expectations could not happen and AI loses its confidence.

Lots of innovations have been made by researchers and technology companies throughout time. These innovations started with the efforts of [Frank Rosenblatt](https://news.cornell.edu/stories/2019/09/professors-perceptron-paved-way-ai-60-years-too-soon) – at the Cornell Aeronautical Laboratory – by combining Donald Hebb’s model of brain cell interaction with Arthur Samuel’s machine learning efforts and created the perceptron model. With the perceptron theorem, optimistic pictures of the [Symbolic AI](http://wiki.pathmind.com/symbolic-reasoning), which is simply an AI system acting like the human brain with defined rules against symbols and abstract concepts, produced by the AI practitioners. But these perceptron models are very limited and the first *AI Winter* appeared after that optimism, and the funding has disappeared. In the early 80s, AI cathed hype again with "expert systems" such as Japan's "Fifth Generation" project and US's "Strategic Computing Initiative". Expert systems relied on humans to create rules, therefore that kind of system was unable to generalize to various domains. As expected, all the funding decreased again.

About the time after that winter, Mitchell gives an anecdote as;
>"Indeed, the late 1980s marked the beginning of a new AI winter, and the field’s reputation suffered. When I received my Ph.D. in 1990, I was advised not to use the term “artificial intelligence” on my job applications."

After all those winters, around the 2000s, statistics-based methods emerged under the roof called [Machine Learning](https://www.ibm.com/cloud/learn/machine-learning), as all we know. These methods are performing specific tasks with "predictive models" rather than building a human-like intelligence. With the developments in the technology and capabilities of computational power, around 2010, [Deep Learning](https://www.ibm.com/cloud/blog/ai-vs-machine-learning-vs-deep-learning-vs-neural-networks) turned back into the business. The Deep Neural Networks showed up around the 70s and the first backpropagation demonstration was provided by [Yann LeCun](http://yann.lecun.com/) at Bell Labs. With today's technology, it has been shown that DL systems can solve unsolved AI challenges and that fact exposed the term "AI" everywhere and a new era of optimism has arrived towards "General AI" or "Human-Level AI".

However, today's AI technology, mainly DL, mostly relies on datasets therefore the AI models can come up with unexpected errors or behaviors. Moreover, the systems sometimes can learn some statistical relationship in the data, in other words, the learning process may be failed since the systems are not learning the concepts we are trying to teach them they learn some shortcuts, for the wrong reasons. DL approaches are not *understand* the concepts the way the human sense of understanding. Mitchell states - I believe this is an important point- ;

>"It’s still a matter of debate in the AI community whether such understanding can be achieved by adding network layers and more training data, or whether something more fundamental is missing."

There are new DL approaches generating optimism about AI such as Self-Supervised Learning (SSL) or [Meta-Learning](https://machinelearningmastery.com/meta-learning-in-machine-learning/). LeCun writes about SSL and states that "Today, We’re sharing details on why self-supervised learning may be helpful in unlocking [the dark matter of intelligence](https://ai.facebook.com/blog/self-supervised-learning-the-dark-matter-of-intelligence/) — and the next frontier of AI".

Even though these new approaches, technologies, and opportunities provide progress and excite us, the way to the human-level AI is still longer than represented in society. There is some lack of understanding and misinterpretation about AI and human intelligence and Mitchell summarized them into four fallacies.

>"While these fallacies are well-known in the AI community, many assumptions made by experts still fall victim to these fallacies, and give us a false sense of confidence about the near-term prospects of "truly" intelligent machines."


![Fallacy One](/assets/img/why_ai_is_harder_than_we_think/narrow_intelligence.webp)

## Fallacy 1: Narrow intelligence is on a continuum with general intelligence

When people see software, algorithms, and machines do unexpected jobs or perform amazingly, they believe the "True AI" is near or the AI is going to behave like a human in near future. The type of AI we are experiencing right now is focused on specific tasks and domains as designed to succeed in them, therefore they are solving problems in a narrow field.

The first fallacy can be named as believing every development is a step through General Intelligence. Of course, every improvement or achievement lets AI handle another task or existing one more accurately but it still cannot be predicted to encounter an unfortunate obstacle through the way of glorious general AI. The engineer Stuart Dreyfus states that the "unexpected obstacle" in the development of AI is being missed and has a funny statement about the continuum of AI;

>"It was like claiming that the first monkey that climbed a tree was making progress towards landing on the moon"

![Fallacy Two](https://c.tenor.com/aqfF_pY1goYAAAAC/boston-dynamics-robot.gif)

## Fallacy 2: Easy things are easy and hard things are hard

We cannot ignore the intelligence of humans, and how we learn, decide, and act if talking about general AI or human-level AI. Some tasks require hours some take years to learn by humans and when it comes to deciding or behaving, some actions are happens in consciousness and some unconsciousness. Solving a calculus problem, and playing go like a professional takes years to learn but today, these tasks are easy for the AI.

>"AI is harder than we think because we are largely unconscious of the complexity of our own thought processes."

Decades of AI research have proven that the hard tasks, those that require conscious attention, are easier to automate. The human behaviors that we cannot describe are the things that are harder for AI to accomplish. Mitchell's second fallacy is related with the **Moravec's Paradox** which states that easy things that a human can do is actually harder for AI and the same goes for hard tasks.

For instance, there are things like linguistic skills, and acting skills that are relatively easy for humans but today's AI cannot accomplish those tasks easily. There are some sensorimotor tasks that are very difficult fields for AI but humans can master them without much training.

Hans Moravec talks related to that fallacy "Encoded in the large, highly evolved sensory and motor portions of the human brain is a billion years of experience about the nature of the world and how to survive in it. The deliberate process we call reasoning is, I believe, the thinnest veneer of human thought, effective only because it is supported by this much older and much more powerful, though usually unconscious, sensorimotor knowledge. We are all prodigious Olympians in perceptual and motor areas, so good that we make the difficult look easy".

![Fallact Three](/assets/img/why_ai_is_harder_than_we_think/ai_reading_book.webp)

## Fallacy 3: The lure of wishful mnemonics

>"Neural networks are loosely inspired by the brain, but with vast differences."

AI is created to accomplish the tasks that humans can do and Deep Learning is inspired by the human brain however, AI is not exactly imitating the human brain. When we use terms like **understand** or **learn** for AI, it is not as same as with the common sense of understanding or learning that happens in the brain. The AI that we called learned something, like a human brain, cannot use the learned context in another field as a human being right now. Of course, there are some studies around *transfer learning*, that would expect to use learned knowledge in another field.

The third fallacy is misusing or misinterpreting terminology that is used about AI. More basically it is about using the same words for human actions and AI capabilities. About a common term, when we use learning for an AI most people assume that as a human-like behaving process, however, it is far different from that and AI learning based on mathematical optimization processes. These complexities lead by media or some research and enable societies and even some researchers to misinterpret the results of AI.

![Fallacy Four](/assets/img/why_ai_is_harder_than_we_think/vitruvian_man.webp)

## Fallacy 4: Intelligence is all in the brain

It is important to look at the statement of Mitchell;

>"The so-called “information-processing model of mind” arose in psychology in the mid-twentieth century. This model views the mind as a kind of computer, that inputs, stores, processes, and outputs information. The body does not play much of a role except in the input (perception) and output (behavior) stages. Under this view, cognition takes place wholly in the brain, and is, in theory, separable from the rest of the body."

The fourth and last fallacy is associating the phenomenon of intelligence with the human brain, not whole-body interactions. While interpreting human intelligence and AI together only the human brain and its acts are considered even though the interaction of the human body with nature is known. 

Several disciplines mentioned the evidence for embodied cognition. There are several cognitive scientists who argue for the centrality of the body in all cognitive activities.  Psychologist Rebecca Fincher-Kiefer states that "Embodied cognition means that the representation of conceptual knowledge is dependent on the body: it is multimodal..., not amodal, symbolic, or abstract". A neuroscientist, Don Tucker mentioned that "There are no brain parts for disembodied cognition".

"Related to the theory of embodied cognition is the idea that the emotions and the **irrational** biases that go along with our deeply social lives," Mitchell says. These irrational biases make us human beings and humans are not "pure intelligence" creations independent from emotions or constraints of the body. Forgetting all the emotions and interactions with the environment can mislead AI to understand the world and can be devastating. The devastation of a super-intelligent system is reflected in the paper with a simple example;

>"What if a superintelligent climate control system, given the job of restoring carbon dioxide concentrations to preindustrial levels, believes the solution is to reduce the human population to zero?... If we insert the wrong objective into the machine and it is more intelligent than us, we lose"

*That quote reminds me of "I, Robot" by Isaac Asimov and the three laws of robotics.*

### Bottom Line

In the conclusion of the paper, in my opinion, and sense of humor, Mitchell states something interestingly funny and on the other side very sharp determination. Actually, Mitchell gives a quote from AI researcher Terry Winograd from 1977; *"In some ways [AI] is akin to medieval alchemy. We are at the stage of pouring together different combinations of substances and seeing what happens, not yet having developed satisfactory theories...but...it was the practical experience and curiosity of the alchemists which provided the wealth of data from which a scientific theory of chemistry could be developed"*. In the end, I believe that funny statement is still true in today's research and AI applications.

These fallacies should be open questions to think about. I believe that while interpreting the results of AI, research and developments should be done in a scientific sense while considering the psychology of humans and the philosophy of AI.

>"Instead of trying to produce a programme to simulate the adult mind, why not rather try to produce one which simulates the child’s?" - Alan Turing
