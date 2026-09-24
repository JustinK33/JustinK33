# Hi, I'm Justin

Computer Science & Data Science @ Rutgers University  <br>
Pragmatic Backend Engineer focused on Distributed Systems, APIs, and Data Pipelines<br>
Software Engineer Intern @ Arka

## About Me

Backend and Data Engineer with a strong foundation in building high-throughput data pipelines, distributed systems, and scalable backend infrastructure.

Proficient in Python and Go, using frameworks like FastAPI and Gin, with strong SQL experience across PostgreSQL, MySQL, and MongoDB, plus streaming and orchestration experience with Kafka, Redpanda, and Airflow. Comfortable working across AWS and GCP for deployment and infrastructure.

My work centers on pipeline performance optimization, event-driven architecture, and building systems that stay reliable under real load.

## 🛠️ Core Stack

**Languages:** Python, Golang, SQL, Java, TypeScript, JavaScript, Bash  
**Concepts**: Distributed Systems, Microservices, Event-Driven Architecture, Message Queues, ETL/ELT, Concurrency, System Design, RAG  
**Frameworks & Libraries:** FastAPI, Gin, LangChain, Airflow, Django, Node.js, Express, gRPC, Celery  
**Databases:** PostgreSQL, MySQL, pgvector, Redis, MongoDB  
**Cloud & Infra:** AWS, GCP, Docker, Kubernetes, Kafka, Nginx, GitHub Actions, Linux, Prometheus, Grafana  
**AI:** LLMs, Model Context Protocol (MCP), Agentic Workflows & Custom Skills, Context Management, Claude, Codex

## 💻 Selected Work

### ⚡ Belady
Go • gRPC • Python • LightGBM • Prometheus • Docker
A distributed cache that uses a machine learning model to decide what to evict, approximating the optimal algorithm instead of falling back on LRU.
The model runs inside the eviction path with a sub-microsecond budget, which forced me to use flattened tree layouts, sharded locking, and zero-allocation request handling.
→ [View Project](https://github.com/JustinK33/Belady)

### 📬 Conduit
Go • Gin • PostgreSQL • Kafka • Redis • Docker
A durable job queue that keeps running jobs through process crashes, broker restarts, and handler failures, with Postgres as the single source of truth.
Handles about 600 jobs/s end to end and 4,600+ requests/s at intake on a single laptop, using fencing tokens to limit duplicate execution.
→ [View Project](https://github.com/JustinK33/Conduit)

### 📊 RiskScore
Python • XGBoost • scikit-learn • FastAPI • pytest
A machine learning pipeline that predicts loan default risk on Lending Club data, built specifically to avoid the data leakage that makes most credit models look better than they are.
The scoring API responds in single-digit milliseconds with a calibrated probability, an approve or decline decision, and SHAP reason codes that explain the result.
→ [View Project](https://github.com/JustinK33/RiskScore)

## 📫 Connect

Email: `justinkong.dev@gmail.com`  
Portfolio: [justinkong.app](https://www.justinkong.app/)  
LinkedIn: [linkedin.com/in/justin-hkong](https://www.linkedin.com/in/justin-hkong/)  
