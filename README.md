# RAG-Pipeline-
RAG pipeline python code by Idris Hull-Delgado

This project provides a fully working Google Colab–based Retrieval-Augmented Generation (RAG) pipeline designed to run on Python 3.12 with minimal setup friction. The workflow supports interactive PDF uploads (no hardcoded files), automatic GGUF model download, and CPU-only inference using llama.cpp, avoiding local compilation issues common in Colab environments.
The notebook installs prebuilt CPU wheels for llama-cpp-python, pins a known-stable version to prevent build failures, and configures LlamaIndex with a Hugging Face embedding model for reliable vector search. A Mistral-7B Instruct GGUF model is downloaded and standardized to a predictable local path to simplify model loading and reuse.
The pipeline extracts text from uploaded PDFs, builds a vector index, and executes semantic queries using a retriever-synthesizer architecture. Default LLM settings are tuned for CPU safety, with clear paths to enable GPU acceleration if the runtime is upgraded. The result is a reproducible, end-to-end RAG example suitable for contracts, documents, and long-form PDFs.

Ideal for developers looking to:
<br>-Run local LLM-powered RAG in Colab without compilation
<br>-Experiment with GGUF models and llama.cpp
<br>-Build document-question-answering systems using LlamaIndex
