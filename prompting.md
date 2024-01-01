---
tags:
  - chain-of-thought
  - prompt
  - Bard
  - Gemini
  - Google
  - DeepMind
---
# Prompting LLMs

Many people approach prompting like they approach internet search. They provide a few keywords and expect 'the answer'. This is the wrong way to think about prompting language models.

Approach language model prompting as if you were having a conversation with a person. This section is about exploring different ways to do this, as well as the implications that arise when we think of interacting with machines through natural human language.

---
## What is a *prompt*?

At the surface level, a prompt is the text (or image) you provide to the language model that initiates your interaction.

At a deeper level, the prompt establishes the context for the interaction.

---

## Structure of a prompt

If your initial prompt isn't very specific, LLMs will generate a superficial output. In these cases, it can feel like you're not getting anywhere because the response to your prompt may not be helpful. This is because your initial prompt was too generic, and generic prompts generate generic outputs.

A useful way to think about structuring prompts for more effective outputs is:

- **Role**: Give the language model a persona where you tell it what it is good at.
- **Goal**: Explain what outcome you're looking for.
- **Instruct**: Tell the language model what you want it to do; ask it for examples and steps to follow.

**Example** (using [Bard](https://bard.google.com/chat), after the [December 2023 update](https://bard.google.com/updates) to [Gemini Pro](./gemini.md)).

```
You are an ICU nurse with 20 years of experience. You have also completed several leadership and conflict resolution courses. I am a second year nursing student and I have a patient with a complicated presentation that I'm uncomfortable dealing with on my own. However, my clinical supervisor isn't the most approachable person and I'm reluctant to ask for help. Please give me some advice on how I might proceed. Give me examples and a series of steps I can follow.
```

[Click here](https://g.co/bard/share/06f3bdc60da9) to see the response from Bard. In this example you may find that the first response is all you need. However, it can sometimes be the case that the initial interaction isn't enough. When this happens you need to understand how to iteratively craft better prompts.

---
## Prompt crafting

Some people refer to this as *prompt engineering* but that feels more like there's a correct way to create the prompt. 'Crafting' brings to mind an iterative process that is more subjective.

Here's an example of someone talking through an iterative approach to crafting a more effective prompt. This is an example of a *conversational prompt* (more on that below).

<iframe width="560" height="315" src="https://www.youtube.com/embed/wbGKfAPlZVA?si=qK5rJIwVtAb7LFNL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

*Mollick, E, and Mollick, A. (2023). Practical AI for Instructors and Students Part 3: Prompting AI.*

There are many examples of these kinds of structures for prompts but I think they mostly follow some version of the one I suggest here. Try not to get too caught up in the details of what makes an ideal prompt; a good first prompt is less important than iterating on that prompt with follow-up interactions that help you to dig deeper.

For example:

- Explain the second paragraph in simpler language.
- What does X mean?
- Define Y.
- Relate your response to... .
- Why is it important to...?
- What else can you tell me about this?
- I'm not familiar with... . Please expand on each item in your list.
- What isn't included in the list you've provided?
- Generate a list of questions that will help me to reflect on this.

When you get into the habit of following up with generative AI, you'll quickly find yourself engaging in what feels like a natural conversation with an expert.

---

## Types of prompts

### Conversational prompting

Most of the prompts you'll use with LLMs are known as *conversational prompts*. 

> Conversational affordances are things like digressions and confessions and bold claims that beg for a rejoinder. Talking to another person is like rock climbing, except you are my rock wall and I am yours. If you reach up, I can grab onto your hand, and we can both hoist ourselves skyward. Maybe that’s why a really good conversation feels a little bit like floating ([Mastroianni, 2022](https://www.experimental-history.com/p/good-conversations-have-lots-of-doorknobs)).

Once you realise that you interact with LLMs through conversations, it opens up a wide range of use-cases. However, it also raises difficult questions. If I can interact with expertise in this way, then how long will it be before patients are interacting with generative AI? And not only the commercially available versions; at some point you'll be able to interact with your own medical record through conversation.

> [!NOTE] Reflection
> Explore the conceptual relationships between conversational prompting in generative AI, and Dianne Laurillard's *conversational framework*.

Conversational prompts are a great way to get started using generative AI. But they're the least powerful form of prompting.

---

### Chain-of-thought prompting

Chain-of-thought prompting is a method that improves the reasoning abilities of large language models by providing a series of intermediate reasoning steps as exemplars in prompting.

This method can improve performance on arithmetic, commonsense, and symbolic reasoning tasks for large language models. The gains in performance can be striking, surpassing even fine-tuned models and achieving new state-of-the-art results.

---

# Additional reading

- Laurillard, D. (2002). *Rethinking University Teaching: A Conversational Framework for the Effective Use of Learning Technologies*.
- Mastroianni, A. (2022). Good conversations have lots of doorknobs. Experimental History. Retrieved from https://www.experimental-history.com/p/good-conversations-have-lots-of-doorknobs
- Mollick, E. (2023). Now is the time for grimoires. One Useful Thing. Retrieved from https://www.oneusefulthing.org/p/now-is-the-time-for-grimoires
- Wei, J., Wang, X., Schuurmans, D., Bosma, M., Chi, E.H., Xia, F., Le, Q., & Zhou, D. (2022). Chain of Thought Prompting Elicits Reasoning in Large Language Models. _ArXiv, abs/2201.11903_ ([link to article in Semantic Reader](https://www.semanticscholar.org/reader/1b6e810ce0afd0dd093f789d2b2742d047e316d5))

---
