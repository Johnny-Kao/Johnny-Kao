_Last updated: **October 2026**_

# Hi there 👋
I'm **Johnny Kao**.

A lot of my formal professional work lives on [johnnykao.com](https://johnnykao.com).  
This GitHub is a bit different: it is the more experimental, technical, and personal side of me — selected code, open-source contributions, passing curiosities, and ideas I feel like keeping around.

I spend most of my time around **finance, strategy, cross-border questions, data, research, and digital systems**, but I have never liked staying in just one lane.

## ⚡ Current Focus

Recently, I have been spending more time on upstream open-source engineering, especially around **performance, correctness, concurrency, and low-level infrastructure**.

A recurring pattern in the work is simple: find an expensive or unsafe path, establish the behavioral boundary, reduce it to the smallest defensible change, benchmark or differential-test it, and upstream it.

## 🔧 Selected Open-Source Work

- **[c-blosc2 #805](https://github.com/Blosc/c-blosc2/pull/805)** — avoided unnecessary parallel startup and worker wakeups for low-parallelism jobs; a targeted 64-byte workload improved from **35.86 μs → 2.02 μs**.
- **[Memray #1035](https://github.com/bloomberg/memray/pull/1035)** — improved Linux/glibc Tracker contention handling, reducing runtime by up to **28% at 256 threads** in an allocation-heavy workload.
- **[urllib3 #5287](https://github.com/urllib3/urllib3/pull/5287)** — optimized the common single-value header path, improving representative request-construction workloads by roughly **9–13%**.
- **[python-blosc2 #728](https://github.com/Blosc/python-blosc2/pull/728)** — removed redundant full-block zeroing in the NumPy miniexpr gather path, improving tested workloads by roughly **2–15%**.

Additional merged correctness work spans **NumPy, SciPy, and free-threaded Python support in python-blosc2**.

## 🧭 Timeline Highlights

- **2026** — 📊 Joined **Bloomberg L.P.** in Tokyo; deepened upstream OSS work across scientific Python, systems, networking, profiling, and compression
- **2025** — 🚀 Moved from consulting into startup finance and corporate development, supporting a multi-billion-JPY fundraising extension and board-level decisions
- **2024** — 🧭 Worked across digital transformation, AI adoption, future banking strategy, and RWA tokenization
- **2022–2023** — 🌐 Worked on institutional digital assets, wealth management, payments, and emerging financial infrastructure
- **2020** — 🧊 Code preserved in GitHub’s **Arctic Code Vault**
- **2019** — 🏦 Worked on virtual banking and cross-border financial infrastructure
- **2015–2018** — 💳 Built and worked around payments, Bitcoin-linked card infrastructure, fintech, SaaS, and digital-asset systems
- **2013** — 🤝 Volunteered in Tunisia

Some repositories here are serious engineering work. Some are experiments. Some exist because I wanted to understand one obscure problem properly.

That distinction is intentional.
