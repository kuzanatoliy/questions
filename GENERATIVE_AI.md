# Generative AI

<details>
  <summary>What are concepts of Generative AI?</summary>

- **Deep learning(DL)** - a type of ML(machine learning) that involves trainign artificial networks;
- **Machine learning(ML)** - a branch of AI that teaches computers to recognize patterns through data and algorithms;
- **Artificial Intelligence(AI)** - a concept referring to a computer's capability to learn and make decisions in a human-like manner.

</details>

<details>
  <summary>What is an Artificial Intelligence?</summary>

AI is a science that helps computers and machines act “smart,” think like humans, and complete tasks on their own. Its main goal is to create systems that understand the world, adapt to changes, and interact well with people. AI aims to boost our abilities, increase efficiency, and transform our lives by learning, reasoning, solving problems, and making decisions.

</details>

<details>
  <summary>What is an Machine learning?</summary>

AI focuses on giving computers human-like abilities, while ML trains them to do these tasks. Unlike traditional programming, ML doesn't use explicit logic coding. Instead of manually setting search engine rules, computer models now learn user preferences and provide personalized content for each person.

</details>

<details>
  <summary>What is an Encoder?</summary>

The encoder takes an input sequence (prompt), scans it by traversing through multiple internal layers, and identifies relevant blocks. It is then passed to the decoder utilizing a self-attention mechanism.

</details>

<details>
  <summary>What is a Self-attention mechanism?</summary>

The self-attention mechanism helps the system comprehend and process the relationships between words in a sentence or a paragraph. It lives within the “context window”, a dynamic memory for your conversation.

</details>

<details>
  <summary>What is a Decoder?</summary>

Decoder receives relevant blocks from the encoder and generates output using the provided context.

</details>

<details>
  <summary>What is a Language Modeling?</summary>

Language modeling is fundamental to LLMs and involves predicting the next word (token) given the context of the preceding words, using mathematical calculations and probability. With its self-attention mechanism, the transformer architecture enables LLMs to effectively learn and generate language by capturing dependencies and patterns within the input data.

</details>

<details>
  <summary>What are Limitations of Generative AI and Mitigation Techniques?</summary>

- **Cognitive Limitations** - LLMs don't think like humans, and they don’t know if their responses are good or bad. They lack introspection, and they can't understand everything. They might make mistakes, produce fake facts (“hallucinate”) or be biased.
- **Output Quality & Transparency Limitations** - LLMs generate answers based on their training, which might be outdated. The quality of their responses also depends on the questions you ask them, and it's hard to know the reasoning behind their answers.
- **Technical Limitations** - LLMs are new technology, so they can be tricked or attacked. Double-check their outputs before accepting an answer.
- **Privacy, Security & Regulatory Limitations** - LLMs may store data and raise privacy concerns, so using them for sensitive information could lead to legal issues. Be mindful of data regulations and potential copyright issues when using LLMs.

</details>

<details>
  <summary>What is a Prompt Engineering?</summary>

Prompt Engineering is a new discipline that investigates how to develop and optimize prompts to efficiently use language models for various applications.

</details>

<details>
  <summary>What is a Zero-Shot technique?</summary>

The Zero-shot prompting is a technique that involves generating text from an LLM without additional training or fine-tuning. Instead, pre-trained models are used to generate text in response to a human-generated prompt. Zero-shot prompting minimizes the need for additional training, as models have already learned the underlying structure of the language.

</details>

<details>
  <summary>What is a Few-Shot technique?</summary>

The Few-shot prompting involves training LLMs on a few training examples to perform specific tasks. Unlike zero-shot prompt generation, few-shot prompting allows for the customization of LLMs to suit specific task requirements. Few-shot models use a few examples to adapt to a specific type of task, making it a useful method for customizing text generation pipelines.

</details>

<details>
  <summary>What is a Chain-of-Thought technique?</summary>

The Chain-of-Thought prompting is an extension of few-shot prompting. It involves training models to learn the type of relationships that exist between different pieces of text. Models are taught to recognize how different pieces of text are connected and use that knowledge to generate text in response to a prompt. This technique is useful in applications such as question-answering and summarization, which require a deep understanding of the relationships between different pieces of text.

</details>
