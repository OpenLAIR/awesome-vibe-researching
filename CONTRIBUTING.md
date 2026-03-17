# Contributing to Awesome Vibe Researching

Thank you for your interest in contributing to Awesome Vibe Researching! This document provides guidelines for contributing to this curated list.

## Table of Contents

- [How to Contribute](#how-to-contribute)
- [Contribution Guidelines](#contribution-guidelines)
- [Quality Standards](#quality-standards)
- [Classification Guide](#classification-guide)
- [Pull Request Process](#pull-request-process)
- [Issue Guidelines](#issue-guidelines)

## How to Contribute

There are several ways to contribute:

1. **Add a new resource** (paper or tool)
2. **Update existing entries** (corrections, new metrics, additional information)
3. **Report gaps** (missing categories, tools, or papers)
4. **Improve documentation** (clarify descriptions, fix typos, enhance formatting)

## Contribution Guidelines

### Adding a New Resource

**Before submitting**, please check:
- [ ] The resource is not already listed
- [ ] The resource is relevant to AI-driven research automation (vibe researching)
- [ ] The resource meets our [Quality Standards](#quality-standards)
- [ ] You have classified the resource correctly (see [Classification Guide](#classification-guide))

### What to Include

**For Papers**:
```markdown
- [Paper Title](URL) `NEW` (arXiv:ID or Venue, Date) -- Description with **key metrics in bold**. *Paper type. Venue: Name (IF X.X).*
```

Required information:
- Full title with direct URL
- `NEW` tag if published 2025-2026
- arXiv ID (if applicable) or publication venue with impact factor for top journals
- Publication date (month/year or year)
- Brief description highlighting main contribution
- **Quantitative findings** (e.g., "89% success rate", "10x speedup") when available
- Paper type in italics (e.g., *Survey paper*, *Empirical study*, *Benchmark paper*)

**For Tools**:
```markdown
- **[Tool Name](URL)** `OSS` -- ([GitHub](repo-url) | **stars**) Description with **quantitative metrics in bold**. *Autonomy level. Pricing model.*
```

Required information:
- Tool name (bold) with official website URL
- Quality tags: `OSS` (open-source), `NEW` (2025-2026), `FREE` (free to use)
- GitHub repository link (if open-source) with star count
- Brief description (1-2 sentences) of main functionality
- **Quantitative metrics** (e.g., "20M users", "80% time savings", "4.9/5 rating") when available
- Autonomy level classification in italics (e.g., *L1 Assist*, *L3 Conditional*)
- Pricing model (Free, Open-source, Freemium, Commercial)

### Where to Add

1. Determine the **Research Stage** (Survey, Ideation, Experiment, Analysis, Writing, Promotion)
2. Determine the **Autonomy Level** (L1-L5, see [Classification Guide](#classification-guide))
3. Add to the appropriate section in README.md
4. Maintain alphabetical order within subsections (Papers first, then Tools)

## Quality Standards

### Papers

**Must meet at least one**:
- Peer-reviewed publication in reputable venue (conference, journal)
- arXiv preprint with substantial community engagement (citations, implementations)
- Technical report from recognized research institution

**Quality indicators**:
- Clear methodology and reproducible results
- Quantitative evaluation (benchmarks, user studies, performance metrics)
- Open-source implementations (preferred but not required)
- Relevant to AI-assisted research workflows

**Exclusions**:
- Blog posts or non-peer-reviewed content (unless exceptional)
- Marketing materials or promotional content
- Duplicate or highly overlapping work (keep the most comprehensive)

### Tools

**Must meet**:
- Actively maintained (last update within 12 months for open-source, currently operational for commercial)
- Clear documentation (README, docs, or website)
- Relevant to research automation (not general-purpose AI tools unless widely used in research)

**Quality indicators**:
- GitHub stars (for open-source): 1k+ preferred, 500+ acceptable
- User base (for commercial): substantial adoption (10k+ users) or industry backing
- Performance metrics or user testimonials
- Open-source preferred but high-quality commercial tools accepted

**Exclusions**:
- Abandoned projects (archived repositories, inactive >12 months)
- Vaporware (announced but not released)
- Tools with no clear differentiation from existing entries
- Purely promotional or low-quality tools

### Descriptions

**Best practices**:
- Concise (1-2 sentences, max 3 for complex tools)
- Factual (no marketing language like "revolutionary", "game-changing")
- Quantitative (include metrics: "80% time savings", not "significant improvement")
- Specific (mention key features, not vague benefits)
- Active voice (e.g., "Automates literature screening" not "Can be used for literature screening")

**Examples of good descriptions**:
- ✅ "Multi-agent framework for ML paper → code generation, 77% user preference, performance on par with author-released repositories"
- ✅ "Fully autonomous solid-state synthesis, 41/58 materials in 17 days, 71% success rate, 10× data collection speedup"
- ❌ "An amazing tool that revolutionizes research"
- ❌ "Helps researchers work faster and better"

## Classification Guide

### Research Stages

| Stage | Scope | Examples |
|-------|-------|----------|
| **Survey** | Literature search, systematic review, knowledge extraction | Elicit, Rayyan, Consensus |
| **Ideation** | Research question formulation, hypothesis generation | AI Scientist (idea generation component) |
| **Experiment** | Protocol design, code implementation, lab execution | GitHub Copilot, A-Lab, ChemCrow |
| **Analysis** | Statistical analysis, visualization, reproducibility | Docker, MLflow, Weights & Biases |
| **Writing** | Manuscript drafting, citation management, formatting | Grammarly, Jenni AI, QuillBot |
| **Promotion** | Presentation slides, video/audio, social media | *Critical gap identified* |

### Autonomy Levels

| Level | Definition | Human Role | AI Role | Examples |
|-------|------------|------------|---------|----------|
| **L1 - Assist** | AI suggests, human drives all decisions | Decides all logic, reviews every suggestion | Provides inline suggestions | GitHub Copilot tab completion, Grammarly grammar hints |
| **L2 - Partial** | AI autonomously handles specific subtasks | Defines task, validates output | Executes specific task end-to-end | Rayyan automated screening, Elicit data extraction |
| **L3 - Conditional** | AI handles full workflows, human checkpoints required | Sets goals, approves at checkpoints, handles exceptions | Executes multi-step workflows between checkpoints | Paperguide (systematic review with validation), LangChain agents |
| **L4 - High** | AI handles extended workflows, human for exceptions only | Defines research question, monitors for failures | Handles normal operation autonomously, alerts for edge cases | A-Lab (self-driving lab with oversight), Agent Laboratory |
| **L5 - Full** | AI operates independently, no human intervention | None (may be reviewer/consumer) | Full autonomy from hypothesis to publication | AI Scientist-v2 (idea → code → experiment → paper) |

**Decision tree for classification**:

```
Q1: Does AI replace human for entire task?
├─ No → Q2: Does AI suggest/assist within human-driven workflow?
│  ├─ Yes → L1 (Assist)
│  └─ No → L0 (out of scope)
└─ Yes → Q3: How many stages/checkpoints?
   ├─ Single subtask → L2 (Partial)
   ├─ Multi-step workflow with required checkpoints → L3 (Conditional)
   ├─ Extended workflow, human only for exceptions → L4 (High)
   └─ End-to-end with no human intervention → L5 (Full)
```

**Critical distinction (L1 vs L2)**:
- **L1**: AI suggests, but human must approve each suggestion (e.g., Copilot tab completion)
- **L2**: AI autonomously executes a complete subtask (e.g., Rayyan screens 1000 papers → outputs relevant subset)

### Tags

Add tags when applicable (not displayed in README, but used for internal classification):
- **Modality**: `computational`, `experimental`, `theoretical`, `data-science`, `literature`
- **Domain**: `chemistry`, `biology`, `materials`, `CS`, `physics`, `neuroscience`, `general`
- **Open Source**: `open-source`, `freemium`, `commercial`, `nonprofit`
- **Maturity**: `prototype`, `beta`, `production`, `research-tool`
- **Key Features**: `multi-agent`, `agentic`, `workflow`, `autonomous`, `collaborative`

## Pull Request Process

### 1. Fork and Clone

```bash
git clone https://github.com/your-username/awesome-vibe-researching.git
cd awesome-vibe-researching
```

### 2. Create a Branch

```bash
git checkout -b add-[tool-name]
# or
git checkout -b update-[section-name]
```

### 3. Make Changes

- Add your resource to the appropriate section in `README.md`
- Follow the formatting standards (see examples above)
- Ensure alphabetical order within subsections
- Check for typos and broken links

### 4. Commit

```bash
git add README.md
git commit -m "Add [Tool Name]: Brief description"
# or
git commit -m "Update [Section]: What changed"
```

Commit message format:
- `Add [Resource Name]: Brief description`
- `Update [Resource Name]: What changed`
- `Fix: Describe the fix`
- `Docs: Documentation improvement`

### 5. Push and Create Pull Request

```bash
git push origin add-[tool-name]
```

Then create a Pull Request with:
- **Title**: Clear, concise description of what you're adding/changing
- **Description**:
  - Why this resource belongs in the list
  - Classification (Stage, Level)
  - Any quantitative metrics or evidence of quality
  - Link to the resource

### 6. Review Process

- Maintainers will review within 7 days
- May request changes (clarifications, better descriptions, different classification)
- Once approved, your PR will be merged and you'll be credited as a contributor

## Issue Guidelines

### Reporting a Gap

Use the "Gap Report" template:

```markdown
**Category**: [e.g., Ideation, Promotion]
**Autonomy Level**: [e.g., L3, L4-L5]
**Description**: [What's missing and why it's important]
**Potential Resources**: [List any tools/papers you're aware of, if any]
```

### Suggesting Improvements

Use the "Improvement Suggestion" template:

```markdown
**Section**: [Which part of the README]
**Current State**: [What's there now]
**Proposed Change**: [What you suggest]
**Rationale**: [Why this improves the list]
```

### Reporting Errors

Use the "Error Report" template:

```markdown
**Location**: [Section and line number, if applicable]
**Error Type**: [Broken link, incorrect metric, typo, etc.]
**Details**: [Describe the error]
**Correction**: [Provide correct information, if known]
```

## Recognition

Contributors will be:
- Listed in the repository contributors page (automatic via GitHub)
- Acknowledged in release notes for significant contributions
- Credited in the Acknowledgments section for major additions (10+ resources)

## Questions?

If you're unsure about:
- **Classification**: Open an issue asking "How should I classify [Resource Name]?"
- **Quality**: If borderline, submit a PR and explain your reasoning - maintainers will discuss
- **Formatting**: Look at existing entries as examples, or ask in an issue

### Quality Tags

When adding entries, use these inline tags where applicable:

| Tag | Meaning | When to use |
|-----|---------|-------------|
| `NEW` | Published/released 2025-2026 | Recent papers or tools |
| `OSS` | Open-source | Tools with public source code |
| `FREE` | Free to use | Tools with no cost for basic usage |

## Code of Conduct

Please note that this project follows the [Contributor Covenant Code of Conduct](CODE_OF_CONDUCT.md). By participating, you agree to uphold this code.

---

## Quick Checklist

Before submitting a PR:
- [ ] Resource is relevant to AI-driven research automation
- [ ] Not already listed in the README
- [ ] Meets quality standards (see above)
- [ ] Correctly classified (Stage + Level)
- [ ] Description is concise, factual, and includes quantitative metrics
- [ ] Links are working
- [ ] Formatting follows existing entries
- [ ] Alphabetically ordered within subsection
- [ ] Commit message follows format guidelines

Thank you for contributing to Awesome Vibe Researching! 🎉
