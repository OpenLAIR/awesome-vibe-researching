# Awesome Vibe Researching [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

<!-- Dynamic badges (auto-update from GitHub) -->
[![GitHub stars](https://img.shields.io/github/stars/OpenLAIR/awesome-vibe-researching?style=social)](https://github.com/OpenLAIR/awesome-vibe-researching/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/OpenLAIR/awesome-vibe-researching?style=social)](https://github.com/OpenLAIR/awesome-vibe-researching/network/members)

<!-- Static badges -->
[![License: CC0-1.0](https://img.shields.io/badge/License-CC0_1.0-lightgrey.svg)](https://creativecommons.org/publicdomain/zero/1.0/)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)
[![Resources](https://img.shields.io/badge/resources-107-blue.svg)](#navigation-guide)
[![Papers](https://img.shields.io/badge/papers-45-orange.svg)](#navigation-guide)
[![Tools](https://img.shields.io/badge/tools-62-purple.svg)](#navigation-guide)
[![Last Updated](https://img.shields.io/badge/last_updated-March_2026-green.svg)](#acknowledgments)

> A curated list of resources for **Vibe Researching** -- AI-driven research automation across the scientific discovery pipeline, from literature review to publication.

**Vibe Researching** extends the concept of "vibe coding" (conversational, AI-assisted programming) to the entire research workflow. This collection covers tools, papers, and frameworks spanning six research pipeline stages (Survey -> Ideation -> Experiment -> Analysis -> Writing -> Promotion) and six autonomy levels (L0 Manual -> L5 Fully Autonomous).

**Legend**: `NEW` = published/released 2025-2026 | `OSS` = open-source | `FREE` = free to use

## Contents

- [What is Vibe Researching?](#what-is-vibe-researching)
- [Navigation Guide](#navigation-guide)
- [Survey & Literature Review](#survey--literature-review)
- [Ideation & Hypothesis Generation](#ideation--hypothesis-generation)
- [Experiment & Implementation](#experiment--implementation)
- [Analysis & Interpretation](#analysis--interpretation)
- [Writing & Publishing](#writing--publishing)
- [Promotion & Dissemination](#promotion--dissemination)
- [Cross-Cutting Tools](#cross-cutting-tools)
- [Related Resources](#related-resources)
- [Contributing](#contributing)
- [License](#license)

## What is Vibe Researching?

**Vibe Researching** is the application of AI agents with skills to the full research pipeline, enabling researchers to:

- **Automate literature reviews** -- 80-90% time savings with tools like Elicit, Rayyan
- **Generate code from academic papers** -- DeepCode: 75.9% success, beats human experts at 72.4%
- **Run autonomous experiments** -- A-Lab: 10x data collection speedup, 71% success rate
- **Produce complete research papers** -- AI Scientist-v2: first peer-reviewed AI-generated paper, 2025

**Key Paper**: [Vibe Researching as Wolf Coming](https://arxiv.org/abs/2602.22401) (arXiv:2602.22401, Feb 2026) -- Introduces the vibe researching paradigm with cognitive task framework

**Community**: [VibeX 2026 Workshop](https://conf.researchr.org/home/ease-2026/vibex-2026) -- 1st International Workshop on Vibe Coding and Vibe Researching @ EASE 2026

## Navigation Guide

### By Research Stage

This list is organized by the **research pipeline** (Survey -> Ideation -> Experiment -> Analysis -> Writing -> Promotion). Each stage has tools and papers at different **autonomy levels**:

| Level | Name | Human Role | AI Role | Example |
|-------|------|------------|---------|---------|
| **L1** | Assist | Drives all decisions | Suggests | Code completion, grammar checking |
| **L2** | Partial | Defines task, validates | Executes specific subtasks | Automated screening, figure generation |
| **L3** | Conditional | Sets goals, approves at checkpoints | Handles full workflows | End-to-end literature review |
| **L4** | High | Monitors for failures | Handles extended workflows | Self-driving labs |
| **L5** | Full | None (reviewer/consumer) | Operates independently | AI Scientist: idea -> paper |

### Level x Stage Matrix

```
                 | Survey | Ideation | Experiment | Analysis | Writing | Promotion |
-----------------+--------+----------+------------+----------+---------+-----------+
Level 1 (Assist) |   8    |    2     |    12      |    3     |    6    |     1     |
Level 2 (Partial)|   6    |    3     |    10      |    7     |    2    |     0     |
Level 3 (Cond.)  |   2    |    2     |     8      |    4     |    1    |     0     |
Level 4 (High)   |   1    |    1     |    12      |    3     |    0    |     0     |
Level 5 (Full)   |   0    |    1     |     6      |    1     |    1    |     0     |
-----------------+--------+----------+------------+----------+---------+-----------+
Total            |  17    |    9     |    48      |   18     |   10    |     1     |
```

### Key Statistics

| Metric | Value | Source/Year |
|--------|-------|-------------|
| Total resources | 107 (45 papers, 62 tools) | This survey, Mar 2026 |
| Developer AI adoption | 92% of US developers use AI coding tools daily | 2025 industry data |
| Code generation share | 41% of all code globally AI-generated (256B lines) | Google, 2024 |
| Lab automation market | $7.84B -> $14.78B (CAGR 6.55%) | 2024-2034 forecast |
| Multimodal AI market | $391B -> ~$2T (CAGR 35.9%) | 2025-2030 forecast |
| Key milestone | AI Scientist-v2: first peer-reviewed AI paper | ICLR 2025 |

---

## Survey & Literature Review

> Tools and papers for literature search, systematic review, knowledge extraction, and gap analysis. (17 items)

### Level 1 -- Assisted Search

**Papers**:

- [Vibe Coding in Practice: Motivations, Challenges, and a Future Outlook](https://arxiv.org/abs/2510.00328) `NEW` -- Grey literature review (arXiv:2510.00328, Sep 2025). Analyzed 101 practitioner sources with **518 firsthand behavioral accounts**. Revealed speed-quality trade-off paradox: **62% motivated by speed**, but code often 'fast but flawed'. *Tags: empirical study, grey literature, developer experience.*

**Tools**:

- **[Google Scholar](https://scholar.google.com/)** `FREE` -- Classic academic search engine with citation tracking, h-index metrics, and researcher profiles. Free access to academic literature across disciplines. De facto standard for citation counts. *L1 Assist.*
- **[Semantic Scholar](https://www.semanticscholar.org/)** `FREE` -- AI-powered academic search from Allen Institute for AI. Features citation contexts, paper recommendations, TLDR summaries, and influential citations analysis. Covers 200M+ papers. *L1 Assist.*

### Level 2 -- Automated Screening & Extraction

**Tools**:

- **[Elicit](https://elicit.com/)** -- AI-powered systematic review platform. 125M+ papers, 545K clinical trials. **80% time savings** for systematic reviews, high precision for preliminary searches. Automated data extraction and evidence synthesis. *L2 Partial. Commercial.*
- **[Rayyan](https://www.rayyan.ai/)** -- AI study screening for systematic reviews. **90% reduction in screening time**, ML-based study suggestion, automatic deduplication. Widely used in biomedical systematic reviews. *L2 Partial. Freemium.*
- **[Consensus](https://consensus.app/)** -- AI academic search engine. 200M+ peer-reviewed papers, evidence-based answers with citation support, automated data synthesis. Focuses on extracting research findings as direct answers. *L2 Partial. Freemium.*
- **[Scite](https://scite.ai/)** -- Smart citation analysis evaluating how publications are cited: supporting, contrasting, or mentioning. Reveals citation context beyond simple counts. *L2 Partial. Commercial.*

### Level 3 -- End-to-End Literature Review

**Tools**:

- **[Paperguide](https://paperguide.ai/)** `NEW` -- Fully automated systematic review: research question -> search -> screening -> report generation. Improved by Deep Research integration (June 2025). Competitive features at lower price than SciSpace. *L3 Conditional. Commercial.*
- **[SciSpace](https://scispace.com/)** -- **10M+ researchers** (2026). Upload PDF, chat with paper, semantic search, automated summarization, reference management, AI copilot. Comprehensive research assistant platform. *L3 Conditional. Freemium.*

### Stage Summary

| Finding | Detail |
|---------|--------|
| Time savings | 80-90% demonstrated by Elicit and Rayyan in systematic review workflows |
| Adoption pattern | Commercial-first: tools emerged 2021-2024, academic evaluation papers followed 2024-2026 |
| Gap | No Level 4-5 tools for autonomous literature synthesis exist yet |

---

## Ideation & Hypothesis Generation

> Tools and papers for research question formulation, hypothesis generation, and novelty checking. (9 items -- under-represented stage)

### Level 1-2 -- Brainstorming & Templates

**Tools**:

- **Brainstorming Assistants** -- GPT-powered conversational agents for research question ideation and problem formulation. General-purpose LLMs (ChatGPT, Claude) serve as interactive brainstorming partners. *L1 Assist.*
- **Hypothesis Generators** -- Template-based tools for structured research question development using PICO/FINER frameworks. *L1 Assist.*
- **Gap Analysis Tools** -- AI-powered literature analysis for identifying research gaps and understudied areas by analyzing citation patterns and topic coverage. *L2 Partial.*

### Level 5 -- Autonomous Ideation

**Papers**:

- [The AI Scientist: Towards Fully Automated Open-Ended Scientific Discovery](https://arxiv.org/abs/2408.06292) (arXiv:2408.06292, 2024, Sakana AI) -- Original autonomous research system producing ML conference-quality LaTeX papers, achieves **'Weak Accept' ratings**. Uses Semantic Scholar for automated citation retrieval. *Foundational paper for AI-driven scientific discovery.*
- [The AI Scientist-v2: Workshop-Level Automated Scientific Discovery via Agentic Tree Search](https://arxiv.org/abs/2504.08066) `NEW` (arXiv:2504.08066, 2025, Sakana AI) -- **First AI-generated paper accepted through peer review** (ICLR 2025 workshop). Removes human templates, uses progressive agentic tree search, generalizes across ML domains. *Milestone: exceeded human acceptance threshold.*

**Tools**:

- **[Sakana AI - AI Scientist](https://sakana.ai/ai-scientist/)** `OSS` -- ([GitHub](https://github.com/SakanaAI/AI-Scientist) | 5k+ stars) End-to-end autonomous research: idea generation -> code implementation -> experiment execution -> LaTeX paper. Open-source reference implementation. *L5 Full.*

### Critical Evaluation

**Papers**:

- [Evaluating Sakana's AI Scientist for Autonomous Research](https://arxiv.org/abs/2502.14297) `NEW` (arXiv:2502.14297, 2025, ACM SIGIR Forum) -- **Critical evaluation** revealing **42% experiment failure rate** due to coding errors, poor novelty assessments (misclassifying established concepts as novel). Important counterpoint to optimistic claims. *Evaluation paper.*

### Stage Summary

| Finding | Detail |
|---------|--------|
| Critical gap | Ideation stage under-represented (9 items total, mostly Level 1-2) |
| Need | Standalone autonomous hypothesis generation tools (Level 4-5), novelty checking systems |
| AI Scientist limitation | 42% failure rate requires human review of all outputs |

---

## Experiment & Implementation

> Tools and papers for protocol design, code implementation, laboratory execution, and data collection. **Largest category** (48 items).

### Vibe Coding (Level 1 -- Code Completion)

**Papers**:

- [A Survey of Vibe Coding with Large Language Models](https://arxiv.org/abs/2510.12399) `NEW` (arXiv:2510.12399, Dec 2025) -- Synthesizes vibe coding practices into **5 development models**: Unconstrained Automation, Iterative Conversational Collaboration, Planning-Driven, Test-Driven, Context-Enhanced. *Survey paper. Tags: taxonomy, development models.*
- [Vibe coding: programming through conversation with artificial intelligence](https://arxiv.org/abs/2506.23253) `NEW` (arXiv:2506.23253, Oct 2025) -- **First empirical study** analyzing **8+ hours of curated video**. Found vibe coding redistributes expertise toward context management and rapid code evaluation. *Empirical study. Tags: think-aloud, expertise.*
- [Academic Vibe Coding: Opportunities for Accelerating Research in an Era of Resource Constraint](https://arxiv.org/abs/2508.00952) `NEW` (arXiv:2508.00952, Aug 2025) -- Structured, prompt-driven code generation embedded in reproducible workflows to **compress idea-to-analysis timeline** and reduce staffing pressure. *Position paper. Tags: academic research, reproducibility.*
- [Vibe Coding for UX Design](https://arxiv.org/abs/2509.10652) `NEW` (arXiv:2509.10652, Sep 2025) -- UX professionals find benefits (productivity, cognitive offloading, learning, creativity) but note **unsuitability for production-level tasks** with complex back-end systems. *User study. Tags: UX, front-end.*
- [Vibe Coding: Toward an AI-Native Paradigm for Semantic and Intent-Driven Programming](https://arxiv.org/abs/2510.17842) `NEW` (arXiv:2510.17842, Oct 2025) -- Proposes AI-native programming paradigm focused on semantic and intent-driven development, moving beyond syntax-level assistance. *Theory paper. Tags: paradigm, semantic programming.*

**Tools**:

| Tool | Type | Key Metric | Pricing |
|------|------|------------|---------|
| **[GitHub Copilot](https://github.com/features/copilot)** | Commercial | **20M users**, 90% of Fortune 100 | $10-39/mo |
| **[Cursor](https://cursor.com/)** | Commercial | **4.9/5 ratings**, $60M Series A | Free-$20/mo |
| **[Claude Code](https://claude.ai/code)** | Commercial | **46% "most loved"** (2026) | Subscription |
| **[Tabnine](https://www.tabnine.com/)** | Commercial | **Air-gapped support**, privacy-first | Freemium |
| **[Continue](https://continue.dev/)** `OSS` | Open Source | [GitHub](https://github.com/continuedev/continue) **15k+ stars** | Free |
| **[Aider](https://aider.chat/)** `OSS` | Open Source | [GitHub](https://github.com/paul-gauthier/aider) **20k+ stars**, ~75% success | Free |

**Tool Details**:

- **[GitHub Copilot](https://github.com/features/copilot)** -- Pioneering inline autocomplete (launched 2021). **20M users** (mid-2025), powers **90% of Fortune 100**. Supports Claude 3 Sonnet, Gemini 2.5 Pro. Agent Mode introduced 2025. *L1 Assist. Commercial: $10/mo individual, $19/mo Business, $39/mo Enterprise.*
- **[Cursor](https://cursor.com/)** -- Developed by Anysphere (2023), **$60M Series A** (Aug 2024). Averages **4.9/5 user ratings** across 2025-2026 roundups. Top-ranked vibe-coding tool in independent benchmarks. *L1 Assist. Commercial: Free tier, $20/mo Pro.*
- **[Claude Code](https://claude.ai/code)** `NEW` -- **46% "most loved" rating** (early 2026) vs Cursor 19%, GitHub Copilot 9%. Terminal-native agentic coding from Anthropic. *L1 Assist. Included in Claude subscription.*
- **[Tabnine](https://www.tabnine.com/)** -- **Privacy-focused** pioneer. Local/private cloud/VPC deployment, **air-gapped support**. Enterprise Context Engine learns org architecture. Best for regulated industries. *L1 Assist. Freemium + Enterprise.*
- **[Continue](https://continue.dev/)** `OSS` -- ([GitHub](https://github.com/continuedev/continue) | **15k+ stars**) Open-source, developer-first coding assistant. Flexible model selection, extensible architecture. *L1 Assist. Free.*
- **[Aider](https://aider.chat/)** `OSS` -- ([GitHub](https://github.com/paul-gauthier/aider) | **20k+ stars**) Repository-level agent handling 50k+ LOC codebases with **~75% success rate**. Multi-file refactors, debugging loops, scoped task execution. *L2 Partial. Free.*

### Code Generation from Papers (Level 2)

**Papers**:

- [Paper2Code: Automating Code Generation from Scientific Papers in Machine Learning](https://arxiv.org/abs/2504.17192) (arXiv:2504.17192, 2024) -- Multi-agent LLM framework: planning -> analysis -> generation. **77% user preference**, **83% practical utility on PaperBench**, performance on par with author-released repos. *Benchmark paper.*
- [DeepCode: Open Agentic Coding](https://arxiv.org/abs/2512.07921) `NEW` (arXiv:2512.07921, 2025) -- **73.5% success** vs PaperCoder 51.1% (+22.4%). **Beats human experts** (75.9% vs 72.4%) on ICML 2024 paper reproduction. Agentic framework for Paper2Code, Text2Web, Text2Backend. *SOTA on PaperBench.*

**Tools**:

- **[PaperCoder / Paper2Code](https://github.com/going-doer/Paper2Code)** `OSS` -- (**2k+ stars**) Multi-agent framework: ML paper -> operational code. **77% user preference**, performance on par with author-released repos (no statistical difference vs Oracle). *L2 Partial.*
- **[DeepCode](https://github.com/HKUDS/DeepCode)** `OSS` `NEW` -- (**1k+ stars**) Open agentic coding for Paper2Code, Text2Web, Text2Backend. **73.5% success on PaperBench**, beats human experts (75.9% vs 72.4%). *L2 Partial.*
- **[Devin](https://devin.ai/)** -- Built by competitive programming champions (Cognition), backed by Founders Fund. **$4B valuation**. Autonomous agent with integrated dev environment, terminal, tests, browser. *L3 Conditional. Commercial.*

### Agentic Frameworks (Level 3)

**Papers**:

- [Automatic Prompt Engineer (APE)](https://www.promptingguide.ai/techniques/ape) (Zhou et al., 2022) -- ([GitHub](https://github.com/keirp/automatic_prompt_engineer)) Instruction generation as natural language synthesis, **black-box optimization**. Discovered better zero-shot CoT prompt than 'Let's think step by step' (**+3% improvement**). *Foundational paper for prompt optimization.*
- [Is It Time To Treat Prompts As Code?](https://arxiv.org/abs/2507.03620) `NEW` (arXiv:2507.03620, 2025) -- Multi-use case study for DSPy prompt optimization. Prompt evaluation criterion task: **46.2% -> 64.0% accuracy improvement (+17.8%)**. *Empirical study.*

**Tools**:

| Tool | Stars | Key Feature | Type |
|------|-------|-------------|------|
| **[LangChain](https://www.langchain.com/)** | [90k+](https://github.com/langchain-ai/langchain) | Most complete production stack | `OSS` |
| **[LangGraph](https://www.langchain.com/langgraph)** | [30k+](https://github.com/langchain-ai/langgraph) | Graph-based stateful agents | `OSS` |
| **[AutoGen](https://microsoft.github.io/autogen/)** | [30k+](https://github.com/microsoft/autogen) | Conversational multi-agent | `OSS` |
| **[CrewAI](https://www.crewai.com/)** | [25k+](https://github.com/joaomdmoura/crewAI) | Role-based, 40% Fortune 500 | `OSS` |
| **[DSPy](https://dspy.ai/)** | [15k+](https://github.com/stanfordnlp/dspy) | Programmatic prompt optimization | `OSS` |

**Tool Details**:

- **[LangChain](https://www.langchain.com/)** `OSS` -- ([GitHub](https://github.com/langchain-ai/langchain) | **90k+ stars**) Most complete stack for production agent workflows. Evolved from chaining library to full orchestration platform. Best-in-class observability with LangSmith. *L3 Conditional.*
- **[LangGraph](https://www.langchain.com/langgraph)** `OSS` -- ([GitHub](https://github.com/langchain-ai/langgraph) | **30k+ stars**) Modern production interface for LangChain. **Graph abstraction for stateful multi-agent apps** with branching, state machines, error handling, checkpointing. *L3 Conditional.*
- **[LangSmith](https://www.langchain.com/langsmith)** -- **Best-in-class observability** for agents. Traces every LLM call, tool invocation, chain step (latency, tokens, errors). Standard production runtime for debugging and monitoring. *L3 Conditional. Commercial.*
- **[CrewAI](https://www.crewai.com/)** `OSS` -- ([GitHub](https://github.com/joaomdmoura/crewAI) | **25k+ stars**) Role-based multi-agent workflows. **40% of Fortune 500** use CrewAI agents. Fastest prototyping (minutes). Structured memory with RAG. *L3 Conditional.*
- **[AutoGen](https://microsoft.github.io/autogen/)** `OSS` -- ([GitHub](https://github.com/microsoft/autogen) | **30k+ stars**) Microsoft's conversational multi-agent model. Agents communicate via natural language. Async task execution, human-in-the-loop oversight. *L3 Conditional.*
- **[DSPy](https://dspy.ai/)** `OSS` -- ([GitHub](https://github.com/stanfordnlp/dspy) | **15k+ stars**) Stanford framework (2023). Abstracts prompts into modular Python (Signatures, Modules). Programmatically creates and refines prompts. Up to **17.8% accuracy improvement**. *L3 Conditional.*

### Self-Driving Laboratories (Level 4-5)

**Papers**:

- [Self-Driving Laboratories for Chemistry and Materials Science](https://pubs.acs.org/doi/10.1021/acs.chemrev.4c00055) (Chemical Reviews, 2024) -- Comprehensive review: SDLs automate experimental workflows with autonomous planning, accelerating chemistry and materials discovery. Demonstrates **10x data collection speedup**. *Review paper. Venue: Chemical Reviews (IF 54.3).*
- [Autonomous 'self-driving' laboratories: a review of technology](https://royalsocietypublishing.org/rsos/article/12/7/250646/235354/) `NEW` (Royal Society Open Science, 2025) -- Most capable SDLs **automate entire scientific method**: hypothesis generation, experimental design, execution, data analysis, conclusion drawing, hypothesis updating. *Review paper.*
- [A Survey of AI Scientists](https://arxiv.org/abs/2510.23045) `NEW` (arXiv:2510.23045, 2025) -- Comprehensive survey of autonomous research agents and **hierarchical multi-agent architectures** with meta-orchestrators spawning domain specialists. *Survey paper.*

**Tools**:

| Tool | Autonomy | Domain | Key Result |
|------|----------|--------|------------|
| **[A-Lab](https://www.matter.toronto.edu/basic-content-page/ai-for-discovery-and-self-driving-labs)** | L5 | Materials | 71% success, 10x speedup |
| **[ChemCrow](https://pubs.acs.org/doi/10.1021/acs.accounts.2c00220)** | L4 | Chemistry | 18 expert tools |
| **[Coscientist](https://www.nature.com/articles/s44160-022-00231-0)** | L4 | Chemistry | <4 min protocol design |
| **[FutureHouse](https://www.futurehouse.org/)** | L4-5 | Biology | 4 specialized agents |
| **[Edison Scientific](https://edisonscientific.com/)** | L5 | Multi | $70M seed, 79.4% accuracy |
| **[Agent Laboratory](https://arxiv.org/abs/2501.04227)** | L4 | ML | 84% cost reduction |

**Tool Details**:

- **[A-Lab](https://www.matter.toronto.edu/basic-content-page/ai-for-discovery-and-self-driving-labs)** (Berkeley Lab) -- Fully autonomous solid-state synthesis. **41/58 DFT-predicted materials** synthesized in **17 days**, **71% success**, minimal human intervention. **10x data collection speedup**. Published in Nature. *L5 Full.*
- **[ChemCrow](https://pubs.acs.org/doi/10.1021/acs.accounts.2c00220)** -- LLM for chemical tasks with **18 expert-designed tools**. Finds molecules, plans synthetic routes, executes synthesis on cloud robotic platforms. *L4 High.*
- **[Coscientist](https://www.nature.com/articles/s44160-022-00231-0)** -- LLM-driven system for autonomous chemical experiment design, planning, robotic control. Successfully optimized **Nobel Prize-winning palladium-catalyzed cross-couplings** without human intervention (**<4 min** protocol design). Published in Nature. *L4 High.*
- **[AlabOS](https://www.oaepublish.com/articles/cs.2025.66)** `NEW` -- **Autonomous Laboratory Operating System**. Reconfigurable workflow management for autonomous materials labs. Orchestrates instruments, robots, and AI planners. *L4 High.*
- **[FutureHouse](https://www.futurehouse.org/)** -- Nonprofit AI-for-science lab (SF, launched Sep 2023). Building AI Scientist with world models. Specialized agents: **Crow, Falcon** (literature search), **Phoenix, Owl** (experimental design). *L4-5.*
- **[Edison Scientific](https://edisonscientific.com/)** `NEW` (FutureHouse spinout) -- **$70M seed at $250M valuation** (co-led Spark Capital, Triatomic Capital). Kosmos platform: reads 1500 papers, runs 42k lines of analysis. Beta users: **6 months work -> 1 day**, **79.4% conclusion accuracy**. *L5 Full. Commercial.*
- **[Agent Laboratory](https://arxiv.org/abs/2501.04227)** `NEW` -- o1-preview driven, **84% reduction in research expenses**. Supports literature review -> experiment -> report writing as end-to-end pipeline. *L4 High.*

### Code Quality & Review

**Tools**:

- **[CodeRabbit](https://coderabbit.ai/)** -- AI code review assistant. Reports AI-generated code has **1.7x more issues**, **2.74x more security vulnerabilities**. Achieves **4x faster PR merge times**. Essential for quality assurance in vibe coding workflows. *L2 Partial. Commercial.*

### Stage Summary

| Finding | Detail |
|---------|--------|
| Developer adoption | 92% of US developers use AI coding tools daily (2025) |
| Code generation | 41% of all code globally AI-generated, 256B lines in 2024 |
| Quality concerns | 1.7x more issues, 2.74x more security vulnerabilities (CodeRabbit 2025) |
| Productivity paradox | Developers felt 20% faster but took **19% longer** after debugging (Stack Overflow 2025) |
| Materials discovery | Years -> weeks compression with self-driving laboratories |
| Market | Lab automation $7.84B (2024) -> $14.78B (2034), CAGR 6.55% |

---

## Analysis & Interpretation

> Tools and papers for statistical analysis, visualization, results interpretation, and reproducibility. (18 items)

### Reproducibility Frameworks (Level 2)

**Papers**:

- [SciRep: Framework for Reproducibility](https://arxiv.org/abs/2503.07080) `NEW` (arXiv:2503.07080, 2025) -- Configuration, execution, packaging of computational experiments. **89% success vs 61%** for Docker/Singularity baselines. Addresses the reproducibility crisis in ML research. *Benchmark paper.*
- [ReproSchema](https://www.jmir.org/2025/1/e63343) `NEW` (JMIR, 2025) -- **Schema-centric survey design** for reproducible data collection. Reusable assessments, validation/conversion tools. Published in peer-reviewed medical informatics journal. *Venue: JMIR (IF 7.4).*

**Tools**:

| Tool | Stars | Focus | Type |
|------|-------|-------|------|
| **[Docker](https://www.docker.com/)** | [100k+](https://github.com/docker/docker) | Standard containerization | `OSS` |
| **[Nextflow](https://www.nextflow.io/)** | [25k+](https://github.com/nextflow-io/nextflow) | Bioinformatics pipelines | `OSS` |
| **[Snakemake](https://snakemake.github.io/)** | [20k+](https://github.com/snakemake/snakemake) | Declarative workflows | `OSS` |
| **[MLflow](https://mlflow.org/)** | [18k+](https://github.com/mlflow/mlflow) | MLOps platform | `OSS` |
| **[DVC](https://dvc.org/)** | [13k+](https://github.com/iterative/dvc) | Data version control | `OSS` |
| **[Apptainer](https://apptainer.org/)** | [10k+](https://github.com/apptainer/apptainer) | HPC containerization | `OSS` |
| **[Weights & Biases](https://wandb.ai/)** | [8k+](https://github.com/wandb/wandb) | ML experiment tracking | Freemium |

**Tool Details**:

- **[SciRep](https://arxiv.org/abs/2503.07080)** `NEW` -- **89% success rate** vs 61% for other tools. Automated configuration, execution, and packaging of computational experiments into reproducible artifacts. *L2 Partial.*
- **[Docker](https://www.docker.com/)** `OSS` -- ([GitHub](https://github.com/docker/docker) | **100k+ stars**) Industry-standard container platform for reproducible scientific computing environments. Foundation for most reproducibility workflows. *L2 Partial. Free.*
- **[Singularity / Apptainer](https://apptainer.org/)** `OSS` -- ([GitHub](https://github.com/apptainer/apptainer) | **10k+ stars**) **HPC-friendly** containerization for scientific workflows. Runs without root access on shared computing clusters. *L2 Partial. Free.*
- **[Snakemake](https://snakemake.github.io/)** `OSS` -- ([GitHub](https://github.com/snakemake/snakemake) | **20k+ stars**) **Declarative workflow management** for bioinformatics and data science. Python-based rule definitions, automatic parallelization. *L2 Partial. Free.*
- **[Nextflow](https://www.nextflow.io/)** `OSS` -- ([GitHub](https://github.com/nextflow-io/nextflow) | **25k+ stars**) **Scalable workflow orchestration** for bioinformatics pipelines. Supports Docker, Singularity, cloud execution. Active nf-core community. *L2 Partial. Free.*
- **[DVC (Data Version Control)](https://dvc.org/)** `OSS` -- ([GitHub](https://github.com/iterative/dvc) | **13k+ stars**) **Git-like version control** for datasets and ML models. Tracks data pipelines, enables experiment reproducibility. *L2 Partial. Free.*
- **[MLflow](https://mlflow.org/)** `OSS` -- ([GitHub](https://github.com/mlflow/mlflow) | **18k+ stars**) Open-source **MLOps platform**: experiment tracking, project packaging, model registry, deployment. *L2 Partial. Free.*
- **[Weights & Biases](https://wandb.ai/)** -- ([GitHub](https://github.com/wandb/wandb) | **8k+ stars**) ML experiment tracking, dataset versioning, model registry, hyperparameter sweeps. Industry-leading visualization. *L2 Partial. Freemium.*

### Stage Summary

| Finding | Detail |
|---------|--------|
| Reproducibility crisis | Only 19.5% of top ML conference papers (2024) provide code |
| SciRep advantage | 89% success vs 61% for Docker/Singularity |
| 2026 vision | Automated reproducibility as byproduct of AI-assisted research |

---

## Writing & Publishing

> Tools and papers for manuscript drafting, citation management, figure/table creation, and formatting. (10 items)

### Level 1 -- Grammar & Style

**Tools**:

- **[Grammarly](https://www.grammarly.com/)** -- Grammar, style, and tone suggestions. Widely used academic writing assistant with clarity improvements and plagiarism detection. *L1 Assist. Freemium.*
- **[QuillBot](https://quillbot.com/)** -- Paraphrasing and grammar correction. **Flow workspace** for end-to-end writing process. Reliable for rephrasing, checking grammar, summarizing. *L1 Assist. Freemium.*
- **[LanguageTool](https://languagetool.org/)** `OSS` -- Open-source grammar checker supporting **30+ languages**. Free alternative to commercial tools. Self-hostable for privacy. *L1 Assist. Free.*

### Level 2 -- Research Writing Assistants

**Tools**:

- **[Jenni AI](https://jenni.ai/)** -- Research and academic writing assistant. **Strong for citations**, outlines, academic formatting. Specialized for research-driven writing tasks with inline citation support. *L2 Partial. Commercial.*
- **[Yomu AI](https://www.yomu.ai/)** -- Excels at **paragraph development and PDF interaction**. Quick paper gist understanding for staying current with literature. *L2 Partial. Commercial.*
- **[SciSpace](https://scispace.com/)** (writing mode) -- **10M+ researchers** (2026). Upload PDF, chat with paper. Semantic search, automated summarization, reference management, AI copilot for writing. *L2 Partial. Freemium.*

### Level 5 -- Fully Automated Paper Generation

**Papers**:

- [The AI Scientist-v2](https://arxiv.org/abs/2504.08066) `NEW` (arXiv:2504.08066, 2025, Sakana AI) -- **First AI-generated paper accepted through peer review** (ICLR 2025 workshop). Removes human templates, uses progressive agentic tree search. *Milestone paper. Venue: ICLR Workshop.*

**Tools**:

- **[Sakana AI - AI Scientist](https://sakana.ai/ai-scientist/)** `OSS` -- ([GitHub](https://github.com/SakanaAI/AI-Scientist) | 5k+ stars) End-to-end paper generation: hypothesis -> code -> experiment -> LaTeX paper. First system to produce peer-review-accepted output. *L5 Full.*

### Stage Summary

| Finding | Detail |
|---------|--------|
| Gap | Level 3-4 tools missing (between Jenni AI L2 and AI Scientist-v2 L5) |
| Need | Automated draft generation with human refinement (RAG for review papers) |
| Milestone | AI Scientist-v2: first AI paper to exceed human acceptance threshold (2025) |

---

## Promotion & Dissemination

> Tools and papers for presentation slides, video/audio narration, social media, and homepage creation. (1 item -- **critical gap**)

### Level 1 -- Slide Templates

**Tools**:

- **Slide Templates** -- AI-suggested layouts and content generation for academic presentations. Basic automation of slide creation from paper content. *L1 Assist.*

### Stage Summary

| Finding | Detail |
|---------|--------|
| CRITICAL GAP | Promotion stage severely under-researched: 1 tool, 0 papers (**96% gap** vs Experiment 48 items) |
| Missing L2-3 | Automated slide generation, poster creation from papers |
| Missing L4-5 | Video narration, social media automation, conference talk generation |
| Potential additions | Beautiful.ai, Tome, Gamma (slides); Descript, Synthesia (video); Buffer, Hootsuite (social media) |

---

## Cross-Cutting Tools

> General-purpose platforms, multimodal AI, and infrastructure supporting multiple research stages.

### Research Platforms

**Papers**:

- [AI for Science 2025](https://www.nature.com/articles/d42473-025-00161-3) `NEW` (Nature, 2025) -- Interdisciplinary knowledge graphs, **RL-driven closed-loop systems**, interactive AI interfaces for scientific theory refinement. *Venue: Nature.*

**Tools**:

- **[NVIDIA BioNeMo](https://www.nvidia.com/en-us/clara/bionemo/)** -- LLM for biology (announced fall 2022). Major expansion to full open development platform. **Lab-in-a-loop workflows** for biology and drug discovery. RNA structure, molecular synthesis, toxicity prediction. *Commercial.*
- **[Eli Lilly x NVIDIA Partnership](https://nvidianews.nvidia.com/news/eli-lilly-nvidia-announce-generative-ai-for-drug-discovery)** -- **$1B 5-year strategic partnership**. AI co-innovation lab (SF Bay Area). Generative AI for drug discovery. *Partnership.*
- **NSF RAISE** -- Research in AI for Science and Engineering. **Democratizing AI access** for researchers through infrastructure and funding. *Government initiative.*
- **National AI Research Resources** -- NSF infrastructure for **democratizing AI access** to computational resources for the research community. *Government initiative.*

### Multimodal AI for Science

**Tools**:

- **[InternVL3-78B](https://github.com/OpenGVLab/InternVL)** `OSS` -- (**5k+ stars**) **72.2 MMMU** (open-source record). Vision-language model for multimodal scientific tasks including figure understanding and data extraction. *Open-source.*
- **[Qwen2.5-VL-32B-Instruct](https://github.com/QwenLM/Qwen2-VL)** `OSS` -- (**10k+ stars**) Vision-language instruction tuning (Alibaba). Strong multimodal understanding and generation capabilities. *Open-source.*
- **GLM-4.5V** -- **MoE architecture**, 3D-RoPE, **72.2 MMMU benchmark** (tied with InternVL3 for top score). Advanced vision-language capabilities. *Commercial.*
- **[MaCBench](https://www.nature.com/articles/s43588-025-00836-3)** `NEW` -- **Benchmark for chemistry/materials tasks**: data extraction, experimental execution, results interpretation. Published in Nature Computational Science. *Venue: Nature Computational Science.*

### Stage Summary

| Finding | Detail |
|---------|--------|
| Market size | Multimodal AI: $391B (2025) -> ~$2T (2030), CAGR 35.9% |
| Strategic investments | $1B+ partnerships emerging (NVIDIA-Eli Lilly) |
| Timeline compression | Discovery cycles compressed from years to weeks with AI + autonomous experimentation |

---

## Related Resources

### Meta-Research

- **[Vibe Researching as Wolf Coming](https://arxiv.org/abs/2602.22401)** `NEW` (arXiv:2602.22401, Feb 2026) -- Introduces **vibe researching concept** using scholar-skill (26-skill plugin for Claude Code, full pipeline idea -> submission). **Cognitive task framework**: codifiability x tacit knowledge. AI agents excel at speed, coverage, scaffolding but struggle with theoretical originality.
- **[VibeX 2026 Workshop](https://conf.researchr.org/home/ease-2026/vibex-2026)** -- **1st International Workshop on Vibe Coding and Vibe Researching** @ EASE 2026. Mixed audience: junior/senior researchers, practitioners. Focus on autonomous AI agents in SE research.

### Awesome Lists

- [Awesome Machine Learning](https://github.com/josephmisiti/awesome-machine-learning) -- Comprehensive ML resources across languages and frameworks
- [Awesome Deep Learning](https://github.com/ChristosChristofidis/awesome-deep-learning) -- Deep learning papers, tutorials, and resources
- [Awesome AI for Science](https://github.com/scibench/awesome-ai4s) -- AI applications in scientific research across domains

### Academic Conferences

| Conference | Relevance |
|------------|-----------|
| **ICLR** | AI Scientist-v2 first peer-reviewed AI paper (2025 workshop) |
| **EASE 2026** | Hosts VibeX 2026 workshop on vibe coding and vibe researching |
| **NeurIPS** | PaperBench benchmark papers, ML reproducibility initiatives |
| **ICML** | DeepCode benchmark (75.9% success on ICML 2024 reproduction) |

---

## Contributing

Contributions welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.

### How to Contribute

1. **Add a resource**: Submit a pull request with the new tool/paper. Include: title, URL, description (1-2 sentences), and classification (Stage, Level).
2. **Update existing entries**: Corrections, updated metrics (GitHub stars, user counts), or additional information.
3. **Report gaps**: Identify missing categories, tools, or papers via Issues.

### Quality Criteria

- **Papers**: Must be peer-reviewed, arXiv preprints, or published in reputable venues. Include arXiv ID or DOI.
- **Tools**: Must be actively maintained (not archived), have clear documentation, and be relevant to research automation.
- **Descriptions**: Concise (1-2 sentences), factual (no marketing language), include quantitative metrics when available.

### Classification Guide

| Level | Definition | Human Role | Example |
|-------|------------|------------|---------|
| **L1** (Assist) | AI suggests, human drives | Decides all logic | Code completion, grammar |
| **L2** (Partial) | AI executes specific subtasks | Defines task, validates | Automated screening |
| **L3** (Conditional) | AI handles workflows with checkpoints | Sets goals, approves | End-to-end literature review |
| **L4** (High) | AI handles extended workflows | Monitors for failures | Self-driving labs |
| **L5** (Full) | AI operates independently | None | AI Scientist: idea -> paper |

**Stages**: Survey, Ideation, Experiment, Analysis, Writing, Promotion

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full classification decision tree and formatting standards.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work. See [LICENSE](LICENSE) for details.

---

## Acknowledgments

This list was compiled through systematic web research (March 2026) covering academic databases (arXiv, Google Scholar, Semantic Scholar), GitHub repositories, and commercial platforms. The survey identified 107 resources (45 papers, 62 tools) across 10 research categories.

**Maintained by**: [OpenLAIR](https://github.com/OpenLAIR)
**Version**: 2.0 (2026-03-16)
**Last Updated**: March 2026

**Citation**: If you use this resource in your research, please cite:
```
@misc{awesome-vibe-researching,
  title={Awesome Vibe Researching: A Curated List of AI-Driven Research Automation Resources},
  author={VibeLab Contributors},
  year={2026},
  howpublished={\url{https://github.com/OpenLAIR/awesome-vibe-researching}},
  note={107 resources across 6 research stages and 5 autonomy levels}
}
```
