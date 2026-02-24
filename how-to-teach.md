# DGX Spark Orientation — Tutor Overview

---

## 1 — Purpose

- Teach clean, reproducible GPU workflows
- Protect DGX OS stability
- Build container-first literacy
- Align with NVIDIA ecosystem

---

## 2 — Core Rule

- No sudo
- No apt install
- No base OS modification
- Everything containerized

---

## 3 — What DGX Spark Is

- Grace Blackwell architecture
- 128GB unified memory
- CUDA 13 preinstalled
- Docker + NVIDIA Container Runtime configured
- Production-adjacent AI workstation

---

## 4 — Access Methods

- NVIDIA Sync (recommended)
- SSH
- DGX Dashboard
- Hybrid workflows supported

Laptop → Sync/SSH → Spark

---

## 5 — Learning Mental Model

DGX OS
↓
Docker Runtime
↓
NGC Containers
↓
ML Workload

Students are learning:

- Containerized GPU systems
- CUDA-compatible frameworks
- Scalable AI infrastructure

---

## 6 — Orientation Phase

- Overview NVIDIA ecosystem
- Where Spark fits
- Show NVIDIA stack diagram
- Explain container runtime
- Basic Docker literacy

---

## 7 — Playbook Phase

- Select official playbook
- Load playbook in browser
- Load user manual
- Open DGX Dashboard
- Reproduce exactly
- Monitor GPU + memory

---

## 8 — Monitoring Discipline

Always visible:

- GPU utilization
- System memory
- Load behavior

Explain unified memory (UMA).

---

## 9 — SSH Tunnel Warning

If using remote UI:

Must tunnel ports:

ssh -L 3000:localhost:3000 -L 8000:localhost:8000 username@spark-xxxx.local

Without tunneling:

- UI/backend mismatch
- Silent failure
- Debug confusion

---

## 10 — Escalation Policy

1. Ask Gemini (manual open)
2. Ask infra tech (system issues only)

Never solve system issues with apt/sudo.

---

## 11 — Outcome

Students leave understanding:

- GPU containers
- AI infrastructure patterns
- Production-aligned workflows
- Enterprise-ready compute habits
