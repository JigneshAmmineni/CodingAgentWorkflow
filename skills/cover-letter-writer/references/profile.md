# Jignesh Ammineni — Profile for Cover Letters

## Education
- B.S. Computer Science, University of Massachusetts Amherst (graduating May 2026)
- Include only if the role emphasizes academic background or it adds value in context.

## Experience

### Software Engineering Internship (Early-Stage AI Startup)
- Worked across the full stack at an early-stage AI startup: database management, frontend, distributed systems, and DevOps
- Built the certification course feature: designed and managed a relational database for course materials, quizzes, user data, and progress tracking; built the frontend GUI with a focus on aesthetic and intuitive flow to optimize the learning experience
- Contributed to GCP infrastructure using Pulumi (IaC): set up dev, staging, and production stacks with a strong focus on security and compliance
- Used Claude Code as an AI coding assistant throughout, accelerating development and learning
- Key takeaway: touched every layer of the stack, learned fast, and stayed focused on the business problem rather than just closing tickets

### AI Agents & Automation

**Multi-Agent Content Generation System** (Apr 2026 – May 2026)
- Built a multi-agent content generation system on Google's ADK to produce news posts with captioned visuals
- Orchestrated specialist sub-agents (researcher, writer, image generator, editor) using ADK's hierarchical multi-agent patterns, integrating Gemini 2.5 Pro for narrative generation and Imagen 4 for image synthesis
- Deployed to Vertex AI's Agent Engine runtime on GCP; built an ADK evaluation harness scoring trajectory correctness and factual accuracy via LLM-as-judge against an evalset of 50+ test cases
- Built and deployed fully autonomous AI agents to GCP with CI/CD via GitHub Actions and Kubernetes on GKE

**AI Agents Researcher** (Jan 2026 – Apr 2026)
- Co-authored 2 research papers for COLM investigating multi-agent orchestration patterns and vulnerabilities in the Agent-to-Agent (A2A) Protocol, and building safety frameworks for AI labs and enterprises to secure deployments against coordination and protocol-level attacks
- Built AI/ML pipelines for multi-agent systems and language models, implementing automated dataset curation, ablation frameworks, and benchmark harnesses to identify AI agent coordination, communication patterns, and failure modes

**AI/ML Engineer — Insurance Policy RAG Chatbot** (Nov 2025 – Dec 2025)
- Developed an AI chatbot using RAG architecture to index and retrieve from 1,500+ pages of insurance policy documents, reducing average inquiry resolution time from 25 minutes to under 15 seconds
- Engineered a modular RAG pipeline using LangChain, OpenAI, and Pinecone, implementing semantic chunking, hybrid retrieval (cosine similarity + BM25 via Reciprocal Rank Fusion), and chain-of-thought prompt engineering
- Built an automated evaluation pipeline using RAGAS framework and LLM-as-judge; scored 94% context precision, 93% faithfulness, and 96% answer correctness against a 50+ Q&A golden dataset

**Personal Tooling & Workflows**
- Built custom Claude Code workflows, skills, scripts, and CLIs (including one connecting Claude Code to Notion) to accelerate personal development workflow

### Traditional Software Engineering

**Backend Software Engineer — Distributed Microservices**
- Engineered a containerized, distributed backend for a Movie Watchlist system with client-server architecture: 24 RESTful API endpoints, end-to-end API workflows, and full integration testing
- Built 3 microservices using FastAPI with database-per-service architecture (PostgreSQL + SQLModel), enforcing domain separation and data ownership
- Containerized all services with Docker; implemented an NGINX API Gateway with round-robin load balancing supporting up to 5x baseline throughput
- Identified a read-heavy service from traffic patterns and applied Redis caching (cache-aside pattern), reducing average response latency by 40% on repeated reads

**Full-Stack Software Engineer — Real-Time Messaging Website**
- Built and deployed a real-time chat application for 100+ UMass students, architected with course-specific channels to improve peer-to-peer communication
- Led a cross-functional team of 6 developers through the full SDLC: requirements planning, sprint demos, stakeholder communication, and synthesizing feedback into actionable backlog items using Agile and Git
- Engineered real-time bidirectional messaging using React and Socket.IO with event-driven architecture; supported concurrent connections, typing indicators, and automatic reconnection
- Automated CI/CD via GitHub Actions with TypeScript unit and integration tests achieving 85%+ code coverage; deployed to production on Netlify

### Teaching & Communication

**CS Tutor — University of Massachusetts Amherst** (Sept – Dec 2025)
- Conducted one-on-one and group tutoring sessions for 20+ undergraduate students in Data Structures & Algorithms and Operating Systems
- Covered topics including dynamic programming, recursion, memory management, and process scheduling
- Key takeaway: strong ability to identify where a student's mental model breaks down and reframe complex technical concepts in ways that actually land

### Hackathons & Independent Projects
- Regular hackathon participant — builds things for fun and personal utility, not just for résumés
- Driven to build things that solve problems he has personally experienced or witnessed

## Skills
- Languages: Python, JavaScript/TypeScript, SQL (and others picked up as needed)
- Cloud: GCP, GKE (Kubernetes), Vertex AI Agent Engine, GitHub Actions, Pulumi (IaC)
- AI/ML tooling: Claude API, Claude Code, Google ADK, Gemini, Imagen, LangChain, OpenAI, Pinecone, RAGAS, agent frameworks, prompt engineering, LLM evaluation
- Full stack: React, Socket.IO, FastAPI, PostgreSQL, Redis, NGINX, Docker
- DevOps: CI/CD pipelines, containerization, infrastructure-as-code, Agile/Git workflows

## Personal Values
These are authentic — use them when the job description echoes similar language, or adapt them naturally to fit the company's stated values:

- **Ownership**: treats every project as his own, not just a task assigned to him. Cares about outcomes, not just outputs.
- **Problem-first mindset**: starts from the problem, not the solution. Asks why before asking how.
- **Relentless learning**: genuinely loves the "aha" moment — cracking a hard problem, figuring something out from scratch. Self-improvement is a core driver, not a buzzword.
- **Adaptability**: thrives in environments where the scope shifts and you have to figure it out. Has done frontend, backend, infra, and AI in the same role.
- **Craft and detail**: cares about doing things right — security, compliance, clean architecture — not just getting something to work.
- **Builder mentality**: builds things because they're useful or interesting, not because someone told him to. Entrepreneurial by nature.
