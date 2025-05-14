# Appendix 1 - Pharmacovigilance

## A theoretical COSMOS implementation

The COSMOS framework could provide an ideal architecture for enhancing pharmacovigilance (PV) operations through its neurologically-inspired design. Applying the COSMOS framework to pharmacovigilance (PV) involves leveraging COSMOS's neurologically inspired architecture to automate and enhance drug safety monitoring and adverse events. This theoretical implementation demonstrates how COSMOS's three primary subsystems and cyclical architecture might be applied to drug safety monitoring and adverse event management in the future. 

## Pharmacovigilance Overview

### 1. Metacognitive Architect for Case Processing

    The Metacognitive Architect subsystem monitors the processing of Individual Case Safety Reports (ICSRs) workflow for reporting the appropriate adverse event, ensuring consistency in their event classification, evaluation of their minimum criteria to classify ICSR cases, appropriate causality assessment, and ensuring regulatory compliance in reporting the ICSRs. This layer identifies conflicting causality assessments, flags contradicting conclusions, cross-references the extracted data with existing available pharmacovigilance databases to identify duplicate or missing data, ensures compliance with evolving and new regulatory guidelines (such as FDA's Emerging Drug Safety Technology Program (EDSTP) for Pharmacovigilance) and highlights errors or uncertainties for human review while generating ICSR case reports. Within the COSMOS framework, this functions as a quality control system that continuously evaluates and refines both the Self-Model (regulatory frameworks, medical terminology, processing protocols) and World-Model (drug safety profiles) based on incoming adverse event data.

### 2. Perceptual Filtering & Attention Mechanisms

    The perceptual filtering and attention mechanism help in Safety Signal Management in Pharmacovigilance for adverse events to identify true safety signals from the non-signals and noises. Filtering occurs on the basis of sufficient evidences such as previous awareness of the safety signal, strength of evidence between signal and the drug, assessment of clinical context on public health such as seriousness of the event, and criteria based on novelty of drugs to classify them as a true signal or not to be worked upon. Within the COSMOS framework, this implements selective attention that focuses on goal-relevant input required to identify true safety signals while suppressing extraneous or redundant information on low priority data such as duplicate signals or erroneous signals, allowing efficient allocation of cognitive resources to the most significant safety concerns.

### 3. Predictive Processing for Risk Mitigation

    Evaluation of usefulness of the medicine (e.g, drugs to a health condition or a disease) in Benefit and Risk Analysis in Pharmacovigilance where determining probability of their positive and negative effects for both new drug and re-purposed drug from the existing data sources such as medical literature, FDA’s adverse event reporting system (AERS), clinical trial data etc. will help in identifying potential adverse events to patient’s health and outcome. The Real-time monitoring of expected adverse event patterns during post-market surveillance of the marketed drugs, can trigger alerts regarding potential safety issues on the usage of particular drug which might change the assessment on their benefits and risks enabling for a proactive step to be taken before large scale impact due to the consumption of the drug.

### 4. Error Monitoring & Self-Correction

    The automated self-monitoring and error correction capabilities with "conditions of success" framework includes such detection of signals that are valid to be considered for a potential adverse event, while categorizing the signals based on specific criteria and appropriate data and ensuring if the signal was identified previously for same adverse events, and if the signal was mitigated differently through different procedures for ensuring patient's safety. In this case, error monitoring can help identify the genuine, valid signals to be worked upon with the aspect of self-correction on identification of their previously documented adverse events from various data sources such as FDA's AERS, Europe's EudraVigilance etc. and understanding the procedure followed to mitigate the risk caused by the signal to the patient. This structured approach facilitates incremental improvement through feedback loops, enabling refinement of both execution and monitoring capabilities within the COSMOS cognitive cycle.

## Architectural Alignment

This hypothetical pharmacovigilance implementation would map to COSMOS's three primary subsystems as follows:

### Metacognitive Architect 

This subsystem handles perception, memory formation, and evaluation in the PV context:

* **Case Processing and Quality Control**: A metacognitive LLM monitors Individual Case Safety Reports (ICSRs), ensuring consistent event classification, appropriate causality assessment, and regulatory compliance. This layer cross-references extracted data with existing pharmacovigilance databases to identify duplicates or missing information, while ensuring adherence to evolving regulatory guidelines (such as FDA's Emerging Drug Safety Technology Program). It highlights errors or uncertainties for human review while monitoring ICSR case reports, functioning as a quality control system.

* **Self-Model Management**: The Architect creates a dynamic self-model containing relevant regulatory frameworks, medical terminology, and processing protocols needed for the current PV task. It is also responsible for updating this model as regulations or procedures change - adding, editing or removing details from Episodic Memory as needed.

* **World-Model Curation**: Information from medical literature, clinical trials, and adverse event databases is continuously filtered and organized into a coherent world-model that represents the current understanding of drug safety profiles and emerging signals.

### Executive Planner

This subsystem handles decision-making and planning in the PV workflow:

* **Safety Signal Management**: The Executive Planner analyzes filtered data to identify genuine safety signals, distinguishing them from noise by evaluating evidence strength, prior awareness, clinical context, and public health impact. It then formulates action plans for signal validation, assessment, and potential regulatory action.

* **Benefit-Risk Analysis**: The Executive Planner evaluates the usefulness of medications by determining probabilities of positive and negative effects based on the curated world-model, supporting both new drug assessments and repurposed medications.

### Sensory Interface

This subsystem handles environmental interaction and implements planned actions:

* **Data Collection and Processing**: The Sensory Interface interacts with various data sources including FDA's adverse event reporting system (AERS), clinical trial databases, medical literature, and real-world evidence platforms.

* **Alert Generation and Reporting**: Based on plans from the Executive Planner, the Sensory Interface generates appropriate regulatory reports, healthcare professional communications, or internal alerts regarding potential safety issues.

## Integrated Cognitive Cycle

The pharmacovigilance implementation operates through a continuous COSMOS cognitive cycle:

1. **Data Acquisition**: The Sensory Interface gathers adverse event reports, literature findings, and regulatory updates.

2. **Information Processing**: The Metacognitive Architect filters this data based on relevance, significance, and alignment with current safety priorities.

3. **Memory Formation**: The Architect updates both the system's understanding of drug safety (world-model) and and the applicable regulatory compliance requirements (self-model).

4. **Planning and Decision-Making**: The Executive Planner analyzes the updated models to identify necessary actions for signal validation, risk assessment, and or regulatory reporting.

5. **Action Implementation**: The Sensory Interface executes these plans through assessment tools/applications, reporting systems, communication channels, or data entry applications.

6. **Outcome Assessment**: The Architect evaluates the effectiveness of actions taken such as impact to the patient or its outcome, refining both models for the next iteration of the cycle.

## Memory Architecture Implementation

The PV implementation utilizes COSMOS's three-tiered memory system:

* **Episodic Memory**: Stores specific ICSR case report histories, regulatory interactions, and historical signal evaluations that can inform and support future assessments.

* **Semantic Memory**: Maintains a structured knowledge base of medical literature terminology, adverse event reactions, drug interaction mechanisms, valid signals and regulatory frameworks in a vector database with knowledge graph overlay.

* **Procedural Memory**: Contains standardized workflows for case processing, signal evaluation, and regulatory reporting as executable tools with defined parameters and information on how to use them.

## Tool Management System

The PV implementation adopts COSMOS's tool management approach:

* **Tool Repository**: Maintains a comprehensive collection of assessment framework and methodologies, statistical tools, reporting templates, and database queries relevant to pharmacovigilance.

* **Dynamic Tool Selection**: For each task, the Architect selects only the relevant tools, such as analysis algorithms for signal detection or regulatory reporting templates for specific jurisdictions.

* **Active Tool Set**: Only task-relevant tools are made available to the Executive Planner, preventing tool overload and inappropriate tool selection.

## Predictive Processing for Risk Mitigation

The Executive Planner implements predictive processing to anticipate safety issues before they escalate:

* Real-time monitoring of adverse event patterns during post-market surveillance enables the system to predict potential safety issues based on emerging data patterns.

* These predictions trigger proactive risk assessment and mitigation planning before widespread impact occurs.

* The system continuously refines its predictive models based on outcome evaluations from the cognitive cycle.

## Error Monitoring & Self-Correction

The PV implementation incorporates COSMOS's error monitoring framework with explicit success conditions:

* Each pharmacovigilance task includes clearly defined "conditions of success" such as detection of valid signals, appropriate categorization based on specific criteria, and verification against historical data.

* The system can evaluate its performance against these conditions and initiate corrective actions when discrepancies are detected.

* This approach ensures that only genuine, valid signals are processed, with self-correction mechanisms for identifying previously documented adverse events from sources like FDA's AERS and Europe's EudraVigilance.

## Goal Management

The PV implementation follows COSMOS's goal management framework:

* **Goal Acquisition**: Primary goals are set by source of the adverse event collected from various sources, their respective regulatory requirements and mitigation strategy of safety signals, with human oversight.

* **Task Decomposition**: Complex pharmacovigilance objectives are broken down into structured tasks with defined dependencies.

* **Success Criteria**: Each task includes explicit conditions of success to enable self-assessment.

* **Progress Monitoring**: The system continuously tracks progress toward drug safety monitoring goals, adapting plans as new data emerges.

## COSMOS-Based Pharmacovigilance in Action: A Step-by-Step Example

The following scenario illustrates how the COSMOS framework operates in a real-world pharmacovigilance context, tracing the complete cognitive cycle for a potential safety signal for a cardiovascular medication.

### Cycle 1: Initial Signal Detection

1. **Data Acquisition (Sensory Interface)**
   * The system ingests 15 new spontaneous adverse event reports for medication NovoCard (hypothetical medication), with 7 reports mentioning unusual liver enzyme elevations.
   * Simultaneously, it detects a recently published research paper describing a potential mechanism for hepatotoxicity in similar compounds.

2. **Information Processing (Metacognitive Architect)**
   * The Architect filters and evaluates these reports against the established safety profile for NovoCard, which previously had no significant liver-related warnings.
   * It identifies a potential statistical signal using a disproportionality analysis algorithm, calculating a reporting odds ratio (ROR) of 3.2 with a confidence interval above 1.0.

3. **Memory Formation (Metacognitive Architect)**
   * The Architect updates the world-model with the emerging signal data.
   * It retrieves relevant episodic memories of similar signals detected for related medications in the same therapeutic class.
   * It accesses semantic memory for liver toxicity assessment frameworks from its knowledge base.

4. **Planning and Decision-Making (Executive Planner)**
   * The Executive Planner, working with the updated models, evaluates the signal against predetermined criteria for validity and prioritization.
   * It formulates a signal validation plan requiring:

       1. retrieval of complete patient records for the cases,
       2. literature review for similar compounds,

5. **Action Implementation (Sensory Interface)**
   * The Sensory Interface sends requests for additional information to reporters.
   * It initiates a structured literature search focused on hepatotoxicity in similar compounds.
   * It consolidates the results and sends them to the Architect.

### Cycle 2: Signal Validation

1. **Data Acquisition (Sensory Interface)**
   * The system receives the requested AE reporter information, at least one identifiable patient, at least one suspected adverse reaction and one suspected medicinal product.
   * The patient records with detailed lab results from their electronic health record is gathered.
   * It gathers results from the literature search and preclinical data review.

2. **Information Processing (Metacognitive Architect)**
   * The Architect analyzes the lab patterns, identifying a consistent signature of hepatocellular injury without cholestasis.
   * It finds two previous publications describing similar reactions in chemically related compounds.

3. **Memory Formation (Metacognitive Architect)**
   * The world-model is updated with the validated pattern of hepatotoxicity.
   * The self-model is updated to include newly relevant regulatory reporting requirements for hepatic adverse events.

4. **Planning and Decision-Making (Executive Planner)**
   * The Executive Planner confirms the signal validity based on the consistency of the lab patterns and supporting literature.
   * It creates a comprehensive risk assessment plan to evaluate incidence rate, risk factors, and potential risk minimization measures.
   * It advises that expedited regulatory reporting is warranted.
   * It writes a search request for similar cases in the data sources.
   * It generates a healthcare professional information request to gather additional data on potential risk factors.

5. **Action Implementation (Sensory Interface)**
   * The Sensory Interface submits expedited reports to regulatory authorities.
   * It initiates the search query to identify similar cases that may have been missed.
   * It sends the healthcare professional information request to gather additional data on potential risk factors.

6. **Outcome Assessment (Metacognitive Architect)**
   * The Architect verifies that all regulatory submissions were completed within required timeframes.
   * It evaluates the search results to identifying additional cases.

### Cycle 3: Risk Assessment and Mitigation

1. **Data Acquisition (Sensory Interface)**
   * The system collects responses from healthcare professionals regarding risk factors.
   * It gathers regulatory feedback requesting a Risk Management Plan update.

2. **Information Processing (Metacognitive Architect)**
   * The Architect analyzes the additional data, identifying patients with pre-existing hepatic impairment as having significantly higher risk.
   * It processes the regulatory requirements for Risk Management Plan updates.

3. **Memory Formation (Metacognitive Architect)**
   * The world-model is updated with the identified risk factors and regulatory expectations.
   * Procedural memory is accessed to retrieve templates and workflows for Risk Management Plan updates.

4. **Planning and Decision-Making (Executive Planner)**
   * Using predictive processing, the Executive Planner models the impact of different risk minimization measures.
   * It develops a risk mitigation strategy recommending:
       1. contraindication in severe hepatic impairment,
       2. monitoring recommendations for moderate impairment,
       3. updated package insert warning.

5. **Action Implementation (Sensory Interface)**
   * The Sensory Interface prepares the Risk Management documentation updatr if the same in the ICSR report.
   * It submits the ICSR report to the respective regulatory authority to expedite the process of mitigating risks from the detected signal.
   * It implements changes to the centralised databases such as FDA's ARES database, and localised database such as company's drug safety and monitoring database to improve future detection of similar cases

6. **Outcome Assessment (Metacognitive Architect)**
   * The Architect evaluates whether the implemented measures meet the success criteria for risk mitigation.
   * It identifies opportunities to improve the signal detection process based on learnings from this case.
   * It updates the tool selection algorithm to prioritize hepatotoxicity assessment tools for this drug class in future evaluations.
