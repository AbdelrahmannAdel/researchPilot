# ResearchPilot

**AI-Based Research Paper Classifier and Summarizer**

Upload a research paper PDF and get an instant classification, summary,
keyword extraction, and ranked paper recommendations in a single pass.

Live at [researchpilot.tech](https://researchpilot.tech)

---

## What it does

| Step | Component | Output |
|------|-----------|--------|
| 01 Upload | PyMuPDF | Extracted text |
| 02 Classify | SciBERT (7 / 42 labels) | Domain + confidence score |
| 03 Summarise | Gemini API | Academic summary |
| 04 Keywords | YAKE | Top-N ranked terms |
| 05 Retrieve | Semantic Scholar API | 20 candidate papers |
| 06 Rank | Sentence-BERT + cosine | Top 10 recommendations |

---

## Tech Stack

- **Frontend** — React, Tailwind CSS
- **Backend** — FastAPI
- **Database** — PostgreSQL
- **Classification** — SciBERT (fine-tuned)
- **Summarisation** — Gemini API
- **Keywords** — YAKE (unsupervised)
- **Retrieval** — Semantic Scholar API
- **Embeddings** — Sentence-BERT

---

## Team

Built as a senior capstone at the **University of Bahrain, 2026**.

- **Abdelrahman Adel** — Team Lead, Backend, Data, SciBERT training
- **Mohammed Al Jariri** — Backend, SciBERT training
- **Mohammed Yaser Al Yusuf** — Frontend, SciBERT training
