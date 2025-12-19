# Dorado AI (Core) 🐋
### The Operating System for Sovereign AI Agents.

[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)
[![Privacy](https://img.shields.io/badge/Data-Local_Only-green)](https://github.com/dorado-ai)
[![Hardware](https://img.shields.io/badge/Hardware-CPU_Optimized-orange)](https://github.com/dorado-ai)

**Dorado** is an open-source framework for deploying **Agentic RAG Workflows** on air-gapped, on-premises infrastructure. It is designed for high-security environments (Defense, Healthcare, Finance) where data cannot leave the VPC.

---

## 🏗 Architecture: Core + Skills

Dorado is built as a modular "Operating System." You deploy the **Core** once, then install **Skills** (Agent Swarms) to handle specific business tasks.

```bash
/dorado-ai
├── /core                 # The Engine
│   ├── /orchestrator     # LangGraph State Manager
│   ├── /memory           # Qdrant Vector Store (Docker)
│   └── /inference        # Llama.cpp / Ollama Connector
│
└── /skills               # The Modules (Installable)
    ├── /skill-rfp        # 🟢 RFP Response & Compliance (Included)
    ├── /skill-contract   # 🟡 Legal Redlining (Coming Soon)
    └── /skill-research   # 🟡 Deep Web Research (Coming Soon)


🚀 The "RFP Response" Skill (Included)
Out of the box, Dorado comes pre-installed with the RFP Skill. It replaces the manual grind of proposal management.

Ingest: Drag-and-drop PDFs, Excel sheets, and Sharepoint folders.

Draft: "Worker Agents" (Llama 3.2) draft answers based only on your verified history.

Verify: A "Critic Agent" (Qwen 2.5) audits every answer against the compliance matrix.
