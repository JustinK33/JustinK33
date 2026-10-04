# Hi, I'm Justin

Computer Science & Data Science @ Rutgers University <br>
Pragmatic Backend Engineer focused on Distributed Systems, APIs, and Data Pipelines

## 👋 About Me

Backend and Data Engineer with a strong foundation in building high-throughput data pipelines, distributed systems, and scalable backend infrastructure.

Proficient in Python and Go, using frameworks like FastAPI and Gin, with strong SQL experience across PostgreSQL, MySQL, and MongoDB, plus streaming and orchestration experience with Kafka, Redpanda, and Airflow. Comfortable working across AWS and GCP for deployment and infrastructure.

My work centers on pipeline performance optimization, event-driven architecture, and building systems that stay reliable under real load.

## 🛠️ Core Stack

**Languages**

Python Go SQL Java TypeScript JavaScript Bash

**Frameworks & Libraries**

FastAPI Gin LangChain Airflow Django Node.js Express gRPC Celery

**Databases**

PostgreSQL MySQL pgvector Redis MongoDB

**Cloud & Infra**

AWS GCP Docker Kubernetes Kafka Nginx GitHub Actions Linux Prometheus Grafana

## 💻 Selected Work

### 📬 Conduit

`Go` • `Gin` • `PostgreSQL` • `Kafka` • `Redis` • `Docker`

A durable job queue built around one rule: Postgres is the only place a job's fate is written. A job is safe the moment its insert commits, so a crashed worker, a restarted broker, or a dropped wake-up costs latency but never work. Workers claim jobs with `FOR UPDATE SKIP LOCKED`, and Kafka and Redis are optional fast paths layered on top of the database.

Exactly-once delivery is not achievable when a worker can die between doing the work and recording it, so Conduit is explicitly at-least-once and uses fencing tokens to shrink the window where a duplicate can run. Benchmarked at about 600 jobs/s end to end (worst p95 1.27 s) and 4,600+ requests/s at intake on a single laptop, with the full methodology and hardware caveats published in the repo.

→ [View Project](https://github.com/JustinK33/Conduit)

### ⚡ Belady

`Go` • `gRPC` • `Python` • `LightGBM` • `Prometheus` • `Docker`

A distributed cache that uses a machine learning model to decide what to evict, approximating the optimal algorithm instead of falling back on LRU. The model runs inside the eviction path with a sub-microsecond budget, which forced me to use flattened tree layouts, sharded locking, and zero-allocation request handling.

→ [View Project](https://github.com/JustinK33/Belady)

### 📊 Pulsegrid

`Python` • `Redpanda` • `Airflow` • `PostgreSQL` • `Pydantic` • `Docker Compose`

An e-commerce event pipeline where a producer publishes clickstream events to Redpanda, a consumer validates each message and batch-loads it into Postgres, and Airflow runs the whole thing as a DAG that ends in funnel and item-popularity summary tables. Invalid messages go to a dead-letter table with the error attached instead of disappearing.

I built it to learn the orchestration and streaming split firsthand, and it taught me two things I now design for up front: Airflow tasks have to terminate, so the consumer drains a bounded batch instead of polling forever, and re-runs duplicate data unless the transform is idempotent, so it rebuilds from deduplicated rows in a single transaction.

→ [View Project](https://github.com/JustinK33/Pulsegrid)

## 📫 Connect

Email: justinkong.dev@gmail.com
Portfolio: [justinkong.app](https://justinkong.app/)
LinkedIn: [linkedin.com/in/justin-hkong](https://linkedin.com/in/justin-hkong)
