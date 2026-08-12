---
title: Data Engineering — 25 Module Master Roadmap
category: Data Engineering
subject: Roadmap
difficulty: Beginner → Advanced
status: Learning
created: 2026-08-10
tags:
  - data-engineering
  - roadmap
  - sql
  - python
  - spark
  - kafka
  - databricks
  - gcp
  - cloud
---

# 🧭 Data Engineering — 25 Module Master Roadmap

> [!abstract] Goal
> Become capable of **understanding → designing → building → debugging → optimizing → explaining → defending** real-world Data Engineering systems.

---

# 🗺️ Complete 25-Module Roadmap

## 🟦 FOUNDATION

### Module 01 — SQL for Data Engineering
- Database & relational concepts
- SQL fundamentals
- Filtering
- Aggregation
- CASE expressions
- NULL handling
- Functions
- JOINs
- Subqueries
- CTEs
- Set operations
- Window functions
- Views
- Transactions
- ACID
- Indexes
- Query execution
- EXPLAIN / EXPLAIN ANALYZE
- Query optimization
- Partitioning
- Analytical SQL
- ETL SQL
- Data cleaning SQL

### Module 02 — Python for Data Engineering
- Python fundamentals
- Data structures
- Functions
- OOP basics
- Exception handling
- File handling
- CSV / JSON
- Datetime
- Modules & packages
- Virtual environments
- pip
- HTTP & APIs
- Logging
- Configuration
- Environment variables
- pandas
- Database connectivity
- ETL programming
- Testing

### Module 03 — Linux + Git/GitHub
- Linux fundamentals
- Filesystem
- Permissions
- Processes
- Environment variables
- Pipes & redirection
- Shell commands
- SSH
- Logs
- Bash basics
- Git fundamentals
- Branching
- Merging
- Pull requests
- GitHub workflow
- Repository management

### Module 04 — Data Engineering Fundamentals
- Data Engineer role
- Data lifecycle
- Data sources
- Data ingestion
- ETL
- ELT
- Batch processing
- Streaming processing
- Data transformation
- Data storage
- Data serving
- Data quality
- Data lineage
- Data governance
- Data formats
- Scalability
- Reliability
- Fault tolerance
- Idempotency
- Observability

### Module 05 — Data Warehousing + Data Modeling
- OLTP
- OLAP
- Database
- Data warehouse
- Data lake
- Data lakehouse
- Data mart
- Fact tables
- Dimension tables
- Star schema
- Snowflake schema
- Normalization
- Denormalization
- Grain
- Keys
- Surrogate keys
- SCD Type 1
- SCD Type 2
- Partitioning
- Clustering

---

# 🟨 DISTRIBUTED DATA PROCESSING

### Module 06 — Apache Spark + PySpark
- Distributed computing
- Parallelism
- Spark architecture
- Driver
- Executors
- Cluster manager
- Jobs
- Stages
- Tasks
- Partitions
- DAG
- Lazy evaluation
- Transformations
- Actions
- DataFrames
- Spark SQL
- PySpark
- Narrow transformations
- Wide transformations
- Shuffle
- Joins
- Window functions
- Caching
- Partitioning
- Data skew
- Spark optimization
- Spark UI
- Adaptive Query Execution

### Module 07 — Apache Kafka + Streaming Fundamentals
- Event-driven architecture
- Kafka architecture
- Broker
- Topic
- Partition
- Producer
- Consumer
- Consumer group
- Offset
- Replication
- Ordering
- Retention
- Delivery semantics
- Serialization
- Schema management
- Kafka Streams concepts
- Kafka + Spark Streaming
- Real-time pipelines
- Exactly-once / at-least-once concepts

---

# 🟧 DATABRICKS + LAKEHOUSE

### Module 08 — Databricks Platform
- Databricks architecture
- Workspace
- Compute
- Clusters
- Serverless
- Notebooks
- SQL Warehouse
- Catalog Explorer
- Data engineering workflows
- Databricks ecosystem

### Module 09 — Delta Lake
- Lakehouse architecture
- Delta tables
- ACID transactions
- Transaction log
- Schema enforcement
- Schema evolution
- MERGE
- UPDATE
- DELETE
- Time travel
- OPTIMIZE
- VACUUM
- Partitioning
- Clustering
- Small-file problem

### Module 10 — Lakeflow
- Lakeflow architecture
- Declarative pipelines
- Batch pipelines
- Streaming pipelines
- Streaming tables
- Materialized views
- Incremental processing
- Data quality expectations
- Pipeline dependencies
- Pipeline monitoring

### Module 11 — Databricks Workflows
- Jobs
- Tasks
- Task dependencies
- Scheduling
- Parameters
- Retries
- Alerts
- Job clusters
- Workflow design
- Monitoring
- Failure handling
- Orchestration

### Module 12 — Unity Catalog + Governance
- Catalog
- Schema
- Tables
- Views
- Volumes
- Managed tables
- External tables
- External locations
- Storage credentials
- Permissions
- Access control
- Data lineage
- Governance
- Security

### Module 13 — Databricks CI/CD
- Git integration
- Repositories
- Branches
- Pull requests
- Testing
- Deployment
- Environments
- Development → Test → Production
- Databricks CLI
- Declarative Automation Bundles
- CI/CD pipelines

### Module 14 — Databricks Monitoring + Optimization
- Spark UI
- Job monitoring
- Query plans
- Cluster sizing
- Partitioning
- Shuffle optimization
- Data skew
- Small files
- Caching
- Broadcast joins
- Liquid clustering
- Predictive optimization
- Performance troubleshooting
- Cost optimization

---

# 🟩 GOOGLE CLOUD DATA ENGINEERING

