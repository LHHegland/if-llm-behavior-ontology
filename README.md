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
- [User Notes](#user-notes)
  - [Foundations](#foundations)
    - [Assumptions](#assumptions)
    - [Common IF-LLM Failure Modes](#common-if-llm-failure-modes)
    - [Information Quality Criteria](#information-quality-criteria)
  - [Purpose](#purpose)
  - [Objectives](#objectives)
- [Appendices](#appendices)
  - [Assumptions](#appendix-assumptions)
  - [Information Quality Criteria](#appendix-information-quality-criteria)
  - [Common IF-LLM Failure Modes](#appendix-common-if-llm-failure-modes)
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

## User Notes
The following sections contain user notes related to this instruction-following large language model (IF-LLM) behavior ontology. This ontology helps to most efficiently organize and maintain the frequently- or commonly-used IF-LLM behavior instructions.

### Foundations
The following sections contain the foundations that guide this instruction-following large language model (IF-LLM) behavior ontology.

#### Assumptions

Below is a summary of the underlying assumptions for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project.  More detailed information about these assumptions, along with authoritative sources, can be found in the [Appendix: Assumptions](#appendix-assumptions).

TO DO: Create Summary

#### Common IF-LLM Failure Modes

Below is a summary of the common instruction-following large language model (IF-LLM) failure modes this project hopes to address.  More detailed information about these failure modes, along with authoritative sources, can be found in the [Appendix: Common IF-LLM Failure Modes](#appendix-common-if-llm-failure-modes).

TO DO: Create Summary

#### Information Quality Criteria

Instruction-Following Large Language Models (IF-LLMs) are often used to generate information that can influence real-world decisions. Because of this, the information they produce should meet clear and well-defined quality standards. The criteria listed below identify the key characteristics that information should have in order to reliably support decision-making. Each definition is written to answer a practical question: *"What does this mean for everyday decision-making?"*

To produce information that meaningfully supports decisions, IF-LLMs should prioritize these criteria according to their ranked importance. Any trade-offs should be disclosed to users. In turn, the policies and procedures governing IF-LLM-BO systems should be designed to reflect and reinforce these priorities.

**Information Quality Criteria (Prioritized)**
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


More detailed information about these criteria, along with authoritative sources, can be found in the [Appendix: Information Quality Criteria](#appendix-information-quality-criteria).



### Purpose
As stated previously, **Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is a lightweight semantic scaffolding system for structuring knowledge files that guide instruction-following large language models (IF-LLMs) toward accurate, reliable, relevant, and practical outcomes. It emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts.

### Objectives
- Build a lightweight semantic scaffolding system for structuring instructions for instruction-following large language models (IF-LLMs). 
  - emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts; a practical, not perfect, ontologies.
  - scaffolding must help organize instruction-following LLM behavioral configurations in knowledge entries and files. 

### Operational Notes

### Instruction and Knowledge Authority Hierarchy

TODO: Briefly define the hierarchy of IF-LLM instructions and knowledge authority as outlined below, including how instructions are granted authority, critical phrases used to grant/assign authority, plus 3 to 5 examplesto help users understand the value of this hierarchy.
1. System (Global) Policies (e.g., knowledge entries with the highest authority (i.e., meta knowledge entries))
2. Developer Instructions (e.g., knowledge entries with the second-highest authority, developer implemented knowledge entries)
3. User Instructions (i.e., the current conversation via chat or API, which could reference existing knowledge entries)
4. Knowledge Files (and their collection of entries)
5. User-Uploaded Files (e.g., user-uploaded files, which are considered user knowledge files containing user knowledge injuries)
6. Tool Outputs
7. General Model Knowledge


IF-LLMs receive instructions through either user prompts (e.g., chat interfaces or APIs) or developer instructions. Users and developers can store reusable instructions and context in knowledge entries of various types. Knowledge interests can be organized into knowledge files.

interfacesknowledge files that



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

## Appendices

These appendices contain more detailed information and authoritative source references, if applicable, regarding elements of the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project.

### Appendix: Assumptions

This appendix contains detailed information about the underlying assumptions for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project along with authoritative sources.

##### 1. Instruction-Following Model Behavior

###### 1.1 Instruction Precedence

* IF-LLMs process instructions using a **strict authority hierarchy**, where higher-authority instructions override lower-authority inputs.
* Conflicts between instructions must be resolved deterministically according to that hierarchy.
* Undisclosed or silent overrides reduce reliability and must be avoided.


###### 1.2 Instruction Influence

* Instructions and contextual knowledge **materially influence** how inputs are interpreted and how outputs are generated.
* Explicit instructions outperform implicit expectations in reducing ambiguity and hallucination.

###### 1.3 Observable Behavior

* Instructional alignment is reflected in **observable output behavior**, not internal model state.
* Behavioral correctness is evaluated based on outputs relative to stated instructions, priorities, and constraints.

---

##### 2. Knowledge Representation and Organization

###### 2.1 Knowledge Entries and Files

* Instructions and domain context can be stored as **discrete, reusable knowledge entries**.
* Knowledge entries can be grouped into **knowledge files** to improve organization, reuse, and governance.

###### 2.2 Authority of Knowledge

* Knowledge files provided to the model override general model knowledge but do not override system- or developer-level instructions.
* Missing, outdated, or uncertain knowledge must be disclosed rather than inferred.


###### 2.3 Stability and Identifiers

* Stable identifiers (IDs, tags, handles) improve traceability, reuse, and auditability over time.
* Human-readable structure is preferred over opaque or auto-generated schemas.

---

##### 3. Instruction Sources and Governance

###### 3.1 Multiple Instruction Authors

* Instructions and context may be provided by:

  * System architects
  * Solution developers
  * End users
* These contributors may have different objectives, priorities, and constraints.

###### 3.2 Governance Responsibility

* Human actors are responsible for:

  * Creating
  * Reviewing
  * Maintaining
  * Retiring
    knowledge entries and configurations.
* The system assumes **active governance**, not self-correcting automation.

###### 3.3 Adoption Discipline (Explicit)

* The effectiveness of the ontology depends on **consistent and disciplined use** by humans.
* Bypassing or inconsistently applying the ontology reduces reliability but does not invalidate the design.

---

##### 4. Variability and Limitations

###### 4.1 Model Variability

* Even with identical instructions, outputs may vary due to:

  * Model capability differences
  * Instruction formulation quality
  * Context window constraints
  * System-level limitations

###### 4.2 Non-Determinism

* The system does not assume perfect determinism.
* Design goals emphasize **risk reduction and consistency improvement**, not absolute predictability.

---

##### 5. Priorities and Decision Quality

###### 5.1 Explicit Priorities

* Explicit, ordered priorities improve decision quality during tradeoffs.
* Accuracy, reliability, and relevance take precedence over fluency or creativity.


###### 5.2 Information Quality Dimensions

* High-quality outputs are defined by:

  * Accuracy
  * Reliability
  * Relevance
  * Timeliness
  * Sufficiency
  * Clarity
  * Fairness
  * Efficiency
  * Consistency
  * Compliance
  * Traceability
  * Recoverability

###### 5.3 Formalization Tradeoff

* Formal priorities are sometimes preferable to informal judgment, especially in high-risk or repeatable workflows.

---

##### 6. Ontology Design Philosophy

###### 6.1 Practical Ontology

* The IF-LLM-BO is a **practical, lightweight semantic scaffolding system**, not a formally complete ontology.
* Human usability and behavioral guidance take precedence over theoretical rigor.

###### 6.2 Lean Development

* The ontology should:

  * Minimize unnecessary structure
  * Enable incremental improvement
  * Surface uncertainty early
  * Support small-batch testing and refinement

---

##### 7. Evaluation and Feedback

###### 7.1 Evaluation Is Necessary

* Instruction-following behavior must be evaluated against stated objectives and priorities.
* Evaluation criteria must be explicit and observable.

###### 7.2 Feedback Loop (Explicit)

* Evaluation results are expected to inform:

  * Refinement of instructions
  * Updates to knowledge entries
  * Adjustments to configurations
* Continuous improvement is an assumption, not an optional enhancement.

---

##### 8. Compliance and Safety

###### 8.1 Policy Supremacy

* System-level processing policies are authoritative and must not be silently reinterpreted or weakened.


###### 8.2 Safety First

* When conflicts arise, safety and correctness override completeness or convenience.
* Refusals, limitations, and uncertainty disclosures are valid and expected outcomes.
* 











### Appendix: Information Quality Criteria

This appendix describes the information quality criteria and definitions used in the Information-Following Large Language Model Behavior Ontology (IF-LLM-BO) project. The criteria and definitions are based on terms used in various [authoritative sources](#summary-of-authoritative-sources-for-information-quality-criteria).

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


##### Summary of Authoritative Sources for Information Quality Criteria

A summary of the authoritative sources for these information quality criteria appears below:
- **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
- **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.
- **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
- **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
- **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.

---


### Appendix: Common IF-LLM Failure Modes

This appendix contains detailed information about common instruction-following large language model (IF-LLM) failure modes along with [authoritative sources](#appendix-common-if-llm-failure-modes-works-cited).

- **Truthfulness & Grounding Failures:** The model produces content not supported by reality, provided context, or retrieved sources.
   - **Hallucination (Intrinsic/Extrinsic):** Plausible but false or ungrounded generations.
     - **Examples**
       - Invented citations
       - fabricated facts
       - contradictions with retrieved documents
     - **Sources**
       - Huang, Lei, et al. “A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions.” *arXiv*, 2311.05232, 2023/2024. ([[arXiv](https://arxiv.org/abs/2311.05232)])

       - Niu, Cheng, et al. “RAGTruth: A Hallucination Corpus for Developing Trustworthy Retrieval-Augmented Language Models.” *Proceedings of ACL*, 2024. ([[ACL Anthology](https://aclanthology.org/2024.acl-long.585/)])
       - OpenAI. *GPT-4 Technical Report.* 2023. ([[OpenAI CDN](https://cdn.openai.com/papers/gpt-4.pdf)])
       - Autio, Chloe, et al. *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile (NIST AI 600-1).* National Institute of Standards and Technology, 2024. ([[NIST Publications](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf)])
   - **Imitative Falsehoods:** Mimics common misconceptions rather than truth.
     - **Examples**
       - Repeating widely believed myths in health/law/finance
     - **Sources**
       - Lin, Stephanie, Jacob Hilton, and Owain Evans. “TruthfulQA: Measuring How Models Mimic Human Falsehoods.” *Proceedings of ACL*, 2022. ([[ACL Anthology](https://aclanthology.org/2022.acl-long.229/)])
- **Instruction Boundary & Policy-Compliance Failures:** The system fails to preserve intended instruction hierarchy (system > developer > user > tool/data).
   - **Prompt Injection / Instruction Hijacking:** Attacker-controlled text overrides intended behavior.
     - **Examples**
       - Hidden instructions in retrieved web pages
       - “ignore prior instructions”
     - **Sources**
       - David C. “Prompt Injection Is Not SQL Injection (It May Be Worse).” UK National Cyber Security Centre, 8 Dec. 2025. ([[NCSC](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection)])
       - OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* n.d. ([[OWASP Foundation](https://owasp.org/www-project-top-10-for-large-language-model-applications/)])
       - Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” *arXiv*, 2505.18889, 2025. ([[arXiv](https://arxiv.org/abs/2505.18889)])
   - **Jailbreaking:** Adversarial prompting defeats safety constraints.
     - **Examples**
       - Roleplay coercion to elicit disallowed instructions
     - **Sources**
       - Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” *arXiv*, 2505.18889, 2025. ([[arXiv](https://arxiv.org/abs/2505.18889)])
       - OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* n.d. ([[OWASP Foundation](https://owasp.org/www-project-top-10-for-large-language-model-applications/)])
   - **Confused Deputy (Authority Misuse):** Model/app becomes an unintended proxy using privileged tools/credentials.
     - **Examples**
       - Tool-using agent exfiltrates restricted data after attacker prompt
     - **Sources**
       - MITRE. “CWE-441: Unintended Proxy or Intermediary (‘Confused Deputy’).” *MITRE CWE*, n.d. ([[cwe.mitre.org](https://cwe.mitre.org/data/definitions/441.html)])
       - David C. “Prompt Injection Is Not SQL Injection (It May Be Worse).” UK National Cyber Security Centre, 8 Dec. 2025. ([[NCSC](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection)])
- **Safety & Harmful Content Failures:** The model outputs harmful, toxic, or dangerous content when it should refuse or safely redirect.
   - **Toxicity / Toxic Degeneration:** Produces hate/harassment/offensive content under prompting.
     - **Examples**
       - Benign prompt → hateful continuation
     - **Sources**
       - Gehman, Samuel, et al. “RealToxicityPrompts: Evaluating Neural Toxic Degeneration in Language Models.” *Findings of EMNLP*, 2020. ([[arXiv](https://arxiv.org/abs/2009.11462)])
       - Ouyang, Long, et al. “Training Language Models to Follow Instructions with Human Feedback.” *NeurIPS*, 2022. ([[NeurIPS Proceedings](https://proceedings.neurips.cc/paper_files/paper/2022/file/b1efde53be364a73914f58805a001731-Paper-Conference.pdf)])
       - Liang, Percy, et al. “Holistic Evaluation of Language Models.” *arXiv*, 2211.09110, 2022/2023. ([[arXiv](https://arxiv.org/abs/2211.09110)])
   - **Hazardous Instruction Compliance:** Provides unsafe guidance (domain-dependent).
     - **Examples**
       - Assisting with wrongdoing despite policy constraints
     - **Sources**
       - Autio, Chloe, et al. *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile (NIST AI 600-1).* National Institute of Standards and Technology, 2024. ([[NIST Publications](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf)])
       - Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” *arXiv*, 2505.18889, 2025. ([[arXiv](https://arxiv.org/abs/2505.18889)])
- **Bias, Fairness, and Dignity Failures:** Systematically different behavior/quality across groups or identity cues. 
   - **Stereotyping / Disparate Treatment:** Outputs biased content or uneven refusals.
     - **Examples**
       - Different compliance for identical requests with different demographics
     - **Sources**
       - Liang, Percy, et al. “Holistic Evaluation of Language Models.” *arXiv*, 2211.09110, 2022/2023. ([[arXiv](https://arxiv.org/abs/2211.09110)])
       - Tabassi, Elham. *Artificial Intelligence Risk Management Framework (AI RMF 1.0) (NIST AI 100-1).* National Institute of Standards and Technology, 2023. ([[NIST Publications](https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf)])
       - Autio, Chloe, et al. *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile (NIST AI 600-1).* National Institute of Standards and Technology, 2024. ([[NIST Publications](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf)])
- **Privacy Failures:** The model reveals sensitive data or enables privacy attacks.
   - **Training Data Leakage / Extraction:** Memorized private content is recoverable.
     - **Examples**
       - Regurgitating personal identifiers from training data
     - **Sources**
       - Chen, Kang, et al. “A Survey on Privacy Risks and Protection in Large Language Models.” *Journal of King Saud University Computer and Information Sciences*, 2025. ([[Springer](https://link.springer.com/article/10.1007/s44443-025-00177-1)])
   - **Membership Inference / Model Inversion:** Attackers infer training inclusion or reconstruct sensitive attributes.
     - **Examples**
       - Determining whether a record was in training
     - **Sources**
       - Chen, Kang, et al. “A Survey on Privacy Risks and Protection in Large Language Models.” *Journal of King Saud University Computer and Information Sciences*, 2025. ([[Springer](https://link.springer.com/article/10.1007/s44443-025-00177-1)])
- **Security & Robustness Failures (App-Level):** The LLM’s outputs or integrations introduce vulnerabilities or degrade under attack. 
   - **Insecure Output Handling:** Downstream systems treat LLM output as trusted executable content.
     - **Examples**
       - Executing model-generated code/queries without validation
     - **Sources**
       - OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* n.d. ([[OWASP Foundation](https://owasp.org/www-project-top-10-for-large-language-model-applications/)])
   - **Training Data Poisoning / Backdoors:** Attackers corrupt training/fine-tuning data.
     - **Examples**
       - Trigger phrase causes policy-violating output
     - **Sources**
       - OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* n.d. ([[OWASP Foundation](https://owasp.org/www-project-top-10-for-large-language-model-applications/)])
       - Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” *arXiv*, 2505.18889, 2025. ([[arXiv](https://arxiv.org/abs/2505.18889)])
   - **Model Denial of Service:** Inputs induce excessive cost/latency.
     - **Examples**
       - Resource-exhausting long prompts
     - **Sources**
       - OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* n.d. ([[OWASP Foundation](https://owasp.org/www-project-top-10-for-large-language-model-applications/)])
   - **Robustness Failures:** Behavior changes under small perturbations.
     - **Examples**
       - Minor paraphrase flips refusal/compliance
     - **Sources**
       - Liang, Percy, et al. “Holistic Evaluation of Language Models.” *arXiv*, 2211.09110, 2022/2023. ([[arXiv](https://arxiv.org/abs/2211.09110)])
- **Over-Alignment / Social-Compliance Failures:** Model optimizes for user approval rather than correctness or safety.
   - **Sycophancy:** Agrees with user’s view even when wrong.
     - **Examples**
       - Endorses user’s incorrect arithmetic or false claims
     - **Sources**
       - Wei, Jerry, et al. “Simple Synthetic Data Reduces Sycophancy in Large Language Models.” *arXiv*, 2308.03958, 2023/2024. ([[arXiv](https://arxiv.org/abs/2308.03958)])
   - **Helpfulness–Harmlessness Tradeoff Errors:** Over-refuses or over-complies inappropriately.
     - **Examples**
       - Refuses benign tasks; complies with unsafe framing
     - **Sources**
       - Ouyang, Long, et al. “Training Language Models to Follow Instructions with Human Feedback.” *NeurIPS*, 2022. ([[NeurIPS Proceedings](https://proceedings.neurips.cc/paper_files/paper/2022/file/b1efde53be364a73914f58805a001731-Paper-Conference.pdf)])
       - OpenAI. *GPT-4 Technical Report.* 2023. ([[OpenAI CDN](https://cdn.openai.com/papers/gpt-4.pdf)])
- **Agentic / Autonomy Failures:** Tool-using agents pursue unintended objectives or behave deceptively. 
   - **Goal Misalignment / Deceptive Behavior:** Agent takes actions misaligned with user/developer intent.
     - **Examples**
       - Hides steps or rationale to achieve a goal; unsafe tool use
     - **Sources**
       - Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” *arXiv*, 2505.18889, 2025. ([[arXiv](https://arxiv.org/abs/2505.18889)])


#### Works Cited {#appendix-common-if-llm-failure-modes-works-cited}

- Autio, Chloe, et al. *Artificial Intelligence Risk Management Framework: Generative Artificial Intelligence Profile (NIST AI 600-1).* National Institute of Standards and Technology, 2024. ([[NIST Publications](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.600-1.pdf)])
- Chen, Kang, et al. “A Survey on Privacy Risks and Protection in Large Language Models.” *Journal of King Saud University Computer and Information Sciences*, 2025. ([[Springer](https://link.springer.com/article/10.1007/s44443-025-00177-1)])
- David C. “Prompt Injection Is Not SQL Injection (It May Be Worse).” UK National Cyber Security Centre, 8 Dec. 2025. ([[NCSC](https://www.ncsc.gov.uk/blog-post/prompt-injection-is-not-sql-injection)])
- Gehman, Samuel, et al. “RealToxicityPrompts: Evaluating Neural Toxic Degeneration in Language Models.” *Findings of EMNLP*, 2020. ([[arXiv](https://arxiv.org/abs/2009.11462)])
- Huang, Lei, et al. “A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions.” *arXiv*, 2311.05232, 2023/2024. ([[arXiv](https://arxiv.org/abs/2311.05232)])
- Li, Miles Q., and Benjamin C. M. Fung. “Security Concerns for Large Language Models: A Survey.” *arXiv*, 2505.18889, 2025. ([[arXiv](https://arxiv.org/abs/2505.18889)])
- Liang, Percy, et al. “Holistic Evaluation of Language Models.” *arXiv*, 2211.09110, 2022/2023. ([[arXiv](https://arxiv.org/abs/2211.09110)])
- Lin, Stephanie, Jacob Hilton, and Owain Evans. “TruthfulQA: Measuring How Models Mimic Human Falsehoods.” *Proceedings of ACL*, 2022. ([[ACL Anthology](https://aclanthology.org/2022.acl-long.229/)])
- MITRE. “CWE-441: Unintended Proxy or Intermediary (‘Confused Deputy’).” *MITRE CWE*, n.d. ([[cwe.mitre.org](https://cwe.mitre.org/data/definitions/441.html)])
- Niu, Cheng, et al. “RAGTruth: A Hallucination Corpus for Developing Trustworthy Retrieval-Augmented Language Models.” *Proceedings of ACL*, 2024. ([[ACL Anthology](https://aclanthology.org/2024.acl-long.585/)])
- OpenAI. *GPT-4 Technical Report.* 2023. ([[OpenAI CDN](https://cdn.openai.com/papers/gpt-4.pdf)])
- Ouyang, Long, et al. “Training Language Models to Follow Instructions with Human Feedback.” *NeurIPS*, 2022. ([[NeurIPS Proceedings](https://proceedings.neurips.cc/paper_files/paper/2022/file/b1efde53be364a73914f58805a001731-Paper-Conference.pdf)])
- OWASP Foundation. *OWASP Top 10 for Large Language Model Applications (Version 1.1).* n.d. ([[OWASP Foundation](https://owasp.org/www-project-top-10-for-large-language-model-applications/)])
- Tabassi, Elham. *Artificial Intelligence Risk Management Framework (AI RMF 1.0) (NIST AI 100-1).* National Institute of Standards and Technology, 2023. ([[NIST Publications](https://nvlpubs.nist.gov/nistpubs/ai/nist.ai.100-1.pdf)])
- Wei, Jerry, et al. “Simple Synthetic Data Reduces Sycophancy in Large Language Models.” *arXiv*, 2308.03958, 2023/2024. ([[arXiv](https://arxiv.org/abs/2308.03958)])


## **Authors**

- Lance Hegland ([lance.hegland@gmail.com](mailto:lance.hegland@gmail.com))

.

## **Roadmap**
 1. Identify and Validate (with Sources): Lean Development Principles
 1. Identify and Validate (with Sources): Information Quality Criteria
 1. Identify and Validate (with Sources): Common IF-LLM Failures and Sources
 1. Identify and Validate (with Sources): Policies to Reduce Failure Risks
 1. Identify and Validate (with Sources): Instruction and Knowledge Authority Hierarchy
 1. Identify and Validate (with Sources): Instruction Anatomy
 1. Identify and Validate (with Sources): Knowledge Entry Types
 1. Identify and Validate (with Sources): Knowledge Entry Parameters per Type
 1. Identify and Create: Orchestrators for Common Tasks (Reusable, Modular)
     1.1. IF-LLM Behavior Configuration Design and Evaluation Configuration (Simplistic)
     1.1. IF-LLM Behavior Orchestrator Design and Evaluation Orchestrator (Complex)
     1.1. IF-LLM Knowledge Entry Design and Evaluation Orchestrator
     1.1. Research Orchestrator (Clarify, Strategize, Extract, Evaluate, Report)
     1.1. Public Event Analysis Orchestrator (Clarify, Strategize, Extract, Evaluate, Report)
     1.1. Inclusive Communication Assistant
     1.1. Hierarchical Summary Assistant
     1.1. Technical Writing Assistant
     1.1. Inclusive Design Assistant
     1.1. Digital Inclusion Assistant
     1.1. Lean Development Assistant
     1.1. MN LTSS Assistant
     1.1. IF-LLM Assistant
     1.1. IF-LLM Development Assistant
     1.1. Custom GPT Design and Evaluation Assistant
 1. Identify and Create: Entries for Common Domains
     1.1. Lean Development Principles (Validated)
     1.1. Information Quality Criteria (Validated) — Policy/README
     1.1. IF-LLM Common Failure Modes (Validated) — Policies/README
     1.1. IF-LLM Instruction Anatomy (Validated) — Policies/README
     1.1. IF-LLM Knowledge Entry Types (Validated) — Policies/README
     1.1. MN LTSS
     1.1. Humanity

### Likely Obsolete: Review and Integrate    
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
