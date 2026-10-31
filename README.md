*Last updated: **October 2026***

# Hi there 👋

I'm **Johnny Kao**.

This GitHub is a second Johnny: it is the more experimental, technical, and personal side of me — selected code, open-source contributions, passing curiosities, and ideas I feel like keeping around.

I spend most of my time around **finance, strategy, cross-border questions, data, research, and digital systems**, but I have never liked staying in just one lane.

## ⚡ Current Focus

Recently, I have been focusing on **upstream open-source engineering**, particularly performance optimization, correctness, concurrency, and foundational infrastructure.

I am interested in finding unnecessary work in widely used software — redundant computation, avoidable memory operations, expensive synchronization, and assumptions that no longer hold.

My approach is simple: understand the bottleneck, preserve behavior, make the smallest maintainable change, and validate the result.

## 🚀 Performance Highlights

Selected upstream contributions and performance research.

- **[pandas #69916](https://github.com/pandas-dev/pandas/pull/69916)** — Removed redundant NA checks. **16.5–24.7% lower execution time** in targeted numeric conversion.
- **[urllib3 #5304](https://github.com/urllib3/urllib3/pull/5304)** — Eliminated redundant gzip decompression copies. **14.7–39.2% faster** in targeted decoder benchmarks.
- **[urllib3 #5287](https://github.com/urllib3/urllib3/pull/5287)** — Optimized HTTP header processing. **9–13% faster** request construction in tested workloads.
- **[LZ4 #1858](https://github.com/lz4/lz4/issues/1858)** — Developed a one-line optimization to skip unnecessary writes. **~10–25% faster** in selected small buffered-write workloads; subsequently integrated upstream.
- **[idna #279](https://github.com/kjd/idna/pull/279)** — Proposed an ASCII domain-label fast path. **79.5–85.1% lower execution time** in candidate benchmarks; the approach was subsequently adopted upstream.
- **[attrs #1636](https://github.com/python-attrs/attrs/pull/1636)** — Optimized `astuple()` for nested atomic sequences. **Up to 3.33× faster** in targeted benchmarks.
- **[Memray #1035](https://github.com/bloomberg/memray/pull/1035)** — Reduced multithreaded allocation contention. **Up to 28% lower runtime** in tested workloads.
- **[c-blosc2 #805](https://github.com/Blosc/c-blosc2/pull/805)** — Eliminated unnecessary parallel overhead. **Up to 17.8× faster** in targeted small-block benchmarks.
- **[python-blosc2 #728](https://github.com/Blosc/python-blosc2/pull/728)** — Removed redundant memory zeroing. **2–15% faster** in targeted workloads.

*Performance figures represent specific benchmark workloads and environments, not universal production speedups.*

## 🛠️ Correctness, Reliability & Concurrency

Small, targeted changes can also eliminate subtle failures and make foundational software more reliable.

- **[NumPy #32802](https://github.com/numpy/numpy/pull/32802)** — Eliminated signed-shift undefined behavior. **UBSan verified; 48,592 tests passed**.
- **[SciPy #26225](https://github.com/scipy/scipy/pull/26225)** — Corrected iteration accounting for four root-finding solvers. **178 tests passed**.
- **[QuickFIX/J #1363](https://github.com/quickfix-j/quickfixj/pull/1363)** — Fixed failed synchronous FIX transport writes being reported as successful. **Merged; 9/9 fork CI jobs passed** across Java 8/11/21 and three operating systems.
- **[python-blosc2 #713](https://github.com/Blosc/python-blosc2/pull/713)** — Fixed two NDArray thread-safety bugs affecting free-threaded Python.

## 🔐 Security Research

- **[CVE-2026-115529](https://github.com/Johnny-Kao/CoreFoundry-Project/blob/main/SECURITY_RESEARCH.md)** — Discovered and reported a curl Schannel TLS session-resumption vulnerability. **CVE assigned, upstream fix committed, and officially credited.**

## 🧪 More About the Work

Many of these contributions involve small changes with measurable impact. The challenging part is often not writing the code, but understanding which work can be safely eliminated without introducing new complexity or changing behavior.

I also explore ideas that never become upstream contributions. Sometimes the research reveals an optimization; sometimes it reveals why the existing implementation should remain unchanged.

For detailed benchmarks, technical analysis, additional research, and the full upstream contribution record, see **[CoreFoundry Project](https://github.com/Johnny-Kao/CoreFoundry-Project)**.

## 🌍 Beyond Code

My background spans **consulting, finance, corporate strategy, digital transformation, and cross-border financial infrastructure**.

I also work on independent writing, publishing, and applied research, including the **[Japan Quarterly of Professional Practice](https://jqpp.org)**.

These interests may look unrelated, but they often involve the same questions: where are the real constraints, what assumptions are being made, and how can a system work better without unnecessary complexity?

## 🧭 Timeline Highlights

- **2026** — 📊 Deepened upstream OSS work across scientific Python, systems, networking, profiling, compression, and security research. Expanded independent publishing and established JQPP.
- **2025** — 🚀 Moved from consulting into startup finance and corporate development, supporting a multi-billion-JPY fundraising extension and board-level decisions.
- **2024** — 🧭 Worked across digital transformation, AI adoption, future banking strategy, and RWA tokenization.
- **2022–2023** — 🌐 Worked on institutional digital assets, wealth management, payments, and emerging financial infrastructure.
- **2020** — 🧊 Code preserved in GitHub's **Arctic Code Vault**.
- **2019** — 🏦 Worked on virtual banking and cross-border financial infrastructure.
- **2015–2018** — 💳 Built and worked around payments, Bitcoin-linked card infrastructure, fintech, SaaS, and digital-asset systems.
- **2013** — 🤝 Volunteered in Tunisia.

---

Some repositories here are serious engineering work. Some are experiments. Some exist because I wanted to understand one obscure problem properly.

That distinction is intentional.
