## Task

Using the provided SQL table schemas (`Claim`, `ClaimDetail`, and `ReinsContract`), write a single SQL query to identify subscribers who have exceeded their specific reinsurance deductible and are eligible for reimbursement.

### **Health Insurance Terminology**

- **Subscriber**: The primary person covered under a health insurance plan. Dependents may also be covered, but the subscriber is typically the policyholder.
- **Claim**: A request for payment submitted by a healthcare provider or insured individual to the insurer, seeking reimbursement for services rendered.
- **Claim Detail**: Breakdown of individual services, procedures, or items billed within a claim.
- **Reinsurance Deductible**: A financial threshold in a reinsurance agreement. If a subscriber's total claim amount exceeds this threshold, the insurer can seek reimbursement from the reinsurer.
- **Specific Deductible**: A type of deductible tied to individual subscribers. Once a subscriber’s claims exceed this specific deductible, further claims may be reimbursed by the reinsurer.

## Submission Guidelines

- **Format**: Submit your solution as a private GitHub Gist or a private repository.
- **Files Required**:
  - `.sql` file containing the SQL query.
  - `.md` file explaining your approach, including details about integration with Metabase and relevant visualizations.
- **Deadline**: Clearly indicate the submission deadline.
- **Evaluation**: Submissions will be assessed based on the rubric below.

## Requirements

1. **Research and Analysis**: Understand the provided table schemas and the relationships between them. You might have to research health insurance terminology to grasp the context.
1. **Join the Tables**: Use appropriate SQL joins to combine data from `Claim`, `ClaimDetail`, and `ReinsContract` tables.
1. **Calculate Breach**: Identify if a subscriber's total claim amount exceeds the `Specific_Deductible` in the `ReinsContract` table.
1. **Output**:
   - `Subscriber_ID`
   - `Group_ID`
   - Total claim amount exceeding the specific deductible.
   - Percentage Exceeding
1. **Additional Considerations**:
   - Provide a clear explanation of the health insurance terminology relevant to the query.
   - Describe how this query can be integrated into Metabase and suggest suitable visualizations (e.g tables to list detailed claims).

## Rubric

1. **Query Performance (25%)**
   - Efficient joins and appropriate use of indexes.
   - Optimization techniques to handle large datasets.
2. **Comments and Documentation (15%)**
   - Clear, concise comments explaining the purpose of each query component.
   - Use of meaningful aliases and variable names.
3. **Structure and Clarity (20%)**
   - Logical flow and well-organized query structure.
   - Effective use of subqueries or Common Table Expressions (CTEs) to enhance readability.
   - Consistent formatting and indentation.
   - Submission of a separate `.md` file with detailed explanations.
4. **Integration with Metabase (20%)**
   - Explanation of query integration with Metabase (e.g., setting up the SQL query in a saved question).
   - Suggestions for visualizations to present breached deductibles (e.g., aggregate totals per subscriber in bar charts or detailed tables).
5. **Industry Terminology Explanation (20%)**
   - Accurate and concise explanation of terms like "reinsurance deductible," "specific deductible," "claim," and "subscriber."
   - Clear connection of terminology to the task requirements.