### Module 15 — Google Cloud Fundamentals
- Cloud computing
- Regions
- Zones
- Compute
- Storage
- Networking
- Managed services
- Serverless
- Scalability
- Availability
- IAM
- Cloud architecture basics

### Module 16 — Google Cloud Storage
- Buckets
- Objects
- Storage classes
- Lifecycle management
- Versioning
- Permissions
- IAM
- Encryption
- Data organization
- Data lake storage

### Module 17 — BigQuery
- BigQuery architecture
- Datasets
- Tables
- Views
- SQL
- Partitioning
- Clustering
- External tables
- Materialized views
- Query optimization
- Query cost
- Slots
- Reservations
- Storage vs compute

### Module 18 — Pub/Sub
- Messaging systems
- Topics
- Subscriptions
- Publishers
- Subscribers
- Pull
- Push
- Acknowledgement
- Retention
- Dead-letter topics
- Ordering
- Delivery semantics
- Event-driven architecture

### Module 19 — Dataflow + Apache Beam
- Dataflow architecture
- Apache Beam
- Pipelines
- PCollections
- Transforms
- Batch processing
- Streaming processing
- Windowing
- Triggers
- Watermarks
- Late data
- Event-time processing
- Stateful processing

### Module 20 — Dataproc + Composer/Airflow
#### Dataproc
- Hadoop
- Spark
- Dataproc
- Dataproc Serverless
- Cluster management
- Spark jobs
- Dataproc vs Dataflow
- Dataproc vs BigQuery

#### Composer / Airflow
- DAG
- Task
- Operator
- Dependency
- Scheduling
- Retry
- Backfill
- Monitoring
- Orchestration

---

# 🟥 PRODUCTION DATA ENGINEERING

### Module 21 — IAM + Security + Data Governance
- Authentication
- Authorization
- IAM
- Roles
- Permissions
- Service accounts
- Least privilege
- Encryption
- Secrets
- Network security
- Data governance
- Privacy
- Compliance
- Access control
- Auditing

### Module 22 — Data Quality + Data Validation
- Data quality dimensions
- Accuracy
- Completeness
- Consistency
- Validity
- Uniqueness
- Timeliness
- Schema validation
- Null validation
- Duplicate detection
- Referential integrity
- Business rules
- Data profiling
- Data contracts
- Bad-record handling

### Module 23 — Monitoring + Reliability + Observability
- Logging
- Metrics
- Tracing
- Alerts
- Pipeline monitoring
- Failure detection
- Retry
- Backoff
- Checkpointing
- Idempotency
- Dead-letter queues
- Recovery
- SLA
- SLO
- Disaster recovery
- Fault tolerance

### Module 24 — Performance + Cost Optimization
- Storage vs compute
- Query optimization
- Partitioning
- Clustering
- Compression
- Data pruning
- Caching
- Parallelism
- Resource sizing
- Autoscaling
- Serverless
- Batch vs streaming
- File optimization
- Cloud cost optimization
- Performance troubleshooting

### Module 25 — Data Architecture + System Design
- Data architecture
- Batch architecture
- Streaming architecture
- Lambda architecture
- Kappa architecture
- Lakehouse architecture
- Data warehouse architecture
- Pipeline design
- Scalability
- Reliability
- Availability
- Consistency
- Fault tolerance
- Data contracts
- Security architecture
- Cost architecture
- Capacity planning
- Trade-offs
- End-to-end system design
- Data Engineer interview architecture

---

# 🏗️ Project Progression

| Stage | Project | Main Skills |
|---|---|---|
| Stage 1 | API → PostgreSQL ETL | Python + SQL |
| Stage 1 | E-commerce Warehouse | SQL + Modeling |
| Stage 1 | Sales Analytics | ETL + SQL |
| Stage 1 | Stage 1 Capstone | Foundations |
| Stage 2 | Large CSV Analytics | PySpark |
| Stage 2 | E-commerce Spark ETL | Spark + Optimization |
| Stage 2 | Log Analytics | Distributed Processing |
| Stage 2 | Spark Performance Lab | Debugging + Optimization |
| Stage 2 | Stage 2 Capstone | Spark |
| Stage 3 | Real-Time Clickstream | Kafka + Spark |
| Stage 3 | Streaming Analytics | Kafka + Streaming |
| Stage 4 | Databricks Lakehouse | Delta + Lakeflow |
| Stage 4 | Production Lakehouse | Databricks |
| Stage 5 | GCP Batch Pipeline | GCS + Dataflow + BigQuery |
| Stage 5 | GCP Streaming Pipeline | Pub/Sub + Dataflow |
| Stage 6 | Production Data Platform | Security + Quality + Monitoring |
| Final | End-to-End Data Platform | Everything |

---

# 📚 Learning Order

```text
01 SQL
   ↓
02 Python
   ↓
03 Linux + Git
   ↓
04 Data Engineering Fundamentals
   ↓
05 Data Warehousing + Modeling
   ↓
06 Spark
   ↓
07 Kafka
   ↓
08 Databricks
   ↓
09 Delta Lake
   ↓
10 Lakeflow
   ↓
11 Workflows
   ↓
12 Unity Catalog
   ↓
13 CI/CD
   ↓
14 Monitoring + Optimization
   ↓
15 GCP Fundamentals
   ↓
16 Cloud Storage
   ↓
17 BigQuery
   ↓
18 Pub/Sub
   ↓
19 Dataflow
   ↓
20 Dataproc + Airflow
   ↓
21 Security
   ↓
22 Data Quality
   ↓
23 Reliability
   ↓
24 Performance + Cost
   ↓
25 Architecture