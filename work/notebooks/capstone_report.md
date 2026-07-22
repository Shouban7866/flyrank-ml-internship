Capstone Report — Content Action Recommendation System
Abstract
This project explores how machine learning can support content review decisions by identifying improvement opportunities from observed data signals.

The workflow covers problem framing, data analysis, baseline comparison, model development, validation, and generating ranked recommendations.

The output is designed as decision-support for human reviewers rather than an automated decision system.

1. Research Question
Question
How can machine learning signals help prioritize content improvement actions?

Decision Supported
This work supports teams in deciding:

Which items should be reviewed first
Which areas need improvement
Which content shows positive performance signals
2. Data
Dataset
A public anonymized dataset was used for analysis.

Data Included
Numerical features
Performance-related signals
Historical observations
Data Excluded
Private information
Client-identifying details
Sensitive records
Only public-safe data was used.

3. Methodology
The workflow included:

Data understanding and quality checks
Feature analysis
Baseline creation
Machine learning model training
Validation and comparison
Recommendation generation
Assumptions
Historical patterns provide useful signals.
Data quality impacts model reliability.
Validation
The model was evaluated using a fixed train/test split.

Leakage checks were performed to ensure target information was not used incorrectly.

4. Results
The developed model was compared against a baseline approach using the same validation split.

Evaluation focused on measured performance differences between baseline and ML model.

Results should be interpreted as observed performance on the selected dataset.

5. Limitations
This project cannot claim:

Perfect future predictions
Causal impact of recommendations
Replacement of human decision-making
The recommendations are directional and require human review.

6. Ranked Recommendations
The system generates an action priority list:

Rank	Recommendation	Reason
1	Improve low performing areas	Low observed performance
2	Review outdated information	Possible stale signals
3	Promote strong performing areas	Positive signals observed
4	Monitor declining trends	Performance change detected
7. Responsible ML
The project follows responsible ML practices:

Results are reported as observed and measured.
Recommendations are decision-support only.
Human review is required before action.
No private client information is included.
8. Artifacts
Generated artifacts:

Model evaluation results
Recommendation tables
Supporting analysis outputs
These artifacts support reproducibility and reporting.

Acknowledgments & Data Credit
This project was completed as part of the FlyRank ML Internship.

Data and project structure were provided through the FlyRank internship program.

https://flyrank.ai
