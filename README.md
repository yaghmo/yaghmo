# Yaghmoracen Belmir

AI engineer in Paris · LLM and RAG, computer vision, audio · PyTorch  
[Portfolio](https://yaghmoracen-belmir.vercel.app) · [LinkedIn](https://www.linkedin.com/in/belmir-yaghmoracen/) · [yaghmo.belmir@gmail.com](mailto:yaghmo.belmir@gmail.com)

I build AI systems end to end and measure them: a baseline, a fixed sample, and the failures read one by one. My background includes medical imaging research at LaTIM.

## Selected work

[kaggle-fast](https://github.com/yaghmo/kaggle-fast) (2026): a Claude Code skill that makes a Hugging Face model start fast on a free Kaggle GPU notebook. With SAM-Audio large on a T4, building the model, loading its weights and copying it to the GPU went from 96 s to 4 s, and the fast path gives the same model (1449 tensors compared, 0 differ).

RAG on financial reports, measured (2026): a document assistant tuned one change at a time on 150 FinanceBench questions, with every failure read. Writing the file name on every passage took the right report in the top 5 from 70.7% to 84.7%. The code is private for now.

[MRI-to-CT synthesis with GANs](https://github.com/yaghmo/mri-to-ct-synthesis-gan) (LaTIM, 2025): Pix2Pix variants that synthesize CT from MRI for radiotherapy dose planning. A structural loss (NGF) raised global SSIM from 0.7134 to 0.7315.

[Self-Representation AI](https://github.com/yaghmo/Self_representation_AI): a chatbot that answers a creator's audience as the creator. Every statement in its profile cites the creator's own words, and without a cite the bot says it does not know.

[Offline multimodal assistant](https://github.com/yaghmo/offline_multimodal_assistant): local LLMs and VLMs with document Q&A over PDF, DOCX, XLSX and PPTX, speech input through faster-whisper, and a streaming FastAPI backend. It runs in Docker with CUDA.

<details>
<summary>More projects</summary>

- [TrendHub](https://github.com/yaghmo/trendhub): GitHub Trending to a Telegram digest to a LinkedIn draft, on free tiers only
- [Lung segmentation benchmark](https://github.com/yaghmo/U_Net-DeepLabV3-FCNN-lung-segmentation): U-Net, DeepLabV3 and FCNN under the same training and evaluation
- [Detection and tracking with spatial relations](https://github.com/yaghmo/yolo-sort-spatial-relations): YOLOv8 and SORT, plus distance, direction and relative motion between objects
- [Multilingual sentiment analysis](https://github.com/yaghmo/sentiment_analysis): language detection, translation, classification and an LLM summary

</details>

## Stack

Python, TypeScript, C, C++ · PyTorch, TensorFlow, Hugging Face, MONAI, Scikit-Learn, OpenCV · llama.cpp, ChromaDB · FastAPI, Streamlit, Next.js, Docker, Cloudflare Workers, Linux
