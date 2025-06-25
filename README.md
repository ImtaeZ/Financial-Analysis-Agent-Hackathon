<ul align="center" style="list-style: none;">
    <summary>
      <h1>Financial Analysis Agent Hackathon (KidDee1)</h1>
    </summary>
</ul>

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
