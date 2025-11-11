---
layout: article
permalink: /articles/group-6-maze-pathfinding.html
title: Maze Pathfinding for Emergency Evacuation
hero_title: Maze Pathfinding for Emergency Evacuation
hero_lead: "Group 6 stress-tests BFS, DFS, and Greedy Best-First Search across 100 randomized mazes to inform evacuation design."
hero_badge: Issue 1 · GLMR
hero_subtitle: Searching Strategy and Its Application
group: "Group 6"
authors:
  - "Mai Huy Dang"
  - "Mai Tuan Manh"
  - "Nguyen Huy Minh"
instructor: "Nguyen Trong Nghia"
presentation_score: 9.0
report_score: 9.2
weighted_score: 9.12
tags:
  - "Maze Search"
  - "BFS"
  - "GBFS"
pdf_read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%206%20Topic%206/Group%206%20report.pdf"
pdf_download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%206%20Topic%206/Group%206%20report.pdf"
presentation_links:
  - label: "Presentation Deck"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/midtermAI_gr6_presentation.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/midtermAI_gr6_presentation.pdf"
highlights:
  - "Generates 100 mazes per size to benchmark average runtime, memory, and path optimality."
  - "Examines trade-offs between optimal BFS routes and heuristic-driven speed via GBFS."
  - "Extends findings to crowd evacuation simulations for large venues."
feedback_positive:
  - "Clear motivation, literature framing, and clinically inspired implications."
  - "Benchmarked BM function and analysis impressed reviewers."
feedback_focus:
  - "Include additional metrics such as iteration counts in future BM function discussions."
  - "Provide consolidated comparison tables on slides for quicker digestion."
---

### Abstract
This report evaluates classical search strategies for guiding evacuees through complex environments. By simulating mazes representing venues of increasing scale, the authors quantify how BFS, DFS, and GBFS balance optimality and response time under pressure.

### Methodology Snapshot
- **Maze generation:** DFS backtracking constructs perfect mazes before selective wall removal introduces realistic loops and multiple exits.
- **Algorithm toolkit:** BFS ensures optimal escape routes, DFS explores deeply with minimal overhead, and GBFS harnesses Manhattan-distance heuristics for speed. 
- **Benchmarking:** Each algorithm runs across 5×5, 7×7, 51×51, and 201×201 mazes, repeated 100 times to smooth variance.
- **Metrics:** Average runtime, peak memory, and path length recorded to evaluate scalability.

### Results & Discussion
BFS delivers optimal paths but incurs mounting memory in large grids. GBFS approaches optimality while cutting runtime and memory, making it suitable for real-time evacuation guidance. DFS proves unpredictable at scale, reinforcing the need for heuristic assistance. The team proposes hybrid strategies merging A* with agent-based simulations for future work.

### Resources & Further Reading
- Report appendices detail the benchmarking harness and statistical summaries.  
- Slides visualize maze instances and evacuation flows for stakeholders.
