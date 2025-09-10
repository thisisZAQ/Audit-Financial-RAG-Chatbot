# Overview
This project builds a Retrieval-Augmented Generation (RAG) chatbot that allows users to interact with the Irish Continental Group’s (ICG) annual reports (2020–2024) using natural language queries.
Instead of manually searching through lengthy PDF reports, consultants and analysts can now ask questions directly — such as:
“What were the main revenue drivers in 2022?”
“How did passenger volumes change post-COVID-19?”
“What strategic risks were highlighted in 2023?”
The chatbot retrieves relevant report sections and provides concise, AI-generated answers backed by source citations.

# Why This Project?
Consultants, financial analysts, and policymakers often rely on company annual reports for due diligence, market research, and strategic insights. However, reports are often:
Lengthy (100+ pages each year)
Technical (dense financial and regulatory language)
Time-consuming to analyze manually
By applying RAG with Pinecone + HuggingFace embeddings, this project streamlines the process, allowing professionals to extract key insights faster and make data-driven recommendations more efficiently.

## Features
📂 PDF ingestion – loads ICG annual reports (2020–2024)
🧩 Chunking – splits reports into semantically meaningful text segments
🧠 Embeddings – generates vector embeddings using HuggingFace (all-MiniLM-L6-v2)
📦 Vector Database – stores embeddings in Pinecone for efficient retrieval
💬 RAG Querying – natural language queries are matched against the most relevant report sections
⚡ Fast & Scalable – optimized with batch embeddings for large document collections

## Tech Stack
Python
LangChain (document loading & text splitting)
HuggingFace Embeddings (sentence-transformers/all-MiniLM-L6-v2)
Pinecone (vector database)
Google Drive / Local PDFs (data source)
