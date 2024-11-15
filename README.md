# mini_GPT: A Smaller Version of ChatGPT-3

**Overview**  
**mini_GPT** is a smaller, custom implementation of a transformer-based language model inspired by ChatGPT-3. Designed to run efficiently on my laptop's **RTX 4060 GPU**, mini_GPT offers a practical foundation for understanding the architecture and key concepts behind large language models (LLMs). This project focuses on hands-on implementation and training of a scaled-down version of GPT, using the **Shakespeare Dataset** as a text corpus.

## Key Features

- **Architecture**: mini_GPT features a transformer-based architecture with:
  - **6 attention heads per layer**
  - **6 total layers**
  - **Embedding size of 384**
  
- **Dataset**: The model was trained on the **Shakespeare Dataset**, offering a rich, text-heavy corpus that allowed for experimentation with natural language generation.

- **Training**:  
  - The model was trained overnight on a **single RTX 4060 GPU (8GB)**.
  - Despite producing nonsensical sentences due to the model’s size, the project provided significant insights into the workings of neural networks for NLP tasks.

## Core Concepts Explored

By implementing mini_GPT from scratch, I gained hands-on experience with the following key concepts fundamental to LLMs:
- **Embeddings**: Converting words or tokens into continuous vector representations.
- **Tokens, Keys, and Queries**: Understanding the attention mechanism and how tokens are processed in relation to each other.
- **Multi-Head Attention**: Distributing attention across multiple heads for improved representation learning.
- **Residual Connections**: Maintaining gradient flow through deep networks by allowing direct connections between layers.

## Project Insights

Although the generated text often didn’t make sense, working with **mini_GPT** deepened my understanding of how LLMs function and how training parameters affect model performance. The experience with embeddings, attention mechanisms, and optimization techniques was invaluable for future work in the field of NLP.

---
