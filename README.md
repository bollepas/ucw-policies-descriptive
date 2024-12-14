# ucw-policies-descriptive
# README: Analysis of UCW Substance Use Policy Implementation

## Descriptive Analysis

### Project Description
Descriptive Analysis of the University Canada West's Substance Use Policy Implementation

### Project Title
Substance Use Policy Analysis at UCW

### Objective
To perform a descriptive analysis of UCW’s Substance Use Policy (Policy Number: 8006), focusing on its scope, compliance measures, and the roles and responsibilities outlined within the policy.

### Dataset
The dataset includes:
- Policy details (e.g., definitions, responsibilities, and scope)
- Associated legislation (e.g., Workers Compensation Act, Occupational Health and Safety Regulation)
- Related policies and procedures referenced within the Substance Use Policy

### Methodology
#### 1. Data Ingestion
- Policy document was ingested into Amazon S3 buckets (`policy-raw-ucw`) for centralized storage and version control.
- File security was ensured using AWS Key Management Service (KMS) encryption for sensitive organizational information.

#### 2. Data Profiling and Cleaning
- AWS Glue DataBrew was utilized to profile the policy document, identifying sections for analysis such as scope, definitions, and responsibilities.
- Cleaning steps included:
  - Standardizing headers and sub-headers for uniform structure.
  - Removing redundant sections for focused analysis.

#### 3. Data Transformation
- AWS Glue ETL jobs automated the segmentation of the document:
  - Extracted sections for responsibilities, safety-sensitive operations, and applicable legislation.
  - Structured definitions and scope into a tabular format for analysis.
  - Ensured schema consistency for downstream querying.

#### 4. Data Consolidation
- Cleaned and transformed data was stored in an AWS S3 bucket (`policy-trf-ucw`), organized for user access and internal reference.

### Tools and Technologies
- **AWS Services:** S3, Glue DataBrew, and Glue ETL for storage, profiling, and transformation.
- **Data Querying:** Amazon Athena for structured querying of policy content.
- **Encryption:** AWS KMS for secure storage and access.

### Deliverables
- A cleaned and segmented policy document stored in AWS S3.
- Key insights into roles and compliance requirements extracted from the policy.
- Summary reports for stakeholders with actionable recommendations.

### Conclusion
The descriptive analysis structured and streamlined the UCW Substance Use Policy into actionable insights. By leveraging AWS services, the analysis ensured secure, scalable, and efficient handling of the policy document while providing clarity on compliance and implementation measures.
