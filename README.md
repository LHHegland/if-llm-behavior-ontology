# Instruction-Following Large Language Model (LLM) Behavior Ontology (IF-LLM-Behavior-Ontology) *[if-llm-behavior-ontology](https://github.com/LHHegland/if-llm-behavior-ontology)*

**NAMESPACE:** me.hegland-lance.if-llm-behavior-ontology

**PURPOSE**
**Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is a lightweight semantic scaffolding system for structuring knowledge files that guide instruction-following large language models (IF-LLMs) toward accurate, reliable, relevant, and practical outcomes. It emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts.

.

## Table of Contents

- [Features](#features)
- [Background](#background)
- [Known Issues](#known-issues)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [Authors](#authors)
- [Roadmap](#roadmap)
- [License](#license)

.

## **Features**

TODO

.

## **Background**

The goal is to build a lightweight semantic scaffolding system for structuring knowledge files that guide instruction-following LLMs toward high-priority results (i.e., accurate, reliable, relevant, specific, clear, practical, fair, and efficient). The scaffolding and LLM processing must align with these priorities. It must emphasize human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts; a practical, not perfect, ontologies. The scaffolding must help organize instruction-following LLM behavioral configurations in knowledge files. The scaffolding so far is as follows:
- **ontology:** *serves as the semantic root for all model behavior.* The ontology defines the canonical concepts, relationships, and behavior guidance that constitute the instruction-following LLM’s shared semantic foundation.
  - **meta:** *provides cross-cutting rules and scaffolding about the ontology itself.* Meta captures naming rules, modeling conventions, global decision policies, ontology versioning, glossaries of meta-terms, and core primitives reused across domains.
  - **tasks:** *defines what the model is expected to do and how success is judged.* Tasks specify objectives, priorities, success criteria, unacceptable outputs, scope boundaries, and workflows, providing explicit guidance on intended outcomes and failure avoidance.
  - **domains:** *constrain what knowledge space the model may operate within.* Domains describe relevant elements and relationships, in-scope and out-of-scope topics, geographic or contextual boundaries, and known uncertainty zones to reduce ambiguity and hallucination.
  - **experts:** *shape how the model reasons about the task.* Experts encode reasoning frameworks, heuristics, and analytical lenses that guide interpretation, tradeoffs, and decision-making without prescribing exact answers.
  - **structures:** *control how outputs are organized and validated.* Structures define required sections, ordering, mandatory and conditional fields, and formatting rules to ensure consistency, completeness, and evaluability of responses.
  - **personas:** *govern how the model communicates.* Personas specify tone, voice, formality, conciseness, and stylistic constraints, aligning outputs with audience expectations without altering underlying task logic.
  - **examples:** *demonstrate acceptable patterns of behavior.* Examples pair representative prompts with corresponding results to illustrate desired reasoning, structure, and boundary handling in concrete terms.
  - **configs:** *compose a complete behavioral profile.* Configurations bind tasks, domains, experts, structures, personas, and examples into a reusable, explicit behavioral setup that enables consistent instruction-following across contexts.

.

## **Known Issues**

TODO

.

## **Requirements**

TODO

1. Familiarity and access to instruction-following LLM like [ChatGPT](https://chatgpt.com/)
1. Familiarity and access to [GitHub](https://github.com/)
1. Agree to the [Creative Commons Attribution Share Alike 4.0 International License (CC-BY-SA-4.0)](LICENSE.txt)
1. Review [README](README.md)

.

## **Installation**

1. Review [README](README.md).
1. Perform the necessary actions to satisfy [minimum requirements](#requirements).
1. From your local projects directory, copy the entire remote GitHub repository into your local project directory.

TODO

.

## **Configuration**

TODO

.

## **Usage**

1. Perform the necessary actions to complete the [installation](#installation).


TODO


**TIPS:** Refer to the following documentation and tools to efficiently develop prompts delivering accurate, reliable, relevant, specific, clear, practical, fair, and efficient results for your users:
- [ChatGPT Prompt Engineering Best Practices](https://help.openai.com/en/articles/10032626-prompt-engineering-best-practices-for-chatgpt)
- [How do I create a good prompt for an AI model?](https://help.openai.com/en/articles/4936848-how-do-i-create-a-good-prompt-for-an-ai-model)
- [OpenAI Prompting Guide](https://platform.openai.com/docs/guides/prompting)
- [OpenAI Prompt Examples)](https://platform.openai.com/docs/examples)
- [OpenAI Prompt Optimizer Tool](https://platform.openai.com/chat/edit?optimize=true)
- [OpenAI Prompt Engineering Guide](https://platform.openai.com/docs/guides/prompt-engineering)
- [OpenAI Reasoning Best Practices](https://platform.openai.com/docs/guides/reasoning-best-practices)
- [OpenAI GPT-5 Prompting Guide](https://cookbook.openai.com/examples/gpt-5/gpt-5_prompting_guide)

.

## IF-LLM Behavioral Ontology User Notes
The following sections contain user notes related to this instruction-following large language model (IF-LLM) behavior ontology. This ontology helps to most efficiently organize and maintain the frequently- or commonly-used IF-LLM behavioral configurations.

### Purpose
As stated previously, **Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is a lightweight semantic scaffolding system for structuring knowledge files that guide instruction-following large language models (IF-LLMs) toward accurate, reliable, relevant, and practical outcomes. It emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts.

### Objectives
TODO: Outline objectives

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


## **Authors**

- Lance Hegland ([lance.hegland@gmail.com](mailto:lance.hegland@gmail.com))

.

## **Roadmap**

  1. Identify the instruction-following large language model (IF-LLM) behavior configurationwith the objective of ** creating and evaluating IF-LLM behavior configurations** (topics: IF-LLM behavior configurations, IF-LLM behavior configuration best practices, IF-LLM behavior configuration policies, IF-LLM behavior configuration policy best practices) named "Blake Carter".
  2. Create and implement *Kendall Evans* behavior configuration.
      1. Ask *Blake Carter* to identify the configuration with the objective of **creating and evaluating IF-LLM knowledge files and entries** (topics: IF-LLM processing policies, IF-LLM processing policy best practices, IF-LLM behavior configuration ontologies, IF-LLM behavior configuration ontology best practices, IF-LLM behavior configuration ontology policies, IF-LLM behavior configuration ontology policy best practices, IF-LLM knowledge files and entries, IF-LLM knowledge file and entry best practices, IF-LLM knowledge file and entry policies, IF-LLM knowledge file and entry policy best practices, ontologies, ontology best practices, ontology policies, ontology policy best practices).
      2. Ask *Kendall Evans* to create configuration knowledge entry and knowledge entries index entry.
  3. Ask *Kendall Evans* to identify the following most significant and commonly-used IF-LLM elements plus purpose and use cases for each:
     - behavioral configuration parameters;
     - knowledge entry types;
     - knowledge file types;
     - schemas for the following:
       - each type of knowledge entry;
       - each type of knowledge file; and,
       - knowledge file headers.
  4. Ask *Kendall Evans* to create configuration knowledge entries, configuration knowledge file, knowledge entries index file, and knowledge entries index entries for *Blake Carter*.
  5. Create and implement *Morgan Parker* behavior configuration.
      1. Ask *Blake Carter* to identify the behavior configuration with the objective of **creating and evaluating IF-LLM policies** aligned with best practices, policies, and priorities (topics: IF-LLM best practices, IF-LLM policies, IF-LLM policy best practices, IF-LLM governance, IF-LLM governance best practices, IF-LLM processing policies, IF-LLM processing policy best practices, IF-LLM knowledge file and entry policies, IF-LLM knowledge file and entry policy best practices).
      2. Ask *Kendall Evans* to create configuration knowledge entry and knowledge entries index entry.
  6. Create, evaluate, refine, and implement the processing policies, including guardrails, default behavioral configuration settings, etc..
      1. Ask *Morgan Parker* (artifact order) to create the policy.
      2. Ask *Morgan Parker* (artifact owner) to evaluate and refine the policy (3 ≤ iterations ≤ 5).
      3. Ask *Morgan Parker*, *Kendall Evans*, and *Blake Carter* (*Knowledge and Processing Compliance Team*) to evaluate and refine the policy (3 ≤ iterations ≤ 5).
      4. Ask *Morgan Parker* (artifact owner) to perform the final evaluation of the policy, implement if no significant concerns.
      5. Implement policy.
          1. Ask *Kendall Evans* to create the meta knowledge entries, meta knowledge files, and knowledge entries index entries for the policy.
          2. Ask *Kendall Evans* (artifact order) to evaluate and refine the policy implementation (3 ≤ iterations ≤ 5).
          3. Ask *Morgan Parker*, *Kendall Evans*, and *Blake Carter* (*Knowledge and Processing Compliance Team*) to evaluate and refine the policy implementation (3 ≤ iterations ≤ 5).
          4. Ask *Kendall Evans* (artifact owner) to perform the final evaluation of the policy implementation, release to production if no significant concerns.
  7. Create, evaluate, refine, and implement the knowledge policies, including file and entry schemas, creating files, creating entries, using entries, updating entries, etc..
      1. Ask *Morgan Parker* (artifact order) to create the policy.
      2. Ask *Morgan Parker* (artifact owner) to evaluate and refine the policy (3 ≤ iterations ≤ 5).
      3. Ask *Morgan Parker*, *Kendall Evans*, and *Blake Carter* (*Knowledge and Processing Compliance Team*) to evaluate and refine the policy (3 ≤ iterations ≤ 5).
      4. Ask *Morgan Parker* (artifact owner) to perform the final evaluation of the policy, implement if no significant concerns.
      5. Implement policy.
          1. Ask *Kendall Evans* to create the meta knowledge entries, meta knowledge files, and knowledge entries index entries for the policy.
          2. Ask *Kendall Evans* (artifact order) to evaluate and refine the policy implementation (3 ≤ iterations ≤ 5).
          3. Ask *Morgan Parker*, *Kendall Evans*, and *Blake Carter* (*Knowledge and Processing Compliance Team*) to evaluate and refine the policy implementation (3 ≤ iterations ≤ 5).
          4. Ask *Kendall Evans* (artifact owner) to perform the final evaluation of the policy implementation, release to production if no significant concerns.
  8. Evaluate, refine, and implement the configuration knowledge file.
      1. Ask *Blake Carter* (artifact owner) to evaluate and refine the related artifacts (3 ≤ iterations ≤ 5).
      2. Ask *Morgan Parker*, *Kendall Evans*, and *Blake Carter* (*Knowledge and Processing Compliance Team*) to evaluate and refine the related artifacts.
      3. Ask *Blake Carter* (artifact owner) to perform the final evaluation of the related artifacts, release to production if no significant concerns.
  9. Evaluate, refine, and implement the entire collection of IF-LLM-BO files.
      1. Ask *Blake Carter* (artifact owner) to evaluate and refine the related artifacts (3 ≤ iterations ≤ 5).
      2. Ask *Morgan Parker*, *Kendall Evans*, and *Blake Carter* (*Knowledge and Processing Compliance Team*) to evaluate and refine the related artifacts.
      3. Ask *Blake Carter* (artifact owner) to perform the final evaluation of the related artifacts, release to production if no significant concerns.
 10. After gathering at least 30 configuration knowledge entries, periodically (monthly) evaluate configuration knowledge entries for overlapping configuration elements (e.g., meta, task, domain, expert,
 11. Create and implement behavior configurations for the following objectives:
     1. Creating evaluating, and refining GitHub README documentation content (topics: GitHub README content, GitHub README best practices, GitHub README policies, GitHub README policy best practices)
     2. Creating, evaluating, and refining hierarchical list content (topics: hierarchical lists, hierarchical list best practices, hierarchical list policies, hierarchical list policy best practices)
     3. Creating, evaluating, and refining "plain language" content (topics: plain language, accessible communication content, plain language best practices, accessible communication best practices, plain language policies, accessible communication policies, plain language policy best practices, accessible communication policy best practices)
     4. Creating, evaluating, and refining document collection summaries (topics: document summaries, document collection summaries, document summary best practices, document collection summary best practices, document summary policies, document collection summary policies, document summary policy best practices, document collection summary policy best practices)
     5.  Comparing documents and summarizing results (topics: significant communication content differences, material communication content differences, document comparison best practices, document comparison policies, document comparison policy best practices)
     6.  
 13. TODO

.

## **License**

Creative Commons Attribution Share Alike 4.0 International License (CC-BY-SA-4.0)

- See [LICENSE.txt](LICENSE.txt)
- See [Creative Commons Attribution Share Alike 4.0 International (CC-BY-SA-4.0)](https://choosealicense.com/licenses/cc-by-sa-4.0/)
