# Aimi Chat

**Enterprise-grade AI platform with multi-modal capabilities, autonomous agents, and real-time inference.**

[Live Demo](https://aimichat.app)

---

## What is Aimi?

Aimi is a next-generation AI chat platform that unifies multiple foundation models, retrieval-augmented generation, autonomous browser agents, and real-time voice into a single seamless experience. Built on a globally distributed serverless architecture for sub-100ms response times worldwide.

---

## Core Capabilities

| Capability | Description |
|------------|-------------|
| **Multi-Model Inference** | Route requests across Cerebras, Amazon Bedrock, and NVIDIA NIM for optimal latency and cost |
| **Deep Research** | Multi-source web research with automatic citation and synthesis |
| **Autonomous Agents** | Browser automation agents that can navigate, extract, and interact with any website |
| **Voice Interface** | Real-time bidirectional voice with streaming transcription and synthesis |
| **Custom Experts** | Build domain-specific AI assistants with custom instructions and knowledge bases |
| **RAG Pipeline** | Vector-based retrieval over uploaded documents (PDF, DOCX, TXT, MD) |
| **Document Export** | Generate PDF, DOCX, PPTX, XLSX from conversations |

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

### Compute Layer
- **AWS Lambda** - Serverless functions with auto-scaling to 10,000+ concurrent executions
- **AWS Lambda@Edge** - Sub-50ms edge compute across 400+ global PoPs
- **Amazon API Gateway** - Managed REST/WebSocket APIs with request throttling

### Data Layer
- **Firebase Firestore** - Multi-region NoSQL with real-time subscriptions
- **Pinecone** - Purpose-built vector database for semantic search
- **Amazon S3** - Durable object storage for knowledge base documents

### AI Layer
- **Amazon Bedrock** - Managed access to Claude, Titan, and other foundation models
- **Amazon Bedrock Agents** - Autonomous multi-step reasoning with tool orchestration
- **Amazon Bedrock Knowledge Bases** - Fully managed RAG with automatic chunking and embedding
- **Cerebras** - Wafer-scale inference for ultra-low latency generation
- **NVIDIA NIM** - Optimized model serving on GPU infrastructure
- **Cloudflare Workers AI** - Edge inference for image generation

---

## AWS Expert Agent

A showcase implementation of Amazon Bedrock Agents for enterprise AWS support:

- **Scope**: All 200+ AWS services, IAM, networking, serverless, containers, databases
- **Capabilities**: Debug issues, review architectures, analyze security, optimize costs
- **Backend**: Claude on Bedrock with optional Knowledge Base for documentation retrieval
- **Integration**: Supports direct invocation, KB-augmented chat, and full agent orchestration

---

## Tech Stack

### Frontend
| Technology | Purpose |
|------------|---------|
| Vite | Build tooling and HMR |
| React 19 | Component architecture |
| Three.js | 3D visualizations |
| Framer Motion | Fluid animations |

### Backend
| Technology | Purpose |
|------------|---------|
| AWS Lambda | Serverless compute |
| Lambda@Edge | Edge computing |
| API Gateway | API management |
| CloudFront | Global CDN |

### AI/ML
| Provider | Use Case |
|----------|----------|
| Amazon Bedrock | Foundation models, agents, knowledge bases |
| Cerebras | High-throughput inference |
| NVIDIA NIM | Premium model serving |
| Jina AI | Text embeddings |
| Pinecone | Vector similarity search |

### Data
| Technology | Purpose |
|------------|---------|
| Firestore | User data, chat history |
| Firebase Auth | Identity management |
| Amazon S3 | Document storage |

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

## Deployment

- **Frontend**: CloudFront + S3 static hosting
- **Backend**: AWS Lambda via SAM/CDK (deployed separately)
- **Edge**: Lambda@Edge for latency-critical paths

---

## License

MIT

---
