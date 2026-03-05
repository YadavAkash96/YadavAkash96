# Akash Yadav - AI Engineer

I build GenAI systems that go beyond demos - RAG pipelines, multimodal applications, and LLM-integrated products that work under real-world constraints.

5 years of experience across production software engineering and applied AI research. Currently finishing my MSc in Artificial Intelligence at FAU Erlangen. My most recent work was inside the RnD division at Carl Zeiss AG, where I spent 9 months on uncertainty estimation in medical image segmentation - one of the few Master's students to work in a team of PhDs on a research problem that actually ships.

I am most interested in the intersection of **generative AI and high-stakes domains** - healthcare, industrial AI, and enterprise LLM products where getting it wrong has real consequences.

---

## Selected Projects

### 🫀 Uncertainty Estimation for Medical Image Segmentation
*Carl Zeiss AG RnD - Master's Thesis*

Segmentation models in medical imaging are dangerously overconfident. A model that says "90% sure" about a cardiac boundary it has never seen before is a liability in clinical settings.

I designed and implemented a VAE-based encoder-decoder to produce pixel-level uncertainty maps on echocardiography data. The system uses multivariate normal weighting and feature space projections to make uncertainty estimates spatially interpretable - showing not just *that* a model is uncertain, but *where* and *why*.

Built on PyTorch Lightning with Comet ML experiment tracking, nnUNet preprocessing, and cross-validation over the CAMUS cardiac ultrasound dataset.

`PyTorch Lightning` `VAE` `Uncertainty Estimation` `Medical Imaging` `nnUNet` `Comet ML`

---

### 🏋️ GymLens - Multimodal RAG Fitness Assistant
[→ Repo](https://github.com/YadavAkash96/XR_RAG_LLM)

A multimodal pipeline that takes a live camera feed and a voice question, identifies the gym equipment in frame, and retrieves the most relevant instructional video through a RAG system - designed as a proof-of-concept for XR deployment.

The interesting engineering is in the pipeline: TensorFlow.js object detection runs client-side to avoid streaming raw frames, a Whisper STT microservice transcribes the voice query, Phi-3 via Ollama extracts structured entities (equipment name, target muscle groups), hybrid search on Qdrant combines metadata filtering with semantic similarity over video transcripts. The whole chain runs over WebSockets with under 3 second latency end-to-end.

`FastAPI` `Qdrant` `RAG` `Whisper` `Ollama / Phi-3` `TensorFlow.js` `Multimodal` `WebSockets`

---

### ✍️ Writer Identification - ICDAR 2017
[→ Repo](https://github.com/YadavAkash96/WriterIdentification)

Unsupervised writer retrieval on historical handwritten documents. The challenge: learn a feature space where documents by the same writer cluster together, without labeled pairs at training time.

Combined NetRVLAD (originally designed for place recognition) with a discriminative DenseNet to learn writer-specific embeddings. Evaluated on the ICDAR 2017 historical handwriting benchmark.

`PyTorch` `DenseNet` `NetRVLAD` `Metric Learning` `Document AI`

---

### ⏱️ Explainability for Multi-Sensor Time Series
[→ Repo](https://github.com/YadavAkash96/XAI-Time-Series)

Industrial sensors produce streams of data. When a fault prediction fires, engineers need to know which sensor caused it - not just that something went wrong.

Built an attention-based LSTM (AT-LSTM) where attention weights directly indicate which sensors and timesteps drove each prediction. Compared attention-based explanations against SHAP to validate interpretability quality.

`PyTorch` `LSTM` `Attention` `XAI` `SHAP` `Industrial AI`

---

## Work History

| | |
|---|---|
| **Carl Zeiss AG** - ML Research Engineer | Erlangen, 2024–2025 |
| **WSAudiology** - AI Engineer (Working Student) | Erlangen, 2024 |
| **Weatherford International** - Software Analytics Engineer | Remote, 2022–2023 |
| **Amdocs / Tata Technologies** - Software Engineer | India, 2019–2022 |

**MSc Artificial Intelligence** - FAU Erlangen-Nürnberg *(ongoing)*

**BTech Information Technology** - BVP Pune

🏆 Hackathon Winner - TUM.ai x BKW Engineering Challenge

📄 Published - Attendance monitoring via computer vision, JETIR

---

## What I'm Looking For

**AI Engineer or ML Engineer roles in Germany** - full-time, hybrid or on-site in the DACH region.

I am most interested in teams building serious GenAI products or applying ML in medical, industrial, or enterprise contexts. I have a valid German work and residence permit and am available immediately.

The kind of work I want: RAG and LLM system design, multimodal pipelines, applied research that ships. Not pure software development. Not tutorial-level AI.

📧 yadavakash1996@outlook.com · [LinkedIn](https://www.linkedin.com/in/akash-yadav-721284141/)
