# Multimodal RAG:

**A typical RAG application has two main components:**

* **Indexing**: a pipeline for ingesting data from a source and indexing it. This usually happens offline.

* **Retrieval and generation**: the actual RAG chain, which takes the user query at run time and retrieves the relevant data from the index, then passes that to the model.

  
<p align="center">
  <img src="https://github.com/GitMeP/Multimodal-RAG/blob/5d5ef342ea74bdbf12cde87f2335af068267eff3/images/rag_model.png" alt="RAG Agent Flow" width="1200">
</p>


Let's consider 1 use case where we have a document that could be a PDF consisting of text and image data as information.
<p align="center">
  <img src="https://github.com/GitMeP/Multimodal-RAG/blob/5d5ef342ea74bdbf12cde87f2335af068267eff3/images/pdf_component.png" alt="RAG Agent Flow" width="600">
</p>
