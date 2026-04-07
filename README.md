# MiniInfer-High-Concurrency-LLM-Inference-Scheduler.
A lightweight AI inference system focused on request scheduling, dynamic batching, and performance optimization under high concurrency.

MiniInfer is a simplified prototype of an LLM inference system designed to simulate real-world AI infrastructure challenges, including:
	•	High-concurrency request handling
	•	Dynamic batching for throughput optimization
	•	Latency vs throughput trade-off
	•	Task scheduling and worker execution
	•	System observability (metrics & monitoring)

                 ┌───────────────┐
                 │    Client     │
                 └──────┬────────┘
                        ↓
               ┌──────────────────┐
               │   API Gateway    │
               └────────┬─────────┘
                        ↓
               ┌──────────────────┐
               │  Request Queue   │
               └────────┬─────────┘
                        ↓
               ┌──────────────────┐
               │ Dynamic Batcher  │
               └────────┬─────────┘
                        ↓
               ┌──────────────────┐
               │   Worker Pool    │
               └────────┬─────────┘
                        ↓
               ┌──────────────────┐
               │  Model Runner    │
               └────────┬─────────┘
                        ↓
               ┌──────────────────┐
               │ Response + Stats │
               └──────────────────┘
              
Key Features
	•	Queue-based request scheduling
	•	Dynamic batching mechanism
	•	Multi-worker execution model
	•	Latency and throughput monitoring
	•	Designed for high-concurrency scenarios

⸻

Design Focus

This project is not about building a powerful model, but about:

Designing an efficient inference system under real-world constraints.
