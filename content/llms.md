# Large language models

A large language model is a language model with many parameters (typically billions of weights), trained on large quantities of unlabeled text, using self-supervised machine learning (or semi-supervised learning).

https://youtu.be/ZRf2BfDLlIA?si=RGv3CPKAGOcbGpkO

https://youtu.be/wbGKfAPlZVA?si=4vvKxNkEr7vHUXTY

## Types of language models

Language models can be categorised in several different ways;

1. License
2. Size

### License

[Open-source language models](./open-source-llm.md) e.g. Llama (Meta), and Mixtral (Mistral).

Commercial language models e.g. GPT (OpenAI), and Gemini (Google).

### Size

Language models come in a wide range of sizes. For example, in 2024 LLaMA 2 was available in 7 billion, 13 billion, and 70 billion parameter sizes. Smaller models are cheaper to deploy and run; larger models are more capable (Facebook research, 2024).

### Deployment

Large language models are deployed and accessed in a variety of ways, including:

1. Self-hosted: Using local hardware to run inference. For example, running Llama 2 on a powerful desktop or laptop using an open-source LLM. This is the best option for privacy/security or if you already have a GPU.
2. Cloud hosted: Using a cloud service provider to deploy an instance that hosts a specific model. For example, running an open-source model on cloud providers like AWS, or Azure. This is the best approach for customising models and their runtime (e.g. fine-tuning a model for your use case).
3. Hosted API: Call LLMs directly via an API. There are many companies that provide language model inference APIs including AWS Bedrock, Replicate, Anyscale, Together and others. This is the easiest option overall.

---

# Additional reading

- https://bdtechtalks.com/2023/04/17/open-source-chatgpt-alternatives/
- facebookresearch. (2024, February 07). llama-recipes. Retrieved from https://github.com/facebookresearch/llama-recipes/blob/main/examples/Prompt_Engineering_with_Llama_2.ipynb