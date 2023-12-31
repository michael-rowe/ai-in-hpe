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

## What is a *prompt*?

At the surface level, a prompt is the text (or image) you provide to the language model that initiates your interaction.

At a deeper level, the prompt establishes the context for the interaction.

## Conversational prompting

Most of the prompts you'll use with LLMs are known as *conversational prompts*.

> Conversational affordances are things like digressions and confessions and bold claims that beg for a rejoinder. Talking to another person is like rock climbing, except you are my rock wall and I am yours. If you reach up, I can grab onto your hand, and we can both hoist ourselves skyward. Maybe that’s why a really good conversation feels a little bit like floating ([Mastroianni, 2022](https://www.experimental-history.com/p/good-conversations-have-lots-of-doorknobs)).

Once you realise that you interact with LLMs through conversations, it opens up a wide range of use-cases. However, it also raises difficult questions. If I can interact with expertise in this way, then how long will it be before patients are interacting with generative AI? And not only the commercially available versions; at some point you'll be able to interact with your own medical record through conversation.

> [!NOTE] Reflection
> Explore the conceptual relationships between conversational prompting in generative AI, and Dianne Laurillard's *conversational framework*.

Conversational prompts are a great way to get started using generative AI but they're the least powerful form of prompting. If your initial prompt isn't very specific, LLMs will generate a superficial output. In these cases, it can feel like you're not getting anywhere because the response to your prompt may not be helpful. This is because your initial prompt was too generic, and generic prompts generate generic outputs.

## Structured prompting

Some people refer to this as *prompt engineering* but that feels more like there's a correct way to create the prompt. 'Crafting' brings to mind an iterative process that is more subjective.

Here's Ethan and Lilach Mollick talking through an iterative approach to crafting a more effective prompt.

<iframe width="560" height="315" src="https://www.youtube.com/embed/wbGKfAPlZVA?si=qK5rJIwVtAb7LFNL" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

*Mollick, E, and Mollick, L. (2023). Practical AI for Instructors and Students Part 3: Prompting AI.*

A useful way to think about structuring prompts for more effective outputs is:

- **Role**: Give the language model a persona where you tell it what it is good at.
- **Goal**: Explain what outcome you're looking for.
- **Instruct**: Tell the language model what you want it to do; ask it for examples and steps to follow.

One of the most interesting things about giving the model a persona is that it doesn't need to be a living person, or even a person. Imagine telling the model that it is 'an overburdened hospital, working to provide services to a resource-constrained community', or that it is a 'ventilator, providing life-support to a terminally ill patient, during visiting hours'. This kind of prompt can generate different perspectives that provide an alternative context for a reflective exercise.

Part of the goal statement might be to include specific detail about what you're looking for. After all, you're the expert in this domain and you probably have a sense of what you're looking for. Giving the model a specific goal will help to limit the total space of possible responses, thereby generating a more useful response.

This is a way of inserting yourself and your experience and insight into the prompt, in a [collaborative interaction](./human-ai collaboration.md) with the model that further enhances the quality of the interaction.

**Example** (using [Bard](https://bard.google.com/chat)).

```
You are an ICU nurse with 20 years of experience. You have also completed several leadership and conflict resolution courses. I am a second year nursing student and I have a patient with a complicated presentation that I'm uncomfortable dealing with on my own. However, my clinical supervisor isn't the most approachable person and I'm reluctant to ask for help. Please give me some advice on how I might proceed. Give me examples and a series of steps I can follow.
```

[Click here](https://g.co/bard/share/06f3bdc60da9) to see the response from Bard. In this example you may find that the first response is all you need. However, it can sometimes be the case that the initial interaction isn't enough. When this happens you need to understand how to iteratively craft better prompts (see the next section).

It's a good idea to familiarise yourself with the capabilities of the chatbot and underlying model. You should know if the model is connected to the internet[^1], or if it includes image generation features, or what kinds of file formats you can attach to the conversation. When you know that a model is connected to the internet, you can include additional context in your prompt. For example, you can tell the chatbot to "Find academic papers to support your claims".

There are many examples of these kinds of structures for prompts[^2] but I think they mostly follow some version of the one I suggest here. Try not to get too caught up in the details of what makes an ideal prompt; a good first prompt is less important than iterating on that prompt with follow-up interactions that help you to dig deeper.

For example:

- Explain the second paragraph in simpler language.
- What does X mean?
- Define Y.
- Relate your response to... .
- Why is it important to...?
- What else can you tell me about this?
- I'm not familiar with... . Please expand on each item in your list.
- I'd like you to insert X into the outline.
- Give me a different example.
- What isn't included in the list you've provided?
- Generate a list of questions that will help me to reflect on this.

When you get into the habit of following up with generative AI, you'll quickly find yourself engaging in what feels like a natural conversation with an expert.

### Chain-of-thought prompting

Chain-of-thought prompting is a method that improves the reasoning abilities of large language models by providing a series of intermediate reasoning steps as exemplars in prompting.

This method can improve performance on arithmetic, commonsense, and symbolic reasoning tasks for large language models. The gains in performance can be striking, surpassing even fine-tuned models and achieving new state-of-the-art results.

## Auto-prompting

Things are going to get *really* interesting when language models start generating their own prompts.

This is known as 'self-prompting' or 'auto-prompting' and refers to the process of developing and executing prompts based on an initial input (presumably from a person).

This becomes especially interesting when the model is connected to the internet, and can also write it's own executable code.

Auto-GPT, [an open-source experiment](https://github.com/Torantulino/Auto-GPT), is an early example of auto-prompt technology.


> [!Related] Related
> [Autonomous AI systems](./autonomy.md).

# Additional reading

- Bastian, M. (2023). GPT-4 goes a little AGI with Auto-GPT. The Decoder blog. Retrieved from https://the-decoder.com/gpt-4-goes-a-little-agi-with-auto-gpt/
- Hardman, D. P. (2023). Structured Prompting for Educators. Dr Phil's Newsletter, Powered by DOMS️ AI. Retrieved from https://drphilippahardman.substack.com/p/structured-prompting-for-educators
- Laurillard, D. (2002). *Rethinking University Teaching: A Conversational Framework for the Effective Use of Learning Technologies*.
- Mastroianni, A. (2022). Good conversations have lots of doorknobs. Experimental History. Retrieved from https://www.experimental-history.com/p/good-conversations-have-lots-of-doorknobs
- Mollick, E. (2023). Now is the time for grimoires. One Useful Thing. Retrieved from https://www.oneusefulthing.org/p/now-is-the-time-for-grimoires
- Mollick, E, and Mollick, L. (2023). Practical AI for Instructors and Students Part 3: Prompting AI.
- Wei, J., Wang, X., Schuurmans, D., Bosma, M., Chi, E.H., Xia, F., Le, Q., & Zhou, D. (2022). Chain of Thought Prompting Elicits Reasoning in Large Language Models. _ArXiv, abs/2201.11903_ ([link to article in Semantic Reader](https://www.semanticscholar.org/reader/1b6e810ce0afd0dd093f789d2b2742d047e316d5))

---

**Footnotes**

[^1]: It can be confusing to talk about the model being online. After all, you're online because that's the only way you could be interacting with the model. However, you're connected to the chatbot i.e. the user-facing part of the system. The chatbot in turn, connects to the model that's running on a server somewhere. And it may not be the case that the model is connected to the internet.
[^2]: Another common example I see often is the CIDI framework: Context, Instruction, Details, and Input.