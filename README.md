# Akash Yadav, AI Engineer

I build GenAI systems that go beyond demos. RAG pipelines, multimodal applications, and LLM-integrated products that work under real-world constraints.

5 years of experience across production software engineering and applied AI research. Currently finishing my MSc in Artificial Intelligence at FAU Erlangen. My most recent work was inside the RnD division at Carl Zeiss AG, where I spent 9 months on uncertainty estimation in industrial image segmentation as one of the few Master's students embedded in a team of PhDs working on a problem that reaches production.

I am most interested in the intersection of **generative AI and high-stakes domains**: healthcare, industrial AI, and enterprise LLM products where getting it wrong has real consequences.

---

## Selected Projects

### 🔬 Bayesian Uncertainty Estimation for Industrial Microscopy Segmentation
*Carl Zeiss AG RnD, Master's Thesis (unpublished, paper in progress)*

In high-throughput industrial microscopy, a segmentation model that confidently misclassifies is worse than one that admits it does not know. The goal of this work was to make uncertainty a first-class output, not an afterthought.

I designed a hybrid Bayesian-deterministic segmentation architecture combining a multi-depth U-Net with contrastive learning and attention-based Bayesian uncertainty estimation. The model produces a unified image-level uncertainty score to separate in-distribution from out-of-distribution samples, enabling reliable decisions at production scale.

Results on 12k high-dimensional microscopic images: Dice 96%, IoU 94%, OOD detection accuracy 95%, false-positive segmentations reduced by 90%. Deployed as an Azure-hosted inference pipeline with live model drift monitoring via W&B.

Work is under NDA. A reproducible public version using open microscopy datasets is in progress.

`PyTorch` `Bayesian Deep Learning` `U-Net` `Contrastive Learning` `Uncertainty Estimation` `Azure` `W&B` `Industrial AI`

---

### 🏋️ GymLens, Multimodal RAG Fitness Assistant
[View Repo](https://github.com/YadavAkash96/XR_RAG_LLM)

A multimodal pipeline that takes a live camera feed and a voice question, identifies the gym equipment in frame, and retrieves the most relevant instructional video through a RAG system. Designed as a proof-of-concept for XR deployment.

TensorFlow.js object detection runs client-side to avoid streaming raw camera frames to the server. A Whisper STT microservice transcribes the voice query. Phi-3 via Ollama extracts structured entities including equipment name and target muscle groups. Hybrid search on Qdrant then combines metadata filtering with semantic similarity over video transcripts. The full chain runs over WebSockets with under 3 seconds latency end-to-end.

`FastAPI` `Qdrant` `RAG` `Whisper` `Ollama / Phi-3` `TensorFlow.js` `Multimodal` `WebSockets`

---

### 🛒 EasyBuy, Agentic Shopping Assistant
[View Repo](https://github.com/YadavAkash96/easybuy-agent)

Tell EasyBuy what you need. It figures out everything else.

Say "I need a skiing kit under 400 EUR" and a multi-agent pipeline decomposes that into every item the kit requires, searches real listings across multiple retail platforms, ranks by price, reviews, and delivery speed, assembles the cart, and delivers a PDF invoice to your inbox. No search bars, no tab switching, no manual filtering.

Five specialized agents each own one stage: intent gathering, kit breakdown with budget allocation, multi-platform product search, transparent ranking with user-controlled filters, and cart assembly with email invoice delivery. Each agent is a dedicated FastAPI endpoint with its own prompt design and structured output schema.

Built in 48 hours at the 4th Hack-Nation Global AI Hackathon, February 2026, VC Track.

`FastAPI` `Google Gemini 2.0` `Agents` `SerpAPI` `Next.js` `Docker` `Agentic AI`

---

### ⏱️ Explainability for Multi-Sensor Time Series
[View Repo](https://github.com/YadavAkash96/XAI-Time-Series)

Industrial sensors produce streams of data. When a fault prediction fires, engineers need to know which sensor actually caused it, not just that something went wrong.

Built an attention-based LSTM where attention weights directly indicate which sensors and timesteps drove each prediction. Compared attention-based explanations against SHAP to validate interpretability quality.

`PyTorch` `LSTM` `Attention` `XAI` `SHAP` `Industrial AI`

---

## Work History

| | |
|---|---|
| **Carl Zeiss AG**, ML Research Engineer | Erlangen, 2024 to 2025 |
| **WSAudiology**, AI Engineer (Working Student) | Erlangen, 2024 |
| **Weatherford International**, Software Analytics Engineer | Remote, 2022 to 2023 |
| **Amdocs / Tata Technologies**, Software Engineer | India, 2019 to 2022 |

**MSc Artificial Intelligence**, FAU Erlangen-Nürnberg *(ongoing)*

**BTech Information Technology**, BVP Pune

🏆 Hackathon Winner, TUM.ai x BKW Engineering Challenge

📄 Published, Attendance monitoring via computer vision, JETIR

---

## What I am Looking For

**AI Engineer or ML Engineer roles in Germany**, full-time, hybrid or on-site in the DACH region.

I am most interested in teams building serious GenAI products or applying ML in medical, industrial, or enterprise contexts. I have a valid German work and residence permit and am available immediately.

The kind of work I want: RAG and LLM system design, multimodal pipelines, applied research that ships. Not pure software development. Not tutorial-level AI.

📧 yadavakash1996@outlook.com · [LinkedIn](https://www.linkedin.com/in/akash-yadav-721284141/)
