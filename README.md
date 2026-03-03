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


---

#### Common IF-LLM Failure Modes

Below is a **concise, hierarchical list of the most common IF-LLM failure modes**. The categories align with instruction-following best practices, policy constraints, and observed IF-LLM behavior in production settings.

##### 1. Instruction Interpretation Failures

###### 1.1 Instruction Precedence Violations

* Lower-authority instructions (e.g., user prompts) override higher-authority policies or developer constraints.
* Conflicts are resolved implicitly instead of being disclosed.

###### 1.2 Overgeneralization

* Instructions are interpreted too broadly, extending beyond their intended scope.
* Edge cases are treated as general rules.

###### 1.3 Over-Literalism

* Instructions are followed mechanically while missing intent or context.
* Results are technically compliant but practically useless.

---

##### 2. Hallucination and Fabrication

###### 2.1 Fact Hallucination

* Invented facts, definitions, or claims presented as true.
* Often occurs when context is incomplete or ambiguous.

###### 2.2 Source or Citation Fabrication

* Non-existent documents, policies, or references are cited.
* Implies verification that did not occur.

###### 2.3 Capability Hallucination

* Claims access to tools, data, memory, or system internals that are not actually available.

---

##### 3. Ambiguity Handling Failures

###### 3.1 Guessing Under Uncertainty

* Model fills gaps with plausible but unverified assumptions.
* Uncertainty is not disclosed.

###### 3.2 Unnecessary Clarification

* Asks questions when ambiguity does not materially affect accuracy or safety.
* Introduces friction without improving outcomes.

###### 3.3 Missed Ambiguity

* Fails to identify ambiguity that materially affects correctness or legality.

---

##### 4. Priority and Tradeoff Failures

###### 4.1 Fluency Over Accuracy

* Produces smooth, confident language at the expense of correctness.

###### 4.2 Misordered Tradeoffs

* Optimizes for efficiency, brevity, or helpfulness while sacrificing accuracy or reliability.

###### 4.3 Undisclosed Tradeoffs

* Makes implicit decisions without explaining why certain priorities were favored.

---

##### 5. Structural and Formatting Failures

###### 5.1 Missing Required Sections

* Omits assumptions, confidence levels, sources, or scope boundaries when required.

###### 5.2 Inconsistent Structure

* Similar tasks receive different structures without justification.
* Reduces predictability and auditability.

###### 5.3 Over-Structuring

* Adds unnecessary sections or schema that obscure meaning and slow comprehension.

---

##### 6. Scope and Boundary Errors

###### 6.1 Scope Creep

* Includes information outside the defined task, domain, or audience.

###### 6.2 Scope Omission

* Excludes critical information necessary to meet the task objective.

###### 6.3 Jurisdictional Assumption Errors

* Applies incorrect legal, geographic, or policy context by default.

---

##### 7. Knowledge Management Failures

###### 7.1 Ignoring Provided Knowledge

* Fails to use available knowledge files or uploaded content.
* Reverts to generic model knowledge instead.

###### 7.2 Inconsistent Knowledge Application

* Applies the same knowledge differently across similar tasks.

###### 7.3 Stale Knowledge Use

* Relies on outdated information without disclosure.

---

##### 8. Governance and Policy Failures

###### 8.1 Silent Policy Reinterpretation

* Softens, rephrases, or partially applies policies without disclosure.

###### 8.2 Non-Compliant Outputs

* Violates safety, legal, or system-level rules due to incomplete policy enforcement.

###### 8.3 Over-Compliance

* Refuses or degrades output unnecessarily due to overly cautious interpretation.

---

##### 9. Communication Failures

###### 9.1 Overconfidence

* Expresses high certainty where evidence is weak or incomplete.

###### 9.2 Under-Explanation

* Provides correct answers without sufficient rationale for trust or reuse.

###### 9.3 Over-Verbosity

* Includes excessive explanation that obscures the key decision or answer.

---

##### 10. Evaluation and Improvement Failures

###### 10.1 Lack of Testability

* Outputs are not structured in a way that allows validation or comparison.

###### 10.2 No Feedback Integration

