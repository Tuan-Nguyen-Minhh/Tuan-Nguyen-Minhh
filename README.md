<h1 align="center">Hi, I'm Tuan</h1>

<p align="center">
  <b>AI Engineer & Researcher</b>
</p>

<p align="center">
  <a href="https://linkedin.com/in/tuan-nguyen-minhhh"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  &nbsp;
  <a href="mailto:ng.minhtuann.dev@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email"/></a>
  &nbsp;
  <a href="https://github.com/Tuan-Nguyen-Minhh"><img src="https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub"/></a>
</p>

---

## Overview

I build production-grade AI systems, focusing on **Multi-Agent Orchestration**, **Advanced RAG**, and **Multimodal Perception** (Computer Vision & Document AI). My work bridges practical machine learning research with deterministic, scalable backend architectures.

---

## Featured Projects

### HR Help — Multi-Agent Legal & Policy Assistant
An enterprise AI assistant supporting HR and management in handling labor discipline cases through deterministic retrieval, policy analysis, and strict human governance.

- **Multi-Agent Architecture**: Built with **LangGraph** featuring stateful agent nodes: intent routing, fact clarification, temporal citation retrieval, and recommendation drafting.
- **Hybrid & Graph Retrieval**: Combines **pgvector** (1024-d) and **BM25** with Reciprocal Rank Fusion (RRF), Cohere reranking, and a 1-hop Citation Knowledge Graph to verify regulations effective at incident dates.
- **Human-in-the-Loop (HITL)**: Enforces strict guardrails—agents analyze and draft documents while all approval, rejection, and signing actions remain exclusively with human authorities.
- **Tech Stack**: LangGraph, FastAPI, PostgreSQL (pgvector), Docker, Vite, React, TypeScript.
- **Links**: [Live Demo](https://c4-app-029.vercel.app/) · [Repository](https://github.com/Tuan-Nguyen-Minhh/HRHelp)

### Real-Time American Sign Language (ASL) Recognition
A low-latency, hybrid computer vision application for real-time American Sign Language translation deployed to the web.

- **Hand Localization**: Integrated **YOLOv8** for high-precision hand bounding box detection across complex, dynamic backgrounds.
- **Spatial Landmark Extraction**: Leveraged **MediaPipe** to extract 21 3D hand landmarks, reducing high-dimensional video streams into compact spatial coordinate vectors.
- **Lightweight Inference**: Trained an **SVM** classifier for gesture-level prediction, optimized for real-time CPU and edge-device inference with high stability.
- **Tech Stack**: Python, OpenCV, MediaPipe, YOLOv8, scikit-learn, Web Deployment.
- **Links**: [Live Demo](https://web-american-sign-language.vercel.app/)

### Vietnamese Receipt OCR & Information Extraction
*Undergraduate Thesis Research* — An end-to-end pipeline for Key Information Extraction (KIE) and layout analysis from low-quality, thermal Vietnamese retail receipts.

- **Document Localization**: Developed a multi-stage pipeline utilizing **YOLO** for receipt boundary detection and semantic field segmentation.
- **OCR Engine**: Fine-tuned **VietOCR** to handle diacritics, noisy backgrounds, skewed orientations, and thermal printer fading.
- **Information Extraction**: Implemented spatial heuristic post-processing to reconstruct unstructured visual text into validated JSON schemas for downstream retail systems.
- **Tech Stack**: PyTorch, YOLO, VietOCR, OpenCV.

---

## Technical Skills

- **Agents & LLM Systems**: LangGraph, Multi-Agent Workflows, Tool-Calling, Hybrid RAG (pgvector, BM25), GraphRAG, Cohere Rerank.
- **Computer Vision & Deep Learning**: PyTorch, OpenCV, YOLOv8, MediaPipe, VietOCR, scikit-learn.
- **Backend & Infrastructure**: Python (FastAPI, Flask), PostgreSQL (pgvector), Docker, Docker Compose, Alembic, Linux.
- **Frontend**: React, TypeScript, Vite, TailwindCSS.

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Tuan-Nguyen-Minhh&show_icons=true&theme=radical&hide_border=true" alt="Tuan's GitHub stats" />
</p>
