_Last updated: **October 2026**_

# Hi there
I'm **Johnny Kao**, an independent upstream open-source contributor based in Tokyo.

My professional background spans **finance, strategy, data, and digital infrastructure**. This GitHub is where I explore the software foundations behind those systems, with a particular focus on **Scientific Python, performance, correctness, and concurrency**.

I look for avoidable work in widely used infrastructure, validate the behavior and trade-offs, and propose small, reviewable upstream changes. The goal is not a benchmark headline; it is a useful improvement that maintainers can accept and downstream users can rely on.

## Selected merged upstream contributions

These are **merged pull requests in the original upstream repositories**, not forks or unmerged experiments. Performance figures are from the linked PRs' specific test workloads, not universal production estimates.

### Scientific Python & data infrastructure

- **[SciPy #26225](https://github.com/scipy/scipy/pull/26225)** — fixed iteration-count reporting on early-return paths in bracketing solvers.
- **[NumPy #32802](https://github.com/numpy/numpy/pull/32802)** — fixed undefined shift behavior in the rational test dtype.
- **[pandas #69916](https://github.com/pandas-dev/pandas/pull/69916)** — removed unnecessary NA-membership checks in a numeric-conversion hot path; approximately **17–25% faster** in targeted benchmarks.
- **[Blosc2 #805](https://github.com/Blosc/c-blosc2/pull/805)** — avoided unnecessary parallel startup and worker wakeups for small compression jobs; **35.86 μs → 2.02 μs** on a targeted 64-byte workload.
- **[python-blosc2 #713](https://github.com/Blosc/python-blosc2/pull/713)** — fixed NDArray thread-safety issues affecting free-threaded Python support.

### Broader Python infrastructure

- **[urllib3 #5304](https://github.com/urllib3/urllib3/pull/5304)** — removed a redundant copy in gzip decompression; approximately **19–23% less client CPU time** for tested 32 MiB HTTP responses.
- **[Memray #1035](https://github.com/bloomberg/memray/pull/1035)** — reduced tracker synchronization contention on Linux/glibc; up to **28% runtime reduction** at 256 threads in the measured workload.
- **[attrs #1636](https://github.com/python-attrs/attrs/pull/1636)** — improved `astuple()` traversal for nested atomic sequences; up to **3.33×** in a reported local benchmark.
- **[packaging #1429](https://github.com/pypa/packaging/pull/1429)** — bypassed general-purpose literal evaluation for ordinary marker strings; approximately **13% faster** on the tested requirements corpus.

Other merged work includes [urllib3 #5287](https://github.com/urllib3/urllib3/pull/5287) and [python-blosc2 #728](https://github.com/Blosc/python-blosc2/pull/728).

## CoreFoundry

**[CoreFoundry Project](https://github.com/Johnny-Kao/CoreFoundry-Project)** documents the broader upstream engineering effort: selected results, reproducible evidence, research priorities, and ongoing PR status.

- **[Contribution ledger](https://github.com/Johnny-Kao/CoreFoundry-Project/blob/main/CONTRIBUTIONS.md)** — upstream links and status, including merged, open, and selected closed work.
- **[Research directions](https://github.com/Johnny-Kao/CoreFoundry-Project/blob/main/RESEARCH_AREAS.md)** — areas of inquiry and their boundaries.
- **[Current work](https://github.com/Johnny-Kao/CoreFoundry-Project/blob/main/CURRENT_WORK.md)** — public-safe work in progress.

The ledger is the source for changing PR status; this profile intentionally stays selective.

## Professional background

My work has included **financial services consulting at BCG**, corporate finance and strategy in a startup, and **data-related work at Bloomberg**. I am interested in the intersection of enterprise dependence on open-source infrastructure, maintainability, and long-term sustainability.

These are personal contributions and views. References to employers or upstream projects do **not** imply their sponsorship, endorsement, or authorization to represent them.

## Beyond the code

I also write and research questions around decision-making, institutional design, financial infrastructure, and technology. Some repositories here are maintained projects; others are research experiments. I keep that distinction explicit.
