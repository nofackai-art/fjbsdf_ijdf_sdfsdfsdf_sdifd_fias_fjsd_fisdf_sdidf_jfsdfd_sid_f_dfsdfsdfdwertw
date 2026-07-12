# Projects

This is the catalog of AI, machine learning, and full-stack projects built and shipped by Moksh Bhardwaj.

---

# Deva AI: Business Insight Creator

## Overview
A fully autonomous AI-powered Business Intelligence agent that transforms raw datasets into actionable insights, visualizations, and predictive analytics.

## Problem Statement
Business teams spend excessive hours manually profiling, cleaning, and visualizing raw dataset uploads. Conversational query interfaces over proprietary CSV files are often unavailable or require writing custom code.

## Solution
An agentic business intelligence dashboard that automates data ingestion, metadata extraction, dynamic chart creation, conversational data analysis, and PDF report compilation.

## Architecture
Built with a multi-step agentic workflow orchestrated by LangGraph and monitored using LangSmith, enabling structured task planning and tool call routing.

## Features
- Ingestion of raw CSV files with automatic shape, null, and duplicate extraction.
- Interactive dashboard generation showing bar, line, scatter, heatmap, and pie charts.
- Conversational chat interface permitting context-aware user queries over uploaded files.
- Predictive forecasting and data trend analysis.
- One-click PDF report export.
- Asynchronous email notifications for analytical summaries.

## Technologies Used
React.js, Vite, FastAPI, Python, Pandas, Recharts, Framer Motion, LangChain, LangGraph, LangSmith, Groq API (LLaMA 3.1, Mixtral), Uvicorn, SMTP.

## AI Components
Orchestrated multi-agent planning with LangGraph using LLaMA 3.1 / Mixtral models for data analysis reasoning and code generation.

## Backend
Python, FastAPI, Uvicorn, LangChain.

## Frontend
React.js (Vite), Recharts, Framer Motion.

## Database
In-memory session state storage and secure sandboxed workspace directories.

## Deployment
Deployed on Vercel (frontend) and Render (backend).

