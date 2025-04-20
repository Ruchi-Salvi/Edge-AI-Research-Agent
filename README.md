# 🤖 Simulated Edge AI Research Agent (LangChain + FAISS)

This project implements a **mock research agentic system** using LangChain with `FakeLLM` and `FakeEmbeddings` — perfect for offline testing and fast prototyping. The system simulates how AI agents can collaborate to collect, organize, and draft answers from research data.

## 🧠 Project Overview

This dual-agent system includes:

- 🕵️‍♂️ **Research Agent** – loads predefined documents related to Edge AI and processes them using text splitting and vector storage.
- ✍️ **Answer Drafter Agent** – retrieves relevant chunks and generates a mock response using LangChain’s `RetrievalQA` chain and a fake LLM.

Designed without any API keys, this system is **safe to run offline**, easy to experiment with, and demonstrates the core components of an agentic research pipeline.

---

## 📂 File Structure

---

## 🏗️ Architecture

```text
[User Input]
   |
   v
[Research Agent (mock documents)]
   |
   v
[Recursive Chunking + FakeEmbeddings]
   |
   v
[FAISS Vector Store (vector index)]
   |
   v
[RetrievalQA + FakeListLLM]
   |
   v
[Final Answer + Source Attribution]
