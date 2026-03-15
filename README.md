# RAG-For-exchange-students
A Retrieval-Augmented Generation (RAG) assistant designed to help exchange students quickly find information about studying and living in Linz using university guide documents.
# Exchange Student RAG Assistant

This project is a Retrieval-Augmented Generation (RAG) question answering system designed to help exchange students quickly find information about studying and living in Linz.

The idea was inspired by my own experience as an exchange student, where I often had many questions regarding application procedures, course registration, accommodation, and daily life in Linz. Usually, the only option was sending emails to the university and waiting for a response.

This project explores how AI can make this information more accessible through a question-answering assistant.

---

## Project Motivation

Before starting my thesis research, I wanted to build a practical system that applies Retrieval-Augmented Generation in a real-world scenario.

This project serves as a **preparation step for my thesis**, where I plan to research improvements in **Multimodal RAG Question Answering systems**.

---

## How It Works

The system follows a typical RAG pipeline:

1. User selects a category and asks a question
2. The query is converted into embeddings
3. A vector search retrieves relevant document chunks
4. A reranker improves retrieval quality
5. The language model generates an answer using the retrieved context

The model is instructed to answer **only using the retrieved document context** to reduce hallucinations.

---

## Technologies Used

- Sentence embeddings: `all-MiniLM-L6-v2`
- Vector search: FAISS
- Reranking model
- LLM generation: Llama 3.3 70B
- Python
- Jupyter Notebook

---

## Data Source

The knowledge base comes from a publicly available exchange student guide from **Johannes Kepler University Linz**.

The document includes information such as:

- Application procedures
- Important deadlines
- Accommodation
- Health insurance
- Arrival to Linz
- Public transportation

---

## Limitations

Some limitations encountered during development:

- Limited availability of legally usable open data sources
- The knowledge base is based mainly on a single document
- Context understanding can still be improved

Despite these limitations, the system already provides reliable answers to many common questions.

---

## Future Work

This project is only an initial prototype.

My upcoming thesis will focus on improving **Multimodal Retrieval-Augmented Generation (RAG)** systems, exploring how models can retrieve and reason over multiple data modalities such as:

- Text documents
- PDFs
- Images
- Structured data

---

## Example Use Case

Example questions the system can answer:

- "How do I register for courses?"
- "What are the important deadlines?"
- "How do I get from the airport to Linz?"
- "Do I need health insurance?"

---

## Author

AI student at Johannes Kepler University Linz working on Retrieval-Augmented Generation and Multimodal AI systems.
