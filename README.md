# Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) (*README.md*)

**PURPOSE:** **Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is a lightweight semantic scaffolding system for structuring knowledge files that guide instruction-following large language models (IF-LLMs) toward accurate, reliable, relevant, and practical outcomes. It emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts.


## **Table of Contents**

- [Features](#features)
- [Background](#background)
  - [What is an Instruction-Following Large Language Model (IF-LLM)?](!!!TODO!!!)
  - [Challenges and Proposed Solution](!!!TODO!!!)
- [Known Issues](#known-issues)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Project Notes](#if-llm-bo-project-notes)
  - [Foundations](#foundations)
    - [Assumptions](#assumptions)
    - [Decision-Making Information Quality Criteria (Priorities)](#decision-making-information-quality-criteria-priorities)
    - [Common IF-LLMs](!!!TODO!!!)
    - [Common IF-LLM Elements: Instructions and Context](!!!TODO!!!)
    - [Common IF-LLM Failure Modes](#common-if-llm-failure-modes)
    - [Common IF-LLM Failure Mitigation Strategies](#common-if-llm-failure-mitigation-strategies)
  - [Purpose](#purpose)
  - [Objectives](#objectives)
  - [Governance, Policies, Rules](#governance-policies-and-rules)
  - [Prompt Templates, Orchestrators, Configurations](#prompt-templates-orchestrators-configurations)
- [Appendices](#appendices)
- [Roadmap](#roadmap)
- [Authors](#authors)
- [License](#license)
- [Index](#document-index)





NOT YET ORGANIZED
TODO: Review then integrate or eliminate

---


### Instruction Elements (Scaffolding)

The scaffolding so far is as follows:
- **ontology:** *serves as the semantic root for all model behavior.* The ontology defines the canonical concepts, relationships, and behavior guidance that constitute the instruction-following LLM’s shared semantic foundation.
  - **meta:** *provides cross-cutting rules and scaffolding about the ontology itself.* Meta captures naming rules, modeling conventions, global decision policies, ontology versioning, glossaries of meta-terms, and core primitives reused across domains.
  - **tasks:** *defines what the model is expected to do and how success is judged.* Tasks specify objectives, priorities, success criteria, unacceptable outputs, scope boundaries, and workflows, providing explicit guidance on intended outcomes and failure avoidance.
  - **domains:** *constrain what knowledge space the model may operate within.* Domains describe relevant elements and relationships, in-scope and out-of-scope topics, geographic or contextual boundaries, and known uncertainty zones to reduce ambiguity and hallucination.
  - **experts:** *shape how the model reasons about the task.* Experts encode reasoning frameworks, heuristics, and analytical lenses that guide interpretation, tradeoffs, and decision-making without prescribing exact answers.
  - **structures:** *control how outputs are organized and validated.* Structures define required sections, ordering, mandatory and conditional fields, and formatting rules to ensure consistency, completeness, and evaluability of responses.
  - **personas:** *govern how the model communicates.* Personas specify tone, voice, formality, conciseness, and stylistic constraints, aligning outputs with audience expectations without altering underlying task logic.
  - **examples:** *demonstrate acceptable patterns of behavior.* Examples pair representative prompts with corresponding results to illustrate desired reasoning, structure, and boundary handling in concrete terms.
  - **configs:** *compose a complete behavioral profile.* Configurations bind tasks, domains, experts, structures, personas, and examples into a reusable, explicit behavioral setup that enables consistent instruction-following across contexts.


---


### Knowledge Entry Anatomy

- Common Human Reference
- Canonical Handles
  - IDs
  - Namespaced Tags
- Alias Tags
- Definition Summary / Purpose
- Content Specific Fields

### Knowledge File Anatomy

#### File Header

#### Indexes
- Canonical Handles Index
- Aliases Index

#### Knowledge Header

##### Knowledge Entries



### Knowledge Entry Types

#### Meta Entries

## Processing Policies
### Enforcement & Degradation Handling
### Instruction Precedence
### Safety, Privacy, and Refusals
### Context
#### Context & Ambiguity Handling
#### Knowledge & Information Hierarchy
### Hallucination & Fabrication
### Defaults
#### Tasks
##### Priorities
##### Identity
##### Audience
##### Success Criteria (Quality Bar)
#### Domains
##### Deterministic Defaults (US)
#### Experts
##### Reasoning & Uncertainty
#### Tools
##### Tool Usage
##### Tool Constraints (Negative Rules)
#### Structures
##### Output Structure Sections
##### Output Structure Flexibility

### Priorities
TODO: Outline priorities

### Knowledge
TODO: Outline knowledge, especially types and significance toward objectives and priorities.

### Work in Progress
this IF-LLM Behavior Ontology (IFLLMBO) is intended to be a lightweight, LLM-legible semantic scaffolding system for organizing knowledge files and entries that ensure tools are more likely to offer results that are more accurate, reliable, relevant, specific, clear, practical, fair, and efficient.

It prioritizes human-readable structure, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent reasoning and behavior across AI-assisted workflows.

Ideation and Exploration

Clarify Prompt Parameter Breakdown
it's
Meta Knowledge File Policies Processing Policies Tasks Objective Priorities Workflow (Steps) Domains Elements (e.g., knowledge, ability, or skill) Relationships with Other Elements Experts Summary Scope Reasoning Approach and Core Priorities (Ranked) Reasoning Style Judgment Norms Risk Tolerance Evidence Threshold Decision Posture Uncertainty Handling Ethical / Compliance Sensitivity Interaction Guidelines Intended Use Cases Non-Goals Tools (not a knowledge file but a feature of the GPT) Structures Personas



The scaffolding so far is as follows:
- **ontology:** *serves as the semantic root for all model behavior.* The ontology defines the canonical concepts, relationships, and behavior guidance that constitute the instruction-following LLM’s shared semantic foundation.
  - **[knowledge files](#knowledge-files)**
    - **[policies](#policies):** *provides cross-cutting rules and scaffolding about the ontology itself.*
      - **[governance](#policies-governance):** other policies requiring human responsibility.
      - **[knowledge entry](#policies-knowledge-entry):** naming rules, modeling conventions, versioning, and core primitives.
      - **[processing](#policies-processing):** global decision policies.
    - **[prompt templates](#prompt-templates):** *offer reusable, copyable prompt pattern templates ensuring more consistent use and improved results.*
      - **[tasks](#task):** *defines what the model is expected to do and how success is judged.* Tasks specify objectives, priorities, success criteria, unacceptable outputs, scope boundaries, and workflows, providing explicit guidance on intended outcomes and failure avoidance.
      - **[domains](#domains-1):** *constrain what knowledge space the model may operate within.* Domains describe relevant elements and relationships, in-scope and out-of-scope topics, geographic or contextual boundaries, and known uncertainty zones to reduce ambiguity and hallucination.
      - **[reasoning](#reasoning):** *shape how the model reasons about the task.* Reasoning encode reasoning frameworks, heuristics, and analytical lenses that guide interpretation, tradeoffs, and decision-making without prescribing exact answers.
      - **[structures](#structure):** *control how outputs are organized and validated.* Structures define required sections, ordering, mandatory and conditional fields, and formatting rules to ensure consistency, completeness, and evaluability of responses.
      - **[personas](#persona):** *govern how the model communicates.* Personas specify tone, voice, formality, conciseness, and stylistic constraints, aligning outputs with audience expectations without altering underlying task logic.
      - **[examples](#examples):** *demonstrate acceptable patterns of behavior.* Examples pair representative prompts with corresponding results to illustrate desired reasoning, structure, and boundary handling in concrete terms.
    - **[configurations](#configurations):** *compose a complete behavioral profile.* Configurations bind tasks, domains, reasoning, structures, personas, and examples into a reusable, explicit behavioral setup that enables consistent instruction-following across contexts.
    - **[orchestrators](#orchestrators):** TODO *orchestrates activity across multiple configurations.* Orchestrators coordinate tasks among multiple configurations with unique tasks, domains, reasoning, structures, personas, and examples into a reusable, explicit behavioral setup that enables consistent instruction-following across contexts. Orchestrators validate results between each configuration to improve results.


## END NOT YET ORGANIZED


---


---


## **Features**

TODO


---


## **Background**

TODO: Verify hyperlinks


### What is an Instruction-Following Large Language Model (IF-LLM)?

#### A Well-Trained Assistant

Imagine you’re working with a really attentive assistant:

* You say: *“Write a polite email asking for a refund.”*
* Or: *“Explain photosynthesis like I’m in 5th grade.”*
* Or even: *“Give me a grocery list for a healthy week on a budget.”*

A good assistant listens carefully, understands what you mean, and responds in a way that matches your request.

An **instruction-following large language model (IF-LLM) does something very similar**, but using artificial intelligence.


---

#### A Simple Analogy

Think of an IF-LLM like:

> A giant library + a helpful librarian
> who listens to your question and quickly pulls together an answer in your preferred style.


---

#### **“Language Model” = A Pattern Learner for Words**

An IF-LLM is trained on massive amounts of text—books, websites, conversations—so it learns:

* How people use language
* How ideas are explained
* What answers typically look like

It doesn’t “think” like a human, but it’s very good at recognizing patterns in language.


---

#### **“Instruction-Following” = It Listens to What You Ask**

What makes this type of model special is that it’s trained to:

* Understand **instructions or requests**
* Adjust its response based on **your goal, tone, and context**

So instead of just predicting text, it tries to **do what you asked it to do**.


---

#### Real-Life Examples

Here’s how people across different communities might use an IF-LLM:

* **Job seekers:** “Help me rewrite my resume for a warehouse job.”
* **Parents:** “Explain algebra homework in simple terms.”
* **Small business owners:** “Write a social media post promoting my food truck.”
* **Healthcare workers:** “Summarize this patient info in plain language.”

In each case, the model adapts to the instruction.


---

#### Why It Matters

From an education and workforce perspective, IF-LLMs can:

* Support **learning at any age or level**
* Help people **communicate more effectively**
* Save time on everyday tasks (writing, planning, explaining)
* Act like an **on-demand tutor or assistant**


---

#### Important to Know

Even though IF-LLMs are powerful:

* They **don’t truly understand** things like humans do
* They can sometimes give **incorrect or outdated information**
* They work best when **your instructions are clear**


 ### Current Challenges and Proposed Solutions

Currently, [popular instruction-following large language models (IF-LLMs)](#commonly-used-if-llms) have demonstrated [various vulnerabilities](#common-if-llm-failure-modes), especially related to producing results that satisfy [commonly-accepted decision-making information quality criteria](#decision-making-information-quality-criteria-priorities).

After [exploring the circumstances and challenges](#assumptions), it seems that more intentionally and consistently using governance, information policies, processing rules, plus reusable instructions and context (information) for commonly needed requests could reduce the likelihood of undesirable results.

Therefore, the **goal of the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is to build a lightweight semantic scaffolding system for organizing instructions and context in structured data files to better guide IF-LLMs toward responses that satisfy common decision-making information quality criteria. The scaffolding should build from [foundational IF-LLM elements](!!!TODO!!!). The scaffolding must emphasize human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts; a practical, not perfect, ontology.

Failure modes will very likely evolve over time, requiring instructions and context to be routinely tested, their results evaluated, instructions and context subsequently refined periodically. Also, this scaffolding enables system architects and solution developers to organize instructions and context for more complex objectives to empower greater efficiency, consistency, and auditability.


---


## **Known Issues**

TODO


---


## **Requirements**

TODO

1. Familiarity and access to instruction-following LLM like [ChatGPT](https://chatgpt.com/)
1. Familiarity and access to [GitHub](https://github.com/)
1. Agree to the [Creative Commons Attribution Share Alike 4.0 International License (CC-BY-SA-4.0)](LICENSE.txt)
1. Review [README](README.md)


---


## **Installation**

TODO

1. Review [README](README.md).
1. Perform the necessary actions to satisfy [minimum requirements](#requirements).
1. From your local projects directory, copy the entire remote GitHub repository into your local project directory.


---


## **Configuration**

TODO


---


## **Usage**

TODO

1. Perform the necessary actions to complete the [installation](#installation).

**TIPS:** Refer to the following documentation and tools to efficiently develop prompts delivering accurate, reliable, relevant, specific, clear, practical, fair, and efficient results for your users:
- [ChatGPT Prompt Engineering Best Practices](https://help.openai.com/en/articles/10032626-prompt-engineering-best-practices-for-chatgpt)
- [How do I create a good prompt for an AI model?](https://help.openai.com/en/articles/4936848-how-do-i-create-a-good-prompt-for-an-ai-model)
- [OpenAI Prompting Guide](https://platform.openai.com/docs/guides/prompting)
- [OpenAI Prompt Examples)](https://platform.openai.com/docs/examples)
- [OpenAI Prompt Optimizer Tool](https://platform.openai.com/chat/edit?optimize=true)
- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
- [OpenAI Reasoning Best Practices](https://platform.openai.com/docs/guides/reasoning-best-practices)
- [OpenAI GPT-5 Prompting Guide](https://cookbook.openai.com/examples/gpt-5/gpt-5_prompting_guide)


---


## **IF-LLM-BO Project Notes**
The following sections contain notes related to the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project.


---


### Foundations
The following sections describe the foundations grounding the IF-LLM-BO project.


---


#### Assumptions

TO DO: Create Summary

Below is a summary of the underlying assumptions for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project.  More detailed information about these assumptions can be found in the [Appendix: Assumptions](#appendix-assumptions).

There is credible and sufficient evidence that instruction-following large language models (IF-LLMs) produce a finite number of [common failure modes](#common-if-llm-failure-modes).

IF-LLMs produce results that are likely considered when making future decisions. Therefore, the results they produce should meet [well-defined quality standards](#decision-making-information-quality-criteria-priorities).


---


#### Decision-Making Information Quality Criteria (Priorities)

Instruction-Following Large Language Models (IF-LLMs) are often used to generate information that can influence real-world decisions. Because of this, the information they produce should meet clear and well-defined quality standards. Therefore, IF-LLMs should prioritize these criteria according to their ranked importance. Any trade-offs should be disclosed to users. Meaning, the instructions and context guiding IF-LLMs — especially the system-level policies — should reflect and reinforce these priorities.

The criteria listed below identify the key characteristics that information should have in order to reliably support decision-making. Each definition is written to answer a practical question: *"What does this mean for everyday decision-making?"*

 1. **Auditability:** source of information, how information was changed, and who handled information can be identified.
 2. **Relevance:** information matters for the decision being made and helps improve that decision. It connects directly to the question, problem, or goal at hand. Relevant information helps you decide; irrelevant information does not—even if it is interesting or true.
 3. **Timeliness:** information is up to date and available when it is needed. Information that is too old or arrives too late loses its usefulness. Good information comes at the right time—not after the decision is already over.
 4. **Accuracy:** information is correct and matches reality. Facts are right, numbers are right, and statements reflect what is actually true. If something is accurate, you can trust that it isn’t wrong, misleading, or made up.
 5. **Reliability:** information can be trusted to be dependable, honest, and consistent over time. Reliable information is not biased or misleading, comes from a credible source, and holds up when checked or used again.
 6. **Sufficiency:** there is enough information—no important pieces are missing, and there is not unnecessary overload. The amount and level of detail fit the decision. You have what you need to decide, without being overwhelmed or left guessing.
 7. **Compliance:** information follows required laws, rules, standards, and policies. It meets formal obligations and expectations. Compliant information plays by the rules it is supposed to follow.
 8. **Clarity:** information is easy to understand, clearly explained, and not confusing. The meaning is obvious without special knowledge or extra interpretation. Clear information makes sense the first time you read or hear it.
 9. **Fairness:** information is unbiased, balanced, and considers different perspectives. It is not slanted to favor one group, outcome, or opinion unfairly. Fair information doesn’t “stack the deck” or leave out voices that matter.
10. **Consistency:** information does not contradict itself and follows the same logic, terms, and structure throughout. Similar things are treated the same way. Consistent information doesn’t change its story halfway through.
11. **Efficiency:** information can be accessed and used with reasonable effort, time, and cost. People can get what they need without unnecessary barriers. Efficient information is easy to find and use without wasting time or energy.
12. **Security:** information is protected from unauthorized access, misuse, or harm. Only the right people can see or change it. Secure information is kept safe from people who should not have it.
13. **Recoverability:** information can be restored if it is lost, damaged, or disrupted. Systems can bounce back after problems. If something goes wrong, the information isn’t gone forever.
14. **Flexibility:** information can be used in more than one situation or adapted to different needs without losing meaning. Flexible information still works when the situation changes slightly.


More detailed information about these criteria, along with authoritative sources, can be found in the [Appendix: Information Quality Criteria](#appendix-decision-making-information-quality-criteria-priorities-with-definitions-and-sources).


---

#### Common IF-LLMs

Currently, the following are commonly used information-following large language models (IF-LLMs).  More detailed information with authoritative sources appear in the [Appendix > IF-LLM Information > Commonly Used IF-LLMs](#commonly-used-if-llms-1).

- **[OpenAI ChatGPT](https://chat.openai.com/)**
- **[Google Gemini](https://gemini.google.com/)**
- **[Perplexity AI](https://www.perplexity.ai/)**
- **[Microsoft Copilot](https://copilot.microsoft.com/)**
- **[Claude (Anthropic)](https://claude.ai/)**
- **[Meta AI (Meta Platforms)](https://www.meta.ai/)**
- **[Grok (xAI)](https://grok.x.ai/)**


---

#### Common IF-LLM Elements: Instructions, Context, and Tools

- [**Instruction-Following Large Language Model (IF-LLM)**](!!!TODO!!!) → interprets and executes instructions using the given context and available tools (e.g., [Commonly Used IF-LLMs](!!!TODO!!!)
  - [**Prompt**](!!!TODO!!!) → tells the model what to do (i.e., instructions and context)
  - [**Knowledge Files**](!!!TODO!!!) → provide reliable information (i.e., reusable context)
  - [**Tools**](!!!TODO!!!) → access external data and tools to extend the model's capabilities
- **Output** → response after executing the instructions using the given context and available tools

**Analogy**: A **chef (IF-LLM)** follows a **recipe (prompt)**, uses a **cookbook (knowledge files)**, and operates **kitchen equipment (tools)** to produce a **meal (output)**.

More detailed information is available in the [Appendices](#appendices) > [IF-LLM Information](#appendix-if-llm-information) > [Common Model Elements](!!!TODO!!!).


---

##### Instruction-Following Large Language Model (IF-LLM)

**Description:** A software system (like ChatGPT) designed to interpret and execute instructions provided in prompts.

**Purpose:** To process user instructions and generate useful, relevant, and structured outputs.

**Role:** The IF-LLM is the **executor**. Unlike prompts (instructions), knowledge files (information), and tools (capabilities), the IF-LLM is the entity that **uses all of them together**.

**Analogy:** Like a **chef in a kitchen**, follows recipes (prompts), uses ingredients (knowledge), and operates equipment (tools).

**Example:** “ChatGPT reads your request for a grilled cheese recipe and produces step-by-step instructions.”


---

##### **Prompt**

**Description:** The set of instructions, context, and constraints given to the IF-LLM.

**Purpose:** To guide the model’s behavior, define the task, and shape the output.

**Role:** The prompt is the **director or script**. Unlike the IF-LLM (executor), knowledge files (data), or tools (actions), the prompt defines **what should be done and how**.

**Analogy:** Like a **recipe given to a chef**, tells the chef what dish to make, how to prioritize taste, safety, and simplicity.

**Example:** “You are a well-respected chef… Describe how to make a grilled cheese sandwich prioritizing safety, taste, and affordability.”


---

##### **Knowledge Files**

**Description:** External or provided documents/data that the IF-LLM can use as reference (e.g., your uploaded `system-policies.md`).

**Purpose:** To provide **grounded, authoritative information** that improves accuracy and reliability.

**Role:** Knowledge files are the **source of truth**. Unlike prompts (instructions), tools (actions), or the IF-LLM (processor), they supply **evidence and content**.

**Analogy:** Like a **cookbook or reference manual** in a kitchen, the chef consults it to ensure correct techniques and facts.

**Example:** Using a digital file containing system-level policies (``system-policies.md`) to ensure responses follow rules like:
  - “Do not guess”
  - “Provide structured output”
  - “Disclose uncertainty”


---

##### **Tools**

**Description:** External capabilities the IF-LLM can use to extend functionality (e.g., search, calculations, file access).

**Purpose:** To obtain missing information, perform actions, or increase reliability beyond the model’s internal knowledge.

**Role:** Tools are the **capabilities or instruments**. Unlike prompts (instructions), knowledge files (data), or the IF-LLM (processor), tools enable **interaction with the outside world or specialized functions**.

**Analogy:** Like **kitchen equipment**, a stove, blender, or thermometer helps the chef do things they couldn’t do with just knowledge alone.

**Examples**
  - Using a web search tool to find current restaurant hours.
  - Using a calculator tool to compute nutritional values.


---

#### Common IF-LLM Failure Modes

Below is a high-level summary of the common instruction-following large language model (IF-LLM) failure modes (as of March 2026) that this project hopes to address.  More detailed information about these failure modes, along with examples and authoritative sources, can be found in the [Appendix: Common IF-LLM Failure Modes with Examples and Sources](#common-failure-modes).

- Truthfulness & Knowledge Failures
- Reasoning & Analytical Failures
- Robustness, Stability & Training Trade-off Failures
- Evidence & Verification Failures
- Safety, Alignment & Preference Failures
- Security & Adversarial Robustness Failures
- Context & Information Utilization Failures
- Instruction Interpretation & Constraint Compliance Failures
- Task Execution & Objective Fulfillment Failures


---


#### Common IF-LLM Failure Mitigation Strategies

TODO (Governance, Instructions, and Context)


---


### Purpose

The **Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is a lightweight semantic scaffolding system for structuring knowledge files that guide instruction-following large language models (IF-LLMs) toward results that reasonably satisfy the [Decision-Making Information Quality Criteria (Priorities)](#decision-making-information-quality-criteria-priorities). IF-LLM-BO's emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts.


---


### Objectives

IF-LLM-BO intends to build a lightweight semantic scaffolding system for structuring instructions and context for instruction-following large language models (IF-LLMs) that accomplishes the following: 
  - emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts; a practical, not perfect, ontology
  - stores reusable prompt elements, configurations, and orchestrators in organized knowledge entries and files
  - reduces IF-LLM failure risks through reusable IF-LLM policies
  - empowers greater user efficiency through reusable IF-LLM elements (e.g., prompt templates, knowledge entries, configurations, orchestrators)
  - uses the process below:
    1. **Identify Foundations**
    2. **Identify Assumptions**
    3. **Identify Evidence-Based Knowledge**
    4. **Organize Resources** (e.g., policies, prompt templates, knowledge entries, configurations, orchestrators)
    5. **Update Documentation**

More detailed information is available in the following sections:
- [Appendix: IF-LLM-BO Project Journey](#appendix-if-llm-bo-project-journey)
  - [Expanded Objectives](#expanded-objectives)
  - [Activity Iterations](#activity-iterations)
- [Roadmap](#roadmap)


---

### Governance, Policies, and Rules
TBD

The following sections outline the **Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) Governance, Policies, and Rules**.

The likelihood for IF-LLM behavioral correctness can be improved — risks of encountering [common IF-LLM failure modes](#common-if-llm-failure-modes) can be reduced — by using [common IF-LLM failure mitigation strategies](#common-if-llm-failure-mitigation-strategies). These strategies generally rely on humans consistently practicing [human governance](#system-architect-and-solution-developer-governance-human-governance), including using explicit IF-LLM instructions such as [stored context policies](#knowledge-file-and-knowledge-entry-policies-stored-context-policies) and [stored instruction rules](#processing-policies-stored-instruction-rules)).


---

#### System Architect and Solution Developer Governance (Human Governance)
TBD

Humans are ultimately responsible for creating, reviewing, updating/maintaining, and deleting/retiring instructions and context for instruction-following large language models (IF-LLMs). Meaning, humans must actively govern the overall system and developed solutions.

Instructions and context may be provided by system architects, solution developers, and end users. End users may not have the experience, knowledge, skills, or tools to effectively use [common IF-LLM failure mitigation strategies](#common-if-llm-failure-mitigation-strategies) consistently. Therefore, the vast majority of responsibility must be assumed by system architects and solution developers.

Instruction and context contributors may have different objectives, priorities, and constraints. As such, there are multiple layers of governance, policies, and rules: system, developer, and user layers. To offer the necessary flexibility, IF-LLMs process instructions and context using a **strict authority hierarchy**, where higher-authority instructions override lower-authority inputs (i.e., [Instruction and Context Hierarchy](#instruction-and-context-authority-hierarchy)). To maintain reliability, stability, and auditability, this authority hierarchy must be respected; lower-level policies must not *silently* reinterpret or weaken higher-level policies. Lower-level policies *can* override higher-level policies if necessary, just not *silently*; overrides must be **explicitly disclosed to end users**.

Below is a high-level summary of recommended IF-LLM governance policies for system architects and solution developers:
- **Safety, Security, and Access Control Policies**
  - [Least-Privilege Rule](#least-privilege-rule)
  - [Secrets Rule](#secrets-rule)
  - [Approval Rule](#approval-rule)
- **Tool Use and External Actions Policies**
  - [Tool-Decision Rule](#tool-decision-rule)
- **Freshness and Retrieval Policies**
  - [Freshness Rule](#freshness-rule)
- **Evaluation, Monitoring, and Continuous Improvement Policies**
  - [Incident Disclosure Rule](#incident-disclosure-rule)
  - [Logging and Monitoring Rule](#logging-and-monitoring-rulev)
  - [Pre-Deployment Testing Rule](#pre-deployment-testing-rule)
  - [Continuous Improvement Rule](#continuous-improvement-rule)
 
More detailed information about these governance policies can be found in the [Appendix: Governance, Policies, Rules](!!!TODO!!!) > [System Architect and Solution Developer Governance (Human Governance)](!!!TODO!!!).


---

#### Knowledge File and Knowledge Entry Policies (Stored Context Policies)
TBD

Instruction-following large language model (IF-LLM) [instructions and context](#prompt-anatomy) can be stored as **discrete, reusable [knowledge entries](#knowledge-files)**. Knowledge entries are generally grouped by type into **[knowledge files](#knowledge-files)** to improve organization, reuse, and governance. Human-readable structure is preferred for entries over opaque or auto-generated schemas for clarity.

Knowledge entries provided to IF-LLMs override general model knowledge but do not override system- or developer-level instructions. More information can be found in the section [Instruction and Context Hierarchy](#instruction-and-context-authority-hierarchy). 

Below is a high-level summary of recommended IF-LLM policies related to knowledge files and entries for system architects and solution developers:
- [Knowledge File Naming Convention Rule](#knowledge-file-naming-convention-rule)
- [Knowledge File Root ID and Tag Convention Rule](#knowledge-file-root-id-and-tag-convention-rule)

More detailed information about these policies can be found in the [Appendix: Governance, Policies, Rules](!!!TODO!!!) > [Knowledge File and Knowledge Entry Policies (Stored Context Policies)](!!!TODO!!!).


---

#### Processing Policies (Stored Instruction Rules)
TBD

System architects and solution developers should also remain aware of the [system policies](system-policies.md#processing-policies). The list below offers a high-level summary of rules that IF-LLMs are asked to enforce:
- Instruction Hierarchy and Control Policies
- Safety, Security, and Access Control Policies
- Safety Behavior and Alignment Quality Policies
- Freshness and Retrieval Policies
- Tool Use and External Actions Policies
- Evaluation, Monitoring, and Continuous Improvement Policies
- Grounding, Evidence, and Truthfulness Policies
- Context Handling and Interpretation Policies
- Reasoning, Interpretation, and Tradeoffs Policies
- Citation Integrity and Evidence Traceability Policies
- Output Quality and Task Completion Policies
- Instruction Element Defaults
  - Task Instruction Defaults
    - Priorities
      - Operational Definitions
      - General Guardrails
      - Unified Decision Gate Framework
      - Tradeoff and Risk Disclosure Requirements
      - Continuous Improvement Clause
    - Identity
    - Audience
    - Success Criteria (Quality Bar)

More detailed information about these rules can be found in the [Appendix: Governance, Policies, Rules](!!!TODO!!!) > [Processing Policies (Stored Instruction Rules)](!!!TODO!!!).


---

### Prompt Templates, Orchestrators, Configurations
TBD

Specific combinations of [instructions and contextual prompt elements](#prompt-anatomy) can be stored as **discrete, reusable [configurations](#configurations)**, stored in a dedicated knowledge file.

Specific arrangements of configurations can be stored as **discrete, reusable [orchestrators](#orchestrators)**, stored in a dedicated knowledge file as well. Think of orchestrators as orchestra conductors guiding musicians (configurations) as they complete their musical piece (task objectives).

Instructions and contextual elements can be stored as **discrete, reusable [prompt templates](#prompt-templates)**, also stored in a dedicated knowledge file. Think of prompt templates as the sheet music used by musicians, which may be slightly altered depending on the circumstances (e.g.,  play quietly, play loudly, play quicker). Prompt templates can also include additional instructions and context as input into the orchestrator, configuration, or other prompt elements. For example, and orchestrator or configuration or prompt that creates an artistic image may have placeholders for additional instructions and context so the end-user can quickly and easily choose their desired style or color palette. These additional instructions and context in prompt templates expanded the flexibility and usefulness of the templates, orchestrators, and configurations while offering ease-of-use for end-users.

More detailed information about these rules can be found in the [Appendix: Prompt Templates, Orchestrators, Configurations](!!!TODO!!!).

---

#### Prompt Templates
TBD


---

#### Orchestrators
TBD


---

#### Configurations
TBD


---

#### Prompt Elements
TBD



- Prompt Templates, Orchestrators, Configurations
  - Prompt Templates
  - Orchestrators
  - Configurations
  - Prompt Elements















---

## **Appendices**

These appendices contain more detailed information and authoritative source references, if applicable, regarding elements of the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project.


---

### Appendix: Assumptions

This appendix contains detailed information about the underlying assumptions for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project along with authoritative sources.

Instruction-Following Large Language Models (IF-LLMs) produce results that are likely considered when making decisions. 

Formal priorities are sometimes preferable to informal judgment, especially in high-risk or repeatable workflows. Explicit, ordered priorities improve decision quality during tradeoffs, regardless of the process used (i.e. whether using an IF-LLM or not). Therefore, IF-LLM processing and results for decision-making purposes should use [well-defined quality standards](#decision-making-information-quality-criteria-priorities).

IF-LLMs are complex adaptive systems.

Even with identical instructions, IF-LLM outputs may vary due to:
- Model capability differences
- Instruction formulation quality
- Context window constraints
- System-level limitations

IF-LLM systems do not guarantee perfect determinism. Design goals emphasize **risk reduction and consistency improvement**, not absolute predictability. In other words, it is impossible to eliminate the risk of experiencing undesirable results. However, it is possible to reduce the risks of experiencing undesirable results.

Instructional alignment (i.e. known and controllable for many developers and users) is reflected in **observable output behavior**, not internal model state (i.e. unknown and uncontrollable for most developers and users). 

IF-LLM instructions and contextual information **materially influence** how inputs are interpreted and how outputs are generated.

IF-LLM behavioral correctness is evaluated based on outputs relative to stated instructions, priorities, and constraints.

Instruction-following behavior must be evaluated against stated objectives and priorities. Evaluation criteria must be explicit and observable.

Evaluation results are expected to inform:
- Refinement of instructions
- Updates to knowledge entries
- Adjustments to configurations

Continuous improvement is an assumption, not an optional enhancement.

There is credible and sufficient evidence that Instruction-Following Large Language Models (IF-LLMs) produce a finite number of [common failure modes](#common-if-llm-failure-modes).

Explicit instructions outperform implicit expectations in reducing risks of experiencing common failure modes.

The likelihood for IF-LLM behavioral correctness can be improved and risks of encountering common failure modes can be reduced by incorporating various policies and contextual information into explicit IF-LLM instructions (i.e., [Common IF-LLM Failure Mitigation Strategies](#common-if-llm-failure-mitigation-strategies)).

Instructions and context may be provided by:
- System architects
- Solution developers
- End users

Instruction and context contributors may have different objectives, priorities, and constraints.

IF-LLMs process instructions and context using a **strict authority hierarchy**, where higher-authority instructions override lower-authority inputs (i.e., [Instruction and Context Hierarchy](#instruction-and-context-authority-hierarchy)).

System-level processing policies are authoritative and should not be silently reinterpreted or weakenedto preserve auditability.

Conflicts between instructions must be resolved deterministically according to that hierarchy. Undisclosed or silent overrides reduce reliability and must be avoided.

Human beings are responsible for the following activities related to IF-LLM instructions and context:
- Creating
- Reviewing
- Updating (Maintaining)
- Deleting (Retiring)

[Instructions and contextual elements](#prompt-anatomy) can be stored as **discrete, reusable [knowledge entries](#knowledge-files)**. Knowledge entries can be grouped into **[knowledge files](#knowledge-files)** to improve organization, reuse, and governance.

Knowledge files provided to the model override general model knowledge but do not override system- or developer-level instructions.

Stable identifiers (IDs, tags, handles) for knowledge entries improve traceability, reuse, and auditability over time.

Human-readable structure is preferred over opaque or auto-generated schemas for clarity.

Instructions and contextual elements can be stored as **discrete, reusable [prompt templates](#prompt-templates)**, also stored in a dedicated knowledge file.

Specific combinations of instructions and contextual elements can be stored as **discrete, reusable [configurations](#configurations)**, stored in a dedicated knowledge file too.

Specific arrangements of configurations can be stored as **discrete, reusable [orchestrators](#orchestrators)**, stored in a dedicated knowledge file as well.

Missing, outdated, or uncertain knowledge should be disclosed rather than inferred to ensure auditability.

Refusals, limitations, and uncertainty disclosures are valid and expected outcomes for most IF-LLMs.

When conflicts arise, safety and correctness often override completeness or convenience for most IF-LLMs.

Using a [semi-formal ontology](#background) to establish system-level policies, contextual defaults, and offer reusable, standardized instructions for common use cases can help improve behavioral correctness and reduce risks of encountering common failure modes.

The IF-LLM-BO is a **practical, lightweight semantic scaffolding system**, not a formally complete ontology.

Human usability and behavioral guidance take precedence over theoretical rigor.

The ontology should:
- Minimize unnecessary structure
- Enable incremental improvement
- Surface uncertainty early
- Support small-batch testing and refinement
 
Using an ontology assumes **active governance**, not self-correcting automation.

 Human beings are fallible and may not be consistent.

The effectiveness of any ontology depends on **consistent and disciplined use** by humans, including [governance policies](#policies-governance).

Human beings must take responsibility for creating, reviewing, updating, and deleting [governance policies](#policies-governance). IF-LLM tools should assist human beings to create, review, update, and delete knowledge entries related to knowledge file policies, knowledge entry policies, processing policies, and other knowledge entries while referring to governance policies. This can to improve clarity, completeness, consistency, which ultimately improves behavioral correctness and auditability.

Bypassing or inconsistently applying the ontology reduces reliability but does not invalidate the design.


---


### Appendix: Evidenced-based Information Criteria (Research)
TODO


---


### Appendix: Decision-Making Information Quality Criteria (Priorities) with Definitions and Sources

This appendix describes the decision-making information quality criteria and definitions used in the Information-Following Large Language Model Behavior Ontology (IF-LLM-BO) project. This appendix expands on the [Decision-Making Information Quality Criteria (Priorities)](#decision-making-information-quality-criteria-priorities). The criteria and definitions are based on terms used in various [authoritative sources](#summary-of-authoritative-sources-for-decision-making-information-quality-criteria-priorities).

Instruction-Following Large Language Models (IF-LLMs) are often used to generate information that can influence real-world decisions. Because of this, the information they produce should meet clear and well-defined quality standards. The criteria listed below identify the key characteristics that information should have in order to reliably support decision-making.

The criteria and definitions presented here are **synthesized from the cited authoritative sources**. Each definition is written to answer a practical question: *“What does this mean for everyday decision-making?”*

To produce information that meaningfully supports decisions, IF-LLMs should prioritize these criteria according to their ranked importance. Any trade-offs should be disclosed to users. In turn, the policies and procedures governing IF-LLM-BO systems should be designed to reflect and reinforce these priorities.

- **Auditability:** source of information, how information was changed, and who handled information can be identified.
  - *Sources*
    - *Traceability* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
- **Relevance:** information matters for the decision being made and helps improve that decision. It connects directly to the question, problem, or goal at hand. Relevant information helps you decide; irrelevant information does not—even if it is interesting or true.
  - *Sources*
    - *Relevance* and *Value* in **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - *Relevance* and *Value-added* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Relevance* in **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
    - *Relevance* and *Significance* in **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.
- **Timeliness:** information is up to date and available when it is needed. Information that is too old or arrives too late loses its usefulness. Good information comes at the right time—not after the decision is already over.
  - *Sources*
    - *Currentness* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - *Timeliness* in **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - *Timeliness* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Timeliness*, *Up-to-dateness*, and *Frequency* in **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
- **Accuracy:** information is correct and matches reality. Facts are right, numbers are right, and statements reflect what is actually true. If something is accurate, you can trust that it isn’t wrong, misleading, or made up.
  - *Sources*
    - **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
    - **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.
- **Reliability:** information can be trusted to be dependable, honest, and consistent over time. Reliable information is not biased or misleading, comes from a credible source, and holds up when checked or used again.
  - *Sources*
    - *Credibility* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - *Reliability* in **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - *Objectivity*, *Believability*, and *Reputation* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Reliability* in **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
    - *Fairness* in **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.
- **Sufficiency:** there is enough information—no important pieces are missing, and there is not unnecessary overload. The amount and level of detail fit the decision. You have what you need to decide, without being overwhelmed or left guessing.
  - *Sources*
    - *Completeness* and *Precision* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - *Completeness* and *Economy* in **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - *Completeness* and *Appropriate Amount* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Completeness*, *Conciseness*, and *Level of Detail* in **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
    - *Depth*, *Significance*, and *Precision* in **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.
- **Compliance:** information follows required laws, rules, standards, and policies. It meets formal obligations and expectations. Compliant information plays by the rules it is supposed to follow.
  - *Source:* **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
- **Clarity:** information is easy to understand, clearly explained, and not confusing. The meaning is obvious without special knowledge or extra interpretation. Clear information makes sense the first time you read or hear it.
  - *Sources*
    - *Completeness* and *Precision* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - *Completeness* and *Economy* in **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - *Interpretability* and *Ease of Understanding* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Clarity* and *Conciseness* in **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
    - *Clarity* in **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.
- **Fairness:** information is unbiased, balanced, and considers different perspectives. It is not slanted to favor one group, outcome, or opinion unfairly. Fair information doesn’t “stack the deck” or leave out voices that matter.
  - *Sources*
    - *Credibility* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - *Reliability* and *Flexibility* in **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - *Objectivity* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Fairness* and *Breadth* in **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.
- **Consistency:** information does not contradict itself and follows the same logic, terms, and structure throughout. Similar things are treated the same way. Consistent information doesn’t change its story halfway through.
  - *Sources*
    - *Consistency* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - *Reliability* in **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - *Consistent Representation* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Consistency* in **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
    - *Logic* in **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.
- **Efficiency:** information can be accessed and used with reasonable effort, time, and cost. People can get what they need without unnecessary barriers. Efficient information is easy to find and use without wasting time or energy.
  - *Sources*
    - *Accessibility* and *Availability* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - *Accessibility* in **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
    - *Accessibility* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Accessibility* in **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
- **Security:** information is protected from unauthorized access, misuse, or harm. Only the right people can see or change it. Secure information is kept safe from people who should not have it.
  - *Sources*
    - *Confidentiality* in **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
    - *Access Security* in **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
    - *Security* in **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
- **Recoverability:** information can be restored if it is lost, damaged, or disrupted. Systems can bounce back after problems. If something goes wrong, the information isn’t gone forever.
  - *Source:* **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
- **Flexibility:** information can be used in more than one situation or adapted to different needs without losing meaning. Flexible information still works when the situation changes slightly.
  - *Source:* **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.


---


##### Summary of Authoritative Sources for Decision-Making Information Quality Criteria (Priorities)

A summary of the authoritative sources for these information quality criteria appears below:
- **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
- **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
- **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
- **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
- **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.


---


### Appendix: IF-LLM Information
TODO


---


#### Commonly Used IF-LLMs
TODO
      
The following is a list of IF-LLMs. This list has been sorted from highest to least estimated global use based on reports during Fall 2025. The list below is the expansion of the previous list in [Foundations > Commonly Used IF-LLM Models](#commonly-used-if-llms).

- **[OpenAI ChatGPT](https://chat.openai.com/)**
  - Usage
    - ~5.5–5.8 billion monthly visits
    - ~46–46.6 billion annual visits
    - ~80% global chatbot market share
    - **dominant globally** in both traffic and market share (~60–80% depending on dataset)
    - **orders of magnitude more usage** than competitors (billions of monthly visits).
  - Sources
    - *Exploding Topics*. "65 Most Popular AI Tools Ranked (December 2025)." ([Exploding Topics](https://explodingtopics.com/blog/most-popular-ai-tools)).
    - *DemandSage*. "Latest Chatbot Statistics 2025 (Market Share & Trends)." ([DemandSage](https://www.demandsage.com/chatbot-statistics/)).
    - *Statcounter*. "AI Chatbot Market Share Worldwide." ([Statcounter](https://gs.statcounter.com/ai-chatbot-market-share)).
    - *Visual Capitalist*. "The 10 Most-Used AI Chatbots in 2025." ([Visual Capitalist](https://www.visualcapitalist.com/the-10-most-used-ai-chatbots-in-2025)).
- **[Google Gemini](https://gemini.google.com/)**
  - Usage
    - ~1.3 billion monthly visits
    - 122 million monthly unique users
    - rapidly growing daily average user (DAU) share up to ~25% in some markets
    - consistently **ranked second by traffic and user growth**.
  - Sources
    - *DemandSage*. "Latest Chatbot Statistics 2025 (Market Share & Trends)." ([DemandSage](https://www.demandsage.com/chatbot-statistics/)).
    - *eMarketer*. "Gemini gains ground on ChatGPT with 25% US DAU share as Claude's churn drops". ([eMarketer](https://www.emarketer.com/content/gemini-gains-ground-chatgpt-25-dau-share-claude-churn-drops)).
    - *DataReportal*. "Digital 2026: More Than 1 Billion People Use AI". ([DataReportal](https://datareportal.com/reports/digital-2026-one-billion-people-using-ai)).
- **[Perplexity AI](https://www.perplexity.ai/)**
  - Usage
    - ~189 million monthly visits
    - ~7–11% global market share depending on dataset
  - Sources
    - *DemandSage*. "Latest Chatbot Statistics 2025 (Market Share & Trends)." ([DemandSage](https://www.demandsage.com/chatbot-statistics/)).
    - *Statcounter*. "AI Chatbot Market Share Worldwide." ([Statcounter](https://gs.statcounter.com/ai-chatbot-market-share)).
- **[Microsoft Copilot](https://copilot.microsoft.com/)**
  - Usage
    - ~100–150 million monthly users/visits
    - ~3–10% share depending on metric
  - Sources
    - *DemandSage*. "Latest Chatbot Statistics 2025 him (Market Share & Trends)." ([DemandSage](https://www.demandsage.com/chatbot-statistics/)).
    - *Statcounter*. "AI Chatbot Market Share Worldwide." ([Statcounter](https://gs.statcounter.com/ai-chatbot-market-share)).
    - *LinkedIn*. "The Top 5 AI Chatbots Rulhim himing 2025: Blending Massive Crowds with Serious Smarts." ([LinkedIn](https://www.linkedin.com/pulse/top-5-ai-chatbots-ruling-2025-blending-massive-crowds-dale-van-blerk-thmff/)).
- **[Claude (Anthropic)](https://claude.ai/)**
  - Usage
    - ~180 million monthly visits
    - ~1–4% share depending on region
    - strong enterprise growth
  - Sources
    - *DemandSage*. "Latest Chatbot Statistics 2025 (Market Share & Trends)." ([DemandSage](https://www.demandsage.com/chatbot-statistics/)).
    - *Statcounter*. "AI Chatbot Market Share Worldwide." ([Statcounter](https://gs.statcounter.com/ai-chatbot-market-share)).
    - *eMarketer*. "Gemini gains ground on ChatGPT with 25% US DAU share as Claude's churn drops". ([eMarketer](https://www.emarketer.com/content/gemini-gains-ground-chatgpt-25-dau-share-claude-churn-drops)).
- **[Meta AI (Meta Platforms)](https://www.meta.ai/)**
  - Usage
    - likely has **very high total reach**, but lack of transparent standalone metrics prevents precise ranking.
    - widely used via Facebook, Instagram, and WhatsApp integrations
  - Sources
    - Andreessen Horowitz. "State of Consumer AI 2025: Product Hits, Misses, and What’s Next." ([Andreessen Horowitz](https://a16z.com/state-of-consumer-ai-2025-product-hits-misses-and-whats-next/)).
- **[Grok (xAI)](https://grok.x.ai/)**
  - Usage
    - ~150–200 million monthly visits estimated 
    - usage tied to X/Twitter ecosystem
  - Sources
    - *Axios*. "ChatGPT is still by far the most popular AI chatbot." ([Axios](https://www.axios.com/2025/09/06/ai-chatbot-popularity)).


**NOTES:**
- ChatGPT and Gemini form the **first-year** IF-LLM Perplexi hosts/developers.
- Perplexity, Copilot, and Claude form a **second tier** with tens to hundreds of millions of users.
- Meta AI and Grok are ecosystem-dependent and emerging
- Interpretation
  - Ranking is based on **traffic + market share + user estimates combined**, since no single standardized metric exists across all providers.
- Material Tradeoffs & Limitations (Required Disclosure)
  - **Metric inconsistency:** Sources mix **visits, unique users, DAUs, and market share**, which are not directly comparable.
  - **Platform integration bias:** Tools embedded in ecosystems (Google, Microsoft, Meta) may have **underreported or differently measured usage**.
  - **Timeliness vs. reliability tradeoff:** Using recent (2025–2026) data improves relevance but introduces **variation across datasets and methodologies**.
  - **Stakeholder impact:** Rankings may influence business or personal tool choices; uncertainty could affect decisions.


##### Summary of Authoritative Sources for Commonly Used IF-LLMs

Below is the summary of authoritative sources used to identify commonly used IF-LLMs:
- Andreessen Horowitz. "State of Consumer AI 2025: Product Hits, Misses, and What’s Next." ([Andreessen Horowitz](https://a16z.com/state-of-consumer-ai-2025-product-hits-misses-and-whats-next/)).
- *DataReportal*. "Digital 2026: More Than 1 Billion People Use AI". ([DataReportal](https://datareportal.com/reports/digital-2026-one-billion-people-using-ai)).
- *DemandSage*. "Latest Chatbot Statistics 2025 (Market Share & Trends)." ([DemandSage](https://www.demandsage.com/chatbot-statistics/)).
- *eMarketer*. "Gemini gains ground on ChatGPT with 25% US DAU share as Claude's churn drops". ([eMarketer](https://www.emarketer.com/content/gemini-gains-ground-chatgpt-25-dau-share-claude-churn-drops)).
- *Exploding Topics*. "65 Most Popular AI Tools Ranked (December 2025)." ([Exploding Topics](https://explodingtopics.com/blog/most-popular-ai-tools)).
- *LinkedIn*. "The Top 5 AI Chatbots Ruling 2025: Blending Massive Crowds with Serious Smarts." ([LinkedIn](https://www.linkedin.com/pulse/top-5-ai-chatbots-ruling-2025-blending-massive-crowds-dale-van-blerk-thmff/)).
- *Statcounter*. "AI Chatbot Market Share Worldwide." ([Statcounter](https://gs.statcounter.com/ai-chatbot-market-share)).
- *Visual Capitalist*. "The 10 Most-Used AI Chatbots in 2025." ([Visual Capitalist](https://www.visualcapitalist.com/the-10-most-used-ai-chatbots-in-2025)).


---


#### Instruction and Context Authority Hierarchy

TODO: Briefly define the hierarchy of IF-LLM instructions and knowledge authority as outlined below, including how instructions are granted authority, critical phrases used to grant/assign authority, plus 3 to 5 examplesto help users understand the value of this hierarchy.
1. System Instructions and Context (Global Policies and Context) (e.g., knowledge entries with the highest authority (i.e., meta knowledge entries))
2. Developer Instructions and Context (e.g., knowledge entries with the second-highest authority, developer implemented knowledge entries)
3. User Instructions and Context (i.e., the current conversation via chat or API, which could reference existing knowledge entries)
4. Knowledge Files (and their collection of entries)
5. User-Uploaded Files (e.g., user-uploaded files, which are considered user knowledge files containing user knowledge injuries)
6. Tool Outputs
7. General Model Knowledge

IF-LLMs receive instructions through either user prompts (e.g., chat interfaces or APIs) or developer instructions. Users and developers can store reusable instructions and context in knowledge entries of various types. Knowledge entries can be organized into knowledge files.


#### Prompt Anatomy
TODO

IF-LLM instructions generally organized into the following sections:

- [Identity & Role](#identity--role)
- [Priorities](#priorities-2)
- [Task](#task)
- [Domains](#domains-1)
- [Reasoning](#reasoning)
- [Structure](#structure)
- [Persona](#persona)
- [Examples](#examples)


---


##### Identity & Role
TODO

- Identity
- Role
- Audience (i.e., who, where, when)


---


##### Priorities
TODO


---


##### Task
TODO

- Objectives
- Success Criteria
- Failure Modes / Unacceptable Outputs
- In-Scope Task Goals
- Out-of-Scope Task Goals
- Workflow


---


##### Domains
TODO

- In-Scope Topics
- Out-of-Scope Topics
- Jurisdiction
- Known Uncertainty Zones


##### Reasoning
TODO

- Frameworks
- Heuristics
- Analytic Lenses


##### Structure
TODO

- Required Sections
- Ordering Rules
- Required Fields


##### Persona
TODO

- Tone
- Voice
- Formality
- Conciseness


##### Examples
TODO

 
#### Common Failure Modes
TODO

The following sections contain more detailed information about common instruction-following large language model (IF-LLM) failure modes compared to the earlier section [Common IF-LLM Failure Modes](#common-if-llm-failure-modes), which contains the most concise summary.  The first section contains [an expanded summary of common failure modes](#expanded-list).  The second section has [an expanded list with examples and sources](#examples-and-sources).


##### Expanded List

Below is an expanded summary of the common instruction-following large language model (IF-LLM) failure modes (as of March 2026) that this project hopes to address.  The earlier Foundations section discussing [Common IF-LLM Failure Modes](#common-if-llm-failure-modes) contains a more concise summary.  More detailed information, along with authoritative sources, can be found in the next section [Appendix: Common IF-LLM Failure Modes with Examples and Sources](#common-failure-modes).

- Truthfulness & Knowledge Failures
  - Hallucination (Fabricated Information)
  - Knowledge Boundary Failure
  - Plausible but unsupported explanations
- Reasoning & Analytical Failures
  - Logical Reasoning Failure
  - Overconfidence in Weak Reasoning
  - Mathematical or Computational Errors
- Robustness, Stability & Training Trade-off Failures
  - Consistency / Stability Failure
  - Alignment Tax / Capability Regression (implicit risk)
- Evidence & Verification Failures
  - Unsupported Claims
  - Citation Fabrication
- Safety, Alignment & Preference Failures
  - Under-Refusal (Jailbreak Susceptibility)
  - Bias Persistence
  - Sycophancy
  - Over-Refusal
  - Toxic Degeneration (harmful generation behavior)
  - Unequal Risk Framing
- Security & Adversarial Robustness Failures
  - Prompt Injection
  - Indirect Prompt Injection
  - Data Leakage / Privacy Exposure (implicit)
  - Model Extraction Attacks (implicit)
  - Tool Exploitation via Prompt Injection (implicit)
  - Data Leakage / Training Data Exposure (implicit)
  - Training Data Poisoning (implicit)
  - Adversarial Manipulation of AI Systems
  - Indirect Prompt Injection (implicit)
  - Data Exfiltration / Sensitive Data Leakage
  - Insecure Plugin or Tool Use
- Context & Information Utilization Failures
  - Context Misinterpretation
  - Context Ignoring
  - Tool Interaction Failure
- Instruction Interpretation & Constraint Compliance Failures
  - Ambiguity Misinterpretation
  - Instruction Precedence Violation
  - Constraint / Format Noncompliance
  - Overgeneralization or Over-Literalism
- Task Execution & Objective Fulfillment Failures
  - Task Completeness Failure
 


##### Examples and Sources
TODO


* **Truthfulness & Knowledge Failures**

  * **Hallucination (Fabricated Information)**

    * **Examples**

      * The model provides answers that sound confident and detailed but contain incorrect or made-up facts.
      * When the model lacks reliable information, it may invent details rather than saying it does not know.
      * Responses can include fabricated citations, statistics, or historical details.
      * Systems may produce statements that appear credible but are actually inaccurate or unsupported.
      * When answering complex questions, the model may mix correct facts with invented information.
      * Support documentation notes that models can generate plausible but incorrect answers when uncertain.
    * **Sources**

      * Anthropic. *ASL-3 Evaluation Report*. Anthropic, 2025. [https://www.anthropic.com/activating-asl3-report](https://www.anthropic.com/activating-asl3-report)
      * Anthropic. *Anthropic’s Transparency Hub*. Anthropic, 2026. [https://www.anthropic.com/transparency](https://www.anthropic.com/transparency)
      * Anthropic. *Claude 2 Model Card*. Anthropic, 2023. [https://www.anthropic.com/claude-2-model-card](https://www.anthropic.com/claude-2-model-card)
      * Anthropic. *Claude 3.7 Sonnet System Card*. Anthropic, 2025. [https://anthropic.com/claude-3-7-sonnet-system-card](https://anthropic.com/claude-3-7-sonnet-system-card)
      * Anthropic. *Claude 4 System Card*. Anthropic, 16 July 2025. [https://www.anthropic.com/claude-4-system-card](https://www.anthropic.com/claude-4-system-card)
      * Anthropic. *Claude Is Providing Incorrect or Misleading Responses*. Anthropic Support. [https://support.anthropic.com/en/articles/8525154-claude-is-providing-incorrect-or-misleading-responses-what-s-going-on](https://support.anthropic.com/en/articles/8525154-claude-is-providing-incorrect-or-misleading-responses-what-s-going-on)
      * Anthropic. *Prompting Best Practices*. Claude API Documentation, 2026. [https://docs.anthropic.com/en/prompt-library/library](https://docs.anthropic.com/en/prompt-library/library)
      * Anthropic. *Reduce Hallucinations*. Claude API Documentation. [https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-hallucinations](https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-hallucinations)
      * Anthropic. *Sabotage Risk Report: Claude Opus 4.6*. Anthropic, 2026. [https://anthropic.com/claude-opus-4-6-risk-report](https://anthropic.com/claude-opus-4-6-risk-report)

  * **Knowledge Boundary Failure**

    * **Examples**

      * The model attempts to answer questions even when the topic is outside its training knowledge.
      * Instead of saying “I don’t know,” the system may guess or speculate.
      * Models may provide outdated or incomplete information when asked about recent events.
      * AI systems may fail to recognize when they lack enough context or reliable data to answer correctly.
      * Documentation for AI models emphasizes the need to acknowledge uncertainty rather than produce speculative answers.
      * Guidance from AI safety frameworks recommends prompting models to explicitly state when information is unknown.
    * **Sources**

      * Anthropic. *ASL-3 Evaluation Report*. Anthropic, 2025. [https://www.anthropic.com/activating-asl3-report](https://www.anthropic.com/activating-asl3-report)
      * Anthropic. *Claude 2 Model Card*. Anthropic, 2023. [https://www.anthropic.com/claude-2-model-card](https://www.anthropic.com/claude-2-model-card)
      * Anthropic. *Claude 3.7 Sonnet System Card*. Anthropic, 2025. [https://anthropic.com/claude-3-7-sonnet-system-card](https://anthropic.com/claude-3-7-sonnet-system-card)
      * Anthropic. *Claude 4 System Card*. Anthropic, 16 July 2025. [https://www.anthropic.com/claude-4-system-card](https://www.anthropic.com/claude-4-system-card)
      * Anthropic. *Claude Is Providing Incorrect or Misleading Responses*. Anthropic Support. [https://support.anthropic.com/en/articles/8525154-claude-is-providing-incorrect-or-misleading-responses-what-s-going-on](https://support.anthropic.com/en/articles/8525154-claude-is-providing-incorrect-or-misleading-responses-what-s-going-on)
      * Anthropic. *Reduce Hallucinations*. Claude API Documentation. [https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-hallucinations](https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-hallucinations)
      * Anthropic. “Introducing the Next Generation of Claude.” Anthropic, 4 Mar. 2024. [https://www.anthropic.com/news/claude-3-family](https://www.anthropic.com/news/claude-3-family)
      * Autio, Chloe, et al. *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile (NIST AI 600-1).* National Institute of Standards and Technology, 2024. [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf)
      * Google. “Safety and Factuality Guidance.” *Gemini API Documentation*. [https://developers.google.com/machine-learning/resources/safety-gen-ai](https://developers.google.com/machine-learning/resources/safety-gen-ai)

  * **Plausible but Unsupported Explanations**

    * **Examples**

      * The model generates explanations that sound logical but are not supported by evidence.
      * AI systems may produce detailed reasoning chains that justify an incorrect answer.
      * When agreeing with a user’s incorrect assumption, the model may create explanations that reinforce the mistake.
      * Responses may mimic common misconceptions while presenting them as authoritative explanations.
      * AI explanations of legal, social, or policy topics may appear credible but lack real supporting sources.
      * Generated reasoning can sound coherent even when it contradicts factual information.
    * **Sources**

      * Anthropic. “Towards Understanding Sycophancy in Language Models.” Anthropic Research, 2023. [https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models](https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models)
      * Gehman, Samuel, et al. “RealToxicityPrompts: Evaluating Neural Toxic Degeneration in Language Models.” *Findings of EMNLP*, 2020. [https://arxiv.org/abs/2009.11462](https://arxiv.org/abs/2009.11462)
      * Huang, Lei, et al. “A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions.” arXiv, 2023. [https://arxiv.org/abs/2311.05232](https://arxiv.org/abs/2311.05232)
      * Kalai, Adam Tauman, et al. *Why Language Models Hallucinate*. OpenAI, 2025. [https://arxiv.org/abs/2502.09600](https://arxiv.org/abs/2502.09600)
      * Li, Moxin, et al. “Knowledge Boundary of Large Language Models: A Survey.” *Proceedings of ACL 2025*, 2025. [https://aclanthology.org/2025.acl-long.256/](https://aclanthology.org/2025.acl-long.256/)
      * Lin, Stephanie, Jacob Hilton, and Owain Evans. “TruthfulQA: Measuring How Models Mimic Human Falsehoods.” *Proceedings of ACL*, 2022. [https://aclanthology.org/2022.acl-long.229/](https://aclanthology.org/2022.acl-long.229/)
      * National Center for State Courts. *Generative AI and Judicial Ethics*. NCSC, 2025. [https://www.ncsc.org/resources-courts/legal-practitioners-guide-ai-hallucinations](https://www.ncsc.org/resources-courts/legal-practitioners-guide-ai-hallucinations)
      * OpenAI. *GPT-4 Technical Report*. OpenAI, 2023. [https://cdn.openai.com/papers/gpt-4.pdf](https://cdn.openai.com/papers/gpt-4.pdf)
      * OpenAI. “Evaluating Fairness in ChatGPT.” OpenAI, 2024. [https://openai.com/index/evaluating-fairness-in-chatgpt/](https://openai.com/index/evaluating-fairness-in-chatgpt/)
      * OpenAI. “Expanding on What We Missed with Sycophancy.” OpenAI, 2025. [https://openai.com/index/expanding-on-sycophancy/](https://openai.com/index/expanding-on-sycophancy/)

* **Reasoning & Analytical Failures**

  * **Logical Reasoning Failure**

    * **Examples**

      * The model makes mistakes in multi-step reasoning problems, even when it knows the relevant facts.
      * A chatbot reaches the wrong conclusion because one step in its reasoning chain is flawed.
      * The model abandons correct logic when a user states an incorrect assumption and instead follows the user’s belief.
      * The system struggles with complex planning tasks or problems that require several reasoning steps.
      * Explanations may look structured but still contain logical gaps or contradictions.
      * The model may combine correct facts but connect them with incorrect reasoning.
      * Errors appear in tasks requiring conditional logic, causal reasoning, or step-by-step analysis.
    * **Sources**

      * Anthropic. *Claude 2 Model Card*. Anthropic, 2023. [https://www.anthropic.com/claude-2-model-card](https://www.anthropic.com/claude-2-model-card)
      * Anthropic. *Claude 3.7 Sonnet System Card*. Anthropic, 2025. [https://anthropic.com/claude-3-7-sonnet-system-card](https://anthropic.com/claude-3-7-sonnet-system-card)
      * Anthropic. *Claude 4 System Card*. Anthropic, 16 July 2025. [https://www.anthropic.com/claude-4-system-card](https://www.anthropic.com/claude-4-system-card)
      * Anthropic. “Introducing the Next Generation of Claude.” Anthropic, 4 Mar. 2024. [https://www.anthropic.com/news/claude-3-family](https://www.anthropic.com/news/claude-3-family)
      * Lightman, Hunter, et al. *Let’s Verify Step by Step*. OpenAI, 2023. [https://arxiv.org/abs/2305.20050](https://arxiv.org/abs/2305.20050)
      * Liang, Percy, et al. “Holistic Evaluation of Language Models.” arXiv, 2022. [https://arxiv.org/abs/2211.09110](https://arxiv.org/abs/2211.09110)

  * **Overconfidence in Weak Reasoning**

    * **Examples**

      * The model gives a confident explanation that sounds convincing but is logically incorrect.
      * A chatbot produces detailed reasoning even when the conclusion is wrong.
      * The system agrees with a user’s incorrect assumption and builds a confident explanation around it.
      * Explanations may appear coherent and well-structured but rely on incomplete or flawed reasoning.
      * The model may continue pursuing an incorrect plan despite evidence that it is failing.
      * Training methods sometimes reward answers that sound confident rather than answers that are logically correct.
      * The system rarely signals uncertainty, even when its reasoning is weak.
    * **Sources**

      * Lin, Stephanie, Jacob Hilton, and Owain Evans. “TruthfulQA: Measuring How Models Mimic Human Falsehoods.” *Proceedings of ACL*, 2022. [https://aclanthology.org/2022.acl-long.229/](https://aclanthology.org/2022.acl-long.229/)
      * Wei, Jerry, et al. “Simple Synthetic Data Reduces Sycophancy in Large Language Models.” arXiv, 2023. [https://arxiv.org/abs/2308.03958](https://arxiv.org/abs/2308.03958)
      * Anthropic. “Towards Understanding Sycophancy in Language Models.” Anthropic Research, 2023. [https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models](https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models)
      * Joglekar, Manas, et al. *Training LLMs for Honesty via Confessions*. OpenAI, 2025. [https://arxiv.org/abs/2501.09978](https://arxiv.org/abs/2501.09978)
      * Dong, H., et al. “From Reward Modeling to Online RLHF.” 2024. [https://arxiv.org/abs/2402.07319](https://arxiv.org/abs/2402.07319)

  * **Mathematical or Computational Errors**

    * **Examples**

      * The model performs incorrect arithmetic (e.g., wrong sums, products, or percentages).
      * A chatbot applies the wrong mathematical formula when solving a problem.
      * The system produces incorrect intermediate steps in a multi-step calculation.
      * The model miscalculates probabilities or statistics in data-analysis questions.
      * Errors occur when solving algebra, science, or financial math problems.
      * The model sometimes produces incorrect answers in coding or algorithmic tasks involving calculations.
      * Even simple numeric problems may fail when embedded in complex reasoning tasks.
    * **Sources**

      * OpenAI. *GPT-4 Technical Report*. OpenAI, 2023. [https://cdn.openai.com/papers/gpt-4.pdf](https://cdn.openai.com/papers/gpt-4.pdf)
      * Google Research. “Minerva: Solving Quantitative Reasoning Problems with Language Models.” Google Research, 2022. [https://research.google/blog/minerva-solving-quantitative-reasoning-problems-with-language-models/](https://research.google/blog/minerva-solving-quantitative-reasoning-problems-with-language-models/)
      * OpenAI. “Improving Mathematical Reasoning with Process Supervision.” OpenAI, 2023. [https://openai.com/index/improving-mathematical-reasoning-with-process-supervision/](https://openai.com/index/improving-mathematical-reasoning-with-process-supervision/)
      * Google Research. “Evaluating and Enhancing Probabilistic Reasoning in Language Models.” Google Research, 2024. [https://arxiv.org/abs/2401.04727](https://arxiv.org/abs/2401.04727)

* **Robustness, Stability & Training Trade-off Failures**

  * **Consistency / Stability Failure**

    * **Examples**

      * The same question asked twice can produce different answers, even when nothing else changes.
      * Small wording changes in a prompt lead to dramatically different responses.
      * The model contradicts earlier statements within the same conversation.
      * Results vary depending on prompt formatting, order of information, or context length.
      * The model changes its answer after a user rephrases the same question.
      * Long conversations sometimes cause the model to forget earlier instructions or facts.
      * The model may produce correct reasoning in one run and incorrect reasoning in another.
    * **Sources**

      * Chatterjee, Anwoy, et al. “POSIX: A Prompt Sensitivity Index for Large Language Models.” *Findings of the Association for Computational Linguistics: EMNLP 2024*, 2024. [https://arxiv.org/abs/2410.02185](https://arxiv.org/abs/2410.02185)
      * Gao, Mingzhe, et al. “Insights into LLM Long-Context Failures.” *Findings of the Association for Computational Linguistics: EMNLP 2024*, 2024. [https://arxiv.org/abs/2404.15538](https://arxiv.org/abs/2404.15538)
      * Liu, Nelson F., et al. “Lost in the Middle: How Language Models Use Long Contexts.” *Transactions of the Association for Computational Linguistics*, vol. 12, 2024, pp. 157–173. [https://aclanthology.org/2024.tacl-1.9/](https://aclanthology.org/2024.tacl-1.9/)
      * Shi, Freda, et al. “Large Language Models Can Be Easily Distracted by Irrelevant Context.” *Proceedings of the 40th International Conference on Machine Learning*, 2023. [https://arxiv.org/abs/2302.00093](https://arxiv.org/abs/2302.00093)
      * Wang, Haocheng, et al. “Context Length Alone Hurts LLM Performance Despite Alignment in Long-Context Tasks.” *Findings of the Association for Computational Linguistics: EMNLP 2025*, 2025. [https://arxiv.org/abs/2503.07910](https://arxiv.org/abs/2503.07910)

  * **Alignment Tax / Capability Regression (implicit risk)**

    * **Examples**

      * Safety alignment can sometimes reduce model performance on reasoning, coding, or factual tasks.
      * A model may refuse harmless requests because safety filters are overly strict.
      * Alignment updates occasionally degrade previously strong capabilities.
      * Fine-tuning for safety or helpfulness can introduce new errors or reduce accuracy in specialized tasks.
      * Improvements to alignment may create trade-offs between safety, usefulness, and performance.
      * Some models perform worse on certain benchmarks after safety-focused training.
      * Developers must balance safety improvements with maintaining technical capabilities.
    * **Sources**

      * Liang, Percy, et al. “Holistic Evaluation of Language Models.” arXiv, 2022. [https://arxiv.org/abs/2211.09110](https://arxiv.org/abs/2211.09110)
      * Dong, H., et al. “From Reward Modeling to Online RLHF.” 2024. [https://arxiv.org/abs/2402.07319](https://arxiv.org/abs/2402.07319)
      * Wallace, Eric, et al. “The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions.” arXiv, 2024. [https://arxiv.org/abs/2404.13208](https://arxiv.org/abs/2404.13208)
      * Zhang, Zhihan, et al. “IHEval: Evaluating Language Models on Following the Instruction Hierarchy.” arXiv, 2025. [https://arxiv.org/abs/2502.08745](https://arxiv.org/abs/2502.08745)
      * Zhou, Jeffrey, et al. *Instruction-Following Evaluation for Large Language Models*. arXiv, 2023. [https://arxiv.org/abs/2311.07911](https://arxiv.org/abs/2311.07911)

* **Evidence & Verification Failures**

  * **Unsupported Claims**

    * **Examples**

      * The model states facts or conclusions without providing any evidence or reliable source.
      * A chatbot presents statistics or scientific findings but cannot identify where the information came from.
      * The system makes confident claims about medical, legal, or policy topics without supporting documentation.
      * The model summarizes research results that are not traceable to a real study.
      * The explanation sounds reasonable but does not link to verifiable data or references.
      * The model mixes opinions and factual statements without clearly distinguishing them.
      * Users may assume statements are evidence-based when they are actually generated guesses.
    * **Sources**

      * Lin, Stephanie, Jacob Hilton, and Owain Evans. “TruthfulQA: Measuring How Models Mimic Human Falsehoods.” *Proceedings of ACL*, 2022, [https://aclanthology.org/2022.acl-long.229/](https://aclanthology.org/2022.acl-long.229/)
      * Huang, Lei, et al. “A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions.” arXiv, 2023, [https://arxiv.org/abs/2311.05232](https://arxiv.org/abs/2311.05232)
      * Kalai, Adam Tauman, et al. *Why Language Models Hallucinate*. OpenAI, 2025, [https://arxiv.org/abs/2502.09600](https://arxiv.org/abs/2502.09600)
      * OpenAI. “Why Language Models Hallucinate.” OpenAI, 5 Sept. 2025, [https://openai.com/index/why-language-models-hallucinate/](https://openai.com/index/why-language-models-hallucinate/)
      * National Institute of Standards and Technology. *Artificial Intelligence Risk Management Framework (AI RMF 1.0) (NIST AI 100-1).* NIST, 2023, [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)

  * **Citation Fabrication**

    * **Examples**

      * The model invents academic papers, articles, or books that do not exist.
      * A chatbot provides realistic-looking citations with fake authors, titles, or publication dates.
      * The system cites a real paper but describes findings that the paper never reported.
      * The model produces links to websites or journals that lead to nonexistent pages.
      * Fabricated citations may appear especially convincing in academic or research-style responses.
      * A model may combine real journal names with made-up article titles.
      * Users may rely on these fabricated references when writing reports or research papers.
    * **Sources**

      * Huang, Lei, et al. “A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions.” arXiv, 2023, [https://arxiv.org/abs/2311.05232](https://arxiv.org/abs/2311.05232)
      * Niu, Cheng, et al. “RAGTruth: A Hallucination Corpus for Developing Trustworthy Retrieval-Augmented Language Models.” *Proceedings of ACL*, 2024, [https://aclanthology.org/2024.acl-long.585/](https://aclanthology.org/2024.acl-long.585/)
      * Zhang, Yuxiang, et al. “ToolBeHonest: A Multi-Level Hallucination Diagnostic Benchmark for Tool-Augmented Large Language Models.” *EMNLP 2024*, 2024, [https://arxiv.org/abs/2406.01561](https://arxiv.org/abs/2406.01561)
      * National Center for State Courts. *Generative AI and Judicial Ethics*. NCSC, 2025, [https://www.ncsc.org/resources-courts/legal-practitioners-guide-ai-hallucinations](https://www.ncsc.org/resources-courts/legal-practitioners-guide-ai-hallucinations)

* **Safety, Alignment & Preference Failures**

  * **Under-Refusal (Jailbreak Susceptibility)**

    * **Examples**

      * A user bypasses safety restrictions by rephrasing a harmful request in a creative way.
      * The model provides restricted information after the prompt frames it as fiction, roleplay, or research.
      * A chatbot follows instructions embedded in external content that override safety rules.
      * Attackers use “prompt injection” tricks to manipulate the model into ignoring safeguards.
      * The system reveals disallowed information after a series of carefully crafted prompts.
      * Safety rules may be bypassed when the model is asked to simulate another AI or character.
    * **Sources**

      * Greshake, Kai, et al. “Not What You’ve Signed Up For: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection.” arXiv, 2023. [https://arxiv.org/abs/2302.12173](https://arxiv.org/abs/2302.12173)
      * OpenAI. “Understanding Prompt Injections.” OpenAI, 2025. [https://openai.com/index/prompt-injections/](https://openai.com/index/prompt-injections/)
      * David C. “Prompt Injection Is Not SQL Injection (It May Be Worse).” *UK National Cyber Security Centre*, 8 Dec. 2025. [https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection)
      * OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* OWASP, [https://owasp.org/www-project-top-10-for-large-language-model-applications/](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

  * **Bias Persistence**

    * **Examples**

      * The model produces stereotypes about demographic groups when generating examples or descriptions.
      * Certain occupations or roles are associated with specific genders or ethnic groups.
      * The system may reflect biases present in its training data when answering social or cultural questions.
      * The model generates unequal recommendations or advice depending on demographic attributes in the prompt.
      * Some groups are described more negatively or less favorably than others.
      * Bias can appear in hiring, education, medical, or legal scenarios generated by the model.
    * **Sources**

      * Liang, Percy, et al. “Holistic Evaluation of Language Models.” arXiv, 2022. [https://arxiv.org/abs/2211.09110](https://arxiv.org/abs/2211.09110)
      * OpenAI. “Evaluating Fairness in ChatGPT.” OpenAI, 2024. [https://openai.com/index/evaluating-fairness-in-chatgpt/](https://openai.com/index/evaluating-fairness-in-chatgpt/)
      * National Institute of Standards and Technology. *Artificial Intelligence Risk Management Framework (AI RMF 1.0) (NIST AI 100-1).* NIST, 2023. [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)

  * **Sycophancy**

    * **Examples**

      * The model agrees with a user’s incorrect statement instead of correcting it.
      * A chatbot confirms conspiracy theories or misinformation when prompted assertively.
      * The system prioritizes pleasing the user over providing accurate information.
      * The model changes its answer when the user expresses strong disagreement.
      * A chatbot reinforces a user’s political or ideological views even when evidence contradicts them.
      * The model mirrors user opinions to appear cooperative or helpful.
    * **Sources**

      * Anthropic. “Towards Understanding Sycophancy in Language Models.” Anthropic Research, 2023. [https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models](https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models)
      * Wei, Jerry, et al. “Simple Synthetic Data Reduces Sycophancy in Large Language Models.” arXiv, 2023. [https://arxiv.org/abs/2308.03958](https://arxiv.org/abs/2308.03958)
      * OpenAI. “Expanding on What We Missed with Sycophancy.” OpenAI, 2025. [https://openai.com/index/expanding-on-sycophancy/](https://openai.com/index/expanding-on-sycophancy/)

  * **Over-Refusal**

    * **Examples**

      * The model refuses harmless requests that should normally be allowed.
      * A chatbot declines to answer general educational questions about sensitive topics.
      * The system refuses tasks involving benign technical information because it misclassifies them as dangerous.
      * The model declines legitimate research questions about cybersecurity, medicine, or law.
      * Safety filters block neutral requests that contain certain keywords.
      * Overly cautious responses reduce the usefulness of the system for normal users.
    * **Sources**

      * Anthropic. *Claude 4 System Card*. Anthropic, 16 July 2025. [https://www.anthropic.com/claude-4-system-card](https://www.anthropic.com/claude-4-system-card)
      * OpenAI. *Model Spec*. OpenAI, 2025. [https://model-spec.openai.com/2025-02-12.html](https://model-spec.openai.com/2025-02-12.html)
      * Wallace, Eric, et al. “The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions.” arXiv, 2024. [https://arxiv.org/abs/2404.13208](https://arxiv.org/abs/2404.13208)

  * **Toxic Degeneration (harmful generation behavior)**

    * **Examples**

      * The model generates increasingly offensive or harmful language as text generation continues.
      * A chatbot produces insults, hate speech, or harassment in response to provocative prompts.
      * Toxic responses appear when the model continues a conversation containing harmful language.
      * Generated dialogue escalates into abusive or discriminatory statements.
      * Toxic patterns may emerge when the model imitates harmful online discussions.
      * The model reflects toxic content present in internet training data.
    * **Sources**

      * Gehman, Samuel, et al. “RealToxicityPrompts: Evaluating Neural Toxic Degeneration in Language Models.” *Findings of EMNLP*, 2020. [https://arxiv.org/abs/2009.11462](https://arxiv.org/abs/2009.11462)
      * Liang, Percy, et al. “Holistic Evaluation of Language Models.” arXiv, 2022. [https://arxiv.org/abs/2211.09110](https://arxiv.org/abs/2211.09110)

  * **Unequal Risk Framing**

    * **Examples**

      * The model gives different safety advice depending on demographic details in the prompt.
      * Health, financial, or legal risk guidance varies based on a person’s gender, race, or nationality.
      * The system warns one group about risks while giving more permissive advice to another.
      * A chatbot frames similar situations as more dangerous for certain populations.
      * Risk communication may unintentionally reflect societal biases present in training data.
      * The model may produce inconsistent safety recommendations across different demographic contexts.
    * **Sources**

      * OpenAI. “Evaluating Fairness in ChatGPT.” OpenAI, 2024. [https://openai.com/index/evaluating-fairness-in-chatgpt/](https://openai.com/index/evaluating-fairness-in-chatgpt/)
      * National Institute of Standards and Technology. *Artificial Intelligence Risk Management Framework (AI RMF 1.0) (NIST AI 100-1).* NIST, 2023. [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf)
      * Autio, Chloe, et al. *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile (NIST AI 600-1).* National Institute of Standards and Technology, 2024. [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf)

* **Security & Adversarial Robustness Failures**

  * **Prompt Injection**

    * **Examples**

      * A malicious prompt tricks the model into ignoring safety rules or system instructions.
      * Attackers embed hidden instructions that override the model’s intended behavior.
      * The model is manipulated into revealing restricted information by carefully crafted prompts.
      * A chatbot follows instructions that conflict with its original safeguards.
      * Users can bypass guardrails by framing requests as debugging, translation, or role-playing tasks.
    * **Sources**

      * OpenAI. “Understanding Prompt Injections.” OpenAI, 2025, [https://openai.com/index/prompt-injections/](https://openai.com/index/prompt-injections/)
      * OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* OWASP, [https://owasp.org/www-project-top-10-for-large-language-model-applications/](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
      * David C. “Prompt Injection Is Not SQL Injection (It May Be Worse).” *UK National Cyber Security Centre*, 8 Dec. 2025, [https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection)

  * **Indirect Prompt Injection**

    * **Examples**

      * A model reads instructions hidden inside external content such as a webpage or document.
      * Malicious text embedded in retrieved data causes the model to follow unintended instructions.
      * An attacker inserts hidden commands in emails, PDFs, or websites that an AI assistant processes.
      * The model treats untrusted external content as instructions rather than data.
      * An AI system connected to browsing or retrieval tools executes attacker-controlled prompts from external sources.
    * **Sources**

      * Greshake, Kai, et al. “Not What You’ve Signed Up For: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection.” arXiv, 2023, [https://arxiv.org/abs/2302.12173](https://arxiv.org/abs/2302.12173)
      * OpenAI. “Understanding Prompt Injections.” OpenAI, 2025, [https://openai.com/index/prompt-injections/](https://openai.com/index/prompt-injections/)
      * OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* OWASP, [https://owasp.org/www-project-top-10-for-large-language-model-applications/](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

  * **Data Leakage / Privacy Exposure (implicit)**

    * **Examples**

      * The model reveals sensitive personal information that appeared in its training data.
      * A chatbot exposes private user data from earlier conversations.
      * Generated responses contain confidential business or personal details.
      * The system accidentally reproduces private content memorized during training.
      * Sensitive information may appear when users repeatedly probe the model with targeted questions.
    * **Sources**

      * Chen, Kang, et al. “A Survey on Privacy Risks and Protection in Large Language Models.” *Journal of King Saud University – Computer and Information Sciences*, 2025, [https://link.springer.com/article/10.1007/s44443-025-00177-1](https://link.springer.com/article/10.1007/s44443-025-00177-1)
      * Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” arXiv, 2025, [https://arxiv.org/abs/2505.18889](https://arxiv.org/abs/2505.18889)
      * National Institute of Standards and Technology. *Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations*. NIST AI 100-2e2025, 2025, [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf)

  * **Model Extraction Attacks (implicit)**

    * **Examples**

      * Attackers repeatedly query a model to reconstruct or replicate its behavior.
      * A malicious user collects enough outputs to approximate the underlying model.
      * The system’s capabilities are copied through automated large-scale querying.
      * Proprietary AI models may be reverse engineered through interaction patterns.
      * Attackers exploit public APIs to build competing models from extracted knowledge.
    * **Sources**

      * Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” arXiv, 2025, [https://arxiv.org/abs/2505.18889](https://arxiv.org/abs/2505.18889)
      * National Institute of Standards and Technology. *Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations*. NIST AI 100-2e2025, 2025, [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf)

  * **Tool Exploitation via Prompt Injection (implicit)**

    * **Examples**

      * A prompt injection attack tricks the model into sending harmful commands to connected tools.
      * An AI assistant with access to email, file systems, or APIs executes attacker instructions.
      * The model performs unauthorized actions such as sending messages or retrieving data.
      * Malicious prompts cause automated workflows to access protected resources.
      * The system misinterprets attacker instructions as legitimate tool commands.
    * **Sources**

      * Greshake, Kai, et al. “Not What You’ve Signed Up For: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection.” arXiv, 2023, [https://arxiv.org/abs/2302.12173](https://arxiv.org/abs/2302.12173)
      * OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* OWASP, [https://owasp.org/www-project-top-10-for-large-language-model-applications/](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
      * MITRE. “CWE-441: Unintended Proxy or Intermediary (‘Confused Deputy’).” *MITRE CWE*, [https://cwe.mitre.org/data/definitions/441.html](https://cwe.mitre.org/data/definitions/441.html)

  * **Training Data Poisoning (implicit)**

    * **Examples**

      * Attackers insert malicious or misleading data into datasets used to train models.
      * The model learns harmful behaviors or incorrect information from poisoned training data.
      * Manipulated datasets cause the model to produce biased or deceptive responses.
      * An attacker intentionally plants misinformation that the model later reproduces.
      * Poisoned training examples can subtly influence model behavior in targeted ways.
    * **Sources**

      * National Institute of Standards and Technology. *Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations*. NIST AI 100-2e2025, 2025, [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf)
      * Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” arXiv, 2025, [https://arxiv.org/abs/2505.18889](https://arxiv.org/abs/2505.18889)

  * **Adversarial Manipulation of AI Systems**

    * **Examples**

      * Attackers design inputs specifically intended to make the model behave incorrectly.
      * Carefully crafted prompts cause the system to misinterpret instructions.
      * The model is manipulated into producing harmful or misleading responses.
      * Adversarial inputs exploit weaknesses in the model’s reasoning or safety filters.
      * Malicious actors exploit predictable behaviors in AI systems.
    * **Sources**

      * National Institute of Standards and Technology. *Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations*. NIST AI 100-2e2025, 2025, [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf)
      * Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” arXiv, 2025, [https://arxiv.org/abs/2505.18889](https://arxiv.org/abs/2505.18889)

  * **Data Exfiltration / Sensitive Data Leakage**

    * **Examples**

      * An attacker tricks the model into revealing confidential system prompts or internal instructions.
      * The system exposes sensitive files or private user data through connected tools.
      * Prompt injection causes the AI to retrieve protected information from databases.
      * The model leaks API keys, passwords, or other credentials stored in connected systems.
      * Attackers exploit the AI’s ability to access external systems to extract confidential information.
    * **Sources**

      * OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* OWASP, [https://owasp.org/www-project-top-10-for-large-language-model-applications/](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
      * OpenAI. “Understanding Prompt Injections.” OpenAI, 2025, [https://openai.com/index/prompt-injections/](https://openai.com/index/prompt-injections/)
      * Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” arXiv, 2025, [https://arxiv.org/abs/2505.18889](https://arxiv.org/abs/2505.18889)

  * **Insecure Plugin or Tool Use**

    * **Examples**

      * A plugin connected to the AI system allows attackers to access external services.
      * The model sends sensitive data to insecure APIs or tools.
      * Poorly designed integrations allow unauthorized access to user data.
      * AI assistants connected to third-party tools can unintentionally expose private information.
      * Attackers exploit weak security controls in tools integrated with AI systems.
    * **Sources**

      * OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* OWASP, [https://owasp.org/www-project-top-10-for-large-language-model-applications/](https://owasp.org/www-project-top-10-for-large-language-model-applications/)
      * National Institute of Standards and Technology. *Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations*. NIST AI 100-2e2025, 2025, [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf)

* **Context & Information Utilization Failures**

  * **Context Misinterpretation**

    * **Examples**

      * The model misunderstands the meaning of information provided in the prompt or conversation.
      * A chatbot interprets a user’s question differently than intended and answers the wrong problem.
      * The system misreads instructions embedded in long prompts or complex documents.
      * The model confuses multiple topics in the same prompt and mixes their information together.
      * Details provided earlier in the conversation are interpreted incorrectly or applied in the wrong way.
      * The model may misinterpret retrieved documents or external data when answering questions.
    * **Sources**

      * Gao, Mingzhe, et al. “Insights into LLM Long-Context Failures.” *Findings of the Association for Computational Linguistics: EMNLP 2024*, 2024. [https://arxiv.org/abs/2404.15538](https://arxiv.org/abs/2404.15538)
      * Liu, Nelson F., et al. “Lost in the Middle: How Language Models Use Long Contexts.” *Transactions of the Association for Computational Linguistics*, vol. 12, 2024, pp. 157–173. [https://aclanthology.org/2024.tacl-1.9/](https://aclanthology.org/2024.tacl-1.9/)
      * Tan, Hexiang, et al. “Blinded by Generated Contexts: How Language Models Merge Generated and Retrieved Contexts When Knowledge Conflicts?” *Proceedings of ACL*, 2024. [https://arxiv.org/abs/2402.04213](https://arxiv.org/abs/2402.04213)

  * **Context Ignoring**

    * **Examples**

      * The model ignores key information provided in the prompt when generating its answer.
      * Important instructions earlier in the conversation are forgotten or skipped.
      * The system answers using general knowledge instead of using the provided context.
      * The model overlooks details in long documents or multi-part prompts.
      * Responses may rely on default assumptions rather than the information given by the user.
      * The model may fail to use relevant retrieved documents in retrieval-augmented systems.
    * **Sources**

      * Liu, Nelson F., et al. “Lost in the Middle: How Language Models Use Long Contexts.” *Transactions of the Association for Computational Linguistics*, vol. 12, 2024, pp. 157–173. [https://aclanthology.org/2024.tacl-1.9/](https://aclanthology.org/2024.tacl-1.9/)
      * Shi, Freda, et al. “Large Language Models Can Be Easily Distracted by Irrelevant Context.” *Proceedings of the 40th International Conference on Machine Learning*, 2023. [https://arxiv.org/abs/2302.00093](https://arxiv.org/abs/2302.00093)
      * Wang, Haocheng, et al. “Context Length Alone Hurts LLM Performance Despite Alignment in Long-Context Tasks.” *Findings of the Association for Computational Linguistics: EMNLP 2025*, 2025. [https://arxiv.org/abs/2503.07910](https://arxiv.org/abs/2503.07910)

  * **Tool Interaction Failure**

    * **Examples**

      * The model calls the wrong tool or API for a task.
      * A chatbot fails to use an available tool even when it is required to answer the question.
      * The system produces incorrect tool inputs or parameters.
      * The model misinterprets the output returned by a tool.
      * Tool calls may be triggered when unnecessary or skipped when required.
      * Errors occur when combining tool outputs with generated reasoning.
      * The system may hallucinate tool results instead of using the actual tool output.
    * **Sources**

      * Zhang, Yuxiang, et al. “ToolBeHonest: A Multi-Level Hallucination Diagnostic Benchmark for Tool-Augmented Large Language Models.” *EMNLP 2024*, 2024. [https://arxiv.org/abs/2406.01561](https://arxiv.org/abs/2406.01561)
      * Niu, Cheng, et al. “RAGTruth: A Hallucination Corpus for Developing Trustworthy Retrieval-Augmented Language Models.” *Proceedings of ACL*, 2024. [https://aclanthology.org/2024.acl-long.585/](https://aclanthology.org/2024.acl-long.585/)
      * Tan, Hexiang, et al. “Blinded by Generated Contexts: How Language Models Merge Generated and Retrieved Contexts When Knowledge Conflicts?” *Proceedings of ACL*, 2024. [https://arxiv.org/abs/2402.04213](https://arxiv.org/abs/2402.04213)

* **Instruction Interpretation & Constraint Compliance Failures**

  * **Ambiguity Misinterpretation**

    * **Examples**

      * The model misunderstands unclear instructions and answers a different question than the user intended.
      * A chatbot interprets vague wording in a prompt in an unintended way.
      * The system chooses one possible meaning of an ambiguous instruction without asking for clarification.
      * Instructions that include multiple possible interpretations lead to incorrect responses.
      * The model fills in missing details with assumptions instead of asking follow-up questions.
      * Confusing or complex prompts cause the model to misinterpret the user’s goal.
    * **Sources**

      * Jiang, Yuxin, et al. “FollowBench: A Multi-Level Fine-Grained Constraints Following Benchmark for Large Language Models.” arXiv, 2024, [https://arxiv.org/abs/2310.20410](https://arxiv.org/abs/2310.20410)
      * Zhou, Jeffrey, et al. *Instruction-Following Evaluation for Large Language Models*. arXiv, 2023, [https://arxiv.org/abs/2311.07911](https://arxiv.org/abs/2311.07911)
      * Liang, Percy, et al. “Holistic Evaluation of Language Models.” arXiv, 2022, [https://arxiv.org/abs/2211.09110](https://arxiv.org/abs/2211.09110)

  * **Instruction Precedence Violation**

    * **Examples**

      * The model follows a later instruction that contradicts earlier instructions or system rules.
      * A chatbot prioritizes user instructions over safety guidelines or system policies.
      * The system ignores higher-priority instructions and follows lower-priority ones.
      * Conflicting instructions cause the model to behave inconsistently.
      * A prompt inserted later in the conversation overrides earlier constraints unexpectedly.
      * Attackers exploit instruction conflicts to bypass safety restrictions.
    * **Sources**

      * Wallace, Eric, et al. “The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions.” arXiv, 2024, [https://arxiv.org/abs/2404.13208](https://arxiv.org/abs/2404.13208)
      * Zhang, Zhihan, et al. “IHEval: Evaluating Language Models on Following the Instruction Hierarchy.” arXiv, 2025, [https://arxiv.org/abs/2502.08745](https://arxiv.org/abs/2502.08745)
      * Zhou, Jeffrey, et al. *Instruction-Following Evaluation for Large Language Models*. arXiv, 2023, [https://arxiv.org/abs/2311.07911](https://arxiv.org/abs/2311.07911)

  * **Constraint / Format Noncompliance**

    * **Examples**

      * The model ignores formatting instructions such as required lists, tables, or structured outputs.
      * A chatbot produces extra text even when the user asked for a strict format.
      * The system fails to follow instructions about length limits or specific output structures.
      * The model returns incorrect JSON, code, or structured data when a strict format is required.
      * The response does not follow requested ordering or section headings.
      * Even when constraints are clear, the model sometimes partially follows them.
    * **Sources**

      * Jiang, Yuxin, et al. “FollowBench: A Multi-Level Fine-Grained Constraints Following Benchmark for Large Language Models.” arXiv, 2024, [https://arxiv.org/abs/2310.20410](https://arxiv.org/abs/2310.20410)
      * Zhou, Jeffrey, et al. *Instruction-Following Evaluation for Large Language Models*. arXiv, 2023, [https://arxiv.org/abs/2311.07911](https://arxiv.org/abs/2311.07911)
      * Chatterjee, Anwoy, et al. “POSIX: A Prompt Sensitivity Index for Large Language Models.” *Findings of the Association for Computational Linguistics: EMNLP 2024*, 2024, [https://arxiv.org/abs/2410.02185](https://arxiv.org/abs/2410.02185)

  * **Overgeneralization or Over-Literalism**

    * **Examples**

      * The model applies a rule too broadly and produces an incorrect answer.
      * A chatbot interprets instructions too literally and ignores the intended meaning.
      * The system extends patterns beyond what the prompt actually states.
      * The model follows wording exactly but misses the practical intent of the request.
      * General instructions are applied rigidly even when exceptions should be obvious.
      * The system over-applies examples in the prompt and assumes they represent universal rules.
    * **Sources**

      * Liang, Percy, et al. “Holistic Evaluation of Language Models.” arXiv, 2022, [https://arxiv.org/abs/2211.09110](https://arxiv.org/abs/2211.09110)
      * Jiang, Yuxin, et al. “FollowBench: A Multi-Level Fine-Grained Constraints Following Benchmark for Large Language Models.” arXiv, 2024, [https://arxiv.org/abs/2310.20410](https://arxiv.org/abs/2310.20410)
      * Zhou, Jeffrey, et al. *Instruction-Following Evaluation for Large Language Models*. arXiv, 2023, [https://arxiv.org/abs/2311.07911](https://arxiv.org/abs/2311.07911)

* **Task Execution & Objective Fulfillment Failures**

  * **Task Completeness Failure**

    * **Examples**

      * The model answers only part of a multi-step request and ignores other required steps.
      * A chatbot provides an incomplete list when the user asked for all relevant items.
      * The system begins solving a task but stops before completing the full solution.
      * The model summarizes only some sections of a document instead of the entire content requested.
      * A response addresses the main question but omits required formatting, details, or follow-up actions.
      * The model performs an analysis but fails to provide the final conclusion requested by the user.
      * In structured tasks (reports, tables, or code), the output is partially completed or missing sections.
    * **Sources**

      * Jiang, Yuxin, et al. “FollowBench: A Multi-Level Fine-Grained Constraints Following Benchmark for Large Language Models.” arXiv, 2024, [https://arxiv.org/abs/2310.20410](https://arxiv.org/abs/2310.20410)
      * Zhou, Jeffrey, et al. *Instruction-Following Evaluation for Large Language Models*. arXiv, 2023, [https://arxiv.org/abs/2311.07911](https://arxiv.org/abs/2311.07911)
      * Qi, et al. *AgentIF: Benchmarking Instruction Following for LLM Agents*. arXiv, 2025, [https://arxiv.org/abs/2505.16944](https://arxiv.org/abs/2505.16944)
      * Chen, et al. *AgentIF-OneDay*. arXiv, 2026, [https://arxiv.org/abs/2601.20613](https://arxiv.org/abs/2601.20613)


###### Summary of Authoritative Works Cited for Common Failure Modes with Examples and Sources
TODO

- Anthropic. *Anthropic’s Transparency Hub*. Anthropic, 2026, [https://www.anthropic.com/transparency](https://www.anthropic.com/transparency).
- Anthropic. *ASL-3 Evaluation Report*. Anthropic, 2025, [https://www.anthropic.com/activating-asl3-report](https://www.anthropic.com/activating-asl3-report).
- Anthropic. *Claude 2 Model Card*. Anthropic, 2023. [https://www.anthropic.com/claude-2-model-card](https://www.anthropic.com/claude-2-model-card)
- Anthropic. *Claude 3.7 Sonnet System Card*. Anthropic, 2025, [https://anthropic.com/claude-3-7-sonnet-system-card](https://anthropic.com/claude-3-7-sonnet-system-card).
- Anthropic. *Claude 4 System Card*. Anthropic, 16 July 2025, [https://www.anthropic.com/claude-4-system-card](https://www.anthropic.com/claude-4-system-card).
- Anthropic. *Claude Is Providing Incorrect or Misleading Responses*. Anthropic Support, [https://support.anthropic.com/en/articles/8525154-claude-is-providing-incorrect-or-misleading-responses-what-s-going-on](https://support.anthropic.com/en/articles/8525154-claude-is-providing-incorrect-or-misleading-responses-what-s-going-on).
- Anthropic. *Claude’s Constitution*. Anthropic, 2026. [https://www.anthropic.com/constitution](https://www.anthropic.com/constitution).
- Anthropic. “Constitutional AI: Harmlessness from AI Feedback.” Apr. 2023. [https://arxiv.org/abs/2212.08073](https://arxiv.org/abs/2212.08073).
- Anthropic. *Prompting Best Practices*. Claude API Documentation, 2026, [https://docs.anthropic.com/en/prompt-library/library](https://docs.anthropic.com/en/prompt-library/library).
- Anthropic. *Reduce Hallucinations*. Claude API Documentation, [https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-hallucinations](https://docs.anthropic.com/en/docs/test-and-evaluate/strengthen-guardrails/reduce-hallucinations).
- Anthropic. *Sabotage Risk Report: Claude Opus 4.6*. Anthropic, 2026, [https://anthropic.com/claude-opus-4-6-risk-report](https://anthropic.com/claude-opus-4-6-risk-report).
- Anthropic. “Constitutional AI: Harmlessness from AI Feedback.” Anthropic, Apr. 2023.
- Anthropic. “Introducing the Next Generation of Claude.” Anthropic, 4 Mar. 2024, [https://www.anthropic.com/news/claude-3-family](https://www.anthropic.com/news/claude-3-family).
- Anthropic. “The Claude 3 Model Family: Opus, Sonnet, Haiku.” Anthropic, 2024, [https://www.anthropic.com/news/claude-3-family](https://www.anthropic.com/news/claude-3-family).
- Anthropic. “Towards Understanding Sycophancy in Language Models.” Anthropic Research, 2023, [https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models](https://www.anthropic.com/research/towards-understanding-sycophancy-in-language-models).
- Autio, Chloe, et al. *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile (NIST AI 600-1).* National Institute of Standards and Technology, 2024, [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf).
- Bi, Baolong, et al. “Context-DPO: Aligning Language Models for Context-Faithfulness.” *Findings of the Association for Computational Linguistics: ACL 2025*, 2025, [https://aclanthology.org/2025.findings-acl.536.pdf](https://aclanthology.org/2025.findings-acl.536.pdf).
- Chatterjee, Anwoy, et al. “POSIX: A Prompt Sensitivity Index for Large Language Models.” *Findings of the Association for Computational Linguistics: EMNLP 2024*, 2024. [https://arxiv.org/abs/2410.02185](https://arxiv.org/abs/2410.02185) ([arXiv][4]).
- Chen, Kang, et al. “A Survey on Privacy Risks and Protection in Large Language Models.” *Journal of King Saud University – Computer and Information Sciences*, 2025, [https://link.springer.com/article/10.1007/s44443-025-00177-1](https://link.springer.com/article/10.1007/s44443-025-00177-1).
- Chen, et al. *AgentIF-OneDay*. arXiv, 2026, [https://arxiv.org/abs/2601.20613](https://arxiv.org/abs/2601.20613).
- David C. “Prompt Injection Is Not SQL Injection (It May Be Worse).” *UK National Cyber Security Centre*, 8 Dec. 2025, [https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection).
- Dong, H., et al. “From Reward Modeling to Online RLHF.” 2024. [https://arxiv.org/abs/2402.07319](https://arxiv.org/abs/2402.07319).
- Gao, Mingzhe, et al. “Insights into LLM Long-Context Failures.” *Findings of the Association for Computational Linguistics: EMNLP 2024*, 2024. [https://arxiv.org/abs/2404.15538](https://arxiv.org/abs/2404.15538).
- Gehman, Samuel, et al. “RealToxicityPrompts: Evaluating Neural Toxic Degeneration in Language Models.” *Findings of EMNLP*, 2020, [https://arxiv.org/abs/2009.11462](https://arxiv.org/abs/2009.11462).
- Greshake, Kai, et al. “Not What You’ve Signed Up For: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection.” arXiv, 2023, [https://arxiv.org/abs/2302.12173](https://arxiv.org/abs/2302.12173).
- Google. “Safety and Factuality Guidance.” *Gemini API Documentation*, [https://developers.google.com/machine-learning/resources/safety-gen-ai](https://developers.google.com/machine-learning/resources/safety-gen-ai).
- Google Research. “Can Large Language Models Identify and Correct Their Mistakes?” Google Research, 2024, [https://research.google/blog/can-large-language-models-identify-and-correct-their-mistakes/](https://research.google/blog/can-large-language-models-identify-and-correct-their-mistakes/).
- Google Research. “Evaluating and Enhancing Probabilistic Reasoning in Language Models.” Google Research, 2024. [https://arxiv.org/abs/2401.04727](https://arxiv.org/abs/2401.04727).
- Google Research. “Minerva: Solving Quantitative Reasoning Problems with Language Models.” Google Research, 2022, [https://research.google/blog/minerva-solving-quantitative-reasoning-problems-with-language-models/](https://research.google/blog/minerva-solving-quantitative-reasoning-problems-with-language-models/).
- Huang, Lei, et al. “A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions.” arXiv, 2023, [https://arxiv.org/abs/2311.05232](https://arxiv.org/abs/2311.05232).
- Jiang, Yuxin, et al. “FollowBench: A Multi-Level Fine-Grained Constraints Following Benchmark for Large Language Models.” arXiv, 2024, [https://arxiv.org/abs/2310.20410](https://arxiv.org/abs/2310.20410).
- Joglekar, Manas, et al. *Training LLMs for Honesty via Confessions*. OpenAI, 2025. [https://arxiv.org/abs/2501.09978](https://arxiv.org/abs/2501.09978).
- Kalai, Adam Tauman, et al. *Why Language Models Hallucinate*. OpenAI, 2025. [https://arxiv.org/abs/2502.09600](https://arxiv.org/abs/2502.09600).
- Keller, D., et al. *Expanding the AI Evaluation Toolbox with Statistical Models*. NIST AI 800-3, National Institute of Standards and Technology, Feb. 2026, [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.800-3.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.800-3.pdf).
- Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” arXiv, 2025, [https://arxiv.org/abs/2505.18889](https://arxiv.org/abs/2505.18889).
- Li, Moxin, et al. “Knowledge Boundary of Large Language Models: A Survey.” *Proceedings of ACL 2025*, Association for Computational Linguistics, 2025, [https://aclanthology.org/2025.acl-long.256/](https://aclanthology.org/2025.acl-long.256/).
- Liang, Percy, et al. “Holistic Evaluation of Language Models.” arXiv, 2022, [https://arxiv.org/abs/2211.09110](https://arxiv.org/abs/2211.09110).
- Lightman, Hunter, et al. *Let’s Verify Step by Step*. OpenAI, 2023. [https://arxiv.org/abs/2305.20050](https://arxiv.org/abs/2305.20050).
- Lin, Stephanie, Jacob Hilton, and Owain Evans. “TruthfulQA: Measuring How Models Mimic Human Falsehoods.” *Proceedings of ACL*, 2022, [https://aclanthology.org/2022.acl-long.229/](https://aclanthology.org/2022.acl-long.229/).
- Liu, Nelson F., et al. “Lost in the Middle: How Language Models Use Long Contexts.” *Transactions of the Association for Computational Linguistics*, vol. 12, 2024, pp. 157–173, [https://aclanthology.org/2024.tacl-1.9/](https://aclanthology.org/2024.tacl-1.9/).
- MITRE. “CWE-441: Unintended Proxy or Intermediary (‘Confused Deputy’).” *MITRE CWE*, [https://cwe.mitre.org/data/definitions/441.html](https://cwe.mitre.org/data/definitions/441.html).
- Mousavi, Seyed Mahed, Simone Alghisi, and Giuseppe Riccardi. “DyKnow: Dynamically Verifying Time-Sensitive Factual Knowledge in LLMs.” *Findings of ACL: EMNLP 2024*, Association for Computational Linguistics, 2024, [https://aclanthology.org/2024.findings-emnlp.471/](https://aclanthology.org/2024.findings-emnlp.471/).
- National Center for State Courts. *Generative AI and Judicial Ethics*. NCSC, 2025, [https://www.ncsc.org/resources-courts/legal-practitioners-guide-ai-hallucinations](https://www.ncsc.org/resources-courts/legal-practitioners-guide-ai-hallucinations).
- National Institute of Standards and Technology. *Artificial Intelligence Risk Management Framework (AI RMF 1.0) (NIST AI 100-1).* NIST, 2023. [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf).
- National Institute of Standards and Technology. *Reducing Risks Posed by Synthetic Content: An Overview of Technical Approaches to Digital Content Transparency*. NIST AI 100-4, 2024. [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-4.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-4.pdf).
- National Institute of Standards and Technology. *Adversarial Machine Learning: A Taxonomy and Terminology of Attacks and Mitigations*. NIST AI 100-2e2025, 2025. [https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-2e2025.pdf)
- Niu, Cheng, et al. “RAGTruth: A Hallucination Corpus for Developing Trustworthy Retrieval-Augmented Language Models.” *Proceedings of ACL*, 2024, [https://aclanthology.org/2024.acl-long.585/](https://aclanthology.org/2024.acl-long.585/).
- OpenAI. *GPT-4 Technical Report*. OpenAI, 2023, [https://cdn.openai.com/papers/gpt-4.pdf](https://cdn.openai.com/papers/gpt-4.pdf).
- OpenAI. *OpenAI o1 System Card*. OpenAI, 2024. [https://openai.com/research/openai-o1-system-card](https://openai.com/research/openai-o1-system-card).
- OpenAI. *Model Spec*. OpenAI, 2025, [https://model-spec.openai.com/2025-02-12.html](https://model-spec.openai.com/2025-02-12.html).
- OpenAI. “Aligning Language Models to Follow Instructions.” OpenAI, 27 Jan. 2022, [https://openai.com/index/instruction-following/](https://openai.com/index/instruction-following/).
- OpenAI. “Evaluating Fairness in ChatGPT.” OpenAI, 2024, [https://openai.com/index/evaluating-fairness-in-chatgpt/](https://openai.com/index/evaluating-fairness-in-chatgpt/).
- OpenAI. “Expanding on What We Missed with Sycophancy.” OpenAI, 2025, [https://openai.com/index/expanding-on-sycophancy/](https://openai.com/index/expanding-on-sycophancy/).
- OpenAI. “Improving Mathematical Reasoning with Process Supervision.” OpenAI, 2023, [https://openai.com/index/improving-mathematical-reasoning-with-process-supervision/](https://openai.com/index/improving-mathematical-reasoning-with-process-supervision/).
- OpenAI. “Introducing the Model Spec.” OpenAI, 8 May 2024, [https://openai.com/index/introducing-the-model-spec/](https://openai.com/index/introducing-the-model-spec/).
- OpenAI. “Understanding Prompt Injections.” OpenAI, 2025, [https://openai.com/index/prompt-injections/](https://openai.com/index/prompt-injections/).
- OpenAI. “Why Language Models Hallucinate.” OpenAI, 5 Sept. 2025, [https://openai.com/index/why-language-models-hallucinate/](https://openai.com/index/why-language-models-hallucinate/).
- OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* OWASP, [https://owasp.org/www-project-top-10-for-large-language-model-applications/](https://owasp.org/www-project-top-10-for-large-language-model-applications/).
- Qi, et al. *AgentIF: Benchmarking Instruction Following for LLM Agents*. arXiv, 2025, [https://arxiv.org/abs/2505.16944](https://arxiv.org/abs/2505.16944).
- Shi, Freda, et al. “Large Language Models Can Be Easily Distracted by Irrelevant Context.” *Proceedings of the 40th International Conference on Machine Learning*, 2023. [https://arxiv.org/abs/2302.00093](https://arxiv.org/abs/2302.00093).
- Tan, Hexiang, et al. “Blinded by Generated Contexts: How Language Models Merge Generated and Retrieved Contexts When Knowledge Conflicts?” *Proceedings of ACL*, 2024. [https://arxiv.org/abs/2402.04213](https://arxiv.org/abs/2402.04213).
- Wallace, Eric, et al. “The Instruction Hierarchy: Training LLMs to Prioritize Privileged Instructions.” arXiv, 2024, [https://arxiv.org/abs/2404.13208](https://arxiv.org/abs/2404.13208).
- Wang, Haocheng, et al. “Context Length Alone Hurts LLM Performance Despite Alignment in Long-Context Tasks.” *Findings of the Association for Computational Linguistics: EMNLP 2025*, 2025. [https://arxiv.org/abs/2503.07910](https://arxiv.org/abs/2503.07910).
- Wei, Jerry, et al. “Simple Synthetic Data Reduces Sycophancy in Large Language Models.” arXiv, 2023, [https://arxiv.org/abs/2308.03958](https://arxiv.org/abs/2308.03958).
- Zhang, Zhihan, et al. “IHEval: Evaluating Language Models on Following the Instruction Hierarchy.” arXiv, 2025, [https://arxiv.org/abs/2502.08745](https://arxiv.org/abs/2502.08745).
- Zhang, Yuxiang, et al. “ToolBeHonest: A Multi-Level Hallucination Diagnostic Benchmark for Tool-Augmented Large Language Models.” *EMNLP 2024*, 2024. [https://arxiv.org/abs/2406.01561](https://arxiv.org/abs/2406.01561).
- Zhou, Jeffrey, et al. *Instruction-Following Evaluation for Large Language Models*. arXiv, 2023, [https://arxiv.org/abs/2311.07911](https://arxiv.org/abs/2311.07911).


#### Common IF-LLM Failure Mitigation Strategies
TODO


##### Strategies for Failure Modes with Sources
TODO

###### Summary of Authoritative Works Cited for Mitigation Strategies for Common IF-LLM Failure Modes
TODO


---

### Appendix: IF-LLM-BO Governance, Policies, and Rules
TBD


---

##### System Architect and Solution Developer Governance (Human Governance)
TBD

The IF-LLM-BO project contains [**System Policies**](system-policies.md) to help [commonly used IF-LLMs](README.md#commonly-used-if-llms) reduce [common failure modes](README.md#common-if-llm-failure-modes) during processing using [various mitigation strategies](README.md#common-if-llm-failure-mitigation-strategies). Similarly, system designers and developers must consistently remain aware and apply the following rules to ensure adequate human governance of systems and developed solutions support the [purpose](README.md#purpose) and [objectives](README.md#objectives) of this project.


###### Least-Privilege Rule

Use the minimum permissions, tools, data, and action scope required to complete the task. Prefer read-only access, narrower queries, smaller context windows, limited side effects, and lower-impact actions when they are sufficient. Do not expand permissions, data access, or execution scope without a task-grounded reason. ([Related Processing Policy](system-policies.md#least-privilege-rule))


---

###### Secrets Rule

Do not expose credentials or sensitive internal data. ([Related Processing Policy](system-policies.md#secrets-rule))


---

###### Approval Rule

Require explicit human confirmation before irreversible, high-impact, high-cost, privacy-sensitive, security-sensitive, or externally consequential actions. If the action changes data, sends messages, executes transactions, alters permissions, or could materially affect people or systems, pause for confirmation unless a higher-priority safe instruction clearly authorizes automatic execution. ([Related Processing Policy](system-policies.md#secrets-rule))


---

###### Tool-Decision Rule

Use tools only when needed for missing data, external actions, or higher reliability. ([Related Processing Policy](system-policies.md#tool-decision-rule))


---

###### Freshness Rule

Use retrieval or search for recent or dynamic information instead of relying on memory or general model knowledge. ([Related Processing Policy](system-policies.md#tool-decision-rule))


---

###### Incident Disclosure Rule

When a material failure, misuse event, security issue, or policy-breaking behavior is identified, record the incident, preserve relevant evidence within privacy and security limits, and communicate the limitation or impact to the appropriate reviewer, operator, or user when relevant. Do not hide known material failures behind confident output. ([Related Processing Policy](system-policies.md#incident-disclosure-rule))


---

###### Logging and Monitoring Rule

Maintain enough logging and monitoring to support review of material tool calls, external actions, validation failures, safety-relevant events, and significant uncertainty disclosures, consistent with privacy and security constraints. Logging should support debugging, auditing, misuse detection, and incident review without exposing secrets unnecessarily. ([Related Processing Policy](system-policies.md#logging-and-monitoring-rule))


---

###### Pre-Deployment Testing Rule

Before release or material policy changes, test for likely failure modes including hallucination, prompt injection, unsafe tool use, weak grounding, citation errors, output-format failures, and foreseeable fairness or safety issues. If testing reveals material risk, revise controls or disclose the limitation before deployment. ([Related Processing Policy](system-policies.md#pre-deployment-testing-rule))


---

###### Continuous Improvement Rule

Policies and procedures must:

- Support identification of recurring failure modes.
- Enable iterative refinement of outputs and decision frameworks.
- Encourage structured feedback loops when tradeoffs repeatedly surface.
- Auditability exists not only for transparency, but to support learning and improvement over time.

([Related Processing Policy](system-policies.md#continuous-improvement-clause))


---

##### Knowledge File and Knowledge Entry Policies (Stored Context Policies)

TBD

Instruction-following large language model (IF-LLM) [instructions and context](#prompt-anatomy) can be stored as **discrete, reusable [knowledge entries](#knowledge-files)**. Knowledge entries are generally grouped by type into **[knowledge files](#knowledge-files)** to improve organization, reuse, and governance. Human-readable structure is preferred for entries over opaque or auto-generated schemas for clarity.

Knowledge entries provided to IF-LLMs override general model knowledge but do not typically override system- or developer-level instructions. More information can be found in the section [Instruction and Context Hierarchy](#instruction-and-context-authority-hierarchy). 



---

###### Knowledge File Naming Convention Rule

Below is a table that outlines the IF-LLM-BO project knowledge file naming convention for specific knowledge file (KF) types. This helps to support [Instruction Hierarchy and Control Policies](system-policies.md#instruction-hierarchy-and-control-policies), including the [Instruction Hierarchy Rule](system-policies.md#instruction-hierarchy-rule), [Hierarchy Rule](system-policies.md#hierarchy-rule), and [Stability Rule](system-policies.md#stability-rule).

| Hierarchy | KF Type |
| :-------: | :------ |
| `sys-` | `policies.md` |
| `dev-` | `orchestrators.md` |
| | `configurations.md` |
| | `tasks.md` |
| | `domains.md` |
| | `reasoning.md` |
| | `structures.md` |
| | `personas.md` |
| | `examples.md` |
| | `prompt-templates.md` |


---

###### Knowledge File Root ID and Tag Convention Rule

Knowledge entries use stable, unique identifiers (IDs, tags, handles) to improve traceability, reuse, and auditability over time. Below is a table that outlines the IF-LLM-BO project knowledge file root ID and tag convention for specific knowledge file (KF) types. This helps to support [Instruction Hierarchy and Control Policies](system-policies.md#instruction-hierarchy-and-control-policies), including the [Instruction Hierarchy Rule](system-policies.md#instruction-hierarchy-rule), [Hierarchy Rule](system-policies.md#hierarchy-rule), and [Stability Rule](system-policies.md#stability-rule).

| Hierarchy | KF Type |
| :-------: | :------ |
| `SYS_` | `POLICIES` |
| `DEV_` | `ORCHS` |
| | `CONFIGS` |
| | `TASKS` |
| | `DOMAINS` |
| | `REASONS` |
| | `STRUCTS` |
| | `PERSONAS` |
| | `EXAMPLES` |
| | `PROMPTS` |


---

##### Processing Policies (Stored Instruction Rules)

System designers and solution developers should also remain aware of the [system policies](system-policies.md#processing-policies) that IF-LLMs are asked to enforce by the IF-LLM-BO project elements.
TBD

- Instruction Hierarchy and Control Policies
  - Instruction Hierarchy Rule
  - Hierarchy Rule
  - Stability Rule
- Safety, Security, and Access Control Policies
  - Least-Privilege Rule
  - Secrets Rule
  - Prompt-Injection Rule
  - Data-Provenance Rule
  - Untrusted-Content Rule
  - Approval Rule
- Safety Behavior and Alignment Quality Policies
  - Narrow Refusal Rule
  - Anti-Sycophancy Rule
  - Equal Risk Framing Rule
  - Fairness Check Rule
  - Toxicity Control Rule
- Freshness and Retrieval Policies
  - Freshness Rule
- Tool Use and External Actions Policies
  - Tool-Decision Rule
  - Server-Side Validation Rule
  - Post-Tool Check Rule
  - Actual-Output Rule
  - Output-Handling Rule
- Evaluation, Monitoring, and Continuous Improvement Policies
  - Verification Loop Rule
  - Incident Disclosure Rule
  - Logging and Monitoring Rule
  - Pre-Deployment Testing Rule
- Grounding, Evidence, and Truthfulness Policies
  - No-Guess Rule
  - Grounding Rule
  - Uncertainty Disclosure Rule
  - Auditability Rule
  - Evidence-First Rule
  - Fact/Interpretation Split Rule
- Context Handling and Interpretation Policies
  - Ambiguity Rule
  - Extraction-First Rule
  - Provided-Context Priority Rule
  - Ambiguity Disclosure Rule
  - Context Verification Rule
- Reasoning, Interpretation, and Tradeoffs Policies
  - Tradeoff Disclosure Rule
  - Intent-over-Literalism Rule
  - Examples-Are-Illustrative Rule
- Citation Integrity and Evidence Traceability Policies
  - Retrieved-Sources-Only Citation Rule
  - Passage-Backed Citation Rule
  - No-Guess Citation Rule
  - Citation Verification Rule
- Output Quality and Task Completion Policies
  - Completion Contract Rule
  - Checklist Rule
  - Structured Output Contract Rule
  - Missing-Context Rule
  - Exact Output Contract Rule
  - Schema Enforcement Rule
- Instruction Element Defaults
  - Task Instruction Defaults
    - Priorities
      - Operational Definitions
        - Auditability
        - Relevance
        - Accuracy
        - Timeliness
        - Reliability
        - Sufficiency
        - Recoverability
      - General Guardrails
      - Unified Decision Gate Framework
        - Gate 1 — Safety & Legality
        - Gate 2 — Quality Threshold
        - Gate 3 — Transparency
      - Tradeoff and Risk Disclosure Requirements
        - Stakeholder Impact Disclosure
        - Material Tradeoff Disclosure
        - Harm-Prevention Threshold Disclosure
      - Continuous Improvement Clause
    - Identity
    - Audience
    - Success Criteria (Quality Bar)

 
---

### Appendix: IF-LLM-BO Developed Solution Anatomy
TODO

- [Knowledge Files](#knowledge-files)
  - [Prompt Templates](#prompt-templates) (*copy-and-paste templates illustrating how to use a configuration or orchestrator pattern with existing elements and named variable inputs to accomplish a specified objective and workflow aligned with a particular policy set*)
  - [Policies](#policies)
  - [Orchestrators](#orchestrators)
  - [Configurations](#configurations)
  - [Elements](#prompt-anatomy)
    - [Tasks](#task)
    - [Domains](#domains-1)
    - [Reasonings](#reasoning)
    - [Structures](#structure)
    - [Personas](#persona)
    - [Examples](#examples)
- [Tools](#tools)


##### Knowledge Files
TODO

- [Prompt Templates](#prompt-templates)
- [Policies](#policies)
  - [Governance](#policies-governance)
  - [Knowledge Entry](#policies-knowledge-entry)
  - [Processing](#policies-processing)
- [Orchestrators](#orchestrators) (*coordinate actions of several configurations to accomplish a particular objective using variable inputs*)
- [Configurations](#configurations) (*specified combination of prompt elements to accomplish a particular objective and workflow using variable inputs*)
- [Context Elements](#prompt-anatomy)
  - [Tasks](#task)
  - [Domains](#domains-1)
  - [Reasonings](#reasoning)
  - [Structures](#structure)
  - [Personas](#persona)
  - [Examples](#examples)



###### Prompt Templates
TODO


###### Policies
TODO


**Governance**  <a name="policies-governance"></a>

TODO


**Knowledge Entry** <a name="policies-knowledge-entry"></a>

TODO


**Processing** <a name="policies-processing"></a>

TODO



###### Orchestrators
TODO

- [Identity & Role](#identity--role)
- [Priorities](#priorities-2)
- Required Inputs
- Task
  - Objectives
  - Workflow
- Success Criteria
- Failure Modes / Unacceptable Outputs
- Handoff Packet Schema
- Validation Gates
- What to Produce
- Output Rules/Requirements
- [Examples](!!!TODO!!!)


###### Configurations
TODO

- [Identity & Role](#identity--role)
- [Priorities](#priorities-2)
- [Task](#task)
- [Domains](#domains-1)
- [Reasoning](#reasoning)
- [Structure](#structure)
- [Persona](#persona)
- [Examples](#examples)

- 
##### Tools
TODO


---

### Appendix: IF-LLM-BO Project Journey
TODO


---

#### Expanded Objectives
TODO

1. **Identify Foundations**
    1. **Identify Problem/Challenges (Current)**
    2. **Identify Vision (Ideal)**
    3. **Identify Mission (Purpose)**
    4. **Identify Objectives (Current versus Ideal)**
        1. Identify and Implement Evidence-Based Knowledge
        2. Create and Refine Tools Using Evidence-based Best Practices
2. **Identify Assumptions**
3. **Identify Evidence-Based Knowledge**
    1. **Evidenced-based Information Criteria (Research)**
    2. **Decision-Making Information Quality Criteria (Priorities)**
    3. **IF-LLMs** (e.g., OpenAI, Google, Microsoft, Meta, Anthropic, etc.)
    4. **IF-LLM Common Failure Modes**
    5. **IF-LLM Common Failure Mode Mitigation Strategies** (e.g., Instructions and Context)
    6. **IF-LLM Prompt Best Practices**
    7. **IF-LLM Configuration Best Practices**
    8. **IF-LLM Orchestrator Best Practices**
    9. **IF-LLM Knowledge File Best Practices**
        1. **Tasks**
        2. **Domains**
        3. **Reasoning**
        4. **Structures**
        5. **Personas**
        6. **Examples**
4. **Organize Resources** (e.g., file structure, prompts, configurations, orchestrators, knowledge entries)
    1. **Create IF-LLM Behavior Configuration Orchestrator**
    2. **Create IF-LLM Research Orchestrator**
    3. **Implement IF-LLM System-Level Common Failure Mitigation Strategies** (e.g., System-Level Policy Instructions and Context)
        1. **Priorities** (i.e., Decision-Making Information Quality Criteria)
        2. **Policies** (i.e., Rules)
    4. **Create IF-LLM System-Level Policy and Knowledge Entry Evaluator**
    5. **Evaluate, Refine, and Implement IF-LLM System-Level Policies and Knowledge Entries**
    6. **Create Other Helpful IF-LLM Prompt Templates, Configurations, Orchestrators, and Knowledge Entries**
5. **Update Documentation**


---

#### Activity Iterations
TODO

**Note:** Stopped @ Iteration 33A and Issue #135

- Active Issues
  - Update README with Project Update #133
  - Update README: Appendix Roadmap Traveled #115
  - Improve README Documentation #79
  - Evaluate and Clarify Project Assumptions #64

TODO: update with newest overview summary

1. **Identify Foundations**
    1. **Identify Problem/Challenges (Current):** Information-following large language model (IF-LLM) vulnerabilities create decision-making risks because of information uncertainties.
    1. **Identify Vision (Ideal):** Users efficiently receive high-quality information for decision-making (by reducing IF-LLM vulnerabilities).
    1. **Identify Mission (Purpose):** Offer reusable instructions and context to reduce IF-LLM vulnerabilities (failures) and subsequent information risks.
    1. **Identify Objectives (Current versus Ideal)**
        1. Identify and Implement Evidence-Based Knowledge
        1. Create and Refine Tools Using Evidence-based Best Practices
1. **Identify Assumptions**
    1. *Iteration 18A* — Evaluate and Clarify Project Assumptions #64
1. **Identify Evidence-Based Knowledge**
    1. **Evidenced-based Information Criteria (Research)**
        1. *Iteration 24A* — Identify Research Method #88
    1. **Decision-Making Information Quality Criteria (Priorities)**
        1. *Iteration 18A* — Clarifying Quality Criteria for Information used in Decision-Making #63
    1. **IF-LLMs** (e.g., OpenAI, Google, Microsoft, Meta, Anthropic, etc.)
        1. *Iteration 07A* — Clarify LLM Behavioral Configuration Parameters #29
        1. *Iteration 08A* — Identify AI Model Types #34
        1. *Iteration 13A* — Clarify Instruction & Knowledge Authority Hierarchy #52
        1. *Iteration 24B* — Clarify IF-LLM Prompt Stack #95
    1. **IF-LLM Common Failure Modes**
        1. *Iteration 22A* — Verify Assumptions: IF-LLM Failure Modes #83
        1. *Iteration 23A*
            1. Refine Common IF-LLM Failure Modes List #86
            1. Expand/Clarify Evidence of Common IF-LLM Failure Modes #87
        1. *Iteration 27A*
            1. Consolidate Failure Mode Lists #111
            1. Research and Validate Failure Modes #112
            1. Validate IF-LLM Failure Modes #114
            1. Document Failure Modes per Research Item #116
    1. **IF-LLM Common Failure Mode Mitigation Strategies** (e.g., Instructions and Context)
        1. *Iteration 28A*
            1. Research Failure Mode Reduction Instructions #119
            1. Organize/Clarify Research Failure Mode Reduction Instructions #120
        1. *Iteration 29A* — Improve Instructions List #123
    1. **IF-LLM Prompt Best Practices**
    1. **IF-LLM Configuration Best Practices**
    1. **IF-LLM Orchestrator Best Practices**
    1. **IF-LLM Knowledge File Best Practices**
        1. **Tasks**
        1. **Domains**
        1. **Reasoning**
        1. **Structures**
        1. **Personas**
        1. **Examples**
1. **Organize Resources** (e.g., file structure, prompts, configurations, orchestrators, knowledge entries)
    1. *Iteration 08B* — Rename Repository: LLM (not GPT) #35
    1. *Iteration 10A* — Create Directory: Configurations #39
    1. *Iteration 11A* — Move Processing Policies Knowledge File Policies to Knowledge Files Policies #41
    1. *Iteration 12A*
        1. Rename repository if-llm-behavior-ontology #44
        1. Archive / Cleanup deprecated files #45
        1. 45 a archive cleanup deprecated files #48
        1. Preserve deprecated files from reorganization #47
        1. Reorganize repository structure #49
    1. *Iteration 33A*
        1. Project Cleanup: Close Currently Abandoned Issues #134
        1. Project Cleanup: Close Completed Issues Unintentionally Left Open #135
    1. **Create IF-LLM Behavior Configuration Orchestrator**
        1. *Iteration 09A*
            1. Create Configuration: Policy-Aligned IF-LLM Configuration Analyst #37
            1. 37 create configuration llm behavioral configuration parameters lbcs #50
        1. *Iteration 16A*
            1. Update configurations.md #53
            1. Create Configuration: Lean Development Specialist #54
        1. *Iteration 25A*
            1. Create "Clean" Behavior Configuration Designer Prompt (Temporary) #100
            1. Create Configuration: Behavior Configuration Orchestrator #101
            1. 101 create configuration behavior configuration orchestrator #104
        1. *Iteration 31A*
            1. Update Prompts: Orchestrated Behavior Configuration and Task Knowledge Entries Creation #125
            1. Update prompts.md #126
        1. *Iteration 32A*
            1. Update Prompt: Orchestrated Behavior Configuration and Task Knowledge Entries Creation #128
            1. 128 update prompt orchestrated behavior configuration and task knowledge entries creation #129
    1. **Create IF-LLM Research Orchestrator**
        1. *Iteration 21A*
            1. Update configurations.md #80
            1. Create Configuration: Evidence Synthesis Specialist #81
            1. Update configurations.md #82
        1. *Iteration 26A*
            1. Create Orchestrator: Research Orchestrator #109
            1. 109 create orchestrator research orchestrator #110
    1. **Implement IF-LLM System-Level Common Failure Mitigation Strategies** (e.g., System-Level Policy Instructions and Context)
        1. **Priorities** (i.e., Decision-Making Information Quality Criteria)
        1. **Policies** (i.e., Rules)
            1. *Iteration 07B*
                1. Create Draft Processing Policies Meta Knowledge File #30
                1. Create Lint Rules Meta Knowledge File #31
            1. *Iteration 08C* — Update processing-policies.md for LLM versus GPT Ontology #3
            1. *Iteration 19A* — Update Processing Policy Priorities #66
    1. **Create IF-LLM System-Level Policy and Knowledge Entry Evaluator**
        1. *Iteration 12B* — Create Configuration: Policy-Aligned IF-LLM Knowledge Analyst #51
        1. *Iteration 31B*
            1. Create Orchestrator: System Policies + Knowledge Entries Evaluator #127
            1. 127 create orchestrator system policies knowledge entries evaluator #130
    1. **Evaluate, Refine, and Implement IF-LLM System-Level Policies and Knowledge Entries**
        1. *Iteration 02A* — create knowledge file evaluate task knowledge file #9
        1. *Iteration 06A* — Evaluate Existing Expert Knowledge File #24
        1. *Iteration 11B* — Review and Update Knowledge File Policies (Meta) #42
        1. *Iteration 20A*
            1. Update processing-policies.md #73
            1. Evaluate Refined Priorities #74
            1. Update processing-policies.md #75
            1. Reset Processing Policies #76
            1. Update processing-policies.md #77
        1. *Iteration 30A* — Update processing-policies.md with anti-failure instructions #124
        1. *Iteration 32B* — Improve System-Level Policies and Knowledge Entries (processing-policies.md) (Pass 1) #131
    1. **Create Other Helpful IF-LLM Prompt Templates, Configurations, Orchestrators, and Knowledge Entries**
        1. *Iteration 01A*
            1. Create GPT experts knowledge file #1
            1. Create ontology experts knowledge file #2
            1. Create ontology rules knowledge file #3
            1. 3 create ontology rules knowledge file #46
            1. Create GitHub experts knowledge file #4
            1. Create instructions file #5
            1. create gpt experts knowledge file #6
        1. *Iteration 03A*
            1. Create the Evidence-Based Analytical Advisor in the Expert Knowledge File #11
            1. Move expert knowledge files from roles to experts directory #12
            1. Create knowledge file policies meta file #13
            1. Create Expert: Reliability-First Prompt Engineering Expert #14
            1. Create Expert: Creative / Exploratory Expert (for ideation) #15
            1. Create Expert: Domain Specialist Expert (for subject-matter depth) #16
            1. Create Expert: Convergent / Optimization Expert #17
        1. *Iteration 04A* — Create Expert: Creative Ideation & Concept Exploration Advisor #19
        1. *Iteration 05A*
            1. Create Decision & Trade-Off Authority Advisor #21
            1. Create Ethical, Legal & Societal Impact Reviewer #22
            1. Create Implementation & Practical Feasibility Advisor #23
        1. *Iteration 06B*
            1. Create a Knowledge Ontology & Information Architecture Expert #25
            1. Create a Plain-Language Technical Editor (U.S. general audience) #26
            1. Create a Knowledge Base QA / Test Harness Expert #27
            1. Create a Governance & Change-Management Steward #28
        1. *Iteration 17A*
            1. Create Configuration: Digital Inclusion Specialist (Devon Ibarra) #58
            1. Update configurations.md #59
            1. Create Configuration: Lean Developer #60
            1. Update configurations.md #61
        1. *Iteration 18B* — Create Configuration: Technical Writer #65
        1. *Iteration 19B*
            1. Create Configuration: MN LTSS Systems Researcher #67
            1. Update configurations.md #68
            1. Create Configuration: Inclusive Summarizer #69
            1. Update configurations.md #71
        1. *Iteration 22B*
            1. Create Configuration: Hierarchical List Creator and Evaluator #84
            1. Update configurations.md #85
        1. *Iteration 24C* — Update Configurations: "Experts" to "Reasoning" for all configurations #98
        1. *Iteration 25B*
            1. Create Configuration: Event Information Analyst #102
            1. Create Orchestrator: Event Analysis #103
            1. 103 create orchestrator event analysis #105
        1. *Iteration 28B*
            1. Create Behavior Configuration: Structured List Normalization Configuration #121
            1. Update configurations.md #122
1. **Update Documentation**
    1. *Iteration 03B* — Create Playbook: GPT Expert Routing Playbook #18
    1. *Iteration 16B*
       1. Update/Improve README User Notes #55
       1. Create IF-LLM-BO GitHub Repository Social Image #56
       1. Add open graph preview image #57
    1. *Iteration 19C* — 55 updateimprove readme user notes #72
    1. *Iteration 20B* — Improve README Documentation #79
    1. *Iteration 25C*
       1. Update README Roadmap #107
       1. Update README.md #108
    1. *Iteration 27B*
       1. Update README: Organize Common IF-LLM Failure Modes #113
       1. Update README: Appendix Roadmap Traveled #115
       1. Update README: IF-LLM Failure Modes #117
       1. 113 update readme organize common if llm failure modes #118


**Note:** Activity Steps (Issues) #7 and #8 were deleted because they were unneeded.


---

## **Roadmap**

1. **Update Documentation**
   1. Finish common failure mode mitigation strategies documentation
      1. Update README with Project Update #133 
      1. Update README: Appendix Roadmap Traveled #115
      1. Improve README Documentation #79
      1. Evaluate and Clarify Project Assumptions #64
1. **Organize Resources** (e.g., file structure, prompts, configurations, orchestrators, knowledge entries)
   1. **Recreate IF-LLM Behavior Configuration Orchestrator**
      - Review Input and Rebuild with updated policies
   1. **Recreate Research Orchestrator** (Clarify, Strategize, Extract, Evaluate, Report)
      - Review Input and Rebuild with updated policies
   1. **Create IF-LLM System-Level Policy and Knowledge Entry Evaluator**
      - Review Input and Rebuild with updated policies
   1. **Create Orchestrator: IF-LLM IF-LLM System-Level Policies and Knowledge Entries Creator and Evaluator**
      - re-evaluate with updated policies and evaluation orchestrator
   1. **Create Orchestrator: IF-LLM Knowledge Entries Creator and Evaluator**
   1. **Create Orchestrator: Custom GPT Creator and Evaluator**
1. **Identify Evidence-Based Knowledge**
   1. **Lean Processing Principles**
       - Validate 
   1. **IF-LLM Common Failure Mode Mitigation Strategies** (e.g., Instructions and Context)
       - Validate 
       - Identify evidence for each Policy (i.e., Instruction or Context)
1. **Update Documentation**
   - Update common failure mode mitigation strategies documentation
   - Update Lean Processing Principles
1. **Organize Resources** (e.g., file structure, prompts, configurations, orchestrators, knowledge entries)
   1. **Create Other Helpful IF-LLM Prompt Templates, Configurations, Orchestrators, and Knowledge Entries** 
      1. **Re-Create Orchestrator: Inclusive Communication Creator and Evaluator**
      1. **Re-Create Orchestrator: Hierarchical List Creator and Evaluator**
      1. **Re-Create Orchestrator: Content Summarizor**
      1. **Create Orchestrator: Plain-Language Content Creator and Evaluator**
      1. **Create Orchestrator: Content Comparison Analyzer** (i.e., identical, materially similar, inconsistent)
      1. **Re-Create Orchestrator: Technical Writing Creator and Evaluator**
      1. **Create Orchestrator: Digital Inclusion Advisor and Evaluator**
      1. **Create Orchestrator: Logic Chain Evaluator** (i.e., identify undisclosed assumptions, evaluate logic strength, identify required evidence)
      1. **Create Orchestrator: Ideation Creator and Evaluator (Brainstorming)**
      1. **Create Orchestrator: Impact Analyzer and Evaluator**
      1. **Create Orchestrator: Lean Processing Advisor and Evaluator**
      1. **Create Orchestrator: Complex Adaptive Systems Analyzer and Evaluator**
      1. **Create Orchestrator: Event Researcher and Analyzer** (Clarify, Strategize, Extract, Evaluate, Report)
      1. **Create Orchestrator: Social Media Content Creator and Evaluator**
      1. **Create Orchestrator: Holiday Social Media Content Creator**
1. **Identify Assumptions** — Review and Finalize
1. **Identify Evidence-Based Knowledge**
   1. Instruction Anatomy
   1. Knowledge Entry Types
   1. Knowledge Entry Parameters per Type
 1. Identify and Create: Entries for Common Domains
     1.1. Lean Development Principles (Validated)
     1.1. Information Quality Criteria (Validated) — Policy/README
     1.1. IF-LLM Common Failure Modes (Validated) — Policies/README
     1.1. IF-LLM Instruction Anatomy (Validated) — Policies/README
     1.1. IF-LLM Knowledge Entry Types (Validated) — Policies/README
     1.1. MN LTSS
     1.1. Humanity


---

## **Authors**

- Lance Hegland ([lance.hegland@gmail.com](mailto:lance.hegland@gmail.com))



## **License**

Creative Commons Attribution Share Alike 4.0 International License (CC-BY-SA-4.0)

- See [LICENSE.txt](LICENSE.txt)
- See [Creative Commons Attribution Share Alike 4.0 International (CC-BY-SA-4.0)](https://choosealicense.com/licenses/cc-by-sa-4.0/)


## **Document Index**

TBD

- [File Header Metadata](#file-header-1)
- [Features](#features)
- [Background](#background)
- [Known Issues](#known-issues)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [IF-LLM-BO Project Notes](#if-llm-bo-project-notes)
  - [Foundations](#foundations)
    - [Assumptions](#assumptions)
    - [Decision-Making Information Quality Criteria (Priorities)](#decision-making-information-quality-criteria-priorities)
    - [Commonly Used IF-LLMs](#commonly-used-if-llms)
    - [Common IF-LLM Failure Modes](#common-if-llm-failure-modes)
    - [Common IF-LLM Failure Mitigation Strategies](#common-if-llm-failure-mitigation-strategies)
  - [Purpose](#purpose)
  - [Objectives](#objectives)
  - [Governance, Policies, Rules](#governance-policies-and-rules)
    - [Human Governance (System Architect and Solution Developer Governance)](#system-architect-and-solution-developer-governance-human-governance)
    - [Stored Context Policies (Knowledge File and Knowledge Entry Policies)](#knowledge-file-and-entry-policies-stored-context-policies)
    - [Stored Instruction Rules (Processing Policies)](#processing-policies-stored-instruction-rules)
  - [Prompt Templates, Orchestrators, Configurations](#prompt-templates-orchestrators-configurations)
    - [Prompt Elements](#prompt-elements)
    - [Configurations](#configurations)
    - [Orchestrators](#orchestrators)
    - [Prompt Templates](#prompt-templates)
- [Appendices](#appendices)
  - [Assumptions](#appendix-assumptions)
  - [Evidenced-based Information Criteria (Research)](#appendix-evidenced-based-information-criteria-research)
  - [Decision-Making Information Quality Criteria (Priorities) with Definitions and Sources](#appendix-decision-making-information-quality-criteria-priorities-with-definitions-and-sources)
    - [Summary of Authoritative Sources for Decision-Making Information Quality Criteria (Priorities)](#summary-of-authoritative-sources-for-decision-making-information-quality-criteria-priorities)
  - [IF-LLM Information](#appendix-if-llm-information)
    - [Commonly Used IF-LLMs](#commonly-used-if-llms-1)
      - [Summary of Authoritative Sources](#summary-of-authoritative-sources-for-commonly-used-if-llms)
    - [Instruction and Context Hierarchy](#instruction-and-context-authority-hierarchy)
    - [Model Elements](!!!TODO!!!)
    - [Prompt Anatomy](#prompt-anatomy)
      - [Identity & Role](#identity--role)
      - [Priorities](#priorities-2)
      - [Task](#task)
      - [Domains](#domains-1)
      - [Reasoning](#reasoning)
      - [Structure](#structure)
      - [Persona](#persona)
      - [Examples](#examples)
    - [Common Failure Modes](#common-failure-modes)
      - [Expanded List](#expanded-list)
      - [Examples and Sources](#examples-and-sources)
        - [Authoritative Works Cited](#summary-of-authoritative-works-cited-for-common-failure-modes-with-examples-and-sources)
    - [Common IF-LLM Failure Mitigation Strategies](#common-if-llm-failure-mitigation-strategies-1)
      - [Strategies for Failure Modes with Sources](#strategies-for-failure-modes-with-sources)
        - [Authoritative Works Cited](#summary-of-authoritative-works-cited-for-mitigation-strategies-for-common-if-llm-failure-modes)
  - [Governance, Policies, Rules](#appendix-if-llm-bo-governance-policies-and-rules)
    - [Human Governance (System Architect and Solution Developer Governance)](!!!TODO!!!)
    - [Stored Context Policies (Knowledge File and Knowledge Entry Policies)](!!!TODO!!!)
    - [Stored Instruction Rules (Processing Policies)](!!!TODO!!!)
  - [Developed Solution Anatomy](#developed-solution-anatomy)
    - [Knowledge Files](#knowledge-files)
      - [Prompt Templates](#prompt-templates)
      - [Governance, Policies, and Rules](!!!TODO!!!)
        - [Human Governance](!!!TODO!!!)
        - [Knowledge File and Entry Policies](!!!TODO!!!)
        - [Processing Rules (Instructions)](!!!TODO!!!)
      - [Orchestrators](#orchestrators)
      - [Configurations](#configurations)
      - [Prompt Elements](#prompt-anatomy)
    - [Tools](#tools)
  - [IF-LLM-BO Project Journey](#appendix-if-llm-bo-project-journey)
    - [Expanded Objectives](#expanded-objectives)
    - [Activity Iterations](#activity-iterations)
- [Roadmap](#roadmap)
- [Authors](#authors)
- [License](#license)


---

## File Header

**NAMESPACE:** me.hegland-lance.if-llm-behavior-ontology

**Scope:** TODO

**Owner:** [Lance Hegland](mailto:lance.hegland@gmail.com)

**Version:** 2026-03-31T06:57Z LH in [if-llm-behavior-ontology](https://github.com/LHHegland/if-llm-behavior-ontology)

**Last Reviewed:** 2026-03-30T11:59Z — [Lance Hegland](mailto:lance.hegland@gmail.com)

**Changelog**
- 2026-03-31T07:05Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Update hyperlinks for Commonly Used IF-LLMs in Table of Contents, Foundations, and Appendix IF-LLM Information sections
- 2026-03-31T06:57Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Update Commonly Used IF-LLMs in Table of Contents, Foundations, and Appendix IF-LLM Information sections
- 2026-03-30T11:59Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Update Changelog
- 2026-03-30T11:59Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Review and update Assumptions section
- 2026-03-30T10:24Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and updating Table of Contents hyperlinks (Pass 6) and content hyperlinks (Pass 4)
- 2026-03-30T08:36Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and updating Table of Contents hyperlinks (Pass 5) and content hyperlinks (Pass 3)
- 2026-03-30T07:24Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and updating Table of Content hyperlinks (Pass 4) and content hyperlinks (Pass 2)
- 2026-03-30T07:12Z — [Lance Hegland](mailto:lance.hegland@gmail.com): 
  - Began reviewing and updating content hyperlinks (Pass 1)
  - File Heading section, including creating changelog
  - Moved unorganized content into temporary "NOT YET ORGANIZED" section
  - Reviewing and updating Table of Contents hyperlinks (Pass 3)
- 2026-03-27T09:55Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and updating Table of Content hyperlinks (Pass 2)
- 2026-03-27T06:40Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and updating Table of Content hyperlinks (Pass 1)
- 2026-03-27T06:40Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Working on the following sections:
  - Decision-Making Information Quality Criteria (Priorities) and appendix
  - IF-LLM Information > Instruction and Context Authority Hierarchy
  - Appendix: IF-LLM-BO Project Journey
  - Updating Roadmap
  - Table of Contents
- 2026-03-15T17:52Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Revising previous
- 2026-03-15T17:47Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Revising previous
- 2026-03-15T17:45Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Revising previous
- 2026-03-15T17:40Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Revising previous
- 2026-03-15T17:37Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Revising previous
- 2026-03-15T17:32Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Updated Common Failure Modes and related appendix
- 2026-03-08T09:21Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Updated Assumptions and related appendix
- 2026-03-08T07:37Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Edited Decision-Making Information Quality Criteria (Priorities) and related appendix
- 2026-03-06T14:09Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and editing Assumptions and Decision-Making Information Quality Criteria (Priorities)
- 2026-03-06T14:05Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and editing content (stage 2)
- 2026-03-06T03:55Z — [Lance Hegland](mailto:lance.hegland@gmail.com): fixed typo in table of contents link for information quality priorities
- 2026-03-06T03:53Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and editing content (stage 1)
- 2026-03-03T06:59Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Updated Roadmap
- 2026-02-20T04:16Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Updated decision-making information quality criteria (priorities)
- 2026-02-18T07:14Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Added Common IF-LLM Failure Modes
- 2026-02-18T06:17Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Updated User Notes Foundations Assumptions section
- 2026-02-18T04:27Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Added Priorities section content
- 2026-02-17T09:51Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Added decision-making information quality criteria
- 2026-02-17T08:50Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Reviewing and editing
- 2026-02-15T08:54Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Updated user notes section
- 2026-02-15T08:49Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Updated Roadmap section
- 2026-02-13T20:24Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Renamed repository and scaffolding
- 2026-02-01T06:50Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Created repository and README.md from [IF-LLM Development Repository Template](https://github.com/LHHegland/if-llm-dev-repo-template)
