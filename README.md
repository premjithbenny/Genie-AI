[![pipeline status](https://opensource.unicc.org/un/itu/genie-ai/badges/main/pipeline.svg)](https://opensource.unicc.org/un/itu/genie-ai/-/pipelines?ref=main)
[![coverage report](https://opensource.unicc.org/un/itu/genie-ai/badges/main/coverage.svg)](https://opensource.unicc.org/un/itu/genie-ai/-/graphs/main/charts)
[![license](https://img.shields.io/badge/license-Apache--2.0-blue.svg)](./LICENSE)
[![Digital Public Good](https://img.shields.io/badge/DPG-aligned-0089D6.svg)](https://www.digitalpublicgoods.net/standard)
[![OSI Open Source AI](https://img.shields.io/badge/OSI%20Open%20Source%20AI-compliant-3DA639.svg)](https://opensource.org/ai/open-source-ai-definition)
[![documentation](https://img.shields.io/badge/docs-GENIE.AI-FF6A00.svg)](https://genie-ai-7e342b.opensource.unicc.org/)

# GENIE.AI

**GENIE.AI** is a sovereign, open-source Retrieval-Augmented Generation (RAG) framework for the public sector. It lets governments and public institutions deploy grounded, multilingual, auditable AI assistants over their own document repositories — on their own infrastructure, with full data sovereignty and no vendor lock-in.

It is compliant with the [OSI Open Source AI Definition](https://opensource.org/ai/open-source-ai-definition) and aligned with the [Digital Public Goods (DPG) Standard](https://www.digitalpublicgoods.net/standard), and integrates [OPEA (Open Platform for Enterprise AI)](https://opea.dev) for its AI/ML services. Initiated under the [ITU OSEE programme](https://www.itu.int/en/ITU-D/ICT-Applications/Pages/Initiatives/OSEEPSI/home.aspx).

## Why GENIE.AI

- **Sovereign by design** — embedding, reranking, generation and translation models run on your infrastructure (OPEA / vLLM / TEI). No third-party model API required.
- **Grounded answers** — the LLM answers only from retrieved knowledge-base content and abstains when the answer is not present.
- **Standards-based, no lock-in** — OIDC identity, OpenTelemetry observability, OpenAI-compatible model APIs, W3C trace context.
- **Multilingual** — English as RAG source of truth, translated UI and answer streams (11+ languages).

→ Full context: [About GENIE.AI](https://genie-ai-7e342b.opensource.unicc.org/about/) and [Project overview](https://genie-ai-7e342b.opensource.unicc.org/docs/core/project-overview/).

---

## Quick start

```bash
# 1. Clone
git clone https://github.com/premjithbenny/Genie-AI.git
cd Genie-AI

# 2. Configure (secrets: ARANGO_PASSWORD, KEYCLOAK_ADMIN_PASSWORD,
#    KEYCLOAK_CLIENT_SECRET, HUGGING_FACE_HUB_TOKEN, VLLM_API_KEY, ...)
cp env .env && $EDITOR .env

# 3. Deploy
docker compose up -d                                  # core services


