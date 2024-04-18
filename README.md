

## Skincare Context Retrieval and Answer Generation System
This repository contains a system that retrieves context from a database based on a query and utilizes a Large Language Model (LLM) to generate an answer from the retrieved context.

## Workflow

1. Scraping Skincare Articles: The system scrapes various skincare articles from the internet to gather data.

2. Preprocessing Articles: The scraped articles undergo preprocessing to prepare them for further processing.

3. Chunking and Embedding: The articles are converted into chunks of 256 tokens, and their embeddings are computed.

4. Database Setup: PostgreSQL Docker image is run, and the vector extension is enabled using pgAdmin4 to facilitate efficient storage and retrieval of chunks and their corresponding embeddings.

5. Data Storage: Chunks and their embeddings are saved in a PostgreSQL database for easy access and retrieval.

6. Querying Related Topics: The system finds related topics from the index given a query to narrow down the search space.

7. Answer Generation: Using the LLM provided by LLMWare, the system generates answers based on the query and related topics retrieved from the database.


Installation:


1. Clone the repository:

2. Install dependencies: pip install -r requirements.txt


Usage

Ensure PostgreSQL Docker image is running with vector extension enabled.

Run the Python script to set up the database and store chunks with embeddings.
