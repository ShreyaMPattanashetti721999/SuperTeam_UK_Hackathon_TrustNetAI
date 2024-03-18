# TrustNetAI

# AI-Enhanced Security for Solana Blockchain

## Introduction

This project aims to leverage artificial intelligence (AI) to enhance the security within the Solana blockchain network. Using advanced AI techniques, we analyze transaction data to detect potential fraud and ensure content integrity, providing a safer blockchain ecosystem for users and developers.

## Methodology

The project utilizes a multi-step process involving data loading, processing, AI model interaction, and indexing via Pinecone, followed by AI analysis for content and transaction security. Here is an overview of the methodology used:

1. **Library Installation**: Essential libraries are installed to support AI model functions, data processing, and vector storage.

2. **Data Loading**: Data is loaded from a PDF, likely containing Solana whitepapers or relevant blockchain transaction data.

3. **Text Splitting**: Loaded data is split into manageable chunks for easier processing.

4. **Embeddings Generation**: Each text chunk is processed to create embeddings that capture the semantic meaning of the text, which are essential for similarity searches.

5. **Vector Storage with Pinecone**: The generated embeddings are stored using Pinecone, a vector database optimized for similarity search.

6. **Similarity Search Setup**: The infrastructure for performing similarity searches on the indexed data is initialized.

7. **AI Model Interaction**: Utilizing a pre-trained model, likely a version of GPT (such as a Llama model), the system is set up to process queries and detect patterns indicative of fraudulent activity.

8. **Index Creation and Management**: An index is created in Pinecone to manage the embeddings, allowing for efficient retrieval during similarity searches.

9. **Model Conversion and Loading**: The AI model is converted to a format suitable for the environment, and loaded for execution.

## Execution Flow

The code in `LLM_SOL.ipynb` appears to follow these steps for execution:

1. Install necessary Python packages using `pip`.
2. Load the dataset from a PDF file, which in this context is the Solana whitepaper.
3. Split the loaded document into smaller chunks using a text splitter.
4. Generate embeddings for each text chunk using a pre-trained model from Hugging Face.
5. Initialize the Pinecone environment and create an index for storing embeddings.
6. Execute similarity search queries to find relevant information within the indexed data.
7. Pass queries through an LLM (large language model) for processing and analysis.
8. Manage the Pinecone index, checking its existence and stats, and performing cleanup if necessary.

## How to Run

Ensure you have Python 3.x installed and then follow these steps to set up the environment:

```bash
pip install -r requirements.txt

Contributing
Contributions are welcome! For major changes, please open an issue first to discuss what you would like to change. Please ensure to update tests as appropriate.

License
This project is open-sourced under the MIT license.


