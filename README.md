# 🧠 RAG Pipeline with LangChain, Chroma, and OpenAI Embeddings

This project demonstrates a **Retrieval-Augmented Generation (RAG)** pipeline using [LangChain](https://www.langchain.com/), [ChromaDB](https://www.trychroma.com/), and [OpenAI Embeddings](https://platform.openai.com/docs/guides/embeddings). It is designed to showcase how structured and unstructured content (like documents, tables, summaries, and metadata) can be indexed and queried to enhance LLM-based question answering.

![RAG Diagram](https://d3lkc3n5th01x7.cloudfront.net/wp-content/uploads/2024/08/26051537/Advanced-RAG.png)

> Inspired by LangChain’s [Semi-Structured and Multi-Modal RAG Cookbook](https://github.com/langchain-ai/langchain/blob/master/cookbook/Semi_structured_and_multi_modal_RAG.ipynb?ref=blog.langchain.dev).

---

## What This Notebook Does

| Step                     | Purpose                                                            |
| ------------------------ | ------------------------------------------------------------------ |
| 1. Setup                 | Configure environment variables and dependencies                   |
| 2. Document Loading      | Load and chunk PDF/text into smaller parts                         |
| 3. Embedding             | Generate semantic embeddings with OpenAI                           |
| 4. Storage               | Store vectors in **ChromaDB** and metadata in **InMemoryDocstore** |
| 5. Multi-Vector Indexing | Index summaries + full content separately                          |
| 6. Retrieval             | Use `MultiVectorRetriever` for hybrid search                       |
| 7. QA Chain              | Answer queries with context-aware LLM responses                    |

---
