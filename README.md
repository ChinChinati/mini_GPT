---
# mini_GPT: A Smaller Version of ChatGPT-3
### Project Source Code: [[Github]](https://github.com/ChinChinati/mini_GPT/)

## **Overview**  
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

## Project Source Code

You can find the complete source code and implementation details in the [mini_GPT GitHub Repository](https://github.com/ChinChinati/mini_GPT/).

---

## Code Usage Guidelines

### Installation
Ensure you have the following required packages installed:  
- `torch==2.4.0+cu121`  
- Python version **3.10**

Install dependencies via pip:
```bash
pip install torch==2.4.0+cu121
```
### Prepare the Dataset

Download the **Shakespeare Dataset** and place it in the `data/` folder.

## Running the Code

The project contains two main files, **`v2.py`** and **`gpt.py`**, which differ in model size. Choose the file that suits your computational resources:

- Adjust the model size in the respective file by editing the configuration parameters such as the number of layers, attention heads, or embedding dimensions.

### Steps to Run:

1. Clone the repository:
   ```bash
   git clone https://github.com/ChinChinati/mini_GPT.git
   cd mini_GPT
   ```

### Run the Training Script

Use one of the following commands to train the model, depending on the model size you prefer:

```bash
python v2.py
# or
python gpt.py
```
