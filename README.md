_Last updated: **October 2026**_

# Hi there 👋
I'm **Johnny Kao**.

This GitHub is a second Johnny: it is the more experimental, technical, and personal side of me — selected code, open-source contributions, passing curiosities, and ideas I feel like keeping around.

I spend most of my time around **finance, strategy, cross-border questions, data, research, and digital systems**, but I have never liked staying in just one lane.

## ⚡ Current Focus

Recently, I have been spending more time on upstream open-source engineering, especially around **performance, correctness, concurrency, and low-level infrastructure**.

A recurring pattern in the work is simple: find an expensive or unsafe path, establish the behavioral boundary, reduce it to the smallest defensible change, benchmark or differential-test it, and upstream it.

## 🔧 Selected Open-Source Work

- **[NumPy #32802](https://github.com/numpy/numpy/pull/32802)** — eliminated a **32-bit** signed-shift undefined-behavior case; UBSan failure reproduced before and absent after the fix. Validation: **48,592 tests passed** (full non-slow suite).
- **[SciPy #26225](https://github.com/scipy/scipy/pull/26225)** — fixed incorrect iteration reporting for **4** bracketing solvers across **2** endpoint-root cases (**0 iterations** expected); **178 tests passed** in the affected test module.
- **[pandas #69916](https://github.com/pandas-dev/pandas/pull/69916)** — skipped redundant NA-membership checks on **1,000,000-element** numeric-conversion workloads, reducing direct benchmark time by **16.5–24.7%** (not end-to-end CSV performance).
- **[c-blosc2 #805](https://github.com/Blosc/c-blosc2/pull/805)** — avoided unnecessary thread startup and worker wakeups; **64 B: 35.86 → 2.02 μs**, **4 KiB: 38.90 → 3.63 μs** in targeted benchmarks; **1,616/1,616 tests passed**.
- **[python-blosc2 #728](https://github.com/Blosc/python-blosc2/pull/728)** — removed redundant full-block zeroing in the NumPy miniexpr gather path; **~2–15% faster** in targeted workloads, with **1,596 relevant tests passed**.
- **[Memray #1035](https://github.com/bloomberg/memray/pull/1035)** — improved Linux/glibc Tracker contention handling; measured runtime reductions of **13.1% at 4 threads**, **24.7% at 16**, and **28.0% at 256** in an allocation-heavy workload.
- **[urllib3 #5287](https://github.com/urllib3/urllib3/pull/5287)** — optimized single-value HTTP header processing; **~9–13% faster** request construction (**0.64–1.36 μs/request** saved) in tested 4–12-header workloads; **15/15** A/B comparisons faster.
- **[urllib3 #5304](https://github.com/urllib3/urllib3/pull/5304)** — avoided redundant gzip output copying; saved **26.1–27.0 μs per 1 MiB** of decoded output in tested single-output cases, with decoder-level gains of **14.7–39.2%** across tested sizes and payloads.

Additional merged correctness work includes **[python-blosc2 #713](https://github.com/Blosc/python-blosc2/pull/713)** — fixed **2** NDArray read-path thread-safety bugs under free-threaded Python; focused concurrent stress repeated **3×**.

*Performance figures are specific to the linked PRs' test environments and workloads, not general production-wide improvements.*

For a complete record of merged contributions and ongoing research, see **[CoreFoundry Project](https://github.com/Johnny-Kao/CoreFoundry-Project)**.

## 🧭 Timeline Highlights

- **2026** — 📊 Deepened upstream OSS work across scientific Python, systems, networking, profiling, and compression
- **2025** — 🚀 Moved from consulting into startup finance and corporate development, supporting a multi-billion-JPY fundraising extension and board-level decisions
- **2024** — 🧭 Worked across digital transformation, AI adoption, future banking strategy, and RWA tokenization
- **2022–2023** — 🌐 Worked on institutional digital assets, wealth management, payments, and emerging financial infrastructure
- **2020** — 🧊 Code preserved in GitHub’s **Arctic Code Vault**
- **2019** — 🏦 Worked on virtual banking and cross-border financial infrastructure
- **2015–2018** — 💳 Built and worked around payments, Bitcoin-linked card infrastructure, fintech, SaaS, and digital-asset systems
- **2013** — 🤝 Volunteered in Tunisia

Some repositories here are serious engineering work. Some are experiments. Some exist because I wanted to understand one obscure problem properly.

That distinction is intentional.
