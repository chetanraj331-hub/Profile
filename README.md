Hi, I'm Chetan Raj 👋
Data & Cloud Engineer → MBA (PGPEx 2027, IIM Mumbai) · 5.5 years across BFSI and healthcare · Agentic AI, data platforms, cloud migration

I build scalable cloud data platforms and, more recently, multi-agent simulations that turn supply-chain risk signals into decisions.

LinkedIn
https://www.linkedin.com/in/chetan-raj-756449143/


🧰 Skills
Area	Tools & Concepts
Data Engineering	ETL/ELT, Data Warehousing (DIM/FACT, delivery layer), Oracle ODI & OWB, large-scale migration
Cloud	Google Cloud Platform, Oracle → GCP modernization, data lakes & warehouses
BI & Analytics	Power BI, ERP reporting, compliance dashboards
AI	Agentic AI (Claude + MCP), multi-agent simulation, Gemini search-grounded APIs
Visualization	D3.js knowledge graphs
Management	Process optimization, cross-functional leadership, IT client management
🚀 Featured Project
Intel Substrate → Packaging → Facility Knowledge Graph · IIM Mumbai capstone, June 2026
An interactive, sourced and weighted knowledge graph plus multi-agent simulation of semiconductor substrate supply risk, tracing raw materials → substrates → packaging tech (EMIB / EMIB-T / Foveros) → facilities → processors → end use, overlaid with PESTEL factors.

~50 nodes, ~100 relationships, 33 cited sources, each node tagged high / medium / estimate confidence
Toggleable agents (Supply Concentration, Cost & Pricing, Capacity & Investment) recompute node weights
Optional live mode using Gemini with Google Search grounding
🔗 Live demo: https://chetanraj331-hub.github.io/intel-substrate-agent-graph/ (works once GitHub Pages is on)
Stack: JavaScript, D3.js, Gemini API


💼 Experience
Consultant, Deloitte USI (Bangalore) · Aug 2024 – Apr 2026

Deployed an agentic AI workflow (Claude + MCP) to automate entity resolution, deduplication and constraint-violation fixes, eliminating pipeline failures
Modernized a 7.2 TB Oracle dataset on GCP for a major healthcare program: queries cut from hours to seconds (~40% faster), $15K+ hardware refresh avoided
Led a team of 3 migrating 2,000+ tables and 28+ modules from Oracle to GCP; built a reusable framework that cut development time 70% (6 → 2 weeks)
Built a cross-platform Oracle ↔ GCP data testing framework, reducing UAT timelines by 60%
Built pipelines for a Supplier Performance Dashboard and unified lease data for ERP profitability reporting
System Engineer, Tata Consultancy Services (Bangalore) · Feb 2021 – Jul 2024

Built 20+ Power BI dashboards digitizing Australian bank DDO compliance (ASIC target-market tracking)
Redesigned liquidity-rerun ETL pipelines, saving $75K a year; automated file generation cutting manual effort by 70%
Built automated ELT pipelines for Basel III liquidity reporting, supporting APRA compliance 1.5 months early
Led a team of 2 and delivered 10 days ahead of schedule · TCS Star Performer
Executive Electrical Engineer, MRF Tyres (Hyderabad) · Nov 2020 – Feb 2021

Value-chain analysis of shop-floor productivity and plant operations
Client work above is confidential, so there is no public code for it. Project write-ups cover approach and outcomes only.

🎓 Education
MBA (PGPEx)	IIM Mumbai	2027
B.Tech, Electrical & Electronics	Cochin University of Science and Technology	9.46 / 10, 2020
🏆 Achievements & Certifications
GATE 2020 qualified (EEE) · Tata Crucible Campus Hackathon 2018, South Zone finalist
2× Deloitte Spot Award (automated data migration; UAT platform) · TCS Star Performer
Lean Six Sigma Green Belt (KPMG) · Modernizing Data Lakes & Warehouses with Google Cloud · Power BI (Udemy) · Product Management Essentials & AI for Business (Coursera)

------------------------------xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx----------------------------------

Substrate → Packaging → Facility Knowledge Graph

An interactive, sourced and weighted knowledge graph with a multi-agent simulation of semiconductor substrate supply risk, built as part of my IIM Mumbai capstone on Intel (June 2026).

🔗 Live demo: https://github.com/chetanraj331-hub/Profile/blob/main/substrate_agent_graph_v2.html

Problem

Advanced packaging for AI and client chips depends on a few chokepoints, such as ABF film, FCBGA substrate makers and a small set of facilities. It is hard to see how a price hike, a capacity expansion or geopolitical risk at one layer moves risk elsewhere in the chain.

What it does
Maps the chain: raw materials → substrate suppliers → packaging tech (EMIB, EMIB-T, Foveros) → facilities (state/country) → processors → end use
Overlays PESTEL factors on the chain
~50 nodes and ~100 relationships; node size and shape show the current weight tier (normal / elevated / high / critical)
33 cited sources; every node carries a confidence tag (high / medium / estimate) and a business-impact note
Agents tab: toggle simulated agents (Supply Concentration, Cost & Pricing, Capacity & Investment) and recompute weights
Live AI tab: optional Gemini call with Google Search grounding, running in the browser (your key stays in memory and is never saved)
Manual override: click a node and drag its weight slider
My role

Designed the model, collected and cited the sources, defined the agent logic and weighting, and built the D3 visualization. The output feeds prioritized capacity-planning recommendations.

Tech

JavaScript, D3.js v7, Gemini API (optional). A single self-contained index.html.

Run locally

Open index.html in a browser. No build step.

Notes and limits

The agent snapshots are static, dated and sourced. They are not a live scraper. Some inputs come from single blog sources and are marked with lower confidence.
