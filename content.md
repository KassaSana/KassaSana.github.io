# Portfolio content (source of truth for index.html)

Edit this file first, then mirror changes into `index.html`.
Lines marked `TODO(kassa)` are for you to write in your own voice.

## Header

**Kassahun Sanayew**
M.S. Computer Engineering student at UF. I build storage engines, real-time data systems, and contribute to database and CUDA libraries.

GitHub: https://github.com/KassaSana · LinkedIn: https://linkedin.com/in/kassahun-sanayew · k.sanayew@ufl.edu · resume.pdf

## Experience

**CVS Health**: Software Engineering Co-op and Intern, 2026
TODO(kassa): confirm dates and wording. Draft: Built backend services for a retrieval-augmented generation (RAG) chatbot. Line 2: one concrete thing you shipped or measured.

**Amazon**: Software Development Engineer Intern, Promotions Platform, Seattle, WA, May–Aug 2024
TODO(kassa): Draft: Built API endpoints for the promotions platform. Line 2: one concrete thing (scale, service, result).

## Open source (merged)

- NVIDIA/cccl: Enable `__float128` in `cuda::std::ceil`, `floor`, `trunc`, `round`. https://github.com/NVIDIA/cccl/pull/12253
- NVIDIA/cccl: Unpin breathe now that 5.1.0 fixes template specialization names. https://github.com/NVIDIA/cccl/pull/12307
- DuckDB: Ensure DISTINCT aggregates share a branch only with a matching ORDER BY. https://github.com/duckdb/duckdb/pull/27852
- Apache DataFusion: CLI respects `sql_parser.recursion_limit` when parsing input. https://github.com/apache/datafusion/pull/25807
- Apache DataFusion: Validate `execution.time_zone` at `SET` time. https://github.com/apache/datafusion/pull/25788
- nba_api: Add the Celtics 2024 championship to static data. https://github.com/swar/nba_api/pull/695

## Projects

### durablekv
Does: A crash-safe LSM-tree key-value store with a write-ahead log, SSTables, leveled compaction, and Bloom filters, verified by kill -9 recovery tests.
Hardest decision: TODO(kassa)
Stack: C++20
Repo: https://github.com/KassaSana/durablekv

### ArbSync
Does: Keeps live L2 order books for Gemini, Coinbase, and Binance in memory, detects cross-exchange arbitrage above a threshold, stores it in SQLite, and streams it to a React dashboard.
Hardest decision: TODO(kassa)
Stack: Python (asyncio), SQLite, React/TypeScript
Repo: https://github.com/KassaSana/ArbSync
Note: no latency figure. The old "p99 27µs" came from a benchmark retired 2026-09-21. Only add a number from the current connected-dashboard harness.

### Snapback
Does: A desktop focus tracker that turns active-window activity into focus signals and helps you return to the task you were on after a distraction.
Hardest decision: TODO(kassa)
Stack: C++
Repo: https://github.com/KassaSana/Snapback

## Education

B.S. Computer Science, University of Florida, 2025
M.S. Computer Engineering, University of Florida, expected May 2027
