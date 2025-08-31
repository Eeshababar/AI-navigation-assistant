# 🦾 AI Navigation Assistant

An **AI-powered mobility assistant** for visually impaired individuals.  
It combines **computer vision**, **generative AI reasoning**, and **agentic workflows** to detect obstacles, estimate distances, generate adaptive guidance, and alert caregivers when necessary.  

---

## 🚀 Features
- 🔍 **Obstacle Detection** – YOLOv12 for robust real-time object recognition  
- 📏 **Distance Estimation** – MiDaS for monocular depth sensing  
- 🤖 **Contextual Reasoning** – GPT-5 for adaptive navigation and situational awareness  
- 🎥 **Video Inference** – Roboflow integration for live object/video stream processing  
- 🗣 **Voice Feedback** – gTTS for natural audio navigation cues  
- 📧 **Caregiver Alerts** – Automated email notifications via **LangGraph agentic workflows**  
- 🧭 **Adaptive Navigation** – Agents plan responses (alert, reroute, stop, proceed)  

---

## 🖼️ System Architecture
```mermaid
graph TD
    A[Camera Input] --> B[YOLOv12 - Obstacle Detection]
    B --> C[MiDaS - Depth Estimation]
    C --> D[GPT-5 - Inference & Decisions]
    D --> E[gTTS - Voice Output]
    D --> F[Roboflow - Video Inference]
    D --> G[LangGraph Agent - Caregiver Email Alerts]
