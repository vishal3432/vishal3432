<h1 align="center">Hey, I'm Vishal Singh 👋</h1>

<p align="center">
  <b>Backend Developer &nbsp;·&nbsp; Python &nbsp;·&nbsp; FastAPI & Django &nbsp;·&nbsp; PostgreSQL &nbsp;·&nbsp; Docker</b>
</p>

<p align="center">
  <a href="https://linkedin.com/in/vishal3432">LinkedIn</a> &nbsp;·&nbsp;
  <a href="https://vishalportfolio7999.lovable.app">Portfolio</a> &nbsp;·&nbsp;
  <a href="mailto:vishals.analyst@gmail.com">Email</a>
</p>

---

## 🙋‍♂️ About Me

I'm a backend developer who genuinely enjoys the problem-solving side of building things — figuring out why a system is slow, how to structure an API cleanly, or how to make two services talk to each other reliably.

Most of my work revolves around Python — building REST APIs with Django and FastAPI, connecting them to PostgreSQL, and packaging everything in Docker so it actually works the same everywhere. I've spent a good amount of time on async systems, background task processing with Celery, and making sure the things I build don't fall apart under real usage.

Right now I'm focused on:
- Building more production-grade backend systems end to end
- Getting comfortable with AWS and cloud deployments
- Improving my understanding of system design and performance at scale

---

## 🛠️ Tech Stack

### 💻 Backend
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)
![Django](https://img.shields.io/badge/Django-092E20?style=flat&logo=django&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat&logo=flask&logoColor=white)
![JWT](https://img.shields.io/badge/JWT-000000?style=flat&logo=jsonwebtokens&logoColor=white)
![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=flat&logo=socketdotio&logoColor=white)

### 🗄️ Database & Cache
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat&logo=redis&logoColor=white)
![SQLAlchemy](https://img.shields.io/badge/SQLAlchemy-CC2927?style=flat&logo=python&logoColor=white)
![Alembic](https://img.shields.io/badge/Alembic-6DB33F?style=flat&logo=python&logoColor=white)

### ⚙️ DevOps & Tools
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white)
![Celery](https://img.shields.io/badge/Celery-37814A?style=flat&logo=celery&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat&logo=nginx&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat&logo=git&logoColor=white)
![Render](https://img.shields.io/badge/Render-46E3B7?style=flat&logo=render&logoColor=white)

### 📊 Data & Scraping
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat&logo=scikitlearn&logoColor=white)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-4B8BBE?style=flat&logo=python&logoColor=white)
![Selenium](https://img.shields.io/badge/Selenium-43B02A?style=flat&logo=selenium&logoColor=white)

### 🤖 AI & LLM
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat&logo=openai&logoColor=white)
![Ollama](https://img.shields.io/badge/Ollama-000000?style=flat&logo=ollama&logoColor=white)

---

## 🔥 Featured Projects

### 1️⃣ AI Automation Pipeline with LLM Routing (Ongoing)
> *Automated customer reply system that routes messages through 3 AI layers — always using the cheapest option first*

A production-ready backend that receives messages from WhatsApp, Email, or any API and replies automatically using AI — no human needed after setup.

Every message goes through a smart routing engine:
- **Template Engine** → instant reply for common questions (greetings, pricing, refunds) — zero cost
- **Local LLM via Ollama/Mistral** → handles complex messages on your own server — near-zero cost  
- **OpenAI GPT** → fallback for anything the local model can't handle — ~$0.002 per message

Responses are cached in Redis so repeated questions cost nothing the second time.

**Tech:** FastAPI · Celery · Redis · PostgreSQL · SQLAlchemy · Alembic · Ollama · OpenAI · Docker  
**Highlights:**
- 3-tier hybrid LLM routing reduces OpenAI API costs by up to 80%
- Async task processing via Celery with full retry logic
- WhatsApp Meta webhook integration with HMAC signature validation
- Database migration system via Alembic with full upgrade/downgrade support
- Per-sender rate limiting, structured JSON logging, and analytics endpoint

🔗 Repo: https://github.com/vishal3432/AI-Automation-Pipeline-with-LLM-Routing

---

### 2️⃣ Ecommerce Smart Recommendation System
> *Django-based recommendation engine that suggests products based on user behaviour*

Built an AI-powered product recommendation system that tracks what users like and dislike, then uses cosine similarity and TF-IDF vectorization to suggest relevant products in real time.

**Tech:** Django · DRF · FastAPI · Scikit-learn · Pandas · PostgreSQL · Docker  
**Highlights:**
- Hybrid architecture — Django handles the storefront, FastAPI serves the ML recommendations
- Cosine similarity over product descriptions for personalized suggestions
- ~30–40% faster response time through optimized query design
- Scalable modular MVT architecture

🔗 Repo: https://github.com/vishal3432/Ecommerce_smart_recommendation

🚀 Live Demo : https://ecommerce-smart-recommendation-crp8.onrender.com

---

### 3️⃣ Rental Property Scraper API
> *Scrapes rental listings, removes duplicates using ML, and recommends similar properties via REST API *

A lightweight scraping API that pulls rental property listings, parses them into structured data, and exports to CSV — deployed live on Render.

**Tech:** FastAPI · BeautifulSoup · Scikit-learn · NumPy · SQLAlchemy · PostgreSQL · Celery · Redis · Docker 
**Highlights:**
 - Scrapes and parses rental listings with address, price, and link extraction
 - Auto-deduplicates listings using TF-IDF + cosine similarity before saving
 - Recommends similar properties based on embedding similarity
 - Async background scraping via Celery with auto-retry and exponential backoff
 - Search by address and filter by price range with pagination
 - Dockerized with PostgreSQL, Redis, and deployed on Render

🔗 Repo: https://github.com/vishal3432/Rental-property-web-scraper-

🚀 Live Demo : https://rental-property-web-scraper-1.onrender.com/docs

---

## 📫 Get in Touch

| | |
|---|---|
| 💼 LinkedIn | [linkedin.com/in/vishal3432](https://linkedin.com/in/vishal3432) |
| 🌐 Portfolio | [vishalportfolio7999.lovable.app](https://vishalportfolio7999.lovable.app) |
| 📧 Email | vishals.analyst@gmail.com |

---

> *I care more about building things that actually work in production than things that just look good in a demo.*
