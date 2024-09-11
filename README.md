# Assessment

### **Assessment Task: Build an AWS API Gateway with Cognito Authentication**

#### **Objective:**

To assess the candidate's ability to design and implement an AWS API Gateway that uses Cognito for authentication and connects to two Lambda functions. Each Lambda function will call an external service of the candidate's choice. The candidate must use CloudFormation scripts to provision the necessary infrastructure and provide clear documentation.

---

### **Task Requirements:**

1. **API Gateway and Cognito Setup:**
   - Create an **API Gateway** with at least two endpoints.
   - Implement **Cognito** as the authentication mechanism for these endpoints. Use an Amazon Cognito User Pool and configure it for secure access to the API.

2. **Lambda Functions:**
   - Develop two AWS **Lambda functions**. Each function should:
     - Call an **external service** of your choice. The services can be any publicly accessible APIs (e.g., weather API, stock market API, etc.).
     - Process the response from the external service and return a meaningful output to the API Gateway.
   
3. **Infrastructure as Code:**
   - Use **AWS CloudFormation** to create all the necessary resources, including:
     - API Gateway
     - Cognito User Pool
     - Lambda Functions
     - Any other resources required (e.g., IAM roles, permissions, etc.).

4. **Documentation:**
   - Write a **README** in Markdown format that:
     - Describes the overall architecture.
     - Provides a step-by-step guide on how to deploy the solution.
     - Details the external services chosen for the Lambda functions.
     - Includes instructions for testing the API endpoints (e.g., sample requests and expected responses).
     - Documents any assumptions, limitations, or additional configurations needed.

---

### **Deliverables:**

1. **CloudFormation Scripts:** 
   - Include all CloudFormation scripts required to deploy the infrastructure.

2. **Source Code for Lambda Functions:**
   - Provide the source code for both Lambda functions, with clear documentation/comments within the code.

3. **README Documentation:**
   - A well-structured README file in Markdown format, following the documentation guidelines.

4. **Repository Structure:**
   - Organize the files in a Git repository with the following structure:
     ```
     /aws-api-gateway-assessment
     ├── README.md
     ├── cloudformation
     │   ├── main.yaml (or .json) - Main CloudFormation script
     ├── lambdas
     │   ├── lambda1
     │   │   └── index.js (or .py, .go, etc.) - First Lambda function
     │   ├── lambda2
     │   │   └── index.js (or .py, .go, etc.) - Second Lambda function
     └── assets (if any)
     ```

5. **Deployment Guide:**
   - A section in the README file that includes:
     - Instructions to deploy using the CloudFormation script.
     - Steps to create and configure the Cognito User Pool.
     - How to invoke the Lambda functions via the API Gateway.
     - Any necessary pre-requisites and dependencies.

---

### **Evaluation Criteria:**

1. **Correctness:**
   - Does the API Gateway properly implement Cognito authentication?
   - Do the Lambda functions successfully call the chosen external services and handle responses correctly?

2. **Completeness:**
   - Are all necessary resources created and configured using CloudFormation?
   - Is the README documentation comprehensive and easy to follow?

3. **Code Quality:**
   - Is the code for Lambda functions clean, well-structured, and documented?
   - Are best practices followed in CloudFormation scripting?

4. **Creativity and Problem Solving:**
   - Are the external services chosen for the Lambda functions meaningful and relevant?
   - How well does the candidate handle potential issues such as error handling, rate limiting, etc.?

5. **Documentation:**
   - Is the documentation clear, detailed, and does it adequately describe the solution and deployment steps?

---

### **Additional Notes:**

- The candidate is free to use any language supported by AWS Lambda (e.g., Node.js, Python, Go).
- Consider using AWS Free Tier eligible services to minimize any costs.
- The candidate should complete the assessment within [specify a reasonable time frame, e.g., 2-3 hours].

---

By structuring the assessment this way, you'll evaluate both the candidate's technical skills and their ability to document and explain their work effectively.