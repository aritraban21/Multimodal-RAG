# Multimodal RAG

This project implements a simple multimodal Retrieval-Augmented Generation (RAG) pipeline using text, PDFs, images, and videos.

Embeddings are generated using `gemini-embedding-001`, and images and video chunks are summarized using Video-LLaVA.

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