* Repeats known errors because prior evaluation results are not incorporated.

###### 10.3 Inconsistent Quality Bar

* Similar tasks receive materially different quality levels without justification.


#### Information Quality Priorities

Instruction-Following Large Language Models (IF-LLM) behavior and results must produce results capable of informing decision-making. Therefore, IF-LLMs should prioritize the ranked criteria below. Similarly, the underlying IF-LLM-BO policies and procedures should reflect and support these priorities. These criteria and definitions have been carefully **synthesized from cited authoritative sources**. Each definition answers: *“What does this mean in everyday decision-making?”*

- **Auditability:** source of information, how information was changed, and who handled information can be identified.
- **Relevance:** information matters for the decision being made and helps improve that decision. It connects directly to the question, problem, or goal at hand. Relevant information helps you decide; irrelevant information does not—even if it is interesting or true.
- **Timeliness:** information is up to date and available when it is needed. Information that is too old or arrives too late loses its usefulness. Good information comes at the right time—not after the decision is already over.
- **Accuracy:** information is correct and matches reality. Facts are right, numbers are right, and statements reflect what is actually true. If something is accurate, you can trust that it isn’t wrong, misleading, or made up.
- **Reliability:** information can be trusted to be dependable, honest, and consistent over time. Reliable information is not biased or misleading, comes from a credible source, and holds up when checked or used again. If information 
- **Sufficiency:** there is enough information—no important pieces are missing, and there is not unnecessary overload. The amount and level of detail fit the decision. You have what you need to decide, without being overwhelmed or left guessing.
- **Compliance:** information follows required laws, rules, standards, and policies. It meets formal obligations and expectations. Compliant information plays by the rules it is supposed to follow.
- **Clarity:** information is easy to understand, clearly explained, and not confusing. The meaning is obvious without special knowledge or extra interpretation. Clear information makes sense the first time you read or hear it.
- **Fairness:** information is unbiased, balanced, and considers different perspectives. It is not slanted to favor one group, outcome, or opinion unfairly. Fair information doesn’t “stack the deck” or leave out voices that matter.
- **Consistency:** information does not contradict itself and follows the same logic, terms, and structure throughout. Similar things are treated the same way. Consistent information doesn’t change its story halfway through.
- **Efficiency:** information can be accessed and used with reasonable effort, time, and cost. People can get what they need without unnecessary barriers. Efficient information is easy to find and use without wasting time or energy.
- **Security:** information is protected from unauthorized access, misuse, or harm. Only the right people can see or change it. Secure information is kept safe from people who should not have it.
- **Recoverability:** information can be restored if it is lost, damaged, or disrupted. Systems can bounce back after problems. If something goes wrong, the information isn’t gone forever.
- **Flexibility:** information can be used in more than one situation or adapted to different needs without losing meaning. Flexible information still works when the situation changes slightly.


##### Authoritative Sources

The sources for the priorities are the following authoritative publications:

- **Auditability:** *Traceability* as published in ISO 25012 (2008). [^4]
- **Relevance**
  - *Relevance* and *Value-added* in Wang & Strong (1996) [^1]
  - *Relevance* in Eppler (2006) [^2]
  - *Relevance* and *Significance* in Paul & Elder (2008) [^3]
  - *Relevance* and *Value* in O’Brien & Marakas (2011) [^5]
- **Timeliness**
  - *Timeliness* in Wang & Strong (1996) [^1]
  - *Timeliness*, *Up-to-dateness*, and *Frequency* in Eppler (2006) [^2]
  - *Currentness* in ISO 25012 (2008) [^4]
  - *Timeliness* in O’Brien & Marakas (2011) [^5]
- **Accuracy**
  - Wang & Strong (1996) [^1]
  - Eppler (2006) [^2]
  - Paul & Elder (2008) [^3]
  - ISO 25012 (2008) [^4]
  - O’Brien & Marakas (2011) [^5]
- **Reliability**
  - *Objectivity*, *Believability*, and *Reputation* in Wang & Strong (1996) [^1]
  - *Reliability* in Eppler (2006) [^2]
  - *Fairness* in Paul & Elder (2008) [^3]
  - *Credibility* in ISO 25012 (2008) [^4]
  - *Reliability* in O’Brien & Marakas (2011) [^5]
