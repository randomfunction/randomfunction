Final-year CS student at IIIT Nagpur, graduating Aug 2027. I build storage engines, vector search and LLM request routing, mostly in C++ and Rust. Currently an SDE intern at Sign3, working on AWS/EKS infrastructure and data pipelines.

Looking for backend, infrastructure, AI-infra and low-level systems roles.

[LinkedIn](https://linkedin.com/in/tanishq52)

### Projects

**[kvroute](https://github.com/randomfunction/kvroute)**: cache-aware routing across LLM inference replicas, in Rust. Phase 1 is four baseline routers and a discrete-event simulator. In a simulated 5.2k-request trace on 4 replicas, prefix routing cut p99 TTFT 61% against round-robin and raised cache hit rate from 70.5% to 85.1%, at the cost of more load imbalance (1.21x vs 1.04x). All results are simulated; there is no live proxy yet, and the session-aware policy is a stub.

**[vector_database](https://github.com/randomfunction/vector_database)**: HNSW search in C++ with AVX2 distance kernels and runtime CPU dispatch. 99.3% Recall@10, 2,215 QPS and 654 µs p99 on SIFT1M ([benchmark script](https://github.com/randomfunction/vector_database/blob/main/scripts/run_sift_benchmark.sh)).

**[LSMTree_engine](https://github.com/randomfunction/LSMTree_engine)**: educational LSM-tree key-value store in C++17, with a WAL, Bloom filters, size-tiered compaction, a skip-list memtable and in-memory MVCC. No range scans, checksums or block cache yet.

### Stack

C++17 · Rust · Java · Python · AWS (EKS, Lambda, Kinesis, DynamoDB) · Kubernetes · ClickHouse · Parquet · Redis · Docker
