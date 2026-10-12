# Yaghmoracen Belmir
AI Engineer | LLM and RAG, Computer Vision, Audio | PyTorch | I measure what I build

I build end-to-end AI systems across language, vision and audio, and I measure them: a baseline, a fixed sample, and the failures read one by one.  
My experience includes medical imaging research, applied deep learning, and building production-oriented AI applications.

---

## Selected Work

### kaggle-fast: 96 seconds of model loading down to 4 (2026)
A Claude Code skill that makes a Hugging Face model start fast on a free Kaggle GPU notebook.
- SAM-Audio large (6.9 GiB checkpoint, fp16) on a T4: build + load weights + copy to GPU from 96 s to 4 s, start to model on GPU from 158 s to 67 s, host RAM peak from 15.9 GiB to 8.5 GiB
- Each cause found with a probe on a free CPU notebook: random init of weights the checkpoint then overwrites, `torch.load` copying the whole file, a checkpoint read by one thread
- The fast path gives the same model: 1449 tensors compared, 0 differ

Repository: [kaggle-fast](https://github.com/yaghmo/kaggle-fast)  
Technologies: PyTorch, Kaggle, uv, Claude Code

---

### RAG on financial reports, measured (2026)
A document assistant tuned one change at a time on 150 questions over annual reports (FinanceBench), with every failure read.
- Writing the file name on every passage: right report in the top 5 from 70.7% to 84.7%, at no cost per question
- A bigger embedding model was worth 7 points alone, and 2 after two cheap fixes
- An LLM judge marked 93.85 wrong against 93.86: the grader gets checked too

Code is private for now; the findings go out as a LinkedIn series.  
Technologies: Python, FastAPI, llama.cpp, hybrid search, rerankers

---

### Self-Representation AI
A page for a content creator with a chatbot that answers the audience as the creator, grounded in a profile they write themselves.
- Every statement in the character profile carries a cite to the creator's own words; without one the bot says it does not know
- Audience chat is read-only (one `recall` tool); edits from the admin console need an explicit confirm
- LLM, embeddings and text-to-speech each run locally or through a hosted API, chosen per role after a hardware probe

Repository: [Self_representation_AI](https://github.com/yaghmo/Self_representation_AI)  
Technologies: FastAPI, Next.js, llama.cpp, Qwen TTS, Docker Compose

---

### MRI-to-CT Synthesis using GANs (LaTIM, 2025)
Generative model for synthesizing CT from MRI to support radiotherapy dose planning.  
- Developed preprocessing and paired dataset preparation pipeline  
- Trained and evaluated Pix2Pix variants with and without a structural loss (NGF)  
- NGF raised global SSIM from 0.7134 to 0.7315 (+2.5%) and Dice from 0.8826 to 0.8851  

Repository / Report: [mri-to-ct-synthesis-gan](https://github.com/yaghmo/mri-to-ct-synthesis-gan)   
Technologies: PyTorch, GANs, Medical Imaging

---

### Offline Multimodal Assistant
A local AI assistant supporting multiple LLMs and VLMs with document Q&A, voice input, and multimodal chat.
- Built a RAG pipeline with ChromaDB and multilingual embeddings for document retrieval over PDF, DOCX, XLSX, PPTX and more
- Integrated local speech-to-text transcription via faster-whisper with automatic language detection
- Designed a FastAPI backend with streaming inference, parallel model loading, and automatic context summarization
- Containerized with Docker and CUDA support for GPU inference
  
Repository: [offline_multimodal_assistant](https://github.com/yaghmo/offline_multimodal_assistant)  
Technologies: Python, FastAPI, Streamlit, Transformers, ChromaDB, Docker

---

### TrendHub
GitHub Trending to a Telegram digest to a LinkedIn draft, on free tiers only.
- Cloudflare Worker on a cron: top trending repos with an overview and two buttons, Draft Post or Skip
- Gemini reads the README and writes the draft; repos already seen are kept in KV and left out of later digests

Repository: [trendhub](https://github.com/yaghmo/trendhub)  
Technologies: TypeScript, Cloudflare Workers, Telegram Bot API, Gemini

---

### Medical Image Segmentation Benchmark
Comparative study of segmentation architectures for lung region extraction.  
- U-Net, DeepLabV3, and FCNN under identical training and evaluation settings  
- Evaluation using Dice, IoU, and boundary metrics  

Repository: [U_Net-DeepLabV3-FCNN-lung-segmentation](https://github.com/yaghmo/U_Net-DeepLabV3-FCNN-lung-segmentation)  
Technologies: PyTorch, Computer Vision

---

### Object Detection and Tracking with Spatial Relation Modeling
Real-time pipeline combining YOLOv8 detection with SORT tracking.  
- Extraction of spatial interaction descriptors (distance, direction, relative motion)  
- Framework supports downstream tasks such as scene understanding or activity prediction  

Repository: [yolo-sort-spatial-relations](https://github.com/yaghmo/yolo-sort-spatial-relations)  
Technologies: YOLOv8, SORT, NumPy, OpenCV

---

### Multilingual Sentiment Analysis System
End-to-end sentiment analysis workflow integrating language identification, translation, classification, and LLM-based summarization.

Repository: [sentiment_analysis](https://github.com/yaghmo/sentiment_analysis)  
Technologies: Python, Transformers, NLP

---

## Research Interests
- Large Language Models, retrieval, and how to evaluate them  
- Computer Vision and Image Understanding  
- Medical Imaging and Scientific Computing  
- Audio: speech, source separation  
- Generative Modeling (GANs, diffusion models)  
- Multimodal AI systems  

---

## Technical Competencies

**Machine Learning:**  
Deep Learning, Computer Vision, NLP, Audio, Generative Models, LLMs, RAG and Evaluation, Representation Learning

**Frameworks:**  
PyTorch, TensorFlow, Hugging Face, MONAI, Scikit-Learn, OpenCV, llama.cpp, ChromaDB

**Systems & Tools:**  
Docker, Git, Linux, FastAPI, Streamlit, Next.js, Cloudflare Workers

**Programming:**  
Python, TypeScript, C, C++

---

## Contact  
<a href="https://www.linkedin.com/in/belmir-yaghmoracen/" target="_blank">
  <img width="52" height="52" alt="linkedin"
       src="https://github.com/user-attachments/assets/8dd53c10-9989-445c-9e8e-4083889a3ea0" />
</a>
<br>

<a href="mailto:yaghmo.belmir@gmail.com" target="_blank">
<img width="52" height="52" alt="yaghmo.belmir@gmail.com" src="https://github.com/user-attachments/assets/506691cf-f436-4012-98e8-d0c3c0e79095" />
</a><br>(yaghmo.belmir@gmail.com)
