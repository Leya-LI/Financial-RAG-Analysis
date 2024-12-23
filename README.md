# Financial-RAG-Analysis

[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Leya-LI/LLM-API-Explorer/blob/main/LICENSE)
[![GitHub issues](https://img.shields.io/github/issues/Leya-LI/LLM-API-Explorer.svg)](https://github.com/Leya-LI/LLM-API-Explorer/issues)
[![GitHub stars](https://img.shields.io/github/stars/Leya-LI/LLM-API-Explorer.svg)](https://github.com/Leya-LI/LLM-API-Explorer/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/Leya-LI/LLM-API-Explorer.svg)](https://github.com/Leya-LI/LLM-API-Explorer/network)

## Overview

Financial-RAG-Analysis is a financial question-answering project that utilizes 10-K filings, Langchain, and Milvus to provide stakeholders with quick and accurate information retrieval and summarization from complex financial documents.

## Features

- **Data Extraction and Preprocessing**: Extract key information from SEC 10-K filings, such as the cover page data.
- **Text Splitting**: Break down long texts into manageable chunks for embedding and retrieval.
- **Embedding Generation**: Use OpenAI embedding technology to convert text into vector representations for storage and retrieval in Milvus.
- **Similarity Search**: Perform vector search through Milvus to quickly find documents most relevant to the query.
- **Question-Answering System**: Combine RAG models to provide context-based question-answering capabilities to generate accurate and specific responses.

## Technology Stack

- **Langchain**: For building and deploying natural language processing pipelines.
- **Milvus**: Open-source vector database for storing and retrieving vector embeddings.
- **OpenAI Embeddings**: For generating vector representations of text.
- **Docker**: Utilized for deploying Milvus on a Windows system, ensuring a seamless and environment-independent setup.
- **Python**: The primary programming language.

## Installation and Deployment

1. Clone the project repository:
   ```
   git clone https://github.com/Leya-LI/Financial-RAG-Analysis.git
   ```
2. Install dependencies:
   ```
   cd Financial-RAG-Analysis
   pip install -r requirements.txt
   ```
3. Install Milvus using Docker on Windows: For Windows users, Milvus can be installed and managed through Docker to ensure an environment-independent setup.
4. Start the Milvus service and ensure it is running on `http://localhost:19530`.
5. Run Jupyter Notebook:
   ```
   jupyter notebook
   ```
   Open the `LangChain_RAG_Financial_Analysis.ipynb` file to explore the project.

## Usage

- Execute the cells in the Jupyter Notebook in order to understand the data flow and model workflow.
- Input your questions into the `query` variable, and the system will return a summary response based on the 10-K filings.

## Contributing

We welcome contributions to the project. If you have any suggestions for improvements or find issues, please contact us by:

- Creating an Issue
- Submitting a Pull Request

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---
