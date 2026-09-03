# Capacity note (team, one page)

## 

## The numbers

* Locked model: Qwen/Qwen2.5-1.5B-Instruct
* Target p95 end-to-end latency (your SLO today): 3.0 seconds
* Knee concurrency (highest concurrency whose p95 is still under target):16
* Tokens per second at the knee: 563.17
* Max sustainable request rate at the target p95:5.20 req/s



## The limiting family

* Memory-bound: throughput is still increasing at concurrency 16 while p95 remains under the target, consistent with decode being limited mainly by memory bandwidth.



## Why the knee, not the peak

* The knee is the highest concurrency that still meets the p95 SLO, while peak throughput may be too slow.

