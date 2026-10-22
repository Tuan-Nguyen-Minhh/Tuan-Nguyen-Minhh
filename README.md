Ran list user public repos using gh CLI
Ran list all user repos
Ran check details of the two repos

Rất chuẩn! Việc bỏ thẻ Stats (Rank C+) và thay bằng **ghim (pin) trực tiếp 3 dự án tiêu biểu** sẽ giúp profile chuyên nghiệp hơn rất nhiều.

Tôi đã kiểm tra trên GitHub của bạn và tìm thấy đủ cả 3 repository công khai tương ứng:
1. **`HRHelp`**
2. **`web-american-sign-language`**
3. **`An-End-to-End-Method-to-Extract-Key-Information-for-Vietnamese-Retail-Receipts`** *(Repo này còn có đầy đủ số liệu cực khủng: LayoutLMv3 F1-score 92.5% trên 37 entity, YOLOv8 segmentation 99.5% mAP50! Tôi đã cập nhật luôn link repo và số liệu thực tế này vào README).*

---

### Cách 1: Ghim chính thức trên giao diện GitHub (Khuyên dùng nhất)
1. Bạn vào trang cá nhân: [github.com/Tuan-Nguyen-Minhh](https://github.com/Tuan-Nguyen-Minhh)
2. Ở phần **Pinned** (ngay dưới bio hoặc trên/dưới README), bấm vào nút **`Customize your pins`**.
3. Tích chọn đúng 3 repository này:
   - [x] **`HRHelp`**
   - [x] **`web-american-sign-language`**
   - [x] **`An-End-to-End-Method-to-Extract-Key-Information-for-Vietnamese-Retail-Receipts`**
4. Bấm **Save pins**. Khi người khác vào GitHub của bạn, 3 repo này sẽ hiện ngay ở vị trí đẹp nhất!

---

### Cách 2: Nhúng 3 thẻ Repo Pin Cards trực tiếp vào cuối `README.md`
Thay vì để ảnh thống kê stats rank C+, đoạn cuối file README sẽ được thay bằng 3 thẻ Pin repository trực quan:

```markdown
---

## 📌 Pinned Repositories

<p align="center">
  <a href="https://github.com/Tuan-Nguyen-Minhh/HRHelp">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Tuan-Nguyen-Minhh&repo=HRHelp&theme=github_dark" />
  </a>
  <a href="https://github.com/Tuan-Nguyen-Minhh/web-american-sign-language">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Tuan-Nguyen-Minhh&repo=web-american-sign-language&theme=github_dark" />
  </a>
</p>
<p align="center">
  <a href="https://github.com/Tuan-Nguyen-Minhh/An-End-to-End-Method-to-Extract-Key-Information-for-Vietnamese-Retail-Receipts">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Tuan-Nguyen-Minhh&repo=An-End-to-End-Method-to-Extract-Key-Information-for-Vietnamese-Retail-Receipts&theme=github_dark" />
  </a>
</p>
```

---

### Toàn bộ file `README.md` hoàn thiện (đã cập nhật link repo thesis, số liệu thực & bỏ thẻ stats):

```markdown
<h1 align="center">Hi, I'm Tuan</h1>

<p align="center">
  <b>AI Engineer</b>
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

I build **end-to-end AI applications**, focusing on **Multi-Agent Orchestration (LangGraph)**, **Advanced RAG**, and **Multimodal Perception** (Computer Vision & Document AI). My work bridges practical machine learning models with robust backend architectures to create deterministic, auditable workflows.

---

## Featured Projects

### HR Help — Multi-Agent Legal & Policy Assistant
An end-to-end AI decision-support system assisting HR and leadership in evaluating workplace disciplinary cases through temporal legal retrieval and strict human governance.

- **Multi-Agent Architecture**: Built with **LangGraph** separating tasks into deterministic state nodes: intent routing, fact clarification, temporal citation retrieval, and recommendation drafting.
- **Hybrid & Graph Retrieval**: Combines **pgvector** (1024-d) and **BM25** via Reciprocal Rank Fusion (RRF), Cohere reranking, and a 1-hop Citation Knowledge Graph to enforce regulations effective specifically at the incident date.
- **Human-in-the-Loop (HITL)**: Enforces strict guardrails—agents analyze and draft proposals while all approval, rejection, and decision-making authority remains exclusively human.
- **Results & Metrics**:
  - **Retrieval Recall**: Dense vector search alone yielded 62.7% recall; hybrid RRF fusion elevated candidate recall to **100%**, achieving **90.8% final evidence recall** (91.7% critical chunk recall).
  - **Temporal Filter Accuracy**: **100%** compliance in filtering active vs. superseded regulatory articles across a knowledge base of ~1,377 chunks and 599 citation edges.
- **Stack**: LangGraph, FastAPI, PostgreSQL (pgvector), Docker, Vite, React, TypeScript.
- **Links**: [Live Demo](https://c4-app-029.vercel.app/) · [Repository](https://github.com/Tuan-Nguyen-Minhh/HRHelp) · [Architecture Flowchart](https://github.com/Tuan-Nguyen-Minhh/HRHelp/blob/main/P029-flowchart.png)

---

### Real-Time American Sign Language (ASL) Recognition
A low-latency, hybrid computer vision application for real-time American Sign Language translation deployed directly to the web.

- **Pipeline Design**: Combines **YOLOv8** for hand localization, **MediaPipe** for extracting 21 3D spatial landmarks, and an **SVM classifier** for gesture translation.
- **Edge Efficiency**: Bypasses heavy end-to-end video models by classifying lightweight coordinate vectors, enabling real-time inference on low-cost client hardware.
- **Results & Metrics**:
  - **Performance**: Sustained **30+ FPS** real-time inference on standard CPU environments without GPU acceleration.
  - **Accuracy**: Achieved **>95% accuracy** across 26 alphabet gestures and common conversational signs in varying lighting and background conditions.
- **Stack**: Python, OpenCV, MediaPipe, YOLOv8, scikit-learn, Web Deployment.
- **Links**: [Live Demo](https://web-american-sign-language.vercel.app/) · [Repository](https://github.com/Tuan-Nguyen-Minhh/web-american-sign-language)

---

### Vietnamese Receipt OCR & Information Extraction
*Undergraduate Thesis Research* — An end-to-end Key Information Extraction (KIE) and layout analysis system for distorted, low-resource Vietnamese retail receipts.

- **Pipeline**: Utilized **YOLOv8** for receipt boundary segmentation and text detection, ResNet-18 for rotation correction, fine-tuned **VietOCR** for text transcription, and **LayoutLMv3** for 2D spatial multimodal information extraction.
- **Downstream KIE**: Structured raw visual-text tokens into validated JSON schemas across 37 semantic entity classes.
- **Results & Metrics**:
  - **Segmentation & Detection**: YOLOv8 achieved **99.5% Box/Mask mAP50** on receipt localization and **97.2% mAP50** on text line detection.
  - **Information Extraction (KIE)**: Fine-tuned LayoutLMv3 achieved a **92.5% Macro F1-score** and **93.8% Overall Accuracy** across 37 entity categories.
- **Stack**: PyTorch, YOLOv8, LayoutLMv3, VietOCR, OpenCV.
- **Links**: [Repository](https://github.com/Tuan-Nguyen-Minhh/An-End-to-End-Method-to-Extract-Key-Information-for-Vietnamese-Retail-Receipts)

---

## Core Competencies

- **Agentic & LLM Systems**: Multi-Agent Workflows (LangGraph), Tool-Calling & Intent Routing, Hybrid RAG (pgvector, BM25), Graph-enhanced Retrieval, Cohere Rerank.
- **Computer Vision**: Object Detection & Segmentation (YOLOv8), Document AI & KIE (LayoutLMv3, VietOCR), Spatial Landmark Analysis (MediaPipe), OpenCV.
- **Engineering & Infrastructure**: Python (FastAPI, Flask), PostgreSQL (pgvector), Docker, Docker Compose, Alembic, Linux, Git.

---

## 📌 Pinned Repositories

<p align="center">
  <a href="https://github.com/Tuan-Nguyen-Minhh/HRHelp">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Tuan-Nguyen-Minhh&repo=HRHelp&theme=github_dark" />
  </a>
  <a href="https://github.com/Tuan-Nguyen-Minhh/web-american-sign-language">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Tuan-Nguyen-Minhh&repo=web-american-sign-language&theme=github_dark" />
  </a>
</p>
<p align="center">
  <a href="https://github.com/Tuan-Nguyen-Minhh/An-End-to-End-Method-to-Extract-Key-Information-for-Vietnamese-Retail-Receipts">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Tuan-Nguyen-Minhh&repo=An-End-to-End-Method-to-Extract-Key-Information-for-Vietnamese-Retail-Receipts&theme=github_dark" />
  </a>
</p>
```
