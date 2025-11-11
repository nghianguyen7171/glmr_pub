---
layout: article
title: Optimizing Multi-Agent Path Finding in Warehouses
hero_title: Optimizing Multi-Agent Path Finding in Warehouses
hero_lead: "Group 4 dissects BFS, independent A*, and Joint A* to orchestrate collision-free robot navigation."
hero_badge: Issue 1 · GLMR
hero_subtitle: Searching Strategy and Its Application
group: "Group 4"
authors:
  - "Dao Ngoc Hien"
  - "Nguyen Thi Nhien"
  - "Le Ngoc Anh Thu"
  - "Tran Khai Van"
presentation_score: 7.0
report_score: 9.3
weighted_score: 8.38
tags:
  - "Multi-Agent Pathfinding"
  - "Joint A*"
  - "Warehouse Automation"
pdf_read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%204%20topic%2016/Group4_report.pdf"
pdf_download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%204%20topic%2016/Group4_report.pdf"
presentation_links:
  - label: "Presentation Deck"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/nh%C3%B3m%204%20-%20topic%2016.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/nh%C3%B3m%204%20-%20topic%2016.pdf"
highlights:
  - "Derives makespan-focused heuristics to guide Joint A* in a 10×10 warehouse grid."
  - "Analyzes vertex and edge conflicts to prevent collisions across synchronized robot moves."
  - "Reports detailed runtime and expansion statistics for increasing task complexity."
feedback_positive:
  - "Interesting topic selection with well-articulated background and motivation."
  - "Application to real-world coordination problems resonated with reviewers."
feedback_focus:
  - "Slides should showcase richer map visualizations instead of abstract graphs."
  - "Trim dense theoretical text and add spoken explanations for critical functions."
---

### Abstract
The report models two cooperative warehouse robots traversing a shared grid while avoiding mutual collisions. By contrasting classic BFS, independent A*, and Joint A*, the team exposes how coordination strategies impact optimality and computational load.

### Methodology Snapshot
- **State modeling:** Each node encodes both robot positions, incorporating wait actions to synchronize arrivals.
- **Search variants:** BFS establishes baseline optimality, independent A* produces initial single-agent paths, and Joint A* enforces collision constraints during search.
- **Heuristics:** Manhattan and makespan heuristics provide admissible guidance for the composite agent.
- **Benchmark suite:** Multiple scenarios (easy through extreme) report solution depth, expanded nodes, and runtime.

### Results & Discussion
Joint A* balances safety and efficiency, delivering optimal collision-free plans at a fraction of BFS’s state expansions. Independent A* offers quick drafts but requires post-processing to resolve conflicts. The authors recommend Joint A* for tightly coupled spaces, highlighting opportunities for scaling via conflict-based search in future work.

### Resources & Further Reading
- Alternate presentation deck available via Issue 1 for extended visuals.  
- Appendix enumerates Python implementations and scenario maps.
