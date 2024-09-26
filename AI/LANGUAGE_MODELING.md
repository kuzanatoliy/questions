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
