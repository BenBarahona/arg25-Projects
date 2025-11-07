# ARG25 Project Submission Template

Welcome to Invisible Garden- ARG25.

Each participant or team will maintain this README throughout the program.  
You’ll update your progress weekly **in the same PR**, so mentors and reviewers can track your journey end-to-end.

## Project Title

**PraxY**:
Integrating AI, Blockchain, and zkProofs for Secure and Scalable Medical Assistance

## Team

- **Claudia Gutierrez** - [GitHub: @22lolo](https://github.com/22lolo) - [Devfolio: @smilehi](https://devfolio.co/@smilehi)
- **Benjamin Barahona** - [GitHub: @BenBarahona](https://github.com/BenBarahona) - [Devfolio: @BenBarahona](https://devfolio.co/@BenBarahona)
- **Jorge Destephen** - [GitHub: @jdestephen](https://github.com/jdestephen) - [Devfolio: @jdestephen](https://devfolio.co/@jdestephen)

## Project Description

PraxY is a medical artificial intelligence agent designed to act as a digital clone of a
Medical Director or Head Physician.

The agent is trained with institutional knowledge, clinical experience, and specific medical
literature relevant to the area of practice.

Its goal is to provide continuous assistance to medical and administrative staff through an
accessible messaging application interface (such as Telegram), offering feedback and recommendations aligned with
institutional protocols.

In order to have access to the chat, users will verify via zkID they are indeed a licence practicioner.

## Tech Stack

- **Docker** - Container orchestration and deployment
- **React** - Frontend framework
- **Python** - Backend development
- **Stylus** - Smart Contract development

## Objectives

Build a Proof of Concept of PraxY using AI integration + zkID validation + On-chain validation.

## Weekly Progress

### Week 1 (ends Oct 31)

**Goals:**

- Refine the core product idea and ensure problem-solution fit
- Define the architecture, tools, and overall application flow
- Identify gaps or risks in the project concept

**Progress Summary:**

Refined the concept based on team feedback to ensure viability without storing excessive user data

- Defined the initial project structure and drafted a high-level user flow
- Began outlining the core components of the solution:
  - **zkID** for user authentication
  - **AI chatbot** for secure chat responses
  - **Stylus-based smart contracts** for verifiable chat integrity (still under exploration)
- Started defining how the AI model will be fed data and operate within the system
- Explored tools such as Nillion and zkID. **Nillion was discarded due to difficulties obtaining an API key**
- Began exploring **vLLM** as the AI model runtime
- Early plans established for:
  - Using zkID as the entry point into a Telegram-based chat
  - Integrating an AI chatbot into that chat
  - Building a simple frontend splash screen for onboarding
- Overall, strong progress was made on architecture clarification, tool research, and defining the solution approach before development begins

### Week 2 (ends Nov 7)

**Goals:**

- Begin MVP
- Create chatbot and Telegram Integration
- Simple frontend for Authentication
- Explore LLM options for chatbot communication

**Progress Summary:**

## Current Architecture

### 1. Frontend (`index.html`)

- Telegram deeplink integration
- Links for group join, messaging, and content sharing

---

### 2. Simple Backend (`app.py`)

Basic Flask API server:

- Serves the frontend (`index.html`)
- Endpoints: `/api`, `/health`, `/api/hello`, `/api/echo`

---

### 3. Telegram Bot (`services/telegram_bot.py`)

Implemented Commands:

- `/start` – Welcome
- `/help` – Usage guide
- `/info` – About PraxY
- `/ask` – Question handling
  Includes logging, error handling, and setup guide (`TELEGRAM_SETUP.md`)

---

### 4. Microservices (`docker-compose.yml`)

Current service definitions:

- **Qdrant**: Vector storage for RAG
- **vLLM**: Local LLM inference engine
- **Gateway**: Intended coordination service

---

### 5. Gateway Service (`services/gateway/`)

(Skeleton Only)
Present but non-functional files:

- `app.py` – Basic FastAPI structure
- `rag.py` – Retrieval functions (commented)
- `model_client.py` – AI client (commented)
- `crypto_audit.py` – Empty

Intended features:

- RAG query handling
- Blockchain audit trail
- Secure onboarding and verification
- Web3 integration

---

### 6. Indexer Service (`services/indexer/`)

Document ingestion pipeline that:

- Loads medical documents
- Generates placeholder embeddings
- Encrypts text via AES-GCM
- Computes verification hashes
- Uploads to Qdrant vector DB

---

## Dependencies & Configuration

### Installed

- Flask + CORS
- python-telegram-bot
- python-dotenv

---

### 🗓️ Week 3 (ends Nov 14)

**Goals:**

**Progress Summary:**

## Final Wrap-Up

_After Week 3, summarize your final state: deliverables, repo links, and outcomes._

- **Main Repository Link:**
- **Demo / Deployment Link (if any):**
- **Slides / Presentation (if any):**

## 🧾 Learnings

_What did you learn or improve during ARG25?_

## Next Steps

_If you plan to continue development beyond ARG25, what’s next?_

_This template is part of the [ARG25 Projects Repository](https://github.com/invisible-garden/arg25-projects)._  
_Update this file weekly by committing and pushing to your fork, then raising a PR at the end of each week._
