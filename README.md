<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:FFDAC1,100:F4A261&height=200&section=header&text=Shirish%20Ghimire&fontSize=52&fontColor=5a3e28&fontAlignY=38&desc=Data%20Analyst%20by%20Day%20%7C%20AI%20Builder%20by%20Night&descAlignY=58&descSize=20&animation=fadeIn" width="100%"/>

<a href="https://readme-typing-svg.demolab.com">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=6E40C9&center=true&vCenter=true&width=600&lines=Data+analytics+at+work.;AI+%26+ML+for+fun+%28and+impact%29.;Building+tools+I+wish+existed." alt="Typing SVG" />
</a>

</div>

---

## 👋 Hey, I'm Shirish

By day, I'm a **Data Analyst at the University of Utah** — building dashboards, writing SQL, and turning messy institutional data into decisions that actually help students and leadership.

By night, I build **AI and ML tools** that I wish existed. The kind that flag a struggling student before they drop out, or help someone figure out exactly what skills a job requires.

> *Analytics pays the bills. AI is where I tinker, learn, and build things that push past the dashboard.*

---

## Featured Projects

### 🎓 Student Dropout Prediction — Early Warning System
> *Can we catch at-risk students before it's too late?*

An end-to-end ML platform that ingests student engagement data and predicts dropout risk — surfacing ranked intervention lists for academic advisors.

- **Models:** Logistic Regression, Random Forest, XGBoost with automated hyperparameter tuning + cross-validation
- **Data handling:** SMOTE for class imbalance, 15-feature pipeline (GPA, attendance, LMS logins, financial aid, etc.)
- **Output:** Risk scores (0–1), ranked at-risk flags for top 20% highest-risk students
- **Stack:** Python · FastAPI · scikit-learn · XGBoost · React/Vite · Railway · Vercel
- **Live:** Auto-deployed on push via Railway (backend) + Vercel (frontend)

[![Repo](https://img.shields.io/badge/GitHub-Student--Dropout--Prediction-6e40c9?style=for-the-badge&logo=github)](https://github.com/shirish1357/Student-Dropout-Prediction)

---

### Job Skill Extractor v2.0 — NLP Skill Intelligence
> *What skills does a job actually require? Let's extract that at scale.*

A dual-engine NLP system that extracts technical and soft skills from job postings using two competing approaches — rule-based and ML-based — then compares their accuracy head-to-head.

- **Rule-based engine:** spaCy PhraseMatcher + regex — fast, precise, production-ready
- **ML engine:** sentence-transformers semantic matching — broader coverage, discovers skill variations
- **Skill database:** 200+ hard skills (languages, frameworks, cloud/DevOps) · 40+ soft skills
- **Data:** LinkedIn job postings pipeline via Kaggle API
- **Stack:** Python · spaCy · sentence-transformers · FastAPI · TypeScript · HTML/CSS · Jupyter
- **Interface:** REST API + interactive web UI for real-time extraction

[![Repo](https://img.shields.io/badge/GitHub-Job__Skill__Extractor__v2.0-6e40c9?style=for-the-badge&logo=github)](https://github.com/shirish1357/Job_Skill_Extractor_v2.0)

---

### 🤖 Lumen — AI Classroom Platform (University of Utah)
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

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:F4A261,100:FFDAC1&height=120&section=footer" width="100%"/>
</div>
