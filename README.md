# 🚦 TrafficVerse AI
### Automated Photo Identification and Classification for Traffic Violations Using Computer Vision

> **Gridlock Hackathon 2.0** · AI-Powered Smart Traffic Management Platform

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Vercel-black?style=for-the-badge&logo=vercel)](http://traffic-verse-ai.vercel.app/)
[![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)](https://github.com/sunita330/TrafficVerse-AI/)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](LICENSE)

---

## Overview

TrafficVerse AI is a futuristic, AI-powered Smart Traffic Management platform that uses Computer Vision to automatically detect and classify traffic violations from surveillance images and videos. The platform presents a complete end-to-end workflow through an immersive, cinematic web interface — from live camera feed ingestion to violation classification, license plate recognition, AI-generated evidence, and intelligent enforcement recommendations.

The current submission is a **fully functional frontend prototype** that demonstrates the complete system workflow, UI/UX, and AI simulation pipeline. The accompanying architecture diagram represents the planned production deployment incorporating real-time YOLO inference, ByteTrack vehicle tracking, and PaddleOCR number plate recognition.

---

## Features

| Feature | Status |
|---|---|
| 🌆 3D Digital Twin Dashboard | ✅ Live |
| 🎯 AI Violation Detection Simulation | ✅ Live |
| 🗺️ Animated Violation Heatmap | ✅ Live |
| 📊 Traffic Analytics Dashboard | ✅ Live |
| ⚡ Risk Engine & Zone Scoring | ✅ Live |
| 🤖 AI Copilot (NLP Interface) | ✅ Live |
| 👮 Officer Command Panel | ✅ Live |
| 🎬 Violation Replay Engine | ✅ Live |
| 📄 Evidence Generation UI | ✅ Live |
| 🌟 Citizen Reporting Module | ✅ Live |
| 🔢 License Plate OCR Simulation | ✅ Live |
| ⏱️ Timeline Replay Slider | ✅ Live |

---

## Violation Types Detected

- ⛑️ Helmet Violation
- 🛵 Triple Riding
- 🚦 Red Light Violation
- ↩️ Wrong-Side Driving
- 🅿️ Illegal Parking
- 🚗 Seatbelt Violation
- ⛔ Stop Line Violation

---

## Tech Stack
Frontend    →  HTML5 · CSS3 · Vanilla JavaScript
Rendering   →  Canvas API (2D)
Charts      →  Chart.js
Deployment  →  Vercel · GitHub Pages
Version     →  Git · GitHub

---

## Proposed Production Architecture
CCTV Cameras / Video Upload
↓
YOLOv11x Object Detection  (GPU · 2.1ms latency)
↓
ByteTrack Vehicle Tracking  (Multi-object persistent IDs)
↓
Violation Rule Engine       (8 violation classifiers)
↓
PaddleOCR Plate Recognition (96.2% accuracy)
↓
FastAPI Backend             (REST + WebSocket)
↓
PostgreSQL + Redis          (Persistence + Real-time cache)
↓
Evidence PDF Generator      (QR-signed, court-admissible)
↓
Dashboard / Officer App     (This prototype)


---

## Getting Started

```bash
# Clone the repository
git clone https://github.com/trafficverse-ai/trafficverse.git
cd trafficverse

# No installation required — open directly in browser
open trafficverse_v2.html

# Or serve locally
npx serve . -p 3000
open http://localhost:3000/trafficverse_v2.html
```

---

## Project Structure

trafficverse/
├── trafficverse_v2.html          # Main platform (start here)
├── trafficverse_replay.html      # Violation Replay Engine
├── trafficverse_pitch.html       # Pitch Deck (9 slides)
├── trafficverse_architecture.html # System Architecture Diagram
├── trafficverse_setup.html       # Setup & API Reference Guide
├── trafficverse_judging_guide.html # Demo & Presentation Guide
└── README.md                     # This file


---

## Architecture Note

The current prototype demonstrates the complete end-to-end workflow through a simulation-driven frontend. The system architecture diagram included in the project represents the planned production deployment, which will incorporate:

- **YOLOv11x** GPU inference for real-time object detection
- **ByteTrack** for persistent multi-object tracking across frames
- **PaddleOCR** for Indian license plate character recognition
- **FastAPI** async backend with WebSocket real-time streaming
- **PostgreSQL + PostGIS** for spatial violation storage
- **Redis** for sub-millisecond pub/sub and caching
- **Docker** containerised GPU deployment on cloud GPU instances

This architecture has been designed for national-scale deployment supporting 10,000+ cameras across 100+ Indian cities.

---

## Team

Built for Gridlock Hackathon 2.0 · Making Indian roads safer, one detection at a time.

---

## License

MIT License · © 2024 TrafficVerse AI
