# PDF ChatGPT

A Streamlit application that allows users to upload PDF documents or PowerPoint presentations and ask questions about their content using OpenAI's language models.

## Project Description

PDF ChatGPT is an interactive tool that leverages the power of OpenAI's language models to enable users to have conversations about the content of their PDF documents or PowerPoint presentations. The application processes the uploaded files, extracts the text content, and creates a searchable knowledge base. Users can then ask questions in natural language, and the application will provide relevant answers based on the document content.

### Features

- Upload PDF documents or PowerPoint (PPTX) presentations
- Extract text content from uploaded files
- Create a searchable knowledge base using text embeddings
- Ask questions about the document content
- Get AI-generated answers based on the document content

## Technologies Used

- Python
- Streamlit (for the web interface)
- LangChain (for processing and chaining language model operations)
- OpenAI API (for language model access)
- PyPDF2 (for PDF parsing)
- python-pptx (for PowerPoint parsing)
- FAISS (for efficient similarity search)

## Setup Instructions

### Prerequisites

- Python 3.7 or higher
- OpenAI API key

### Installation

1. Clone the repository:
   ```
   git clone https://github.com/a19hu/pdf_chatgpt.git
   cd pdf_chatgpt
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```
   python -m venv enva
   source enva/bin/activate  # On Windows, use: enva\Scripts\activate
   ```

3. Install the required dependencies:
   ```
   pip install streamlit PyPDF2 langchain openai python-pptx faiss-cpu python-dotenv
   ```

4. Set up your environment variables:
   - Copy the example environment file:
     ```
     cp .env.example .env
     ```
   - Edit the `.env` file and add your OpenAI API key:
     ```
     OPENAI_API_KEY = your_openai_api_key_here
     ```

## Running the Application

1. Make sure your virtual environment is activated (if you're using one).

2. Run the Streamlit application:
   ```
   streamlit run app.py
   ```

3. The application should now be running at http://localhost:8501 (or a similar address as indicated in your terminal).

## Usage Guide

1. Open the application in your web browser.
2. Upload a PDF document or PowerPoint presentation using the file uploader.
3. Once the file is processed, enter your question in the text input field.
4. The application will analyze the document and provide an answer based on its content.