## GitHub Repository
[AI-Agent-For-Business-Insights](https://github.com/0001Moksh/AI-Agent-For-Business-Insights)

## Live Demo
[deva-ai-business-insight-creator.vercel.app](https://deva-ai-business-insight-creator.vercel.app)

## Technical Challenges
Ensuring secure execution of dynamic code for dataset calculations and compiling PDF reports asynchronously.

## My Contributions
Designed the complete multi-agent workflow, configured LangGraph routing, and developed the Recharts dashboard.

## Future Improvements
Implement support for Excel and SQL database connections.

---

# OutreachX Deva

## Overview
A production-ready multi-agent AI cold outreach platform designed to automate lead generation, personalization, campaign creation, and marketing analytics.

## Problem Statement
Cold outreach campaigns suffer from low conversion rates due to lack of personalization and high manual overhead in researching leads.

## Solution
An automated multi-agent framework that conducts background lead research, generates custom personalizations, builds outreach campaigns, and provides performance metrics.

## Architecture
Multi-agent design containing specialized Campaign, Research, Lead, Template, and General agents routing tasks using LangGraph.

## Features
- Background lead and company intelligence research via Tavily search.
- Hyper-personalized AI email text generation tailored to target leads.
- Campaign dashboards tracking delivery, opens, and replies.
- Secure user authentication and template builder.

## Technologies Used
React, FastAPI, Python, LangGraph, LiteLLM, Google Gemini, Groq, OpenRouter, MongoDB, Docker, SMTP, JWT.

## AI Components
Multi-provider LLM routing through LiteLLM utilizing Gemini 1.5, Groq LLaMA, and OpenRouter GPT models for research and text generation.

## Backend
FastAPI, Python, Uvicorn.

## Frontend
React, Tailwind CSS.

## Database
MongoDB for user, lead, and campaign storage.

## Deployment
Dockerized containers deployed on AWS ECS / Render.

## GitHub Repository
[OutreachX-AI-Cold-Mail-Sender](https://github.com/0001Moksh/OutreachX-AI-Cold-Mail-Sender)

## Live Demo
[outreachx-deva.vercel.app](https://outreachx-deva.vercel.app/)

## Technical Challenges
Managing LLM rate limits and fallback configurations across multiple providers during bulk personalization tasks.

## My Contributions
Built the multi-agent graph architecture, configured LiteLLM fallback routers, and built the FastAPI backend.

## Future Improvements
Integrate Webhook tracking for real-time open and bounce metrics.

---

# Deva: AI Admin Chatbot

## Overview
An AI-powered administrative assistant built for academic project management, letting coordinators manage students, supervisors, and teams using natural language.

## Problem Statement
Academic coordinators navigate complex UI panels or direct databases to align students, teams, supervisors, and project workflows.

## Solution
A natural language chat interface executing CRUD commands, assigning teams, and rendering real-time statistics natively through custom UI widgets.

## Architecture
Stateful conversational agent utilizing LangGraph memory, parser interfaces, and WebSockets for real-time state synchronization.

## Features
- Natural language updates for student, supervisor, and team records.
- Fail-safe delete flows with interactive UI confirmation widgets.
- Interactive project workload routing.
- Real-time admin KPIs and PostgreSQL state sync.

## Technologies Used
React.js, FastAPI, Python, PostgreSQL, LangChain, LangGraph, LangSmith, Groq API (LLaMA 3.3), WebSockets, psycopg2.

## AI Components
LLaMA 3.3 70B via Groq API utilizing custom function calling and output parsing to convert chat prompts into structured SQL operations and UI actions.

## Backend
FastAPI, Python, WebSockets.

## Frontend
React.js, Tailwind CSS.

## Database
PostgreSQL for transactional academic data.

## Deployment
Render (backend) and Vercel (frontend).

## GitHub Repository
[deva-ai-agent](https://github.com/0001Moksh/deva-ai-agent)

## Live Demo
Not Applicable (Local/Private Server)

## Technical Challenges
Parsing unstructured user intentions into precise relational database actions while maintaining integrity constraints.

## My Contributions
Designed the PostgreSQL schema, built the LangGraph state machine, and created the custom WebSocket parser.

## Future Improvements
Implement automated supervisor matching algorithms.

---

# Aushadhi 360

## Overview
A complete medical store workflow system to automate pharmaceutical stock management, safety validations, and customer billing.

## Problem Statement
Traditional pharmacy software lacks active medical validation checks, OCR-based stock entry, and intuitive symptom-to-medicine semantic search.

## Solution
A React-Flask ecosystem integrating dual-LLM validations, OCR bills parsing, and hybrid drug searches.

## Architecture
Flask web server communicating with MongoDB, utilizing PyTesseract OCR and FAISS for vector indexing.

## Features
- Dashboard with stock level alerts, expiry notifications, and active reports.
- Automated billing with PDF receipt generation and email invoices.
- OCR scanning of medicine receipts to populate stock entries automatically.
- AI search for drugs based on symptoms or matching names.

## Technologies Used
React, Node.js, Python, Flask, MongoDB, Google Gemini API, PyTesseract, FAISS, SMTP.

## AI Components
Gemini API for symptom analysis and receipt OCR correction; FAISS vector database for drug semantic search.

## Backend
Python, Flask, REST APIs.

## Frontend
React, Tailwind CSS.

## Database
MongoDB for user profiles, stock logs, and billing history.

## Deployment
Deployed on Render.

## GitHub Repository
[aushadhi-360](https://github.com/0001Moksh/aushadhi-360)

## Live Demo
[aushadhi-360.vercel.app](https://aushadhi-360.vercel.app/)

## Technical Challenges
Handling variations in scanned paper receipt formats during OCR processing.

## My Contributions
Developed the backend Flask server, implemented FAISS drug indexing, and built the PyTesseract receipt parser.

## Future Improvements
Add drug-to-drug interaction checks using clinical database APIs.

---

# Seema IQ

## Overview
An AI-powered interview preparation web platform that conducts mock interviews, evaluates user answers, and provides performance reviews.

## Problem Statement
Job seekers struggle to find realistic, interactive, and role-specific interview practice with detailed feedback.

## Solution
An online mock portal parsing candidate resumes to dynamically generate HR, Managerial, and Technical interview rounds.

## Architecture
Next.js serverless functions communicating with Google Gemini and MongoDB.

## Features
- Resume upload with automated profile parsing.
- Stateful, multi-round chat interviews (HR, Manager, Technical).
- Real-time answer analysis and score generation.
- Interactive dashboards tracking candidate progress.

## Technologies Used
Next.js, React, TypeScript, MongoDB, Google Gemini API, Google Services, SMTP.

## AI Components
Google Gemini API for dynamic question generation, resume information parsing, and textual evaluation.

## Backend
Next.js API Routes (Node.js).

## Frontend
Next.js, React, TypeScript, Tailwind CSS.

## Database
MongoDB for user profiles and session logs.

## Deployment
Vercel.

## GitHub Repository
[seemaIQ](https://github.com/0001Moksh/seemaIQ)

## Live Demo
[seema-iq.vercel.app](https://seema-iq.vercel.app/)

## Technical Challenges
Maintaining context across multi-round interview stages without hitting token buffer boundaries.

## My Contributions
Developed the candidate dashboard, wrote TypeScript API routes, and structured the Gemini prompts.

## Future Improvements
Add voice-to-text integration for spoken interview rounds.

---

# Import Medicine

## Overview
An inventory enrichment app designed to import bulk Excel sheets of medicine records, validate details, and append missing metadata using AI.

## Problem Statement
Stock datasets from medical distributors often contain incomplete fields, typos, and missing therapeutic categories.

## Solution
An automated pipeline processing uploaded Excel sheets and querying dual LLM agents to populate clean, validated drug databases.

## Architecture
Flask API pipeline orchestrating Excel parse, LLM enrichment, and MongoDB storage.

## Features
- Upload panel supporting Excel/CSV files.
- Double-agent LLM verification loop to resolve drug information inconsistencies.
- Automated database upserting.

## Technologies Used
Python, Flask, openpyxl, MongoDB, Google Gemini API.

## AI Components
Dual Google Gemini model nodes collaborating to cross-check clinical data points.

## Backend
Python, Flask.

## Frontend
HTML5, Bootstrap, vanilla JS.

## Database
MongoDB.

## Deployment
Local Server / Render.

## GitHub Repository
[Import Medicine using 2 LLM](https://github.com/0001Moksh/Aushidi-360-Sub-Projects/tree/main/Import%20Medicine%20using%202%20LLm)

## Live Demo
Not Applicable (Sub-project module)

## Technical Challenges
Parsing varying column structures from raw Excel spreadsheets.

## My Contributions
Authored the parser using openpyxl and configured the validation agent logic.

## Future Improvements
Add database rollback capabilities for failed upload processes.

---

# Symptoms to Medicine

## Overview
A healthcare sub-app offering semantic symptoms-to-medication recommendations based on user descriptions.

## Problem Statement
Traditional query interfaces fail when users describe their physical symptoms instead of searching for exact drug names.

## Solution
A semantic search application converting physical symptoms into clinical drug recommendations using vector embeddings.

## Architecture
Semantic embedding search using FAISS vector store linked with Google Gemini reasoning.

## Features
- Free-form text symptoms search.
- Structured JSON recommendation payload returned to clients.
- Doctor-style guidelines appended to recommendations.

## Technologies Used
Python, Flask, dotenv, SentenceTransformer, FAISS, Google Gemini API.

## AI Components
SentenceTransformer model for embedding symptoms; FAISS database for vector similarity calculations; Google Gemini for advice generation.

## Backend
Python, Flask.

## Frontend
HTML, Bootstrap.

## Database
FAISS vector database indexes.

## Deployment
Render.

## GitHub Repository
[Symptoms to Medicine using LangChain](https://github.com/0001Moksh/Aushidi-360-Sub-Projects/tree/main/Symptoms%20to%20Medicine%20using%20langchain%20%2B%201%20LLM)

## Live Demo
Not Applicable (Sub-project module)

## Technical Challenges
Ensuring the AI does not recommend high-risk prescription-only drugs without proper medical disclaimers.

## My Contributions
Created the SentenceTransformer vector search logic and configured the FAISS indexes.

## Future Improvements
Incorporate medical dictionary mappings (SNOMED/RxNorm) for accurate matching.

---

# Medicine Filtering

## Overview
A vector-indexed retrieval tool designed to perform typo-tolerant and semantic searches over medical datasets.

## Problem Statement
Simple database queries fail when spelling errors occur in drug names or when searches rely on related symptom concepts.

## Solution
A hybrid search backend blending RapidFuzz string distance computations with FAISS semantic retrieval.

## Features
- Typo-tolerant search for drug names.
- Batch medical ID filtering.
- Semantic similarity similarity score mapping.

## Technologies Used
Python, Flask, FAISS, SentenceTransformer, RapidFuzz.

## AI Components
SentenceTransformer for semantic embedding generation and FAISS for cosine similarity searches.

## Backend
Python, Flask.

## Frontend
HTML5, Bootstrap.

## Database
FAISS local index storage.

## Deployment
Render.

## GitHub Repository
[Medicine Filtering using Embeddings](https://github.com/0001Moksh/Aushidi-360-Sub-Projects/tree/main/Medicine%20Filtering%20using%20Embedding%20%2B%20Vector%20DB)

## Live Demo
Not Applicable (Sub-project module)

## Technical Challenges
Balancing execution speed between RapidFuzz fuzzy matches and SentenceTransformer embeddings.

## My Contributions
Integrated RapidFuzz alongside FAISS semantic calculations.

## Future Improvements
Expose search interfaces via highly scalable REST API endpoints.

---

# AI Resume Analyzer

## Overview
A document analysis app that parses candidate resumes, extracts core profile points, and provides interactive Q&A capabilities.

## Problem Statement
Recruiters spend considerable time reading resumes to map candidate credentials and evaluate their suitability.

## Solution
An automated PDF analyzer extracting structured text and rendering a stateful Q&A chat window over candidate details.

## Architecture
Flask web application utilizing PyPDF2 parsing and Google Generative AI processing.

## Features
- PDF/DOCX resume file upload.
- Automated skill and experience metadata extraction.
- Conversational chat interface to query candidate credentials.

## Technologies Used
Python, Flask, PyPDF2, MongoDB, Google Generative AI.

## AI Components
Google Generative AI models for profile analysis and context-guided resume query answering.

## Backend
Python, Flask.

## Frontend
HTML5, CSS3, JavaScript.

## Database
MongoDB for parsed records metadata.

## Deployment
Render.

## GitHub Repository
[AI-Resume-Analyzer](https://github.com/0001Moksh/AI-Resume-Analyzer)

## Live Demo
[ai-resume-analyzer-9jxc.onrender.com](https://ai-resume-analyzer-9jxc.onrender.com/)

## Technical Challenges
Accurately parsing complex multi-column PDF resumes and layout formatting.

## My Contributions
Built the file upload pipeline, integrated PyPDF2, and configured the Flask server.

## Future Improvements
Incorporate automated candidate-to-job matching scorecards.

---

# Diabetes Prediction App

## Overview
A data science machine learning application predicting patient diabetes risk based on medical metrics.

## Problem Statement
Clinical diagnosis processes require early screening metrics to flag patient risk factors before complex tests.

## Solution
An interactive Streamlit interface letting users key in physical metrics to receive immediate probability analysis from scikit-learn models.

## Architecture
Streamlit application loading pre-trained Scikit-Learn classification pipelines.

## Features
- Real-time diagnostic risk prediction.
- Scikit-learn model comparisons and feature importance visualizations.
- Interactive parameter sliders for user convenience.

## Technologies Used
Python, Streamlit, scikit-learn, Pandas, Seaborn, Matplotlib.

## AI Components
Supervised classification model (Scikit-Learn Random Forest/Logistic Regression).

## Backend
Python, Streamlit Server.

## Frontend
Streamlit UI components.

## Database
None (In-memory processing).

## Deployment
Streamlit Community Cloud.

## GitHub Repository
[Diabetes-Prediction-App](https://github.com/0001Moksh/Diabetes-Prediction-App)

## Live Demo
Not Applicable (Local/Private Server)

## Technical Challenges
Addressing model feature scale requirements to prevent training variance during patient inputs.

## My Contributions
Cleaned the PIMA Indians Diabetes Dataset, built classification models, and developed the Streamlit frontend.

## Future Improvements
Implement secure clinical database storage for patient logs.

---

# AI Interviewer

## Overview
An educational web app that evaluates candidate Excel skills through structured, stateful mock interviews.

## Problem Statement
Standard software questionnaires do not gauge candidates' logical approaches or troubleshooting capabilities in Excel workflows.

## Solution
A chatbot interviewing applicants on Excel operations and recording scores on a public leaderboard.

## Architecture
Flask web server interacting with Google Gemini API and Firebase databases.

## Features
- Stateful Excel technical questioning.
- Automated grading metrics.
- Global leaderboard syncing candidate scores.

## Technologies Used
Python, Flask, Google Gemini LLM, Firebase, HTML5, CSS3.

## AI Components
Google Gemini model for technical question generation and candidate answer evaluation.

## Backend
Python, Flask.

## Frontend
HTML5, Vanilla CSS, JS.

## Database
Firebase Realtime Database for leaderboard tracking.

## Deployment
Render.

## GitHub Repository
Not Applicable (Private source repository)

## Live Demo
[ai-interviewer-by-moksh.onrender.com](https://ai-interviewer-by-moksh.onrender.com/)

## Technical Challenges
Generating context-appropriate technical Excel queries tailored to candidate answer trends.

## My Contributions
Programmed the Flask controller and configured the Firebase database.

## Future Improvements
Support multiple skill topics beyond MS Excel.

---

# Deva Voice Chatbot

## Overview
A voice-enabled AI chat assistant presenting audio feedback using multiple character personas.

## Problem Statement
Standard chatbot platforms rely on text exchanges, making interaction inaccessible or less engaging.

## Solution
A voice portal utilizing Google Text-to-Speech (gTTS) to play back dynamic audio responses based on selected personas.

## Architecture
Flask server querying Gemini API for answers and routing text strings to gTTS.

## Features
- Audio voice playback supporting Deva (male) and Devi (female) characters.
- In-browser voice input recording.
- Session-based conversation logs.

## Technologies Used
Python, Flask, Google Gemini API, gTTS, HTML5 Audio API.

## AI Components
Google Gemini API for conversational context; gTTS for speech synthesis.

## Backend
Python, Flask.

## Frontend
HTML, CSS, JavaScript (Audio API).

## Database
None (Session-based cache).

## Deployment
Render.

## GitHub Repository
Not Applicable (Private source repository)

## Live Demo
[deva-voice-chat.onrender.com](https://deva-voice-chat.onrender.com/)

## Technical Challenges
Reducing backend latency between text generation and speech synthesis to keep responses fast.

## My Contributions
Configured gTTS processing pipeline and integrated audio playback interfaces.

## Future Improvements
Integrate WebSockets for streaming audio packages directly to clients.

---

# HaritAI

## Overview
An AI-powered environmental application that generates sustainable product ideas from waste item images.

## Problem Statement
Individuals and recycling groups struggle to brainstorm useful upcycling ideas for waste materials.

## Solution
An image-input interface running waste classification and generating step-by-step upcycling suggestions.

## Architecture
Flask web server parsing uploaded images and routing them to Gemini Multimodal models.

## Features
- Waste object image classification.
- Interactive step-by-step DIY upcycling ideas.
- Responsive image previews.

## Technologies Used
Python, Flask, Pillow (PIL), Google Gemini AI, Bootstrap.

## AI Components
Gemini Vision models for object classification and generation of DIY instructions.

## Backend
Python, Flask.

## Frontend
HTML5, Bootstrap, JavaScript.

## Database
None (Transient file processing).

## Deployment
Render.

## GitHub Repository
Not Applicable (Nexyug Tech internal product code)

## Live Demo
[haritai.onrender.com](https://haritai.onrender.com/)

## Technical Challenges
Handling varying image qualities and backgrounds during vision classification.

## My Contributions
Built the image upload handler using Pillow and configured the Gemini Vision system.

## Future Improvements
Integrate community sharing boards for upcycling projects.

---

# Deva Chatbot

## Overview
A conversational AI chatbot utilizing Google Gemini to answer questions while formatting raw answers using clean HTML.

## Problem Statement
Standard model outputs contain raw markdown tags, which look unpolished when rendered directly in basic HTML containers.

## Solution
A Flask chatbot using BeautifulSoup parsing to guarantee clean HTML rendering of conversational text.

## Features
- Interactive conversation interface.
- Automatic cleaning of raw markdown tags into valid HTML classes.
- Session-based database caching.

## Technologies Used
Python, Flask, BeautifulSoup, markdown2, Google Gemini API.

## AI Components
Google Gemini API for conversational responses.

## Backend
Python, Flask.

## Frontend
HTML, CSS, JavaScript.

## Database
In-memory session cache.

## Deployment
Render.

## GitHub Repository
Not Applicable (Private source repository)

## Live Demo
[deva-chatbot.onrender.com](https://deva-chatbot.onrender.com/)

## Technical Challenges
Ensuring the BeautifulSoup parser does not strip critical formatting elements during cleaning.

## My Contributions
Developed the text processing middleware and clean rendering modules.

## Future Improvements
Implement multi-language customer routing capabilities.

---

# Deva Voice Assistant

## Overview
An offline-capable PyQt5 desktop assistant running PyQt visual components and voice system control commands.

## Problem Statement
Web-based voice assistants cannot execute system control operations or access local desktop files directly.

## Solution
A PyQt5 Python desktop client capturing voice commands to perform local operating system control actions.

## Architecture
PyQt5 application calling local OS commands and Google Gemini APIs.

## Features
- Voice-controlled operating system commands.
- Real-time language translation.
- Task scheduler and productivity checklist.

## Technologies Used
Python, PyQt5, Google Gemini API.

## AI Components
Google Gemini API for parsing user intent and language translation commands.

## Backend
Python, local OS system script execution.

## Frontend
PyQt5 GUI desktop application.

## Database
Local file storage (JSON files).

## Deployment
Local Python desktop execution.

## GitHub Repository
Not Applicable (Academic showcase module)

## Technical Challenges
Implementing real-time microphone listeners without freezing the PyQt5 application thread.

## My Contributions
Designed the PyQt5 GUI, programmed the background threading, and configured the local system commands.

## Future Improvements
Add support for custom desktop application plugins.
