# Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) (*README.md*)

**PURPOSE:** The **Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is a lightweight semantic scaffolding system for organizing [instruction-following large language model (IF-LLM) elements](!!!TODO!!!) to guide [IF-LLMs](!!!TODO!!!) toward [higher-quality responses](#decision-making-information-quality-criteria-priorities). IF-LLM-BO emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across objectives, workflows, contexts, and audiences.


## **Table of Contents**

- TO DO: [Unorganized Content](#not-yet-organized-1)
- [Features](#features)
- [Background](#background)
- [Known Issues](#known-issues)
- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Usage](#usage)
- [IF-LLM-BO Project](!!!TODO!!!)
  - [Foundations](#foundations)
    - [Assumptions](#assumptions)
    - [Decision-Making Information Quality Criteria (Priorities)](#decision-making-information-quality-criteria-priorities)
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
- [File Header](#file-header)


## NOT YET ORGANIZED

TODO: Review then integrate or eliminate [content that is not yet organized](#not-yet-organized-1)


## **Features**

TODO


## **Background**

TODO


## **Known Issues**

NONE — There are no know issues as of April 2026. However, the IF-LLM sub-industry is evolving quickly and is still in its public infancy. Therefore, information should be periodically reviewed, verified, and refined.


## **Requirements**

1. Familiarity using and access to [an instruction-following large language model (IF-LLM)](#common-if-llms)
1. Familiarity using and access to [GitHub](https://github.com/)
1. Agree to the [Creative Commons Attribution Share Alike 4.0 International License (CC-BY-SA-4.0)](LICENSE.txt)
1. Review [README's Table of Contents](README.md) plus [Challenges and Solutions](!!!TODO!!!) sections


## **Installation**

1. Perform the necessary actions to satisfy the [minimum requirements](#requirements).
1. From your local projects directory, copy [the entire IF-LLM-BO project's remote GitHub repository](https://github.com/LHHegland/if-llm-behavior-ontology/tree/main) into your local project directory.
1. Upload the following files to a new conversation in [your favorite instruction-following large language model (IF-LLM)](!!!TODO!!!) to give the model access to the stored instructions and context (relevant background information) for that conversation.
   - ~~system-knowledge-policies.md~~ — *NOT YET AVAILABLE*
   - system-processing-policies.md
   - ~~system-tasks.md~~ — *NOT YET AVAILABLE*
   - ~~system-domains.md~~ — *NOT YET AVAILABLE*
   - ~~system-reasonings.md~~ — *NOT YET AVAILABLE*
   - ~~system-structures.md~~ — *NOT YET AVAILABLE*
   - ~~system-personas.md~~ — *NOT YET AVAILABLE*
   - ~~system-examples.md~~ — *NOT YET AVAILABLE*
   - system-configurations.md
   - system-orchestrators.md
1. Copy the following prompt and paste it into the IF-LLM prompt field (or perform the necessary steps if you are using an API).
    ```
    # Configuration
    
    Please use the following uploaded files for purposes indicated below during this conversation:
    - `system-processing-policies.md` contains **System-Level Processing Policies**
    - `system-configurations.md` contains **System-Level Behavior Configurations**
    - `system-orchestrators.md` contains **System-Level Behavior Orchestrators**   
    ```


## **Configuration**

NONE — No configuration is required.


## **Usage**

1. Perform the necessary actions to complete the [installation](#installation).
1. Submit your task prompt or question to the IF-LLM.
   1. Optional:
      1. Review [`system-prompt-templates.md`](system-prompt-templates.md) to find a prompt to achieve your desired objective.
      1. Copy and paste the prompt into the IF-LLM prompt field.
      1. Overwrite the variable input placeholders with your input data (i.e., `<variable input placeholder>`) (e.g., `<full name>` → `Pat Smith`, `<topic>` → `entomology`, `<objective>` → `better understand the risks to human health from flying insects`, `<audience>` → `average people from the many, widespread, and diverse communities throughout the United States of America today`).
      1. Submit your prompt to the IF-LLM.

---


## **IF-LLM-BO Project Notes**

The following sections contain notes related to the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project:
- [Foundations](#foundations)
  - [Assumptions](#assumptions)
  - [Decision-Making Information Quality Criteria (Priorities)](#decision-making-information-quality-criteria-priorities)
  - [Common IF-LLM Failure Modes](#common-if-llm-failure-modes)
  - [Common IF-LLM Failure Mitigation Strategies](#common-if-llm-failure-mitigation-strategies)
- [Purpose](#purpose)
- [Objectives](#objectives)
- [Governance, Policies, Rules](#governance-policies-and-rules)
- [Prompt Templates, Orchestrators, Configurations](#prompt-templates-orchestrators-configurations)


---

### Foundations

The following sections describe the foundations grounding the IF-LLM-BO project:
- [Assumptions](#assumptions)
- [Decision-Making Information Quality Criteria (Priorities)](#decision-making-information-quality-criteria-priorities)
- [Common IF-LLM Failure Modes](#common-if-llm-failure-modes)
- [Common IF-LLM Failure Mitigation Strategies](#common-if-llm-failure-mitigation-strategies)


---

#### Assumptions

TO DO: Create Summary

Below is a summary of the underlying assumptions for the Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO) project.  More detailed information about these assumptions can be found in the [Appendix: Assumptions](#appendix-assumptions).

There is credible and sufficient evidence that instruction-following large language models (IF-LLMs) produce a finite number of [common failure modes](#common-if-llm-failure-modes).

IF-LLMs produce results that are likely considered when making future decisions. Therefore, the results they produce should meet [well-defined quality standards](#decision-making-information-quality-criteria-priorities).


---


#### Decision-Making Information Quality Criteria (Priorities)

[Instruction-following large language models (IF-LLMs)](!!!TODO!!!) are often used to generate information that can influence decisions impacting people and other systems. Because of this, the responses they produce should meet clear and well-defined quality standards. Therefore, IF-LLMs should prioritize these quality standards according to their ranked importance. Any trade-offs should be disclosed to users. Meaning, the [instructions and context guiding IF-LLMs](!!!TODO!!!) — especially the system-level policies — should reflect and reinforce these priorities.

The priorities listed below identify the key criteria that information should have in order to reliably support decision-making. Each definition answers a practical question: *"What does this mean for everyday decision-making?"*

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

#### Common IF-LLM Failure Modes

Below is a high-level summary of the common instruction-following large language model (IF-LLM) failure modes (as of March 2026).  More detailed information about these failure modes, along with examples and authoritative sources, can be found in the [Appendix: Common IF-LLM Failure Modes with Examples and Sources](#common-failure-modes).

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

The **Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is a lightweight semantic scaffolding system for organizing [instruction-following large language model (IF-LLM) elements](!!!TODO!!!) to guide [IF-LLMs](!!!TODO!!!) toward [higher-quality responses](#decision-making-information-quality-criteria-priorities). IF-LLM-BO emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across objectives, workflows, contexts, and audiences. It includes [Governance, Policies, and Rules](#governance-policies-and-rules) plus [Prompt Templates, Orchestrators, and Configurations](#prompt-templates-orchestrators-configurations) to most efficiently fulfill its purpose.


---

### Objectives

First, the IF-LLM-BO project intends to build a lightweight semantic scaffolding system for structuring instructions and context for instruction-following large language models (IF-LLMs) that accomplishes the following: 
  - emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across objectives, workflows, contexts, and audiences; a practical, yet not perfect, ontology
  - empowers [human governance](#system-architect-and-solution-developer-governance-human-governance) (i.e., for system architects and solution developers)
  - reduces IF-LLM failure risks through validated, stored, and reusable IF-LLM [knowledge policies (i.e., validated, stored, and reusable instructions and context](#knowledge-file-and-knowledge-entry-policies-stored-context-policies) and [processing rules (i.e., validated, stored, and reusable instructions](#processing-policies-stored-instruction-rules).
  - stores validated, reusable prompt elements, configurations, and orchestrators in structured knowledge entries and files
  - empowers greater user efficiency through easily reusable templates combining relevant user inputs with various validated, stored, and reusable IF-LLM elements (e.g., prompt templates, configurations, orchestrators)
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

The likelihood for IF-LLM behavioral correctness can be improved — risks of encountering [common IF-LLM failure modes](#common-if-llm-failure-modes) can be reduced — by using [common IF-LLM failure mitigation strategies](#common-if-llm-failure-mitigation-strategies). These strategies generally rely on humans consistently practicing [human governance](#system-architect-and-solution-developer-governance-human-governance), including using explicit IF-LLM instructions such as [stored knowledge (context) policies](#knowledge-file-and-knowledge-entry-policies-stored-context-policies) and [stored instruction rules](#processing-policies-stored-instruction-rules)).


---

#### System Architect and Solution Developer Governance (Human Governance)

Humans are ultimately responsible for creating, reviewing, updating/maintaining, and deleting/retiring instructions and context for instruction-following large language models (IF-LLMs). Meaning, humans must actively govern the overall system and developed solutions.

Instructions and context may be provided by system architects, solution developers, and end users. End users may not have the experience, knowledge, skills, or tools to effectively use [common IF-LLM failure mitigation strategies](#common-if-llm-failure-mitigation-strategies) consistently. Therefore, the vast majority of responsibility must be assumed by system architects and solution developers.

Instruction and context contributors often have different objectives, priorities, and constraints. As such, there are multiple layers of governance, policies, and rules: system, developer, and user layers. To offer the necessary flexibility, IF-LLMs process instructions and context using a **strict authority hierarchy**, where higher-authority instructions override lower-authority inputs (i.e., [Instruction and Context Hierarchy](#instruction-and-context-authority-hierarchy)). To maintain reliability, stability, and auditability, this authority hierarchy must be respected; lower-level policies must not *silently* reinterpret or weaken higher-level policies. Lower-level policies *can* override higher-level policies if necessary, just not *silently*; overrides must be **explicitly disclosed to end users**.

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
 
More detailed information about these governance policies can be found in the [Appendix: Governance, Policies, Rules](#appendix-if-llm-bo-governance-policies-and-rules) > [System Architect and Solution Developer Governance (Human Governance)](#system-architect-and-solution-developer-governance-human-governance-1).


---

#### Knowledge File and Knowledge Entry Policies (Stored Context (Knowledge) Policies)
TBD

Instruction-following large language model (IF-LLM) [instructions and context](!!!TODO!!!) can be stored as **discrete, reusable [knowledge entries](!!!TODO!!!)**. Knowledge entries are generally grouped by type into **[knowledge files](!!!TODO!!!)** to improve organization, reuse, and governance. Human-readable structure is preferred for entries over opaque or auto-generated schemas for clarity.

Knowledge entries provided by the users to IF-LLMs override general model knowledge but do not override system- or developer-level instructions. More information can be found in the section [Instruction and Context Hierarchy](#instruction-and-context-authority-hierarchy). 

Below is a high-level summary of recommended IF-LLM policies related to knowledge files and entries for system architects and solution developers:
- [Knowledge File Naming Convention Rule](#knowledge-file-naming-convention-rule)
- [Knowledge File Root ID and Tag Convention Rule](#knowledge-file-root-id-and-tag-convention-rule)

More detailed information about these policies can be found in the [Appendix: Governance, Policies, Rules](#appendix-if-llm-bo-governance-policies-and-rules) > [Knowledge File and Knowledge Entry Policies (Stored Context Policies)](#knowledge-file-and-knowledge-entry-policies-stored-context-policies-1).


---

#### Processing Policies (Stored Instruction Rules)

System architects and solution developers should also remain aware of the [system-level processing policies](system-policies-processing.md#processing-policies). The list below offers a high-level summary of rules that IF-LLMs are asked to enforce as part of the IF-LLM-BO project:
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

More detailed information about these rules can be found in the [Appendix: Governance, Policies, Rules](#appendix-if-llm-bo-governance-policies-and-rules) > [Processing Policies (Stored Instruction Rules)](#processing-policies-stored-instruction-rules-1).


---
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

[Instructions and contextual elements](!!!TODO!!!) can be stored as **discrete, reusable [knowledge entries](!!!TODO!!!)**. Knowledge entries can be grouped into **[knowledge files](!!!TODO!!!)** to improve organization, reuse, and governance.

Knowledge files provided to the model override general model knowledge but do not override system- or developer-level instructions.

Stable identifiers (IDs, tags, handles) for knowledge entries improve traceability, reuse, and auditability over time.

Human-readable structure is preferred over opaque or auto-generated schemas for clarity.

Instructions and contextual elements can be stored as **discrete, reusable [prompt templates](!!!TODO!!!)**, also stored in a dedicated knowledge file.

Specific combinations of instructions and contextual elements can be stored as **discrete, reusable [configurations](!!!TODO!!!)**, stored in a dedicated knowledge file too.

Specific arrangements of configurations can be stored as **discrete, reusable [orchestrators](!!!TODO!!!)**, stored in a dedicated knowledge file as well.

Missing, outdated, or uncertain knowledge should be disclosed rather than inferred to ensure auditability.

Refusals, limitations, and uncertainty disclosures are valid and expected outcomes for most IF-LLMs.

When conflicts arise, safety and correctness often override completeness or convenience for most IF-LLMs.

Using a [semi-formal ontology](!!!TODO!!!) to establish system-level policies, contextual defaults, and offer reusable, standardized instructions for common use cases can help improve behavioral correctness and reduce risks of encountering common failure modes.

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

Instruction-following large language models (IF-LLMs) are often used to generate information that influence decisions impacting people and other systems. Because of this, the responses they produce should meet clear and well-defined quality standards. The quality standards listed below identify the key criteria that information should have in order to reliably support decision-making. To produce information that meaningfully supports decisions, IF-LLMs should prioritize these criteria according to their ranked importance. Any trade-offs should be disclosed to users. In turn, the policies and procedures governing IF-LLM-BO systems should be designed to reflect and reinforce these priorities. The criteria listed below are shown in their order of importance; their priorities.

The criteria and definitions presented here are **synthesized from the cited authoritative sources**. Each definition is written to answer a practical question: *“What does this mean for everyday decision-making?”*

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

### Appendix: IF-LLM Instruction and Context Authority Hierarchy

TODO: Briefly define the hierarchy of IF-LLM instructions and knowledge authority as outlined below, including how instructions are granted authority, critical phrases used to grant/assign authority, plus 3 to 5 examplesto help users understand the value of this hierarchy.
1. System Instructions and Context (Global Policies and Context) (e.g., knowledge entries with the highest authority (i.e., meta knowledge entries))
2. Developer Instructions and Context (e.g., knowledge entries with the second-highest authority, developer implemented knowledge entries)
3. User Instructions and Context (i.e., the current conversation via chat or API, which could reference existing knowledge entries)
4. Knowledge Files (and their collection of entries)
5. User-Uploaded Files (e.g., user-uploaded files, which are considered user knowledge files containing user knowledge injuries)
6. Tool Outputs
7. General Model Knowledge

IF-LLMs receive instructions through either user prompts (e.g., chat interfaces or APIs) or developer instructions. Users and developers can store reusable instructions and context in knowledge entries of various types. Knowledge entries can be organized into knowledge files.


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

- TO DO: [Unorganized Content](!!!TODO!!!)
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
    - [Common IF-LLM Failure Modes](#common-if-llm-failure-modes)
    - [Common IF-LLM Failure Mitigation Strategies](#common-if-llm-failure-mitigation-strategies)
  - [Purpose](#purpose)
  - [Objectives](#objectives)
  - [Governance, Policies, Rules](#governance-policies-and-rules)
    - [Human Governance (System Architect and Solution Developer Governance)](#system-architect-and-solution-developer-governance-human-governance)
    - [Stored Context Policies (Knowledge File and Knowledge Entry Policies)](#knowledge-file-and-entry-policies-stored-context-policies)
    - [Stored Instruction Rules (Processing Policies)](#processing-policies-stored-instruction-rules)
  - [Prompt Templates, Orchestrators, Configurations](#prompt-templates-orchestrators-configurations)
- [Appendices](#appendices)
  - [Assumptions](#appendix-assumptions)
  - [Evidenced-based Information Criteria (Research)](#appendix-evidenced-based-information-criteria-research)
  - [Decision-Making Information Quality Criteria (Priorities) with Definitions and Sources](#appendix-decision-making-information-quality-criteria-priorities-with-definitions-and-sources)
    - [Summary of Authoritative Sources for Decision-Making Information Quality Criteria (Priorities)](#summary-of-authoritative-sources-for-decision-making-information-quality-criteria-priorities)
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

**Version:** 2026-04-09T02:51Z LH in [if-llm-behavior-ontology](https://github.com/LHHegland/if-llm-behavior-ontology)

**Last Reviewed:** 2026-03-30T11:59Z — [Lance Hegland](mailto:lance.hegland@gmail.com)

**Changelog**
- 2026-04-09T02:51Z — [Lance Hegland](mailto:lance.hegland@gmail.com): Split IF-LLM eBook and IF-LLM-BO projects
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











## NOT YET ORGANIZED

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
