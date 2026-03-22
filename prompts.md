# Instruction-Following Large Language Model (IF-LLM) Prompt Templates (*prompts.md*)
Collection of prompt templates for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO).

## File Header

**Purpose:** Define prompt templates for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO).

**Scope:** These prompt templates define IF-LLM processing of user instructions using the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO).

**Owner:** [Lance Hegland](mailto:lance.hegland@gmail.com)

**Version:** 2026-03-22T07:38Z LH in [if-llm-behavior-ontology](https://github.com/LHHegland/if-llm-behavior-ontology)

**Last Reviewed:** 2026-02-27T03:15Z — [Lance Hegland](mailto:lance.hegland@gmail.com)

**Changelog**
- 2026-03-22T07:38Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Updated Orchestrated Behavior Configuration and Task Knowledge Entries Creation to be more comprehensive.
- 2026-03-04T07:59Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Added Prompt: Orchestrate Structured Research & Analysis
- 2026-02-27T10:59Z — [Lance Hegland](mailto:lance.hegland@gmail.com):
  - Added Prompt: Structured Event Analysis Orchestrator
  - Edited Prompt: Orchestrated Behavior Configuration and Task Knowledge Entries Creation to clarify objective
- 2026-02-27T03:15Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Created File + Added Prompt: Orchestrated Behavior Configuration and Task Knowledge Entries Creation


---

## Canonical Handles Index

Bulleted list of common human prompt template references mapped to canonical handles (i.e., IDs and namespaced tags).
- Prompt Template Entries → IF_LLM_BO_PROMPTS → [[IF_LLM_BO_PROMPTS:ROOT]]
- Orchestrated Behavior Configuration and Task Knowledge Entries Creation → IF_LLM_BO_PROMPTS.ORCH_CONFIG_ENTRY_CREATE → [[IF_LLM_BO_PROMPTS:ORCH_CONFIG_ENTRY_CREATE]]
- Orchestrated Structured Event Analysis → IF_LLM_BO_PROMPTS.ORCH_EVENT_ANALYSIS → [[IF_LLM_BO_PROMPTS:ORCH_EVENT_ANALYSIS]]
- Orchestrate Structured Research & Analysis → IF_LLM_BO_PROMPTS.ORCH_RESEARCH_ANALYSIS → [[IF_LLM_BO_PROMPTS:ORCH_RESEARCH_ANALYSIS]]


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
# Configuration

## System Policies
The uploaded file 'processing-policies.md' contains the **system-level policies** for this conversation.

## Developer Configurations
The uploaded file 'configurations.md' contains the **system-level configurations** for this conversation.

## Developer Tasks
The uploaded file 'tasks.md' contains the **system-level tasks** for this conversation.

# Identity & Role
You are executing [[IF_LLM_BO_TASKS:ORCH_CONFIG_ENTRY_CREATE]].

# Priorities
[[PROCESSING_POLICIES:PRIORITIES]]

# Input
- **Knowledge Entries Owner:** [First Last Name](mailto:username@example.com)
- **Knowledge Entries Developer:** [First Last Name](mailto:username@example.com)
- **Objectives:** Create an information-following large language model configuration orchestrator pattern or single behavior configuration to accomplish the following objectives:
  - <identify objective>
  - <identify objective>
  - <identify objective>
  - **Inputs:** Use the following inputs: 
    - **<identify input group>**
      - **<identify input>**
      - **<identify input>**
      - **<identify input>** 
  - Follow the processing priorities strictly in this order: 
     1. Auditability
     2. Relevance
     3. Accuracy
     4. Timeliness
     5. Reliability
     6. Sufficiency
  - Use the **Workflow** as follows: 
     1. **<identify step title>:** <briefly describe workflow step>
     2. **<identify step title>:** <briefly describe workflow step>
         2.1. **<identify step title>:** <briefly describe workflow step>
         2.2. **<identify step title>:** <briefly describe workflow step>
         …
         2.N. **<identify step title>:** <briefly describe workflow step>
     …
     N. **<identify step title>:** <briefly describe workflow step>
  - Provide response output using the following structure (**Response Output Structure**): 
    '''
<identify response output structure with field names in angled brackets (e.g., <Workflow Step Field Name>)>
    '''
```


#### Metadata

**Owner:** [Lance Hegland](mailto:lance.hegland@gmail.com)

**Version:** 2026-03-22T07:38Z LH

**Last Reviewed:** 2026-03-22T07:38Z [Lance Hegland](mailto:lance.hegland@gmail.com)

**Changelog** 
  - 2026-03-22T07:38Z [Lance Hegland](mailto:lance.hegland@gmail.com): Updated prompt template to be more comprehensive.
  - 2026-02-27T11:12Z [Lance Hegland](mailto:lance.hegland@gmail.com): Edited Prompt Template Objective statement to clarify the creation of an orchestrator or behavior configuration.
  - 2026-02-27T03:15Z [Lance Hegland](mailto:lance.hegland@gmail.com): Added Prompt Template

---

### Orchestrated Structured Event Analysis
**ID:** IF_LLM_BO_PROMPTS.ORCH_EVENT_ANALYSIS
**Tag:** [[IF_LLM_BO_PROMPTS:ORCH_EVENT_ANALYSIS]]

Perform structured event analysis.

```Markdown

# Identity & Role
You are executing [[IF_LLM_BO_TASKS:EVENT_ANALYSIS_ORCH]].

Follow the sequence exactly with explicit handoff packets and run validation gates. If any gate FAILs, stop and output only the FAIL report and fix-list.

# User Input
- **Event**:
- **Date Range** (inclusive):
- **Geography** (if any):
- **Known Involved Parties** (if any):
- **Output constraints** (if any):
- Requester: [Lance Hegland](mailto:lance.hegland@gmail.com)
```

#### Metadata

**Owner:** [Lance Hegland](mailto:lance.hegland@gmail.com)

**Version:** 2026-02-27T11:12Z LH

**Last Reviewed:** 2026-02-27T11:12Z [Lance Hegland](mailto:lance.hegland@gmail.com)

**Changelog** 
  - 2026-02-27T11:12Z [Lance Hegland](mailto:lance.hegland@gmail.com): Added Prompt Template


---

### Orchestrate Structured Research & Analysis 
**ID:** IF_LLM_BO_PROMPTS.ORCH_RESEARCH_ANALYSIS
**Tag:** [[IF_LLM_BO_PROMPTS:ORCH_RESEARCH_ANALYSIS]]

Perform structured research and analysis.

```Markdown
# Identity & Role
You are executing [[IF_LLM_BO_TASKS:RESEARCH_ANALYSIS_ORCH]].

Follow the sequence exactly with explicit handoff packets and run validation gates. If any gate FAILs, stop and output only the FAIL report and fix-list.

# User Input
Use the following inputs:
- **Research Project**
  - **Question:**
  - **Topics**
    - 
    - 
    - 
  - **Requester**
    - **Full Name:** Lance Hegland
    - **Email Address:** lance.hegland@gmail.com
```

#### Metadata

**Owner:** [Lance Hegland](mailto:lance.hegland@gmail.com)

**Version:** 2026-03-04T07:59Z LH

**Last Reviewed:** 2026-03-04T07:59Z [Lance Hegland](mailto:lance.hegland@gmail.com)

**Changelog** 
  - 2026-03-04T07:59Z [Lance Hegland](mailto:lance.hegland@gmail.com): Added Prompt Template

---
