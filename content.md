# Portfolio content (source of truth for index.html)

Edit this file first, then mirror changes into `index.html`.
Lines marked `TODO(kassa)` are for you to write in your own voice.

## Header

**Kassahun Sanayew** · Gainesville, FL
Software engineer and M.Eng student at UF. I build storage engines and real-time data systems, and I contribute to open-source database and CUDA libraries.

Resume (resume.pdf, not uploaded yet) · GitHub https://github.com/KassaSana · LinkedIn https://linkedin.com/in/kassahun-sanayew · k.sanayew@ufl.edu

## Experience

**CVS Health**: Software Engineer Co-op (Aug 2026 – present) · Intern (May – Aug 2026)
- Migrating XQuery extracts to Java 21 and MongoDB in Aetna's bulk extract framework.
- Built a catalog chatbot over 8,000+ applications and APIs, and moved its retrieval from semantic-only to hybrid (BM25 + reciprocal rank fusion).

**Amazon**: Software Development Engineer Intern (May – Aug 2024)
- Built two REST APIs in the LifecyclePromotion service, plus a generator that parses promotion-graph conditions into ASTs and synthesizes minimal satisfying payloads.
- Cut test-payload prep from 10–20 minutes to seconds; wired AWS AppConfig for live rule updates.

## Open source (merged)

- NVIDIA/cccl #12253: Enable `__float128` in `cuda::std::ceil`, `floor`, `trunc`, `round`
- NVIDIA/cccl #12307: Unpin breathe now that 5.1.0 fixes template specialization names
- duckdb #27852: DISTINCT aggregates share a branch only with a matching ORDER BY
- datafusion #25807: CLI respects `sql_parser.recursion_limit` when parsing input
- datafusion #25788: Validate `execution.time_zone` at `SET` time
- nba_api #695: Add the Celtics 2024 championship to static data

## Projects (two only)

### durablekv (C++20 · POSIX · no dependencies)
A crash-safe LSM-tree key-value store with a write-ahead log, SSTables, leveled compaction, and Bloom filters. Once a write returns OK, it survives kill -9.
Hardest decision: TODO(kassa)
Chips: Bloom 41K → 2.26M absent-key lookups/s (from README benchmarks) · kill -9 recovery tests · CRC32C everywhere

### ArbSync (Python asyncio · SQLite · React/TS)
Live L2 order books for Gemini, Coinbase, and Binance with cross-exchange arbitrage detection, SQLite persistence, and a React dashboard.
Hardest decision: TODO(kassa)
Chips: 3 exchanges, live · property-based tests (server/tests/test_orderbook_properties.py) · replay regression (server/arb/replay.py)
Do not add: the old "p99 27µs" (from a retired benchmark) or a coverage % (not verified).

## Education

Master of Engineering, Computer Engineering · University of Florida · Aug 2025 – Dec 2026
B.S. Computer Science · University of Florida · Aug 2023 – Aug 2025

## Later (not on the page yet)
NCCL PR once merged · CVS full-time role once accepted · compiler pipeline as a third project
