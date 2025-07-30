📚 GeoRAG-Qinhang
GeoRAG-Qinhang is an open-source, retrieval-augmented generation (RAG) question-answering system for geological domains. This project demonstrates how to build a domain-specific QA pipeline using large language models (LLMs) and semantic vector retrieval, with a case study focused on the Qinhang Metallogenic Belt in South China.

🔍 Overview
This repository provides an end-to-end pipeline for domain-specific knowledge engineering and QA generation, including:

PDF Extraction – Extract and clean geological knowledge from scientific documents.

Text Embedding – Transform QA pairs into vector representations.

Semantic Retrieval – Retrieve relevant answers from a domain-specific corpus.

LLM Integration – Generate answers using retrieval-augmented large language models.

🧠 Built with modularity and extensibility in mind: you can easily replace the corpus and apply the method to other metallogenic belts or geoscientific domains.


🌐 Qinhang Metallogenic Belt Corpus
The QA corpus includes over 100 bilingual questions and answers related to:

Geological background

Ore-forming processes

Structural settings

Representative ore deposits

Tectonic evolution

Mineral resources and exploration potential

These are derived from domain literature and are integrated into the RAG system to support intelligent, contextualized responses from LLMs.

🚀 How to Use

1.Install dependencies:
pip install -r requirements.txt

2.Run PDF to TXT processing:
python src/1_pdf_to_txt.py

3.Convert TXT to vector index:
python src/2_txt_to_vector.py

4.Perform semantic retrieval:
python src/3_retrieval.py

5.Generate answers via RAG + LLM:
python src/4_rag_generation.py
Or use the Jupyter Notebook: notebooks/demo_workflow.ipynb

🔁 Adaptation to Other Domains
To apply this system to other regions (e.g., Tianshan, Qilian), simply replace the corpus_qinhang.xlsx file with a new QA dataset, and rerun steps 2–5.

📜 Citation & License
This project is part of a research submission to Minerals (MDPI).
If you use this project or dataset, please cite accordingly (citation to be added upon acceptance).

License: MIT

📫 Contact
For questions or collaboration inquiries, please contact:
Jianhua
Email: 05161935@cumt.edu.cn
Institution: Sun Yat-sen University, China
