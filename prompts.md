# Instruction-Following Large Language Model (IF-LLM) Prompt Templates (*prompts.md*)
Collection of prompt templates for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO).

## File Header

**Purpose:** Define prompt templates for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO).

**Scope:** These prompt templates define IF-LLM processing of user instructions using the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO).

**Owner:** [Lance Hegland](mailto:lance.hegland@gmail.com)

**Version:** 2026-02-27T03:15Z LH in [if-llm-behavior-ontology](https://github.com/LHHegland/if-llm-behavior-ontology)

**Last Reviewed:** 2026-02-27T03:15Z — [Lance Hegland](mailto:lance.hegland@gmail.com)

**Changelog**
- 2026-02-27T03:15Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Created File + Added Prompt: Orchestrated Behavior Configuration and Task Knowledge Entries Creation


---

## Canonical Handles Index

Bulleted list of common human prompt template references mapped to canonical handles (i.e., IDs and namespaced tags).
- Prompt Template Entries → IF_LLM_BO_PROMPTS → [[IF_LLM_BO_PROMPTS:ROOT]]
- Orchestrated Behavior Configuration and Task Knowledge Entries Creation → IF_LLM_BO_PROMPTS.ORCH_CONFIG_ENTRY_CREATE → [[IF_LLM_BO_PROMPTS:ORCH_CONFIG_ENTRY_CREATE]]


---

## Prompt Template Entries
**ID:** IF_LLM_BO_PROMPTS
**Tag:** [[IF_LLM_BO_PROMPTS:ROOT]]

Collection of prompt templates for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO).

---


### Orchestrated Behavior Configuration and Task Knowledge Entries Creation
**ID:** IF_LLM_BO_PROMPTS.ORCH_CONFIG_ENTRY_CREATE
**Tag:** [[IF_LLM_BO_PROMPTS:ORCH_CONFIG_ENTRY_CREATE]]

Translate user-provided project input into copyable behavior configurations and task knowledge entries to be pasted into the appropriate knowledge files.

```
# Identity & Role
You are executing [[IF_LLM_BO_TASKS:ORCH_CONFIG_ENTRY_CREATE]].

# Input
- **Priorities:** [[PROCESSING_POLICIES:PRIORITIES]] 
- **Objectives**
  - 
  - 
  - 
- **Topics**
  - 
  - 
  - 
- **Knowledge Entries Owner:** [First Last Name](mailto:username@example.com)
- **Knowledge Entries Developer:** [First Last Name](mailto:username@example.com)
```


#### Metadata

**Owner:** [Lance Hegland](mailto:lance.hegland@gmail.com)

**Version:** 2026-02-27T03:15Z LH

**Last Reviewed:** 2026-02-27T03:15Z [Lance Hegland](mailto:lance.hegland@gmail.com)

**Changelog** 
  - 2026-02-27T03:15Z [Lance Hegland](mailto:lance.hegland@gmail.com): Added Prompt Template

---
