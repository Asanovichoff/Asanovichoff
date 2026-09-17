Hi, I'm Akan Abdireshov 👋

Backend-focused software engineer in the Greater Seattle Area. I build distributed, event-driven systems, developer tools for AI coding assistants, and travel products for Kyrgyzstan.

Lately most of my time goes into three things: event-driven backends (Kafka, Redis, FastAPI, Spring Boot), tooling around Claude Code and MCP, and shipping dacantours.com.

💼 Experience

Software Engineer Intern, Akyldoo AI · Seattle, WA · Apr 2026 – Aug 2026

Found the five slowest SQL queries with pg_stat_statements and optimized three (index tuning, no SELECT *, keyset instead of OFFSET pagination), cutting primary database CPU by ~20%.
Built semantic code search and contextual Q&A across repositories, so developers locate relevant files 3× faster.
Streamed OpenAI responses over Server-Sent Events, taking perceived latency from ~20 seconds to under 1 second.

Software Engineer Intern, Ak-Sai · Seattle, WA · May 2025 – Sep 2025

Built proximity-aware listing search with PostGIS and GiST KNN indexing.
Eliminated double-booking race conditions with PostgreSQL pessimistic row locking and a date-overlap check.
Drove the migration from a monolith to Docker-containerized microservices, increasing deployment velocity by 40%.
🛠 Tech

Languages: Java, Python, TypeScript, JavaScript, SQL, Dart Backend: Spring Boot, FastAPI, NestJS, Flask, REST APIs, Server-Sent Events Data & Messaging: PostgreSQL (PostGIS), Redis, Apache Kafka, MySQL, SQLite Cloud & Infrastructure: AWS, GCP, Docker, Kubernetes, Terraform, GitHub Actions, Prometheus, Grafana, Cloudflare Workers Frontend & Mobile: Next.js, React, React Native (Expo), Flutter, Tailwind CSS AI Tooling: MCP servers, Claude Agent Skills, semantic search, LLM streaming Systems: Distributed systems, event-driven architecture, microservices, concurrency

🚀 Featured Projects
🛡 GuardStream – Real-Time API Threat Detection

A two-path, event-driven architecture that separates enforcement from analysis, so threat detection never adds latency to the API. Highlights: Redis Lua sliding window and blocklist on the fast path (avg 0.9 ms, p99 2.6 ms); Kafka consumer groups run four deterministic detectors for credential stuffing, DDoS, scraping, and sequential enumeration, then write block rules back to Redis. Production-style AWS infrastructure in Terraform across 13 services (MSK, ECS Fargate, ElastiCache, Aurora Serverless v2, CloudWatch, WAF, ALB, and more), testable locally with LocalStack. Stack: Python, FastAPI, Apache Kafka, Redis, AWS, Terraform, Docker

🧠 OyHub

A local, always-on MCP server that gives Claude Desktop, Claude Code, and Cursor one central skill library and persistent memory across sessions. Highlights: per-project skill activation, Obsidian vault + SQLite FTS5 memory, background curator loop, WAL mode and file-locked atomic writes validated with parallel-writer tests (8 threads, zero lost updates), prompt-injection scanning on writes, FastAPI dashboard, Prometheus metrics with a provisioned Grafana board, CI on a 6-way OS/Python matrix. Zero runtime dependencies, published on PyPI. Stack: Python (stdlib), MCP, SQLite, FastAPI, Docker, Prometheus, Grafana

✅ skill-lint

A linter for Claude Agent Skills. Checks SKILL.md bundles against the Agent Skills spec and the Skills API upload requirements before a failed upload tells you. Highlights: 15 error rules and 17 warning rules, --target spec|claude-code|both, JSON output for CI, installable as a skill itself. Standard library only. Stack: Python, GitHub Actions

📈 claude-token-tracker

Tracks Claude Code token usage across every session and project through a Stop hook. Comes as a CLI and a VS Code extension sharing one local SQLite database. Highlights: today/week/all-time views, cost estimates, per-model breakdown, per-turn session replay. No API keys, no network, no dependencies. Stack: TypeScript, Node.js, SQLite, VS Code Extension API

🌍 DACANTOURS

The live site for dacantours.com: a Kyrgyzstan expedition plus five US national park tours. Rebuilt from the original React + Flask app into a fully static site. Stack: Next.js 16, TypeScript, Tailwind CSS v4, Cloudflare Workers Also in progress: travel-platform, the full-stack version (Next.js, NestJS, Directus, PostgreSQL, Zod, Docker).

🏔 KyrgyzExplore

Cross-platform mobile app for travelers in Kyrgyzstan: car rentals, stays, and local activities, with host-side listing management. Think Airbnb + Turo for Kyrgyzstan. Stack: Flutter, Spring Boot 3 (Java 21), PostgreSQL + PostGIS, Redis, Stripe Connect, AWS S3, Docker

🚗 Auction Prep

Offline-first iOS app for small used-car dealers: capture a VIN at the auction, decode it, and get a bid ceiling before the car rolls through. All data stays on the device. Stack: React Native, Expo, TypeScript, SQLite

🤝 Team Projects & Open Source
focusn't – a focus timer that uses in-browser computer vision (MediaPipe) to detect distraction, with a Three.js galaxy that grows with each completed session.
psxdata – contributed Docker support and a health endpoint for the FastAPI service of this Pakistan Stock Exchange data library.
Poly Predictor Kit – QuackHack hackathon project.
AI Visual Novel Creator – CodeDay Seattle 2025 winner (see below).
🧩 Practice

leetcode-java-solutions – 180+ LeetCode solutions in Java, organized by topic, updated daily.

📊 Earlier ML Work

Product Review Analyzer (NLP sentiment, Streamlit) · Thompson Sampling News Recommender (Bayesian RL) · Logistic Regression Traveler Analysis

🎓 Education
A.S. in Computer Science, Cascadia College, Bothell, WA (2026)
B.S. in Electrical and Computer Engineering, Osh State University, Kyrgyzstan (2023)
🏆 Achievements
🥇 CodeDay Seattle 2025 – Best Use of AI Award for AI Visual Novel Creator
🏊‍♂️ Half Ironman trainee – the same consistency goes into daily LeetCode
📫 Connect
LinkedIn: linkedin.com/in/akan-abdireshov
Website: dacantours.com
Email: asanovich.02@gmail.com
