<h1 align="center">JinYan Su</h1>

<p align="center">
  <b>LLM Serving Infrastructure / Rust + CUDA / KV Cache Systems</b>
</p>

<p align="center">
  <b>I build the systems path between model weights and production tokens.</b>
</p>

<p align="center">
  Inference runtime, decode fast paths, KV cache movement, GPU offload, SSD tiering, RDMA transport, NUMA-aware memory, and vLLM/SGLang/Mooncake integration.
</p>

<p align="center">
  <a href="https://github.com/xiaguan?tab=followers">
    <img src="https://img.shields.io/github/followers/xiaguan?label=GitHub&style=flat-square" alt="GitHub followers" />
  </a>
  <a href="https://github.com/xiaguan/pegainfer">
    <img src="https://img.shields.io/github/stars/xiaguan/pegainfer?label=pegainfer&style=flat-square" alt="pegainfer stars" />
  </a>
  <a href="https://github.com/novitalabs/pegaflow">
    <img src="https://img.shields.io/github/stars/novitalabs/pegaflow?label=pegaflow&style=flat-square" alt="pegaflow stars" />
  </a>
  <a href="https://www.linkedin.com/in/%E9%87%91%E9%98%B3-%E8%8B%8F-10973a281/">
    <img src="https://img.shields.io/badge/LinkedIn-JinYan%20Su-0a66c2?style=flat-square" alt="LinkedIn" />
  </a>
  <a href="https://susun-blog.com/">
    <img src="https://img.shields.io/badge/Blog-susun--blog.com-2ea44f?style=flat-square" alt="Blog" />
  </a>
  <a href="https://www.zhihu.com/people/yixie-gu-zhou-6-9">
    <img src="https://img.shields.io/badge/Zhihu-profile-1772f6?style=flat-square" alt="Zhihu" />
  </a>
</p>

## What I am building

I work on the serving substrate for large language models: the layer where CUDA kernels, Rust runtimes, KV cache systems, RDMA transport, and production schedulers meet.

My public work is concentrated in one direction: make LLM serving faster, more observable, and more predictable when the bottleneck is no longer just the model, but memory movement, cache layout, GPU/CPU coordination, and distributed serving behavior.

## Public signal

| System | What I push on |
| --- | --- |
| [pegainfer](https://github.com/xiaguan/pegainfer) | Pure Rust + CUDA inference runtime, Kimi/DeepSeek/Qwen decode paths, PPLX EP, CuTeDSL/cuBLAS prefill kernels, benchmark gates, nsys profiling |
| [PegaFlow](https://github.com/novitalabs/pegaflow) | KV cache storage for vLLM/SGLang, GPU offloading, SSD caching, RDMA QPs, pinned memory, NUMA placement, cache metrics, vLLM E2E gates |
| [Mooncake](https://github.com/kvcache-ai/Mooncake) | Store/transfer engine work, client metrics, RDMA device setup, NUMA binding, SGLang HiCache documentation and integration paths |
| [LMCache](https://github.com/LMCache/LMCache) | Mooncake connector performance, zero-copy get/put, NUMA-aware operations, vLLM scheduler/cache behavior |
| [SGLang](https://github.com/sgl-project/sglang) | HiCache/Mooncake integration, NUMA detection, cache prefetch fixes, serving-path reliability |
| [vLLM ecosystem](https://github.com/vllm-project/vllm) | Scheduler/cache issues, router fixes, connector behavior, large-scale serving ergonomics |

## Where I go deep

- Rust inference runtimes and CUDA-backed model execution
- Decode hot paths for Kimi, DeepSeek, and Qwen-style serving workloads
- KV cache transport across GPU memory, CPU pinned memory, SSD, and RDMA
- NUMA-aware allocation, pinned pool startup, CUDA IPC, and long-tail latency control
- vLLM/SGLang connector behavior under real cache pressure
- Benchmarking, profiling, CI gates, and release paths for serving infrastructure

## Current stack

`Rust` / `CUDA` / `C++` / `Python` / `RDMA` / `vLLM` / `SGLang` / `Mooncake` / `LMCache` / `PegaFlow`

## Contact

- LinkedIn: [JinYan Su](https://www.linkedin.com/in/%E9%87%91%E9%98%B3-%E8%8B%8F-10973a281/)
- Blog: [susun-blog.com](https://susun-blog.com/)
- Zhihu: [yixie-gu-zhou-6-9](https://www.zhihu.com/people/yixie-gu-zhou-6-9)
