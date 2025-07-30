📚 GeoRAG-Qinhang: Domain QA System for the Qinhang Metallogenic Belt
GeoRAG-Qinhang is an open-source, retrieval-augmented generation (RAG) question-answering system tailored for geological research. This project integrates domain-specific knowledge from the Qinhang Metallogenic Belt with modern large language models (LLMs), showcasing an end-to-end pipeline for intelligent question answering based on scientific literature.

This repository is part of a research submission to Minerals (MDPI) and demonstrates how RAG techniques can be applied to support mineral resource analysis, structural geology interpretation, and exploration decision-making in a specific tectonic setting.

🔍 Overview: End-to-End GeoQA Workflow
This repository offers a fully modular and reproducible pipeline for constructing geological QA systems, including:

📄 PDF Parsing – Extract geological knowledge from scientific literature (English and Chinese).

✂️ Text Cleaning & Chunking – Preprocess documents into semantically coherent text blocks.

📊 Vector Embedding – Encode text chunks using multilingual semantic models.

🔍 Semantic Retrieval – Search relevant context using FAISS-based vector databases.

🤖 LLM Answer Generation – Use large language models (e.g., GLM-4) for contextualized QA.

The entire system is built for adaptability across languages, domains, and geological regions.

🌐 Qinhang QA Corpus: Structured Geological Knowledge
To support intelligent question answering, we have developed a high-quality, bilingual (Chinese-English) QA dataset specific to the Qinhang Metallogenic Belt, featuring:

Geological setting and tectonic framework

Ore-forming processes and metallogenic stages

Representative deposits and ore types

Magmatic and structural controls

Crustal evolution and metallogenic events

Resource potential and metallogenic zoning

The dataset includes 100+ manually curated QA pairs derived from authoritative geological sources and is fully integrated into the RAG pipeline.

🚀 How to Use

# 1. Install required packages
pip install -r requirements.txt

# 2. Convert PDFs to cleaned text blocks
python src/1_pdf_to_txt.py

# 3. Embed text blocks and build FAISS index
python src/2_txt_to_vector.py

# 4. Perform semantic retrieval
python src/3_retrieval.py

# 5. Run full RAG-based QA using an LLM
python src/4_rag_generation.py
▶️ Or explore the end-to-end process in the Jupyter notebook:
notebooks/demo_workflow.ipynb

🔁 How to Adapt to Other Regions
This system can be adapted to other metallogenic belts or geoscientific domains (e.g., Tianshan, Qilian) by:

Replacing the QA dataset (corpus_qinhang.xlsx) with a new set of domain-specific questions and answers.

Running Steps 2–5 to regenerate the vector index and QA capabilities.

The modular design ensures fast migration with minimal code changes.

📜 Citation & License
This project supports a manuscript submission to Minerals (MDPI).
If you use this code or dataset in your research, please cite this repository (citation information will be added upon acceptance).

License: MIT

📫 Contact
Author: Jianhua
Institution: Sun Yat-sen University, China
Email: 05161935@cumt.edu.cn

