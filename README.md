<ul align="center" style="list-style: none;">
    <summary>
      <h1>Financial Analysis Agent Hackathon (KidDee1)</h1>
    </summary>
</ul>

<div style="list-style: none;">
    <summary>
      <h1>Gemini-2.5-Flash</h1>
    </summary>
</div>
## Agent Design and Functionality
This repository contains a financial analysis agent developed to compete in the "financial-analysis-agent" competition on Kaggle. The agent is designed to respond to multiple-choice and open-ended financial questions using a zero-shot approach, powered by Google's Gemini 2.5 Flash model.

## Core Functionality
The primary function of this agent is to analyze and answer a diverse set of financial queries. These queries, which are provided in both English and Thai, cover a wide range of financial topics. The agent is engineered to provide precise and concise answers, making it ideal for automated financial analysis tasks.

## Technical Implementation
The agent is implemented in a Python environment, leveraging several key libraries and APIs:

- Google Colab: The agent is designed to run in a Google Colab environment, which provides the necessary computational resources for a wide range of data science and machine learning tasks.

- Kaggle API: The agent uses the Kaggle API to download the competition dataset, which includes the financial queries that the agent is designed to answer.

- Pandas: The agent uses the Pandas library for data manipulation and analysis, allowing it to efficiently process the competition data.

- Gemini 2.5 Flash: The agent uses the Gemini 2.5 Flash API to generate answers to the financial queries. This model is well-suited for this task due to its balance of speed and performance.

## Error Handling and Post-Processing
The agent includes error handling to manage potential issues during the data processing and answer generation phases. Additionally, the agent performs post-processing on the generated answers to ensure that they are in the correct format for the competition submission. This includes extracting the first character of the answer and mapping it to the appropriate response (e.g., 'Rise' or 'Fall').

This agent showcases a practical application of large language models in the financial domain, providing a robust solution for automated financial analysis.

<div style="list-style: none;">
    <summary>
      <h1>Qwen/Qwen3-8B</h1>
    </summary>
</div>

## Agent Design and Functionality
This repository contains a sophisticated financial analysis agent designed for the "Financial Analysis Agent Hackathon." The agent leverages the powerful Qwen/Qwen3-8B model to analyze and answer complex financial questions in both English and Thai.

## Core Functionality
The agent's primary function is to provide expert-level answers to a variety of financial queries. It employs a multi-step reasoning process to deconstruct and analyze each question before formulating a final answer. This Chain-of-Thought (CoT) approach enhances the accuracy and relevance of the agent's responses.

## Technical Implementation
The agent is built using Python and relies on the Hugging Face transformers library to work with the Qwen model. Here's a breakdown of the key components:

- Environment Setup: The agent is configured to run in an environment with specific package requirements and sets up cache directories for Hugging Face models, datasets, and other assets to ensure efficient execution.

- Model and Tokenizer: The agent utilizes the Qwen/Qwen3-8B model and its corresponding tokenizer, which are loaded and cached locally. The model is configured to automatically use available GPUs for optimized performance.

- Data Handling: The agent uses the pandas library to load and manage the competition's test data, as well as to store and export the results.

## Multi-Step Reasoning Process
The agent follows a structured, three-stage process to generate its answers:

1. Concept Identification: In the first stage, the agent analyzes the query to identify the key financial concepts, the type of reasoning required, and the potential data needed to answer the question. This is guided by a system prompt that primes the model to act as a financial question analyst.

2. Critical Analysis: Next, the agent performs a critical analysis of the question's structure, clarity, and logic. This step is guided by a system prompt that encourages the model to think like a senior critical-analysis assistant and evaluate the question's quality.

3. Final Answering: In the final stage, the agent synthesizes the original query, the identified concepts, and the critical analysis to generate a final answer. A specific system prompt is used to ensure the model provides a concise answer in the required format (e.g., "A," "B," "Rise," or "Fall").

## Answer Post-Processing
After generating the answers, the agent performs a cleaning step to format the output correctly. This includes removing any extraneous text, such as "Answer:," and standardizing terms (e.g., converting "ขึ้น" to "Rise" and "ลง" to "Fall") to meet the competition's submission requirements.

## Evaluation
The agent's performance is evaluated by comparing its generated answers with a baseline dataset, using accuracy as the primary metric. This demonstrates a commitment to quality and continuous improvement.

This multi-faceted approach allows the agent to tackle a wide range of financial questions with a high degree of accuracy and domain-specific expertise, making it a powerful tool for financial analysis.
