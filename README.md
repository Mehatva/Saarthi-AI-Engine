# Saarthi AI Edge Engine 🚑

An intelligent, full-stack emergency response and medical triage application designed to operate in high-stress, low-connectivity environments. This system combines a cross-platform **Flutter** mobile interface with an ultra-lightweight **Edge AI Python backend** for sub-millisecond triage decision-making.

---

## 🚀 System Architecture

This repository is split into two primary components, ensuring strict separation of concerns between the user interface and the machine learning inference engine.

### 1. The Mobile Frontend (`/saarthi_flutter`)
*Built with Flutter & Dart*
- **Cross-Platform Delivery:** Compiles to both iOS and Android natively.
- **Real-Time Telemetry:** Captures vital inputs (heart rate, stress indicators, symptoms) and transmits them to the edge server via RESTful APIs.
- **Intuitive UI/UX:** Designed specifically for high-stress emergency scenarios, ensuring users can navigate the triage workflow with minimal cognitive load.

### 2. The Edge Inference Engine (`/saarthi-ai`)
*Built with Python, FastAPI, NumPy*
- **Lightweight Classification:** Replaced bulky machine learning frameworks with pure NumPy arrays and deterministic state machines, achieving `<0.1 ms` latency.
- **Medical State Machine:** A deterministic routing algorithm that analyzes the user's symptoms and physiological markers to route them through precise medical subtypes (e.g., Trauma, Cardiac, Respiratory).
- **Edge-Optimized:** Designed to run locally on constrained edge devices or embedded hardware (e.g., Raspberry Pi) without requiring a cloud connection for inference.

---

## 🛠️ Tech Stack
- **Frontend App:** Flutter, Dart
- **Backend Service:** Python, FastAPI, Uvicorn
- **AI/ML Engine:** Custom NumPy classifiers, Deterministic State Machines
- **Architecture Pattern:** Edge Computing, RESTful Microservices

---

## 📈 Impact & Vision
In critical medical situations, cloud latency and dead-zones can cost lives. By pushing the machine learning inference directly to the edge, the Saarthi Engine guarantees immediate triage recommendations regardless of network conditions.
