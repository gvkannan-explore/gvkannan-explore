# Vignesh Kannan

**ML Engineer · FDA-cleared medical imaging · LLM agents & inference**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-VigneshKannan-blue)](https://www.linkedin.com/in/vignesh-kannang/)
[![Email](https://img.shields.io/badge/Email-gvkannan.work%40gmail.com-red)](mailto:gvkannan.work@gmail.com)
[![Website](https://img.shields.io/badge/Website-gvkannan--explore.github.io-black)](https://gvkannan-explore.github.io)

## About me

ML Engineer at SimBioSys with 4+ years of experience taking deep learning models for medical imaging from prototype to four FDA 510(k) clearances, under FDA and HIPAA requirements. I also build LLM pipelines and agents for clinical documents and research.

### Areas of expertise
- **Deep learning:** PyTorch, TensorFlow, MONAI, Hugging Face Transformers
- **LLMs and agents:** LangGraph, LangChain, vLLM, LangSmith, Pydantic
- **Medical imaging:** DICOM, NIfTI, 3D Slicer
- **Cloud and MLOps:** AWS (S3, EC2, ECR, Batch), Docker, MLflow, W&B
- **Data science:** Python, SQL, Pandas, Scikit-Learn
- **Methods:** Segmentation, classification, clustering, survival analysis, retrieval

## Work at SimBioSys

1. **Breast DCE-MRI segmentation (FDA-cleared: K231130, K243189, K251766)**
   - Led the design, development and deployment of 3D multi-label segmentation models for breast DCE-MRI and cut the false-negative rate from ~45% to under 10%.
   - Cut per-case inference time from 20 to ~3 minutes with bfloat16, TorchScript and GPU selection.
   - Built an evaluation pipeline that scores each major model iteration on ~26 metrics and gates every release tag on pytest performance tests and expert review in staging.
   - Built a Git-versioned AWS pipeline (S3, ECR, EC2) for multi-GPU training that cut development and deploy cycles from 2 weeks to 2 days.
   - [View Project](https://simbiosys.com/tumorsight-viz/)

2. **Recurrence risk model (FDA-cleared: K260023)**
   - Co-led an FDA-cleared multimodal survival model that combines structured clinical data with MRI imaging features to predict 5-year recurrence risk.

3. **Clinical document extraction with small LLMs**
   - Cut manual curation by 40% with a HIPAA-compliant pipeline (OCR and small LLMs), deployed internally on ~3,000 pathology reports, that returns source-cited Pydantic outputs and sends low-confidence cases to human review.

## Selected publications
- **Seeing beyond cancer: multi-institutional validation of object localization and 3D semantic segmentation using deep learning for breast MRI.** SPIE Medical Imaging, 2024. [SPIE](https://journals.spiedigitallibrary.org/conference-proceedings-of-spie/12927/129270H/Seeing-beyond-cancer--multi-institutional-validation-of-object-localization/10.1117/12.3009341.short) · [arXiv](https://arxiv.org/abs/2311.16213)
- **Performance of an AI-powered visualization software platform for precision surgery in breast cancer patients.** npj Breast Cancer, 2024. [npj](https://doi.org/10.1038/s41523-024-00696-6) · [ASCO abstract](https://ascopubs.org/doi/10.1200/JCO.2024.42.16_suppl.e12618)
- **A 3D visualization method for breast cancer surgeons and patients.** AACR. [Link](https://aacrjournals.org/cancerres/article/83/5_Supplement/P4-02-29/717901/Abstract-P4-02-29-A-3D-Visualization-Method-for)

## Personal projects

1. **MedScout: clinical trial triage agent** *(in progress)*
   - Building a LangGraph agent that monitors and triages clinical trials through the ClinicalTrials.gov API.
   - Evaluating it against a small set of patient profiles, with tracing in LangSmith.

2. **PubMed RAG** *(in progress)*
   - Building a RAG system over breast cancer PubMed abstracts that cites the PMIDs it retrieves and flags unsupported claims with a deterministic validator.
   - Its eval harness scores retrieval quality, citation faithfulness and how well an LLM judge agrees with human labels.
   - [View Project](https://github.com/gvkannan-explore/rag-project)

3. **MultiLabel_N24: fine-tuning vs zero-shot LLMs**
   - Fine-tuned RoBERTa and ModernBERT on N24News and benchmarked them against zero-shot LLMs served through vLLM.
   - The fine-tuned models beat the zero-shot LLMs on 8 out-of-distribution news articles from 2025-2026.
   - [View Project](https://github.com/gvkannan-explore/MultiLabel_N24)

### Earlier projects

1. **COVID detection and severity assessment**
   - Created a pipeline using DenseNet variants for detecting COVID-19 and assessing severity from CXR images.
   - Made the models less sensitive to adversarial examples and data noise.
   - [View Project](https://github.com/gvigkannan/COVID_CXR)

2. **Ensemble-based grasp detection using neural networks**
   - Compared ensembling techniques for deep-learning robot grasping algorithms.
   - [View Project](https://github.com/gvigkannan/Stacking_Cornell/tree/main)

3. **Benchmarking 3D segmentation competitions in under $50** *(paused)*
   - An nnU-Net-style segmentation pipeline for testing off-the-shelf models with little manual intervention.
   - The goal is an end-to-end pipeline that delivers a dockerized best model with a model card.
   - [View Project](https://github.com/gvkannan-explore/AbdomenCT_Seg)

## Writing

*Coming soon. I have 10 drafts going. If I don't publish one before the end of 2026, I owe you a cup of coffee.*

---

Open to collaborating on AI and healthcare projects. Reach out on [LinkedIn](https://www.linkedin.com/in/vignesh-kannang/).
