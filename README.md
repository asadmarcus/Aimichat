# Aimi Chat

**Enterprise-grade AI platform with multi-modal capabilities, autonomous agents, and real-time inference.**

[Live site](https://aimichat.app) • [API Docs](https://aimichat.app/api-docs.html)

---

## What is Aimi?

Aimi is a next-generation AI chat platform that unifies multiple foundation models, retrieval-augmented generation, autonomous browser agents, and real-time voice into a single seamless experience. Built on a globally distributed serverless architecture for sub-100ms response times worldwide.

---

##  Pricing

| Tier | Credits/Day | Price | Quality Modes |
|------|-------------|-------|---------------|
| **Free** | 100 | $0 | Standard |
| **Plus** | 500 | $15/mo | Fast (0.5x) & Balanced (1x) |
| **Ultra** | 2,000 | $50/mo | Fast, Balanced & Premium |

---

## Core Capabilities

| Capability | Description |
|------------|-------------|
| **Genius Mode** | 5-agent multi-AI collaboration using Claude Opus 4.5, GPT-5.2, and Gemini 3 Pro |
| **Deep Research** | Academic-grade research with 200M+ peer-reviewed papers and proper citations |
| **Reasoning** | Step-by-step logical reasoning with transparent chain-of-thought |
| **Voice Interface** | Real-time TTS with word-level highlighting and 11 neural voices |
| **Image Generation** | 4K AI images with 20+ art styles and prompt enhancement |
| **Browser Agents** | Autonomous browser automation with live streaming view |
| **Aimi Health** | Medical AI with image analysis and 8+ trusted health sources |
| **Code Execution** | Python/JS in browser with 75+ packages (NumPy, Pandas, etc.) |
| **Coder Mode** | GLM-4.7 480B - world's best coding model (73.8% SWE-bench) |
| **Presentations** | AI-generated PowerPoint with 6+ types and PPTX export |
| **Study Lab** | NotebookLM-style learning with flashcards, quizzes, mind maps |
| **Memory System** | Cross-chat persistent memory that learns about you |
| **Custom Experts** | 50+ pre-built AI experts + create your own with knowledge bases |
| **API Access** | REST API with OpenAI-compatible format |

---

##  Genius Mode

Genius is Aimi's premium multi-agent reasoning system that orchestrates multiple frontier AI models to deliver comprehensive, well-researched answers with adversarial verification.

### How It Works

Five specialized AI agents collaborate on each query:

| Step | Agent | Model | Role |
|------|-------|-------|------|
| 1 | Deconstructor | Claude Opus 4.5 | Break query into verifiable claims and sub-questions |
| 2 | Evidence Hunter | Gemini 3 Pro | Find evidence FOR and AGAINST each claim with web search |
| 3 | Adversary | GPT-5.2 | Steel-man opposing arguments, identify blind spots |
| 4 | Integrator | Claude Opus 4.5 | Reconcile conflicts into structured synthesis |
| 5 | Verifier | Gemini 3 Pro | Fact-check claims, fix unsupported statements, final polish |

### Features

- **Multi-source research**: Web search, ArXiv papers, Semantic Scholar full-text, Google Scholar
- **Adversarial verification**: Every claim challenged with evidence gathered for both sides
- **Transparent reasoning**: View full thinking process from each agent
- **Confidence scoring**: Calibrated confidence ratings with justification
- **Self-correction**: Verifier fixes any unsupported claims before final output
- **Credit cost**: Reason (200) • Research (250)

### Requirements

- Ultra tier subscription
- Reason or Research mode selected

---

## Deep Research

Academic-grade research with proper citations from 200M+ peer-reviewed papers.

### Data Sources

| Database | Papers | Coverage |
|----------|--------|----------|
| OpenAlex | 200M+ | All disciplines |
| CrossRef | 140M+ | DOI-verified |
| arXiv | 2M+ | STEM preprints |

### Features

- **17 output types**: Research Paper, Literature Review, Case Study, White Paper, Meta-Analysis, etc.
- **Parallel querying**: Searches all databases simultaneously
- **Proper citations**: Inline with DOI links, APA/MLA/Chicago styles
- **Semantic chunking**: Prioritizes abstract, methodology, conclusions
- **Text-first output**: View formatted text, download as PDF on demand

### Limits by Tier

| Tier | Academic Papers | Web Sources | Min Words |
|------|-----------------|-------------|-----------|
| Free | 12 | 6 | 1,500 |
| Plus | 16 | 8 | 2,000-3,000 |
| Ultra | 25 | 10 | 3,000-5,000 |

---

##  Browser Agents

Autonomous browser automation with live streaming view. Watch AI navigate in real-time.

### Features

- **Live streaming**: See the browser as AI controls it
- **Persistent profiles**: Stay logged into sites across sessions
- **Session management**: Save and resume browser states
- **File handling**: Upload/download files
- **OAuth integration**: Connect accounts securely
- **Secrets vault**: Store credentials safely
- **Task templates**: Reusable automation workflows
- **Human handoff**: Take control when AI needs help

### Capabilities

Navigate websites • Fill forms • Extract data • Take screenshots • Download files • Multi-step workflows • Error recovery

### Requirements

- Ultra tier only

---

##  Aimi Health

Privacy-focused health companion with medical API integration and image analysis.

### Medical Sources

NIH • Mayo Clinic • CDC • WHO • OpenFDA • RxNorm • MedlinePlus • ClinicalTrials.gov

### Features

- **Medical image analysis**: X-rays, ECGs, lab reports, skin conditions
- **Lab interpretation**: Values with reference ranges
- **Drug info**: Interactions, dosages, side effects
- **Symptom analysis**: Plain language explanations
- **Appointment prep**: Questions to ask your doctor
- **Mental wellness**: Support and resources

### Models

| Tier | Vision Model |
|------|--------------|
| Free | Gemini 2.5 Flash-Lite |
| Plus/Ultra | Mistral Large 2512 |

*Always reminds users to consult healthcare professionals.*

---

## 💻 Code Execution & Coder Mode

### In-Browser Execution (All Tiers)

Execute Python and JavaScript directly in the browser with instant output.

- **Python 3.11** via Pyodide (WebAssembly)
- **JavaScript ES2022+** (native browser)
- **HTML/CSS** live preview
- **75+ packages**: NumPy, Pandas, Matplotlib, SciPy, scikit-learn
- **Secure sandbox**: Isolated execution environment

### Coder Mode (Ultra Only)

Specialized coding assistant using GLM-4.7 (480B parameters).

- **73.8% SWE-bench** score
- **84.9% LiveCodeBench** pass rate
- **16K token** output limit
- **Production-quality** code without placeholders
- **60x credit multiplier**

---

## 📊 Other Features

### 🎤 Voice Mode
Neural TTS with 11 ElevenLabs voices, word-level highlighting, and streaming playback.

### 🖼️ Image Generation
4K AI images, 20+ art styles, intelligent prompt enhancement, ~15 second generation.

### 📊 Presentations
AI PowerPoint with 6+ types (Pitch Deck, Business Review, Technical, etc.), speaker notes, PPTX export.

### 🧠 Memory System
AI learns about you across conversations. 6 categories, privacy controls, cross-chat persistence.

### 👩‍💼 Custom Experts
50+ pre-built AI experts + create your own with custom instructions and knowledge files.

---

## 🔌 API Access

REST API with OpenAI-compatible format.

```bash
curl -X POST https://aimichat.app/api/ai/v1/chat/completions \
  -H "Authorization: Bearer YOUR_API_KEY" \
  -H "Content-Type: application/json" \
  -d '{
    "messages": [{"role": "user", "content": "Hello!"}],
    "stream": true
  }'
```

### Rate Limits

| Tier | Requests/Day |
|------|--------------|
| Free | ~100 |
| Plus | ~500-1000 |
| Ultra | ~650-4000 |

---

## Architecture

### Infrastructure

```
                         Global Edge Network
                                 |
            +--------------------+--------------------+
            |                    |                    |
      [CloudFront]         [Lambda@Edge]        [API Gateway]
            |                    |                    |
            v                    v                    v
      Static Assets      Edge Compute           Lambda Functions
                                                      |
                    +----------------+----------------+
                    |                |                |
              [Firestore]     [Vector DB]      [AI Providers]
                    |                |                |
               User Data        RAG Index       Model Inference
```

### AI Layer

| Provider | Use Case |
|----------|----------|
| Amazon Bedrock | Foundation models, agents, knowledge bases |
| Cerebras | Ultra-fast inference (world's fastest) |
| NVIDIA NIM | Premium DeepSeek R1, Kimi K2, GLM-4.7 |

---

## Performance

| Metric | Target |
|--------|--------|
| Time to First Token | < 200ms |
| Edge Latency (p95) | < 50ms |
| Concurrent Users | 10,000+ |
| Availability | 99.9% |

---

## Local Development

```bash
npm install
npm run dev
```

---

## License

MIT
