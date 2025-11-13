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

PraxY is an innovative AI and blockchain-based platform designed to replicate the expertise, reasoning, and clinical judgment of senior medical professionals through a secure digital assistant. This intelligent agent, referred to as a digital medical clone, provides continuous, protocol-aligned decision support to healthcare personnel, accessible via familiar communication channels such as WhatsApp.

By combining AI training with encrypted verification and zero-knowledge identity (zkID) technology, PraxY ensures that only verified medical professionals interact with the system and that all communications remain encrypted and private. The result is a secure, always-available AI mentor that enhances the accuracy, efficiency, and safety of clinical practice.

### Spanish
PraxY es una plataforma innovadora basada en inteligencia artificial y blockchain que replica la experiencia y el juicio clínico de profesionales médicos senior mediante un asistente digital seguro. Este **clon médico digital** ofrece soporte de decisiones alineado con los protocolos institucionales, accesible a través de canales como WhatsApp.

Todas las interacciones se encuentran **cifradas** y sólo se pueden **desencriptar mediante acceso zkID** verificado, preservando la confidencialidad y la integridad de las consultas. PraxY busca reducir los errores médicos, mejorar la eficiencia clínica y fortalecer la confianza en los servicios de salud públicos y privados.

## Tech Stack

- **Docker** - Container orchestration and deployment
- **React** - Frontend framework
- **Python** - Backend development
- **Stylus** - Smart Contract development
- **Privy & Semaphore** - Account Abstraction and user authentication

## Objectives

## Vision: Digital Medical Clones

PraxY envisions a healthcare ecosystem where institutional knowledge and clinical experience are preserved and shared through intelligent, secure digital replicas of key medical figures. These digital clones are trained on validated protocols, case histories, and the professional expertise of department heads or senior practitioners.

Each clone is designed to serve as a **real-time medical consultant**, available 24/7 through encrypted chat interfaces, providing insights and guidance consistent with institutional standards and medical best practices.

The Problem: Medical Errors and Systemic Fragility

Medical errors remain one of the leading causes of preventable harm worldwide. According to the **World Health Organization (WHO)**:
- Up to **1 in 10 patients** experience an adverse event while receiving hospital care.
- Approximately **50% of these events** are preventable.

Economic impact:
- Globally, medical errors are estimated to cost **over $40 billion annually**.
- In Latin America, studies show that preventable clinical errors contribute to **3–5% of hospital expenditures**, particularly affecting public institutions.
- In Argentina, estimates suggest that **mala praxis incidents** cost the public sector millions annually, due to extended hospital stays, legal expenses, and reputational loss.

The lack of standardized, easily accessible clinical guidance at the point of care — especially in high-pressure environments like emergency rooms and neonatal units — amplifies this systemic fragility. PraxY directly addresses this gap.

## The Solution: PraxY AI

PraxY introduces a **knowledge-preserving AI system** capable of replicating the cognitive model of experienced medical leaders. The AI acts as a secure, conversational interface for clinical decision support, improving alignment with institutional protocols.

**Core capabilities:**
- Access to structured medical knowledge, including institutional protocols and validated medical databases.
- Simulation of a department leader's reasoning model, adapted for safe, compliant interaction.
- Real-time encrypted feedback and validation of medical actions or queries.

## Architecture & Components

PraxY integrates three key technological layers:

### 1. AI Core
A hybrid model combining general medical training data with institution-specific knowledge, continuously refined through supervised feedback and real-world case validation.

### 2. Verification & Integrity Layer
Built with **zkID verification**, ensuring that only certified medical staff can interact with the AI. All conversations are **encrypted end-to-end**, preserving the integrity of consultations. Data is decrypted only upon authenticated zkID access, protecting both patient data and institutional knowledge.

### 3. Communication Interface
The chatbot interface integrates with **WhatsApp and internal hospital communication platforms**, making PraxY accessible without disrupting existing workflows.

---

## 6. Training Methodology: Knowledge Upload & Continuous Feedback

