<img width="2633" height="876" alt="image" src="https://github.com/user-attachments/assets/f11d3b40-8fef-4a9d-b3c7-613e55c58079" />

# Microsoft AI-300 Study Hub
### Operationalizing Machine Learning and Generative AI Solutions

This repository is dedicated to study materials, hands-on labs, and practice questions for the **Microsoft AI-300** certification.

## Official Resources
* [Official Study Guide](https://learn.microsoft.com/en-us/credentials/certifications/resources/study-guides/ai-300)
* [Exam Landing Page & Skills Measured](https://learn.microsoft.com/en-us/credentials/certifications/operationalizing-machine-learning-and-generative-ai-solutions/)

## Exam Topics
1. Design a machine learning solution.
2. Build and train models.
3. Deploy and operationalize solutions.
4. Manage and monitor solutions.

## Overview
**Exam AI-300** is the successor to DP-100, shifting the focus from data science experimentation to **Production-Grade Engineering**. It targets the **AI/MLOps Engineer** role, emphasizing automation, infrastructure, and the scaling of Generative AI systems.

---

## Complex Core Domains

### 1. Advanced MLOps Infrastructure
Moving beyond the GUI, AI-300 requires proficiency in **Infrastructure as Code (IaC)**.
* **Provisioning:** Using **Bicep** and **Azure CLI** to deploy secure ML Workspaces.
* **Networking:** Implementing **Private Endpoints** and Virtual Networks (VNETs) to secure model traffic.
* **Orchestration:** Setting up **GitHub Actions** for automated CI/CD triggers (e.g., triggering a build when a `model.json` version changes).

### 2. GenAIOps & Microsoft Foundry
This is the most modern part of the exam, focusing on the lifecycle of Large Language Models (LLMs).
* **Foundry Environments:** Managing managed identities and RBAC for AI Projects.
* **Prompt Flow:** Designing DAGs (Directed Acyclic Graphs) for LLM workflows, including versioning and deployment.
* **Agentic Frameworks:** Orchestrating multi-agent systems and managing their state and memory.

### 3. QA, Observability & AI Safety
In GenAI, traditional metrics (Accuracy/F1) aren't enough. AI-300 covers:
* **AI-Assisted Metrics:** Measuring **Groundedness**, **Relevance**, and **Coherence**.
* **Drift & Safety:** Setting up **Content Safety** filters and monitoring for "model drift" in production.
* **Cost Management:** Tracking token usage and latency to optimize ROI.

### 4. RAG & Performance Optimization
* **Retrieval-Augmented Generation (RAG):** Optimizing vector database indexing and embedding model selection.
* **Fine-Tuning:** Implementing advanced fine-tuning techniques using synthetic datasets.
* **Synthetic Data:** Using LLMs to generate high-quality training data for smaller, specialized models.

---

## Knowledge Map (Technical Weighting)

| Domain | Weight | Key Technical Focus |
| :--- | :--- | :--- |
| **Infrastructure** | 20% | Bicep, Azure CLI, Networking, IAM |
| **ML Lifecycle** | 30% | MLflow, Pipelines, Managed Endpoints |
| **GenAIOps** | 25% | Microsoft Foundry, Prompt Flow, Agents |
| **QA & Safety** | 15% | Groundedness, Toxicity, Token Monitoring |
| **Optimization** | 10% | RAG Tuning, Advanced Fine-tuning |

---

## Key Tools to Master
* **SDKs:** Azure Machine Learning SDK v2 (Python).
* **Frameworks:** MLflow, LangChain (basics), and Prompt Flow.
* **CLI:** Azure CLI (`az ml` extension).
* **DevOps:** GitHub Actions & YAML-based pipeline definitions.

---
## Key skills validated by this Certification

| Skill area | Exam AI-300 (new) | Exam DP-100 (old) |
| :--- | :--- | :--- |
| **MLOps infrastructure** | Full CI/CD, IaC (Bicep, Azure CLI), GitHub Actions | Basic workspace and compute setup |
| **Model lifecycle management** | Core focus, including registration, versioning, rollout/rollback, monitoring | Full lifecycle from training to deployment |
| **GenAIOps infrastructure** | End-to-end lifecycle, including security, automation, and model management with Foundry | Basic generative AI setup and experimentation |
| **QA and observability** | Generative AI evaluation, tracing, safety metrics, drift detection, cost monitoring | Model evaluation and responsible AI principles |
| **Generative AI performance optimization** | RAG optimization, embedding model selection and tuning, advanced fine-tuning, synthetic data management | Basic prompt engineering and fine-tuning |


# 📝 Interactive AI-300 Practice Test
*Click on "View Answer & Explanation" after deciding on your choice.*

---

### Question 1
**Which Azure service is primarily used to manage the machine learning lifecycle in production?**
* A. Azure Machine Learning
* B. Azure Functions
* C. Azure DevOps
* D. Azure Monitor

<details>
<summary>✅ <b>View Answer & Explanation</b></summary>
<br>
<b>Correct Answer: A</b>
<p><b>Explanation:</b> Azure Machine Learning provides a complete platform for managing the full lifecycle of machine learning models including training, deployment, monitoring, and governance.</p>
</details>

---

### Question 2
**Which deployment type is best suited for real-time inference in Azure ML?**
* A. Batch endpoint
* B. Real-time endpoint
* C. Scheduled pipeline
* D. Data store

<details>
<summary>✅ <b>View Answer & Explanation</b></summary>
<br>
<b>Correct Answer: B</b>
<p><b>Explanation:</b> Real-time endpoints are designed for low-latency predictions where immediate responses are required.</p>
</details>

---

### Question 3
**Which feature allows tracking of experiments and metrics in Azure ML?**
* A. Pipelines
* B. MLflow
* C. Compute instances
* D. Data labeling

<details>
<summary>✅ <b>View Answer & Explanation</b></summary>
<br>
<b>Correct Answer: B</b>
<p><b>Explanation:</b> MLflow integration in Azure Machine Learning enables logging of metrics, parameters, and artifacts during experiments.</p>
</details>

---

### Question 4
**Which deployment strategy minimizes downtime during model updates?**
* A. Rolling deployment
* B. Canary deployment
* C. Blue/green deployment
* D. Shadow deployment

<details>
<summary>✅ <b>View Answer & Explanation</b></summary>
<br>
<b>Correct Answer: C</b>
<p><b>Explanation:</b> Blue/green deployment maintains two identical environments, allowing traffic to switch instantly from the old version to the new one.</p>
</details>

---

### Question 6 (Advanced)
**Which tool in Azure Machine Learning is specifically used to orchestrate complex LLM workflows, including branching and evaluation?**
* A. Azure Logic Apps
* B. Prompt Flow
* C. MLflow
* D. Azure Data Factory

<details>
<summary>✅ <b>View Answer & Explanation</b></summary>
<br>
<b>Correct Answer: B</b>
<p><b>Explanation:</b> Prompt Flow is the primary tool for designing, evaluating, and deploying LLM-based applications.</p>
</details>

---

### Question 7 (Advanced)
**To reduce hallucinations in a Generative AI application using enterprise data, which architecture should be implemented?**
* A. Fine-tuning with a JSONL dataset
* B. Increasing the model's Temperature setting
* C. Retrieval-Augmented Generation (RAG)
* D. Blue/Green deployment

<details>
<summary>✅ <b>View Answer & Explanation</b></summary>
<br>
<b>Correct Answer: C</b>
<p><b>Explanation:</b> RAG (Retrieval-Augmented Generation) "grounds" the model by providing it with external, trusted data before it generates a response.</p>
</details>

---

### Question 8
**Which metric specifically measures how well a model's response is supported by the provided source context?**
* A. Fluency
* B. Groundedness
* C. Coherence
* D. Latency

<details>
<summary>✅ <b>View Answer & Explanation</b></summary>
<br>
<b>Correct Answer: B</b>
<p><b>Explanation:</b> Groundedness checks for factual consistency between the retrieved documents and the LLM's final response.</p>
</details>

---

### Study Resource
For a full database of these types of questions and detailed study material, check out:
👉 **[itexamscerts.com](https://www.itexamscerts.com)**
