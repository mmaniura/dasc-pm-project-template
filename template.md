This extended template covers the key areas according to DASC-PM. Each work step is explained, contains guiding questions, and shows iteration possibilities and SCRUM tips.
[[_TOC_]]

# 1.  Domain & Project Initiation
This phase establishes the project's foundation by defining the problem, identifying stakeholders, and understanding domain-specific constraints. Clear objectives and success criteria are set to guide the project, ensuring feasibility and alignment with business or scientific needs.
    
## Work steps and explanations

### Define project idea and objectives
Describe the concrete problem as well as the benefits and expected added value.
Guiding questions:
What is the core problem? Why is it relevant? What is to be achieved?

### Identify stakeholders
Identify all affected groups and key people.
Guiding questions:
Who is directly/indirectly involved or affected? Who makes decisions? Who are potential opponents?

### Analyze domain specifics
Document special features of the subject domain and their influence on the data project.
Guiding questions:
Are there technical terms, standards, or legal requirements (e.g., GDPR)?

### Set success criteria
Record concrete criteria/metrics for evaluating project success.
Guiding questions:
When is the project considered successful? Which KPIs/metrics are accepted?
        
### Ensure feasibility
Check whether implementation is possible with available resources and technology.
Guiding questions:
Are necessary data, know-how, IT, and time available? Are there critical dependencies/risks?
        
## Iteration possibilities
After insights from the data or analysis phase, returning is possible, e.g., to adjust the goal definition.
    
## SCRUM recommendations
- Plan user stories for goal clarification and stakeholder interviews separately (e.g. "Identify and include stakeholders").
- Clearly separable acceptance criteria (e.g., "Project goals agreed with management and released").
    
# 2.  Data
This area focuses on identifying, accessing, and understanding the data sources relevant to the project. It ensures that data availability, quality, legality, and access rights are properly assessed to provide a solid basis for further analysis
    
## Work steps and explanations

### Identify data sources:
Record all available (internal/external) sources including their owners.
Guiding questions:
Where is relevant data located (databases, files, third-party systems)? How current and accessible are they?
        
### Clarify data access (legal, technical)
Deal with permissions, interfaces, security and data governance.
Guiding questions:
Who is allowed to access which data? Have agreements on data protection and security been made?
        
### Acquire and inspect data
Request test datasets or real-world examples and do a first suitability check.
Guiding questions:
Are the data complete/well documented? What formats and structures are available?

### Document data volumes/formats
Document size, structure and peculiarities in writing.
Guiding questions:
How large are the data volumes? Are there different formats (e.g., CSV, JSON, images, time series)?
        
## Iteration possibilities
If quality problems or new data requirements are detected, feed back to data identification/procurement.
    
## SCRUM recommendations
Stories per data source as well as separate stories for access, data protection approvals, quality checks.
    
# 3. Data Preparation & Exploratory Analysis
Here, raw data is cleaned, transformed, and explored to uncover patterns and characteristics. This step lays the groundwork for modeling by constructing meaningful features and assessing data quality and limitations.

## Work steps and explanations

### Preprocessing
Cleansing, integration, transformation: Clean data (duplicates, errors, missing values), standardize structures.
Guiding questions:
What typical problems exist (outliers, null values)? Must values be aggregated or normalized?

### Feature engineering/construction:
Derive/create new, task-relevant features.
Guiding questions:
What additions or combinations of existing data could improve the model?

### Exploratory visualization & statistics
Use visualization, statistics and correlations to recognize structures and patterns.
Guiding questions:
What relationships, trends, clusters or outliers are visible? What is the distribution of the target variable?
        
### Document data quality
Document results and remaining uncertainties in writing.
Guiding questions:
Where do uncertainties/risks persist? What limitations does the data still have?
        
## Iteration possibilities
- If problems with features or data quality occur, return to data inspection or feature engineering.
    
## SCRUM recommendations
- Stories for each task: cleansing, feature engineering, visualization.
- Separate documentation story for "finalizing the data base", documenting all quality aspects.
    
# 4.  Analytical Methods/Modeling
This key area involves selecting and applying appropriate analytical or machine learning methods to extract insights or build predictive models. It emphasizes iterative development, evaluation, and validation to ensure robust and useful results.

## Work steps and explanations

### Specify requirements for analytical procedures
Define goal (e.g., classification, regression, clustering) and constraints.
Guiding questions:
What should the model achieve? Are there requirements for speed, interpretability, or accuracy?
        
### Select appropriate algorithms/methods
Select algorithms suitable for the goal and data.
Guiding questions:
Which methods are suitable? Are there proven baselines or new variants?
        
### Specify tools and libraries
Decide on technologies, frameworks, and libraries.
Guiding questions:
Which tools are allowed? Which interfaces are important for integration?

