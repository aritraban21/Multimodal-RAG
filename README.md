# Multimodal RAG

This project implements a simple multimodal Retrieval-Augmented Generation (RAG) pipeline using text, PDFs, images, and videos.

Embeddings are generated using `gemini-embedding-001`, and images and video chunks are summarized using Video-LLaVA.

### Example 1 (Pdf-based)

**Query:**
> What are big hurdles for quantum computers ?

**Answer:**
> Quantum systems suffer from decoherence, and noise and error rates are major obstacles. Scalability remains an engineering challenge. Additionally, many quantum computers use superconducting circuits which must be cooled to near absolute zero temperatures.

---

### Example 2 (Image-based)

**Query:**
> Explain the email process flowchart ?

**Answer:**
> The email process flowchart is drawn on a white piece of paper and maps the workflow from start to finish through several stages:
> **Request for Data:** Located at the top left corner.
> **Data Input:** Located below the "Request for Data" box.
> **Email Setup** and **Mail Send:** Two boxes following underneath each other.
> **Email Received**, **Read by Recipient**, **Response Sent**, and **Response Read:** Four boxes arranged in sequence further down.

---

### Example 3 (Video-based)

**Query:**
> What is the color of the purse carried by the woman in the white dress ?

**Answer:**
> The purse is silver in color.

---

### Example 4 (Hallucination-test)

**Query:**
> What are topological qubits and how do they reduce decoherence?

**Answer:**
> Not found in documents.

---

## Setup

1. Download `documents.zip` (Code provided in the script for this)
2. Run the code in scripts folder

Note : It is recommended to run this on Google Colab with A100 GPU and High RAM.

Put documents and media in the following folder structure :
```
    ├── documents
    │   ├── image
    │   │   └── img1.png
    │   │   └── img2.png
    │   │   └── ...    
    │   ├── video
    │   │   └── vid1.mp4
    │   │   └── vid2.mp4
    │   │   └── ...    
    │   ├── pdf
    │   │   └── doc1.pdf
    │   │   └── doc2.pdf
    │   │   └── ...   
    │   ├── text
    │   │   └── file1.txt
    │   │   └── file2.txt
    │   │   └── ...   
```
