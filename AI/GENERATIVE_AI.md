# Generative AI

<details>
  <summary>What are concepts of Generative AI?</summary>

- **Deep learning(DL)** - a type of ML(machine learning) that involves trainign artificial networks;
- **Machine learning(ML)** - a branch of AI that teaches computers to recognize patterns through data and algorithms;
- **Artificial Intelligence(AI)** - a concept referring to a computer's capability to learn and make decisions in a human-like manner.

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

<details>
  <summary>What is a Tree of Thoughts technique?</summary>

An even more intriguing method for prompting, known as the Tree of Thoughts (ToT), has been proposed by a team of researchers aiming to enhance the problem-solving abilities of LLMs. They introduced a framework that can potentially improve the planning and decision-making processes carried out by models, building upon the previously mentioned techniques.

</details>

<details>
  <summary>What fine-tuning process steps could be mention?</summary>

1. **(Re)Validte an Idea** - Before starting to work with a language model, it's crucial for you to have a clear and well-defined idea of what you want to achieve. This involves understanding the problem you're trying to solve and determining if a language model is the right tool for the job. When framing your idea, make sure it is specific, well-articulated, and leaves little room for interpretation.
2. **Improve Prompt or Data** - Once you have a clear idea, the next step is to create or adjust your prompt and (or) data. This involves experimenting with different prompt structures, wording, and parameters to find the most effective combination. Keep in mind that prompt engineering is an evolving field, and staying up-to-date with the latest techniques and best practices can help you get the most out of your language models.
3. **Evalueate Results** - After adjusting your prompt or data, it's essential for you to evaluate the results to determine if they meet your expectations or require further adjustments. This involves comparing outputs, checking for consistency, assessing relevance, evaluating clarity, and testing with multiple examples. Based on your evaluation, you may need to iterate and refine your prompt until you achieve the desired results.

</details>

<details>
  <summary>What are goals of Prompt Formatting?</summary>

Choosing the right prompt format aims to achieve the following objectives:

- **Clarity:** A well-structured prompt provides clear instructions and reduces misinterpretation by LLM.
- **Context:** A prompt serves as a framework for the model to comprehend and address the given question or problem.
- **Specificity:** Well-structured prompts guide the model to generate focused and targeted responses.
- **Consistency:** Providing prompts in a specific format guides the model to respond in the same format. However, if required by your flow, you can request an explicit response format.
- **Efficiency:** A properly formatted prompt can increase cost efficiency and performance, as API users typically incur charges based on the number of prompt tokens used.

</details>

<details>
  <summary>What are goals of Output Formatting?</summary>

Choosing the right result format aims to achieve the following objectives:

- **Readability:** A formatted result makes the generated output easy to read and understand.
- **Presentation:** A well-structured output makes the presentation visually appealing.
- **Accessibility:** Formatted results can be seamlessly integrated and utilized across different platforms and applications.
- **Relevance:** A well-structured output allows for the easy extraction of relevant information and supports efficient analysis and decision-making.
- **Alignment:** Well-shaped results align with the user's purpose and specific requirements.

</details>
