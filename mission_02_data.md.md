### \# Mission 02: Understand Data: What does an ML system learn from?



#### 1\. Research Questions \& Core Explanations:



###### What does it mean to learn a pattern from data?



Learning a pattern from data means using mathematical and statistical algorithms to discover hidden relationships, trends, and correlations across input features without a human explicitly coding those rules. Rather than memorizing individual examples, an ML system generalizes these underlying statistical relationships so it can make accurate predictions or decisions when presented with brand new, unseen data.



#### 2\. Core Terminology Dataset: 



A complete collection of data records or instances used for analysis, training, and testing.   Sample / Observation: A single row or individual instance representing one data point (e.g., a manufactured microchip die).   Feature: An individual measurable property, attribute, or independent variable used as input for a model.   Label / Target: The dependent variable, ground-truth answer, or correct outcome the model is trying to predict in supervised learning







#### 3\. Key Data Distinctions



1\. Structured vs. Unstructured Data





|FEATURE|STRUCTURED DATA|UNSTRUCTURED DATA|
|-|-|-|
|FORMAT|Highly organized, usually in rows and columns (tables).|No predefined format or specific organizational structure.|
|STORAGE|Relational databases (SQL), spreadsheets (Excel, CSV).|NoSQL databases, data lakes, audio/video/text files.|
|SEARCHABILITY|Easy to search using queries (like SQL).|Difficult to search without preprocessing or specialized tools.|
|EXAPMLES|Dates, phone numbers, credit card numbers, transaction history.|Text files, emails, images, videos, audio recordings, PDFs.|





2\. Numerical vs. Categorical Features



Data features (columns/variables) are generally split into two main types based on what they represent:

• Numerical Features: Represent measurable quantities or counts. You can perform mathematical operations (like adding or averaging) on them.

&#x09;• Continuous: Can take any value within a range (e.g., height, salary, temperature).

&#x09;• Discrete: Can only take distinct, countable values (e.g., number of rooms in a house, number of children).

• Categorical Features: Represent qualitative traits or characteristics. They group data into distinct categories or labels.

&#x09;• Nominal: Categories with no inherent ordering or ranking (e.g., eye color, country of birth, gender).

&#x09;• Ordinal: Categories that have a meaningful, logical order or rank (e.g., education level (High School, Bachelor's, PhD), customer satisfaction ratings (Poor, Good, Excellent)).





3\. Labelled vs. Unlabelled Examples



This distinction determines whether the data is ready for supervised learning (prediction) or unsupervised learning (pattern finding):

• Labelled Examples: Data points that contain both the input features (the characteristics) and the target output (the answer or label).

&#x09;• Example: A dataset of house features (square footage, bedrooms) that includes the actual sale price.

&#x09;• Use case: Used to train Supervised Learning models to predict future outcomes.

• Unlabelled Examples: Data points that contain only the input features but do not have the target output or answer key.

&#x09;• Example: A collection of customer purchase histories without any classification of whether they are "high-value" or "low-value" customers.

&#x09;• Use case: Used in Unsupervised Learning to find hidden patterns, groupings (clustering), or structures in the data.



#### 4\. Data Collection, Cleaning, and Common Issues



Data Preparation Pipeline: Real-world engineering data is rarely pristine. Machine learning workflows require collecting raw logs, filtering out noise, handling missing values, standardizing formats, and correcting inconsistent labels.



Missing Values: Instances where specific sensor measurements failed or were not recorded. These must be statistically imputed or dropped.



Noisy Data: Random sensor errors, calibration drifts, or extreme outliers that obscure the true underlying relationship.



Inconsistent Labels: Logging errors where identical chip performance profiles are tagged with conflicting target outcomes (e.g., a passing chip incorrectly labeled as a fail).



Why Data Quantity ≠ Quality: Having massive volumes of data ("big data") is useless if the dataset contains bias, systematic noise, data leakage, or incorrect labels ("garbage in, garbage out"). High data quality, balanced feature distribution, and accurate labeling matter far more than sheer scale.



#### How Data Quality Affects a Model (Two Key Ways)



Impact of Sensor Noise on Generalization: If temperature sensors during data collection had calibration errors and consistently reported temperatures 

10 

∘

&#x20;C too high, the model learns false mathematical boundaries. When deployed in production with accurate sensors, it will misclassify timing performance and yield incorrect Pass/Fail predictions.



Impact of Class Imbalance and Incorrect Labelling: If a dataset meant to predict chip failures contains inconsistent labels (e.g., failing dies incorrectly tagged as "Pass" due to testbench glitches), the model receives contradictory training signals. It will fail to separate safe operational margins from failure zones, resulting in high error rates during post-silicon validation.

