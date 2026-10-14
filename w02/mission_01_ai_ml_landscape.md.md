###### \# Mission 01: Build the AI and ML Landscape

###### 

#### \## 1. Concept Map: AI, ML, and Related Fields

###### 

###### ```mermaid

###### graph TD

###### &#x20;   AI\[Artificial Intelligence] --> Rule Based\[Rule-Based / Conventional Systems]

###### &#x20;   AI --> ML\[Machine Learning]

###### &#x20;   ML --> SL\[Supervised Learning]

###### &#x20;   ML --> UL\[Unsupervised Learning]

###### &#x20;   ML --> RL\[Reinforcement Learning]

###### &#x20;   ML --> DL\[Deep Learning]

###### &#x20;   DL --> Gen AI\[Generative AI]

###### &#x20;   Gen AI --> LLMs\[Large Language Models]





#### 2\. Five Key Distinctions



###### Artificial Intelligence vs. Machine Learning: 



Artificial Intelligence (AI) is the broad discipline of creating systems capable of human-like intelligence. Machine Learning (ML) is a specific subset of AI where systems learn patterns automatically from data rather than following explicitly coded instructions.



###### Conventional Automation vs. Machine Learning:



&#x20;Traditional programming relies on fixed, hand-written rules (Input + Rules = Output). Machine learning flips this paradigm by deriving the rules itself from training data (Input + Target Output = Learned Rules).



###### Deep Learning vs. Traditional Machine Learning: 



Deep Learning uses multi-layered artificial neural networks capable of learning complex representations directly from unstructured data, whereas traditional ML often depends on manually engineered features.



###### Generative AI vs. Traditional ML Models: 



Traditional ML typically focuses on classification, regression, or pattern detection. Generative AI focuses on producing new content—such as text, images, or code—based on learned underlying patterns.



###### LLMs vs. Generative AI:



&#x20;Generative AI includes all models that create content (images, audio, text). Large Language Models (LLMs) are a specific type of Generative AI based on transformer architectures trained primarily to process and generate human text.







#### 3\. Why Automation ≠ AI \& Why AI ≠ ML



###### Why automation is not necessarily AI: 



Standard automated systems (like a simple script or fixed microchip state machine) execute static rules. They cannot adapt or generalize to unseen scenarios beyond their coded conditions.



###### Why AI does not always mean ML:



&#x20;Early AI systems utilized rule-based expert systems, decision trees, and logic solvers. These are AI systems because they display intelligent decision-making, yet they do not learn from data.



#### 4\. Explicitly Programmed vs. Learned Capabilities :





|**Feature / Category**|**Explicitly Programmed Systems**|**Learned from Data (Machine Learning)**|
|-|-|-|
|core logic|Hardcoded if-else rules written by humans|Statistical weights and parameters derived from data|
|Handling Edge Cases|Must be anticipated and manually added to code|Generalizes to new variations if trained on representative data|
|maintenance|Requires manual rewriting of logic as conditions change|Requires model retraining with updated datasets|







#### 5\. Three Classified Real-World Examples :



##### Rule-Based DRC (Design Rule Checking) in VLSI



###### Classification: Conventional Automation / Rule-Based AI



Reason: DRC tools check layout features against fixed geometric rules (e.g., minimum trace width) explicitly defined by semiconductor foundries.



##### Automated Defect Classification in Wafer Inspection



###### Classification: Machine Learning / Deep Learning



Reason: The system learns to identify silicon wafer defects from image datasets rather than relying on hand-written visual features.



##### AI Coding Assistants for Verilog Synthesis



###### Classification: Generative AI / LLM



Reason: These tools generate new Hardware Description Language (HDL) code based on natural language inputs using underlying transformer models.