The training process for each digital medical clone involves several stages:

1. **Knowledge Aggregation:** Collecting institutional documents, clinical protocols, case studies, and recorded expertise from key medical professionals.
2. **Cognitive Mapping:** Structuring information to mirror clinical reasoning pathways and decision trees.
3. **Supervised Reinforcement:** Medical staff provide feedback on AI outputs to refine tone, accuracy, and decision patterns.
4. **Continuous Updates:** The clone evolves as new research, guidelines, and hospital data become available.

---

## 7. Clinical and Ethical Impact

PraxY directly contributes to **reducing preventable errors**, **standardizing medical decision-making**, and **protecting institutional reputation**. It enhances knowledge continuity when experienced professionals retire or relocate.

From an ethical standpoint, the system enforces:
- **Encrypted communication** to protect patient confidentiality.
- **Transparent access control** through zkID verification.
- **Audit-ready logs** (decrypted only under authorized review) for quality assurance and accountability.

By ensuring that every consultation remains private and secure, PraxY fosters a culture of safety and trust within the healthcare system.

## Weekly Progress

### Week 1 (ends Oct 31)

**Goals:**

- [x] Refine the core product idea and ensure problem-solution fit
- [x] Define the architecture, tools, and overall application flow
- [x] Identify gaps or risks in the project concept

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

- [x] Begin MVP
- [x] Create chatbot and Telegram Integration
- [x] Simple frontend for Authentication
- [x] Explore LLM options for chatbot communication

**Progress Summary:**

We began work on a simple front-end, defined our authentication option using Privy, and explored methods for integrating the LLM to communicate with the chatbot. Additionally, the Telegram chatbot has been configured and is currently in testing. Next week, we plan to connect it to the LLM and bring all the core components together.

This week progress was made on the following:
- Telegram deeplink integration/testing used for messaging with the future chatbot
- Backend for Telegram chatbot communication and bot configuration on telegram itself
- Explored LLM interface engine microservices and began creating docker files for containers related to LLM we wish to use
- Began a service to be used for the LLM to communicate with the application and AI client
- Explored how to feed data to the model
- Setup an indexer service that loads medical documents and uploads to Qdrant vector DB

### 🗓️ Week 3 (ends Nov 14)

**Goals:**
- [x] Finish front end and user facing interface for identity verification
- [x] Authentication access to chat 
- [ ] Chat interface and communication with LLM
- [ ] Feed LLM data on medical records as a test

**Progress Summary:**

Week 3 was split into two parts: finalizing the frontend and user authentication flow using zkIDs and configuring the LLM we want to use, feeding it the data, and finalizing the API communications part so the frontend application can send and receive responses from it.
Early on the week, we encountered a blocker with the telegram integration, so we decided to drop that functionality and create a simple chat interface on the application.  This chat route would only be accesible to verified users.  Users would have to first enter their medical credentials, and after a confirmation from a trusted authority, they would generate a zkproof that would then be verified by the server to grant access to the chat interface.

*TODO: Add LLMM progress summary*


## Final Wrap-Up

_After Week 3, summarize your final state: deliverables, repo links, and outcomes._

- **Main Repository Link:**
  https://github.com/BenBarahona/invisible_garden_praxy

- **Demo / Deployment Link (if any):**
- **Slides / Presentation (if any):**

## 🧾 Learnings

PraxY represents a transformative step toward a resilient, intelligent healthcare ecosystem. Through AI replication of medical expertise and blockchain-based integrity protection, it bridges the gap between human experience and digital precision.

By integrating encrypted communication, zero-knowledge verification, and continuous learning, PraxY not only prevents medical errors but also elevates the entire standard of care.

## Next Steps

_If you plan to continue development beyond ARG25, what’s next?_

_This template is part of the [ARG25 Projects Repository](https://github.com/invisible-garden/arg25-projects)._  
_Update this file weekly by committing and pushing to your fork, then raising a PR at the end of each week._