### Perform analysis/modeling
Implement, train models and document them in a reproducible way.
Guiding questions:
How is the model quality evaluated? Are all hyperparameters and methods documented?
        
### Evaluate and validate modeling results:
Reconcile objective and subjective results with stakeholders.
Guiding questions: Are results stable, understandable, and do they meet the goals? What can be improved?
        
## Iteration possibilities
*   Typical interplay between feature engineering, model training, and validation ("fail fast" principle).
    
## SCRUM recommendations
*   Stories by method/model and for every major result evaluation.
    
# 5.  Utilization (Deployment & Operationalization)
The focus is on translating analytical outputs into actionable solutions that stakeholders can use. It covers result presentation, system integration, and documentation to enable practical deployment and sustainable use.
    
## Work steps and explanations

### Preparing results for stakeholders (reporting, presentation, dashboard): Comprehensible and addressee-appropriate presentation.
Guiding questions:
What formats are ideal for user groups (graphics, text, interactive dashboards)?
        
### Integration into target system (production, API, dashboard, etc.)
Implement stepwise technical integration.
Guiding questions:
Which interfaces need to be served? What is the API/dashboard specification?
        
### Documentation & traceability
Document central decisions and result validations.
Guiding questions:
Are all steps, assumptions and decisions documented? Is it traceable how the result was created?
        
## Iteration possibilities
- If there is feedback regarding comprehensibility, data integration, or result utilization: adjustments and new loops.
    
## SCRUM recommendations
- Stories per result format (e.g. "Provide dashboard v1"), API integration.
- Separate story for traceability and documentation.
    
# 6.  Usage (operation, monitoring, maintenance)
This ongoing phase monitors model performance and system health, collects user feedback, and manages model updates or retraining. It ensures that the deployed solutions remain effective and relevant in changing conditions.
    
## Work steps and explanations

### Monitoring & performance control:
Monitor model results and system performance in ongoing operation.
Guiding questions:
Which indicators are tracked during operation? How and when does monitoring trigger?
        
### Collect and evaluate user feedback
Actively collect feedback for continuous improvement.
Guiding questions: How do end users perceive the system or insights? Are there misunderstandings or bottlenecks?
        
### Model adjustments and retraining
Retrain or adjust models as needed or in case of performance decline.
Guiding questions:
When is a model update needed? How does the update process work? Are automatic processes in place?
        
## Iteration possibilities
- Continuous improvement (CIP): feedback and monitoring lead to new data or model iteration.
    
## SCRUM recommendations
- Stories for monitoring enhancements, feedback analyses, and model retrainings planned separately.
    
# 7.  IT infrastructure (cross-sectional)
Supporting all project phases, this area addresses the technical environment, including computational resources, storage, security, and automation. It ensures that infrastructure meets performance and compliance requirements for development and production.

## Work steps and explanations

### Needs analysis for resources (compute, storage, security, etc.)
Technical requirements for runtime environments and security.
Guiding questions:
What hardware/cloud services are needed? Are there security and compliance requirements?
        
### Provide and configure infrastructure:
Set up all systems for development, test, and production.
Guiding questions:
How is deployment done (containers, VMs)? Who operates and maintains the infrastructure?
        
### Implement interfaces (such as data lake, ML pipelines)
Technical integration with other systems.
Guiding questions:
Where do interfaces need to be created? Are there standard formats or special requirements?
        
### Automation (CI/CD, monitoring, logging, etc.)
Build/improve automatic deployment and operations processes.
Guiding questions:
How can builds, tests, and deployments be automated? Are logs and monitoring integrated?
        
## Iteration possibilities
- Insights from the business units or scaling needs lead to expansion or adjustment of the infrastructure.
    
## SCRUM recommendations
- Write stories per layer (storage, compute, deployment, security, etc.). Treat automation issues as separate stories.
    
# 8.  Scientific approach & meta aspects (cross-sectional)
This overarching area guarantees methodological rigor through hypothesis management, transparent documentation, reviews, and lessons learned. It fosters continuous improvement and replicability throughout the data science project lifecycle.
    
## Work steps and explanations
### Hypothesis management/hypothesis testing
Traceable, documented assumptions and findings.
Guiding questions: What hypotheses exist? How are they tested?
        
## Documentation, review & lessons learned:
Systematic documentation of results, reviews, retrospectives, key learnings.
Guiding questions:
Is the entire process documented transparently? What best practices and sources of error have been discovered?
        
## Iteration possibilities
- After every milestone/retro, adjust approach or documentation quality as needed.
    
## SCRUM recommendations
- Plan reviews, retrospectives, and lessons learned workshops as their own stories/tasks.
