# QA Bot for PDF Files

## Overview

This project is a QA bot designed to handle PDF files. It extracts text from PDFs, generates embeddings, and stores them in a Pinecone vector database. Users can query the system, which retrieves relevant text chunks based on similarity scores. The system integrates with the Gemini model for refining user queries.

## Features

- Extracts text from PDF files
- Segments text into chunks
- Generates embeddings using the Gemini model
- Stores embeddings in Pinecone vector database
- Handles user queries and retrieves relevant text chunks
- Refines user queries using the Gemini model
- Maintains user query context for up to 5 consecutive questions

## Requirements

- Docker
- Python 3.8+
- Pip

## Setup

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/qa-bot-pdf.git
   cd qa-bot-pdf
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

3. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up Pinecone:
   - Sign up at [Pinecone](https://www.pinecone.io/) and get your API key.
   - Replace `'your-pinecone-api-key'` in the code with your Pinecone API key.

5. Run the Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

## Usage

1. Open the Jupyter Notebook file `qa_bot_solution.ipynb`.
2. Follow the instructions in the notebook to extract text from PDFs, generate embeddings, store them in Pinecone, and handle user queries.

## Security Considerations

- Ensure that your Pinecone API key is stored securely and not hard-coded in the source code.
- Use authentication and authorization mechanisms to protect access to your system.
- Implement data encryption for sensitive data both at rest and in transit.
- Regularly update dependencies to patch security vulnerabilities.
