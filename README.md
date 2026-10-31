*Last updated: **October 2026***

# Hi there 👋

I'm **Johnny Kao**.

This GitHub is a second Johnny: it is the more experimental, technical, and personal side of me — selected code, open-source contributions, passing curiosities, and ideas I feel like keeping around.

My background spans **consulting, finance, corporate strategy, digital transformation, and cross-border financial infrastructure**. My interests also include **data, research, digital systems, independent writing, and publishing** — I've never liked staying in just one lane.

## ⚡ Current Focus

Recently, I have been focusing on **upstream open-source engineering**, particularly performance optimization, correctness, concurrency, and foundational infrastructure.

I look for unnecessary work and hidden assumptions in widely used software — redundant computation, memory operations, synchronization, and subtle correctness boundaries.

My approach is to understand the system, make the smallest maintainable change, and validate its impact. Not every promising idea belongs upstream; sometimes the research explains why the existing design should remain.

For detailed benchmarks, technical research, and my full contribution record, see **[CoreFoundry Project](https://github.com/Johnny-Kao/CoreFoundry-Project)**.

## 🚀 Performance Highlights

Selected upstream contributions and performance research.

| Project | Optimization | Measured result |
|---|---|---|
| **[pandas #69916](https://github.com/pandas-dev/pandas/pull/69916)** | Removed redundant NA checks in numeric conversion | **16.5–24.7% less time** |
| **[urllib3 #5304](https://github.com/urllib3/urllib3/pull/5304)** | Avoided redundant gzip decompression copies | **14.7–39.2% faster** |
| **[urllib3 #5287](https://github.com/urllib3/urllib3/pull/5287)** | Optimized HTTP header processing | **9–13% faster** |
| **[LZ4 #1858](https://github.com/lz4/lz4/issues/1858)** | Skipped unnecessary zero-length writes; later integrated upstream | **~10–25% faster** |
| **[idna #279](https://github.com/kjd/idna/pull/279)** | Proposed an ASCII domain-label fast path; approach later adopted upstream | **79.5–85.1% less time** (original candidate) |
| **[attrs #1636](https://github.com/python-attrs/attrs/pull/1636)** | Optimized `astuple()` for nested atomic sequences | **Up to 3.33× faster** |
| **[Memray #1035](https://github.com/bloomberg/memray/pull/1035)** | Reduced multithreaded allocation contention | **Up to 28% lower runtime** |
| **[c-blosc2 #805](https://github.com/Blosc/c-blosc2/pull/805)** | Eliminated unnecessary parallel overhead | **Up to 17.8× faster** |
| **[python-blosc2 #728](https://github.com/Blosc/python-blosc2/pull/728)** | Removed redundant memory zeroing | **2–15% faster** |

*Performance figures reflect specific benchmark workloads, not general production-wide speedups.*

## 🛠️ Correctness, Reliability & Concurrency

| Project | Improvement | Validation / outcome |
|---|---|---|
| **[NumPy #32802](https://github.com/numpy/numpy/pull/32802)** | Eliminated signed-shift undefined behavior | **UBSan verified · 48,592 tests passed** |
| **[SciPy #26225](https://github.com/scipy/scipy/pull/26225)** | Fixed iteration accounting for four root-finding solvers | **178 tests passed** |
| **[QuickFIX/J #1363](https://github.com/quickfix-j/quickfixj/pull/1363)** | Prevented failed synchronous FIX writes from reporting success | **Merged · 9/9 fork CI jobs passed** |
| **[python-blosc2 #713](https://github.com/Blosc/python-blosc2/pull/713)** | Fixed two thread-safety bugs affecting free-threaded Python | **Merged · concurrent stress validated** |

## 🔐 Security Research

- **[CVE-2026-115529](https://github.com/Johnny-Kao/CoreFoundry-Project/blob/main/SECURITY_RESEARCH.md)** — Discovered and reported a curl Schannel TLS session-resumption vulnerability. **CVE assigned, upstream fix committed, and officially credited.**

<details>
<summary><strong>🧭 Timeline Highlights</strong></summary>


- **2026** — 📊 Deepened upstream OSS work across scientific Python, systems, networking, profiling, compression, and security research. Expanded independent publishing and established JQPP.
- **2025** — 🚀 Moved from consulting into startup finance and corporate development, supporting a multi-billion-JPY fundraising extension and board-level decisions.
- **2024** — 🧭 Worked across digital transformation, AI adoption, future banking strategy, and RWA tokenization.
- **2022–2023** — 🌐 Worked on institutional digital assets, wealth management, payments, and emerging financial infrastructure.
- **2020** — 🧊 Code preserved in GitHub's **Arctic Code Vault**.
- **2019** — 🏦 Worked on virtual banking and cross-border financial infrastructure.
- **2015–2018** — 💳 Built and worked around payments, Bitcoin-linked card infrastructure, fintech, SaaS, and digital-asset systems.
- **2013** — 🤝 Volunteered in Tunisia.

</details>
