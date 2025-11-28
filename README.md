# Build-a-Complete-Medical-Chatbot-with-LLMs-LangChain-Pinecone-Flask-AWS
This project is a Medical Chatbot designed to help medical students quickly access information without reading large medical encyclopedias. For example, a book like **Gale Encyclopedia of Medicine** has 4505 pages, which is overwhelming to read cover-to-cover. This chatbot allows students to ask questions and get relevant, precise answers from medical documents using AI Gemini, LangChain, and Pinecone.

Its main purpose is to save time, improve learning, and provide easy access to medical knowledge in a user-friendly way.

## Features

* PDF upload and text extraction

* Semantic search using embeddings

* RAG pipeline with Pinecone Vector DB

* AI responses via Gemini 2.5 Pro 

* Flask backend with HTML/CSS frontend

* AWS deployment ready

* Docker containerized for easy deployment

## Tech Stack

* Backend: Python, Flask, LangChain, Gemini 2.5 Pro, Pinecone, Sentence Transformers, pypdf
* Frontend: HTML, CSS
* Database: Pinecone Vector Store
* Deployment: AWS EC2, ECR, Docker

## Installation

### Clone the repository

### Create a conda environment after opening the repository


* conda create -n medibot python=3.10 -y

* conda activate medibot

### install the requirements

* pip install -r requirements.txt


### Create a `.env` file in the root directory and add your Pinecone & genai credentials as follows:

```ini
PINECONE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
GOOGLE_API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxx"
```


```bash
# run the following command to store embeddings to pinecone
python store_index.py
```

```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up localhost:
```

