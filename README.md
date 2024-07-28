# RAG-Based Chatbot for Therapy Sessions

## Overview
This project focuses on the evaluation and optimization of a Retrieval-Augmented Generation (RAG) pipeline for a chatbot designed to assist in therapy sessions. The chatbot uses a combination of retrieval and generation models to provide relevant and accurate responses based on pre-embedded transcripts from therapy sessions. The primary goal is to calculate and improve key performance metrics to enhance the chatbot's effectiveness.

## Demo
YouTube link: [Therapist Helper ChatBot](https://youtu.be/c3FsyAKlvtc)

## Table of Contents
1. [Introduction](#introduction)
2. [Setup](#setup)
3. [Usage](#usage)
4. [Performance Metrics](#performance-metrics)
5. [Improvements Implemented](#improvements-implemented)
6. [Challenges](#challenges)
7. [Contributions](#contributions)
8. [License](#license)

## Introduction
The chatbot is designed to assist therapists by providing contextually relevant information and responses based on past therapy sessions. It uses OpenAI's language models for both retrieval and generation tasks, ensuring a comprehensive understanding of the user's queries and generating accurate responses.

## Setup
### Prerequisites
- Python 3.7 or higher
- Required Python libraries: OpenAI, scikit-learn, numpy, pandas, transformers, tiktoken

### Installation
1. Clone the repository:
   ```bash
   git clone ithub.com/Mansi-Dabriwal/TherapistHelper.git
   cd therapistBot
   ```
2. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

3. Set up OpenAI API key:
   - Create a `.env` file in the root directory with the following content:
     ```
     OPENAI_API_KEY=your-openai-api-key
     ```

## Usage
### Running the Evaluation
1. **Run the Application**:
   ```bash
   python fastApi.py
   ```
2. **Run the Streamlit Application**:
   ```bash
   streamlit run app.py
   ```
3. **Run the Evaluation**:
   ```bash
   python evaluation.py
   ```
   This script calculates the performance metrics and outputs the results.

### Metrics Calculation
- The project includes scripts for calculating various performance metrics, such as Context Precision, Context Recall, Faithfulness, and more.

## Performance Metrics
The following metrics are calculated to evaluate the chatbot's performance:

1. **Retrieval Metrics**:
   - Context Precision
   - Context Recall
   - Context Relevance
   - Noise Robustness

2. **Generation Metrics**:
   - Faithfulness
   - Answer Relevance
   - Information Integration
   - Counterfactual Robustness
   - Negative Rejection
   - Latency

## Improvements Implemented
1. Enhanced context retrieval to improve recall and relevance.
2. Introduced cross-verification of generated answers to increase faithfulness.
3. Developed filters and validation checks for better handling of counterfactual and negative queries.

## Challenges
- Handling noisy or irrelevant inputs without compromising the quality of retrieved contexts.
- Managing token limits for both retrieval and generation stages.
- Ensuring the faithfulness of generated answers to the source material.

## Contributions
Contributions are welcome! Please fork the repository and submit a pull request with your changes. For major changes, please open an issue first to discuss what you would like to change.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
