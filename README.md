# Email-GPT

#### Overview
This project explores the application of transformers in text generation. Specifically, the focus is on implementing a smaller version of the GPT (Generative Pre-trained Transformer) model to generate streams of characters that can form coherent sentences.

#### Dataset
1. The **"tiny shakespeare"** dataset is utilized, which comprises samples of text from Shakespeare's works. It provides a rich variety of linguistic patterns, making it an excellent choice for text generation tasks.
2. **Enron Email Dataset**: Sourced from CMU, this dataset contains a large number of emails from the Enron Corporation. The emails offer diverse styles of communication, from formal to informal, making it a compelling choice for text generation and style imitation. (https://www.cs.cmu.edu/~./enron/)

#### Overview:
Transformers, introduced in the paper "Attention Is All You Need", have revolutionized many tasks in the NLP domain. The GPT model, a variant of transformers, employs stacked decoder-only transformers. Its architecture is particularly adept at text generation because of its capacity to capture long-term dependencies in text. By training on datasets like "tiny shakespeare" and the Enron email corpus, the GPT model can learn and generate intricate patterns, structures, and styles inherent in the source texts.

#### Causal Self-Attention in Transformers
Overview
This repository provides an implementation and exploration of the causal self-attention mechanism, a foundational component in Transformer architectures, especially tailored for generative tasks.

#### What is Causal Self-Attention?
Causal self-attention is a variant of the standard self-attention mechanism. Unlike traditional self-attention, where each token can attend to all other tokens in the sequence, causal self-attention restricts each token to attend only to its predecessors and itself. This ensures that when generating a sequence token-by-token, the model doesn't have premature information about future tokens.

#### Key Characteristics:
1. Unidirectionality: Tokens can only "look back" and not "look forward."
2. Masking Strategy: The attention scores for future tokens are masked, ensuring they don't influence the current token.
3. Generative Advantage: Especially useful for generative tasks like text generation where the sequence is constructed one token at a time.

### Applications:
While models like BERT use bidirectional attention for tasks like text classification, models tailored for generation, such as GPT (Generative Pre-trained Transformer), employ causal self-attention to ensure genuine autoregressive sequence generation.
