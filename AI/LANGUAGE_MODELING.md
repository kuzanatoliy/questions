# Language modeling

<details>
  <summary>What types of language mdels could be mentioned?</summary>

**Large Language Models (LLMs)** - the advanced version of LMs, are trained on larger datasets and use advanced techniques such as deep learning and transformers to analyze complex relationships between words.

**Small language models (SLMs)** - are compact versions of LLMs that require less training data, have simpler architectures, and are quicker to develop. They are suitable for specific tasks and domains, offering focused expertise and devices with limited processing power.

</details>

<details>
  <summary>What is an Output?</summary>

Since the tokens are generated one at a time, the process of detokenization is also sequential. Based on the model's vocabulary, each token ID is mapped to a specific token. Then tokens are converted into the text output.

</details>

<details>
  <summary>What is a Decoder?</summary>

Decoder receives relevant blocks from the encoder and generates output using the provided context.

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
  <summary>What is a Positional Encoding?</summary>

The model processes embeddings using many layers of neural networks. An essential part of this processing is positional encoding, where special vectors are added directly to the embeddings. They have the same dimension as embeddings and help to preserve sequence information. Thus, even if the same word appears in different positions, its resulting vector representation will be different.

</details>

<details>
  <summary>What is an Embedding?</summary>

After IDs are assigned to tokens, they need to be converted into a set of numbers that define each token's initial semantic meaning. This process employs neural networks and is called embedding. The result of the embedding process is a set of vectors called embeddings. They are used in the transformer model for further processing.

</details>

<details>
  <summary>What is an Input?</summary>

The input or prompt is then tokenized, converting the text into smaller units. Each token is assigned a numberid ID based on the model's vocabulary. This vocabulary is a list where each unique token from the training dataset is associated with a unique index.

</details>

<details>
  <summary>What is a Prompt?</summary>

A prompt is a set of instructions or a question that acts as the initial input for an LLM. It essentially defines the task you want the LLM to perform. It provies context, specifies the desired output format or style, and guides the LLM towards a specific outcome.

</details>

<details>
  <summary>What is a Prompt engineering?</summary>

The prompt engineering is a crucial skill in artificial intelligence, involving crafting prompts to guide an AI tool's responses. To gain this skill, one must learn about AI behavior, language nuances, and the specific requirements of the AI tool.

</details>

<details>
  <summary>What is a Transformer Atchitecture?</summary>

The operation of transformers relies on generating output based on the probability distribution of the next token in a sequence. This process naturally leads to non-deterministic responses, allowing for varied outputs under identical initial conditions.

</details>

<details>
  <summary>What is a Training Data?</summary>

LLMs produce text based on examples and patterns observed in their training data. They mirror all the characteristics of this data, including biases, inaccuracies, and topic specification. The training dataset is relevant up to the cut-off date of the training process. After this date, the model's database does not receive updates or incorporate new information unless retrained or supplemented with external, up-to-date data sources.

</details>

<details>
  <summary>What is a Decision Logic Transparency?</summary>

LLMs perform extensive computations using a complex array of internal settings and parameters. This complexity often makes the input-output relationships within these models difficult to decipher, causing most commercial LMSs to operate as "black boxes".

</details>

<details>
  <summary>What are limitations of LLMs?</summary>

- **Cognitive Constraints and Interaction Challenges** - LLMs perceive and process information differently from humans, leading to potential output limitations. They might make mistakes, produce fake facts, or generate biased responses.
- **Security Risks** - The complex nature of LLMs does not make them immune to risks. They may be susceptible to various forms of cyber threats, including being tricked, attaked, or misused.
- **Privacy and Legal Concerns** - LLMs may store and utilize input data. As such, issues surrounding data protection responsibilities, rights, and compliance with legal regulations arise when using LLMs.

</details>

<details>
  <summary>What are types of hallucinations?</summary>

- **Factual Inaccuracies** - This type of hallucination includes generation text that contains factual errors or that is not based on reality due to a lack of explicit real-world knowledge.
- **Fabrication or Misrepresentation** - This type of hallucination includes creating atrificial sources, making unfonded claims, or designing entirely fictional scenarios. No such links, presentations, or articles exist in this case, but the names and links look like real ones.
- **Nonsensical Output** - LLMs may somethimes respond with completely random, unrelated, or nonsensical answers in real-world context.

</details>

<details>
  <summary>What are types of Security Risks?</summary>

- **Jaibreak Attacks** - This term refers to attempts to `break out` of the restrictions intentionally set by the development team to prevent the model's misuse for illegal or unintended purposes. Attackers often employ various tricks, such as inputting specific combinations of symbols, letters, binary code, base-64 encoding, or queries in different languages.
- **Prompt Injection** - It is about manipulating an LLM or LLM-based application and giving it what looks like new instructions and basically hijacking the system.
- **Data Pisoning/Backdoor Attacks** - LLMs learn from the data on which they are trained. If this training data contains harmful or malicious content, it can influence the model's behavior, leading to dangerous and harmful outputs.

</details>

<details>
  <summary>What are technical parameters of LM?</summary>

- **Model Type & Complexity** - Different models excel at various tasks. Identify your use case to determine the most suitable model type. Model complexity, often measured by the number of parameters, influences performance and resource requirements. More complex models can handle more sophisticated tasks. However, they require more computing power, ptentially increasing training and inference costs.
- **Training Data Size & Diversity** - Larger and more diverse datasets generally lead to better model performance. LLMs trained on extensive data often generalize better accross various tasks. However, this comes at the cost of interpretability. SLMs, with their focused training, provide more interpretable outputs, which can be crucial for tasks like sentiment anlysis. It's essential to note that details regarding training datasets may be considered proprietary and not disclosed by model vendors.
- **Consuming Options & Scalability** - Consider how you'll consume the model and whether your needs might grow over time. Choose a model with a deployment option that suits your infrastructure and scales to meet your evolving demands.
- **Context Window** - Determines how much "memory" the model has when processing information. The context window includes the sizes in tokens of your inputs and model outputs within one dialogue. A larger context size can lead to a better understanding of complex relationships within text. It also increases computaitonal demands and makes it harder for the model to focus on the most relevant information.
- **Knowledge Cut-Off** - Refers to the date the model's training data is current. Recent knowledge cut-off is crucial for tasks requiring up-to-date information or projects in fast-changing fields. However, knowledge cut-off might be less critical for tasks not relying on recent information or where factual accuracy isn't primary.
- **Cost** - Consider the contimuous costs of utilizing the model. LLMs often demand more resources than their smaller, less sophisticated SLM counterparts. This could lead to increased costs for tasks needing frequent model interaction. Pricing strategies for commercial models and tools can range from pay-per-use, where costs depend on the volume of tokens processed, to subscription models, where you pay a fixed rate and gain access to a certain capacity or number of tokens per period. Remember that the model considers all your history inside one dialogue when counting the cost of conversation.

</details>

<details>
  <summary>What are behavioral parameters of LM?</summary>

- **Performance** - This ecompasses accuracy, fluency, and coherence in the model's output. Evaluate how well them model performs on tasks specific to your needs. Consider factors like generalizability to handle various real-world data and processing speed.
- **Explainability & Transparency** - Understanding how the model arrives at its outputs can be crucial. Some models offer more interpretable outputs than others using clear terms, which might be important for tasks requiring reasoning behind the model's decisions.
- **Bias and Fairness** - Language models can inherit biases from their training data. Assess potential biases to ensure the model aligns with your ethical considerations.
- **Safety and Security** - Security features are crucial to prevent model misuse and ensure data privacy. Assess the models regarding their compliance with industry or regional stanards and your project requirements.

</details>