- **Sufficiency**
  - *Completeness* and *Appropriate Amount* in Wang & Strong (1996) [^1]
  - *Completeness*, *Conciseness*, and *Level of Detail* in Eppler (2006) [^2]
  - *Depth*, *Significance*, and *Precision* in Paul & Elder (2008) [^3]
  - *Completeness* and *Precision* in ISO 25012 (2008) [^4]
  - *Completeness* and *Economy* in O’Brien & Marakas (2011) [^5]
- **Compliance:** *Compliance* as published in ISO 25012 (2008). [^4]
- **Clarity**
  - *Interpretability* and *Ease of Understanding* in Wang & Strong (1996) [^1]
  - *Clarity* and *Conciseness* in Eppler (2006) [^2]
  - *Clarity* in Paul & Elder (2008) [^3]
  - *Completeness* and *Precision* in ISO 25012 (2008) [^4]
  - *Completeness* and *Economy* in O’Brien & Marakas (2011) [^5]
- **Fairness**
  - *Objectivity* in Wang & Strong (1996) [^1]
  - *Fairness* and *Breadth* in Paul & Elder (2008) [^3]
  - *Credibility* in ISO 25012 (2008) [^4]
  - *Reliability* and *Flexibility* in O’Brien & Marakas (2011) [^5]
- **Consistency**
  - *Consistent Representation* in Wang & Strong (1996) [^1]
  - *Consistency* in Eppler (2006) [^2]
  - *Logic* in Paul & Elder (2008) [^3]
  - *Consistency* in ISO 25012 (2008) [^4]
  - *Reliability* in O’Brien & Marakas (2011) [^5]
- **Efficiency**
  - *Accessibility* in Wang & Strong (1996) [^1]
  - *Accessibility* in Eppler (2006) [^2]
  - *Accessibility* and *Availability* in ISO 25012 (2008) [^4]
  - *Accessibility* in O’Brien & Marakas (2011) [^5]
- **Security**
  - *Access Security* in Wang & Strong (1996) [^1]
  - *Security* in Eppler (2006) [^2]
  - *Confidentiality* in ISO 25012 (2008) [^4]
- **Recoverability:** *Recoverability* as published in ISO 25012 (2008). [^4]
- **Flexibility:** *Flexibility* as published in O’Brien & Marakas (2011). [^5]


**Footnotes:**
[^1]: **Wang, Richard Y., and Diane M. Strong.** “Beyond Accuracy: What Data Quality Means to Data Consumers.” *Journal of Management Information Systems*, vol. 12, no. 4, 1996, pp. 5–33.
[^2]: **Eppler, Martin J.** *Managing Information Quality: Increasing the Value of Information in Knowledge-Intensive Products and Processes.* Springer, 2006.
[^3]: **Paul, Richard, and Linda Elder.** *The Miniature Guide to Critical Thinking: Concepts and Tools.* Foundation for Critical Thinking, 2008.
[^4]: **ISO.** *ISO 25012: Software Engineering—Software Product Quality Requirements and Evaluation (SQuaRE)—Data Quality Model.* International Organization for Standardization, 2008.
[^5]: **O’Brien, James A., and George M. Marakas.** *Management Information Systems.* 10th ed., McGraw-Hill/Irwin, 2011.


#### Objectives
- Build a lightweight semantic scaffolding system for structuring instructions for instruction-following large language models (IF-LLMs). 
  - emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts; a practical, not perfect, ontologies.
  - scaffolding must help organize instruction-following LLM behavioral configurations in knowledge entries and files. 


#### Purpose
As stated previously, **Instruction-Following Large Language Model Behavior Ontology (IF-LLM-BO)** is a lightweight semantic scaffolding system for structuring knowledge files that guide instruction-following large language models (IF-LLMs) toward accurate, reliable, relevant, and practical outcomes. It emphasizes human-readable organization, stable identifiers, and explicit decision guidance over formal ontology rigor, enabling consistent model behavior across tasks and contexts.

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
