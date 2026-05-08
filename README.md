# SUKH AI Wellness Platform — v3 Refactor
# 🌿 SUKH AI Wellness Platform

> AI Knowledge Operating System for Thai Wellness  
> Local-first · RAG · MCP · Vector Search · Data Platform

---

# 🚀 OVERVIEW

SUKH (สุข) คือระบบ AI ที่:
- ingest ความรู้จากไฟล์ (PDF / DOCX / CSV / Image)
- แปลงเป็น vector knowledge
- ใช้ RAG + MCP เพื่อให้คำตอบจากข้อมูลจริง

---

# 🎯 SYSTEM GOAL

- สร้าง AI Wellness Advisor
- ใช้ข้อมูลสมุนไพรไทย + งานวิจัย
- ขยายเป็น AI Platform

---

# 🧩 SYSTEM ARCHITECTURE

Frontend (React)
   ↓
Backend (FastAPI)
   ↓
-----------------------------------
| SQL DB | Vector DB | File Storage |
-----------------------------------
   ↓
RAG Pipeline + MCP
   ↓
AI Response

---

# 🧠 AI FLOW

User Query
 → Embed
 → Vector Search (FAISS)
 → Context Retrieval
 → MCP Tool
 → AI Response

---

# 📂 DATA ARCHITECTURE

## Data Sources
- Admin: PDF, DOCX, CSV, JSON, Images
- User: Queries, Logs

## Pipeline
Upload → Parse → Clean → Chunk → Embed → Store

---

# 🗄️ STORAGE

## SQL
users, herbs, knowledge, uploads, logs

## Vector DB
- embeddings (1536 dim)
- text chunk
- metadata

## File Storage
/uploads/

---

# 🔄 DATA FLOW

## Ingestion
Upload → Parse → Embed → Store

## Query
Query → Embed → Search → Context → AI → Response

---

# 🌿 HERB DATA

- ขมิ้นชัน → ลดอักเสบ (NF-kB)
- ฟ้าทะลายโจร → เสริมภูมิ
- ใบบัวบก → ฟื้นฟูสมอง

---

# 🔐 SECURITY

- JWT Auth
- Role-based access

---

# ⚙️ STACK

Frontend: React  
Backend: FastAPI  
Vector: FAISS  
AI: OpenAI  

---

# ▶️ RUN

Backend:
uvicorn app.main:app --reload

Frontend:
npm run dev

---

# 📌 NOTE

AI-powered knowledge system (not just chatbot)

