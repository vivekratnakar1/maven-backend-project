# ⚡ Java Rate Limiter

A high-performance, low-latency rate limiting library for Java applications. Protect your APIs from abuse, handle traffic spikes gracefully, and enforce fair-use policies with minimal overhead.

---

## 🚀 Features

* **Multiple Algorithms** — Supports Token Bucket, Leaky Bucket, and Fixed Window.
* **Thread-Safe** — Optimized for high-concurrency environments using lock-free atomic operations.
* **Zero Dependencies** — Lightweight footprint with no external runtime third-party libraries.
* **Distributed Ready** — Optional Redis backing for multi-instance cluster synchronization.

---

## 🛠️ Core Algorithms

| Algorithm | Best For | Pros | Cons |
| :--- | :--- | :--- | :--- |
| **Token Bucket** | Burst traffic | Smooth average rate, handles bursts | Memory overhead per bucket |
| **Leaky Bucket** | Smooth egress traffic | Strict data rate control | Can delay request processing |
| **Fixed Window** | Basic API quotas | Simple to implement, low memory | Bursting at window boundaries |
