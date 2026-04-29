<div align="center">

# Shirish Ghimire

Data Analyst by Day | AI Builder by Night

</div>

---

## Hey, I'm Shirish

By day, I'm a **Data Analyst at the University of Utah** — building dashboards, writing SQL, and turning messy institutional data into decisions that actually help students and leadership.

By night, I build AI and ML tools that I wish existed. The kind that flag a struggling student before they drop out, or help someone figure out exactly what skills a job requires.

> *Analytics pays the bills. AI is where I tinker, learn, and build things that push past the dashboard.*

---

## Featured Projects

### Medicare Patient Segmentation (CMS DE-SynPUF)
> *Among Medicare beneficiaries with chronic conditions, which patient segments drive disproportionate cost — and how should a health system prioritize them for outreach?*

End-to-end population health segmentation pipeline on synthetic Medicare claims data. Built as a rigorous portfolio piece: installable Python package, validated clusters, interactive dashboard, and an executive briefing rendered in Quarto.

- **Cohort:** 45,305 fee-for-service Medicare beneficiaries, 2009 baseline features, 2010 outcomes held out
- **Methods:** K-Means and GMM swept across K=2–10; algorithm selected on Hennig-style Jaccard stability (20-iteration 80% subsample validation)
- **Result:** 5 stable segments with distinct cost, utilization, and condition profiles; prioritization framework maps each segment to CMS care management codes
- **Stack:** Python · scikit-learn · pandas · Plotly Dash · Quarto · GitHub Actions CI
- **Tests:** 27 unit tests covering cohort logic, Charlson CCI mapping, and Jaccard stability

[![Repo](https://img.shields.io/badge/GitHub-patientsegmentation-6e40c9?style=for-the-badge&logo=github)](https://github.com/shirish1357/patientsegmentation)

---

### Student Dropout Prediction — Early Warning System
> *Can we catch at-risk students before it's too late?*

An end-to-end ML platform that ingests student engagement data and predicts dropout risk — surfacing ranked intervention lists for academic advisors.

- **Models:** Logistic Regression, Random Forest, XGBoost with automated hyperparameter tuning + cross-validation
- **Data handling:** SMOTE for class imbalance, 15-feature pipeline (GPA, attendance, LMS logins, financial aid, etc.)
- **Output:** Risk scores (0–1), ranked at-risk flags for top 20% highest-risk students
- **Stack:** Python · FastAPI · scikit-learn · XGBoost · React/Vite · Railway · Vercel
- **Live:** Auto-deployed on push via Railway (backend) + Vercel (frontend)

[![Repo](https://img.shields.io/badge/GitHub-Student--Dropout--Prediction-6e40c9?style=for-the-badge&logo=github)](https://github.com/shirish1357/Student-Dropout-Prediction)

---

### Lumen — AI Classroom Platform (University of Utah)
> *Turn any topic or syllabus into a full semester-scale AI classroom.*

A university-branded fork of [OpenMAIC](https://github.com/THU-MAIC/OpenMAIC) (Tsinghua University, published JCST 2026). The base project gives you a single AI classroom session — I extended it into a complete semester-scale study tool. Everything below was built on top of the original engine.

**Added on top of OpenMAIC:**

- **Industry Expert Agent** — new `industry-expert` role with teacher-level permissions; 4 built-in personas (SWE · PM · UX · Data Science) with full create/edit dialog, avatar picker, and color swatches; director prompt updated to route experts as primary speakers
- **Program Catalog** — 557 University of Utah degree programs (undergrad, grad, certificates, PhDs) loaded as searchable context; live Program Picker injects full curriculum (courses, outcomes, requirements) into the generation prompt
- **Syllabus → Course Pipeline** — inline duration picker (Quick → 15 weeks); topic + duration → AI week-by-week plan; syllabus PDF import (AI extracts topics, user reviews before confirming); manual planning mode
- **Course Generation Dashboard** (`/course-generation`) — up to 3 weeks generated in parallel; lazy generation (Week N+1 starts only after Week N completes); per-week progress phases; each week saved to IndexedDB for offline playback
- **Course Library** (`/library`) — persistent dashboard with progress tracking (not started / in-progress / done), Start / Continue / Review per week, quiz score badges (green/amber/red)
- **End-of-Classroom Quiz** — auto-triggered when a session ends; 5 questions (3 single-choice, 1 multiple-choice, 1 short-answer); choice questions graded locally, short-answer graded via LLM; scores persisted in IndexedDB
- **Interview Mode** (`/interview`) — dedicated mock interview flow (4 expert types); stateless SSE streaming; ends with an AI evaluation card; pre-fills topic from the course library
- **Course Progress Sidebar** — week navigator inside the classroom (completed / current / upcoming); jump between weeks without leaving the session; correctly threads `genParams` so lazy generation continues
- **Model Selector** — provider + model switcher was wired in the codebase but never rendered; surfaced it in Settings → System so users can actually switch LLM providers

**Stack:** Next.js 15 · React 19 · TypeScript · Tailwind CSS 4 · LangGraph · Zustand · IndexedDB (Dexie) · SSE streaming

[![Repo](https://img.shields.io/badge/GitHub-lumen--ai--classroom-6e40c9?style=for-the-badge&logo=github)](https://github.com/shirish1357/lumen-ai-classroom)

---

## Other Projects

| Project | What it does | Stack |
|--------|-------------|-------|
| [**Job Skill Extractor v2.0**](https://github.com/shirish1357/Job_Skill_Extractor_v2.0) | Dual-engine NLP (rule-based + semantic) to extract skills from job postings at scale | Python · spaCy · sentence-transformers · FastAPI · TypeScript |
| [**HigherEdAssist**](https://github.com/shirish1357/HigherEdAssist) | Conversational AI for academic program advising | Python · LLMs · ChromaDB · FastAPI · Next.js |
| [**OncoAI**](https://github.com/shirish1357/OncoAI) | AI oncology support assistant for patient education | Python · OpenAI API · Gradio |
| [**twin**](https://github.com/shirish1357/twin) | AI digital twin of me — full-stack with infra | Python · TypeScript · Terraform |

---

## Tech Stack

<div align="center">

**Languages & ML**

[![Skills](https://skillicons.dev/icons?i=python,r,js,ts&theme=dark)](https://skillicons.dev)

**ML / AI**

![scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-FF6600?style=flat-square)
![spaCy](https://img.shields.io/badge/spaCy-09A3D5?style=flat-square&logo=spacy&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logo=huggingface&logoColor=black)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-6e40c9?style=flat-square)

**Backend & Infra**

[![Skills](https://skillicons.dev/icons?i=fastapi,docker,aws,terraform,github&theme=dark)](https://skillicons.dev)

**Frontend & Viz**

[![Skills](https://skillicons.dev/icons?i=react,nextjs,vite&theme=dark)](https://skillicons.dev)
![Tableau](https://img.shields.io/badge/Tableau-E97627?style=flat-square&logo=tableau&logoColor=white)

**Databases**

[![Skills](https://skillicons.dev/icons?i=postgres,mysql&theme=dark)](https://skillicons.dev)
![ChromaDB](https://img.shields.io/badge/ChromaDB-6e40c9?style=flat-square)

</div>

---

## Let's Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Shirish%20Ghimire-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/shirishghimire)
[![Email](https://img.shields.io/badge/Email-Get%20in%20Touch-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shirish.ghm@gmail.com)

</div>
