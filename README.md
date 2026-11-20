## Hi, I'm Hardik

I'm an AI/ML engineer at Genpact. I build AI systems that know when to ask a person: LLM pipelines, RAG, evaluation and guardrails on AWS Bedrock, with a human in the loop wherever the model isn't sure.

### Featured project: [ComplaintOps](https://github.com/hardikbahri/complaintops)

Complaint triage trained on 335K public CFPB consumer complaints.

- A LoRA-tuned DistilBERT, served as int8 ONNX (91 ms on a plain CPU), answers 72.6% of complaints on its own at 93.9% accuracy.
- Everything below 0.8 confidence goes to a person. A LangGraph agent with MCP tools finds similar past complaints in pgvector and writes a note for the reviewer. The LLM never sets the label.
- An evaluation gate blocks weak models before they ship, drift monitoring flags when new complaints stop looking like the training data, and every change runs through CI.

[Live demo](https://huggingface.co/spaces/hb-007/complaintops) | [Code](https://github.com/hardikbahri/complaintops)

### Other projects

- [Event-driven flight alerts](https://github.com/hardikbahri/notifications_microservice): MongoDB change streams publish to Kafka, and a consumer emails every affected passenger.
- [Delivery route planner](https://github.com/hardikbahri/Delivery-optimization-simulator): Floyd-Warshall, K-means and a greedy TSP to plan routes for several drivers at once, in C++.
- [Blockchain messaging between vehicles](https://github.com/hardikbahri/Vanet): 11 cars and a roadside unit exchange messages through Ethereum smart contracts, with trust scores.

### What I work with

Python, PyTorch, Hugging Face, LangGraph, LangChain, AWS Bedrock, FastAPI, PostgreSQL and pgvector, MLflow, ONNX, Docker

### Get in touch

[Portfolio](https://hardikbahri.github.io) | [LinkedIn](https://www.linkedin.com/in/hardik-bahri/) | hardik.bahri@gmail.com
