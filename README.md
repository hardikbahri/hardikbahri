## Hi, I'm Hardik

I'm an AI/ML engineer at Genpact in Bengaluru with 2+ years of experience. I build AI systems that know when to ask a person: LLM pipelines, multi-agent workflows, RAG, evaluation and guardrails on AWS Bedrock, with a human in the loop wherever the model isn't sure.

### What I build at Genpact

- **Multi-agent email triage for a bank:** LangGraph + FastAPI on AWS Bedrock. It sorts emails into 45 intents, extracts a 250-field schema and sends low-confidence cases to human review. +65% throughput, −70% QC cost.
- **RAG from reviewer corrections:** dynamic few-shot retrieval with Titan embeddings and pgvector. My evaluation suite found a threshold blocking 85% of retrievals; fixing it took intent accuracy from 69% to 86%. An HNSW index cut p50 retrieval from 279 ms to 2 ms.
- **LLMOps and model selection:** benchmarked TF-IDF + logistic regression against the LLM pipeline on 490 real emails, then cut cost 2.7× per email with batching and token tracking. Claude Haiku + RAG matched Sonnet at 1/14 the cost.
- **AI Trust Gateway:** reversible PII redaction and guardrails in front of LLM calls, adopted across Genpact's Agentic AI practice. Fine-tuned GLiNER for NER at ~0.90 F1 on adversarial tests.
- **Synthetic finance data:** a ~10K-line generator of labelled Record-to-Report data used to benchmark reconciliation agents, with KPIs reported in Power BI.

### Featured project: [ComplaintOps](https://github.com/hardikbahri/complaintops)

Complaint triage trained on 335K public CFPB consumer complaints.

- A LoRA-tuned DistilBERT, served as int8 ONNX (91 ms on a plain CPU), answers 72.6% of complaints on its own at 93.9% accuracy.
- Everything below 0.8 confidence goes to a person. A LangGraph agent with MCP tools finds similar past complaints in pgvector and writes a note for the reviewer. The LLM never sets the label.
- An evaluation gate blocks weak models before they ship, drift monitoring flags when new complaints stop looking like the training data, and every change runs through CI.

[Live demo](https://huggingface.co/spaces/hb-007/complaintops) | [Code](https://github.com/hardikbahri/complaintops) | [Model](https://huggingface.co/hb-007/complaintops-distilbert-lora-onnx)

I wrote up why the LLM doesn't make the calls: [My LLM was confident 99% of the time. It was right 39% of the time.](https://medium.com/@hardik.bahri/my-llm-was-confident-99-of-the-time-it-was-right-39-of-the-time-84c6fc2e34f3)

### Skills

**Generative AI and agents:** LLMs, RAG, LangGraph, LangChain, multi-agent systems, MCP, tool calling, human-in-the-loop, prompt engineering, LLM evaluation (LLM-as-a-judge, golden sets), Langfuse, guardrails, PII redaction, AWS Bedrock (Claude, Titan embeddings)

**Machine learning and NLP:** PyTorch, Hugging Face Transformers, LoRA/PEFT fine-tuning, scikit-learn, XGBoost, Optuna, text classification, NER (GLiNER), embeddings and semantic search, ONNX quantization

**MLOps:** MLflow, evaluation gates, drift monitoring (Evidently, PSI), Docker, Kubernetes, GitHub Actions CI/CD, model deployment and monitoring

**Data and cloud:** AWS (Bedrock, S3, Lambda), PostgreSQL, pgvector, SQL, pandas, NumPy, Databricks, Power BI

**Backend:** Python, FastAPI, Django, Flask, REST APIs, pytest, Streamlit

### Other projects

- [Event-driven flight alerts](https://github.com/hardikbahri/notifications_microservice): MongoDB change streams publish to Kafka, and a consumer emails every affected passenger.
- [Delivery route planner](https://github.com/hardikbahri/Delivery-optimization-simulator): Floyd-Warshall, K-means and a greedy TSP to plan routes for several drivers at once, in C++.
- [Blockchain messaging between vehicles](https://github.com/hardikbahri/Vanet): 11 cars and a roadside unit exchange messages through Ethereum smart contracts, with trust scores.

### Get in touch

[Portfolio](https://hardikbahri.github.io) | [LinkedIn](https://www.linkedin.com/in/hardik-bahri/) | hardik.bahri@gmail.com
