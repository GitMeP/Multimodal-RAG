# Multimodal RAG:

**A typical RAG application has two main components:**

* **Indexing**: a pipeline for ingesting data from a source and indexing it. This usually happens offline.

* **Retrieval and generation**: the actual RAG chain, which takes the user query at run time and retrieves the relevant data from the index, then passes that to the model.

  
<p align="center">
  <img src="https://github.com/GitMeP/Multimodal-RAG/blob/5d5ef342ea74bdbf12cde87f2335af068267eff3/images/rag_model.png" alt="RAG Agent Flow" width="1200">
</p>


Let's consider 1 use case where we have a document that could be a PDF consisting of text and image data as information.
<p align="center">
  <img src="https://github.com/GitMeP/Multimodal-RAG/blob/5d5ef342ea74bdbf12cde87f2335af068267eff3/images/pdf_component.png" alt="RAG Agent Flow" width="400">
</p>

### Storing and Retrieving Text + Image Data

We should be able to retrieve information based on both the **images** and **text** provided, and then generate the output. However, we first need to determine how to store this combined data (**text + image**) in a vector store.

- For **text data**, we already have various types of embeddings available.
- For **image data**, we need to explore the available embedding methods.
We also need to understand how retrieval will work when querying by **text** and querying by **image**.
---
We'll need a **Multimodal LLM** — meaning a language model trained on both image and text data.  

* Standard LLMs (like GPT) are trained primarily on textual data.  

**Examples of available Multimodal LLMs:**  
- **OpenAI - GPT-4.1**  
- **Google - Gemini Flash 2.5**

### Steps to be followed to be able to solve the problem:
Data Source - PDF (Text & Images)
<p align="center">
  <img src="https://github.com/GitMeP/Multimodal-RAG/blob/26734e0ed69b94079d5c71e785aaf92635c66768/images/pdf_steps.png" alt="RAG Agent Flow" width="1200">
</p>
