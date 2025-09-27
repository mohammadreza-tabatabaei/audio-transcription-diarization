# 🎙️ Speaker Diarization Pipeline

## 📌 Overview
This project implements an **end-to-end pipeline** for multi-speaker transcription and diarization.  
It processes noisy audio, transcribes it with **Whisper (OpenAI)**, separates speakers using **Pyannote.audio**, and outputs structured results with **visualizations** and an **interactive Gradio demo**.

---

## 🚀 Features
- **Preprocessing**: Resampling (16kHz), mono conversion, denoising, normalization.  
- **ASR with Whisper**: Word-level timestamps + confidence scores.  
- **Speaker Diarization**: Separation of multiple speakers (unsupervised clustering).  
- **Alignment**: Words mapped to speaker segments.  
- **Exports**: CSV + JSONL outputs.  
- **Visualizations**: Speaking time, speaker turns, confidence distributions.  
- **Interactive Demo**: Upload your own audio via **Gradio**.  

## 📂 Project Structure
├── final_pipeline.ipynb # Full Jupyter Notebook pipeline
├── final_output.csv # Transcript with speaker labels
├── final_output.jsonl # Same transcript in JSONL format
├── Speaker_Diarization_Project_Report.pdf
├── Cover_Letter_Mohammadreza_Tabatabaei.pdf
├── charts/ # Visualization images
└── README.md

---

## ⚙️ Requirements
Main dependencies:
- Python 3.10+
- `torch==2.2.0`, `torchaudio==2.2.0`, `torchvision==0.17.0`
- `openai-whisper`
- `pyannote.audio==3.1`
- `librosa`, `matplotlib`, `pandas`, `seaborn`
- `gradio`

Install all dependencies:
```bash
pip install -r requirements.txt
---

## ⚙️ Results

**Test file:** 4:45 minutes audio with 3 speakers (two male + one female).

**Outputs:**
- Accurate transcription
- Clear speaker separation (**silhouette score ≈ 0.85**)
- Word-level confidence scores

### Example Visualizations
- Speaker Timeline  
- Speaking Time per Speaker  
- Speech Proportion  

---

## 🌍 Applications
- Meeting transcription  
- Call center analytics  
- Sports commentary & media production  

---

## ✨ Author
**Mohammadreza Tabatabaei**  


