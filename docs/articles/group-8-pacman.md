---
layout: article
title: Pac-Man Pathfinding with A*
hero_title: Pac-Man Pathfinding with A*
hero_lead: "Group 8 adapts A* and BFS to guide Pac-Man through maze environments while collecting food efficiently."
hero_badge: Issue 1 · GLMR
hero_subtitle: Searching Strategy and Its Application
group: "Group 8"
authors:
  - "Nguyen Quang Huy"
  - "Nguyen Tuan Anh"
  - "Nguyen Xuan Kiet"
  - "Tran Minh Hoang"
  - "Vu Quoc Huy"
instructor: "Nguyen Trong Nghia"
presentation_score: 8.0
report_score: 8.0
weighted_score: 8.00
tags:
  - "Game AI"
  - "A* Search"
  - "Heuristic Design"
pdf_read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%208%20topic%204/Group%208%20report.pdf"
pdf_download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%208%20topic%204/Group%208%20report.pdf"
presentation_links:
  - label: "Presentation Deck"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Group%208's%20Presentation_.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Group%208's%20Presentation_.pdf"
highlights:
  - "Integrates heuristic tuning within the classic Pac-Man environment for real-time decision making."
  - "Contrasts BFS baseline with A* to highlight improvements in path optimality and responsiveness."
  - "Discusses extensions for multi-goal search and obstacle handling."
feedback_positive:
  - "Slides were clear, motivating, and visually engaging."
  - "Demonstrated coherent linkage between algorithm design and gameplay."
feedback_focus:
  - "Trim nonessential sections and provide deeper commentary when presenting code."
  - "Consider tightening reasoning flow to stay within allotted time."
---

### Abstract
The project adapts the Pac-Man maze to evaluate how informed search strategies outperform uninformed traversal when collecting distributed food pellets. The authors focus on maintainable heuristics that keep gameplay brisk without sacrificing completeness.

### Methodology Snapshot
- **Maze model:** Pac-Man grid converted into weighted graph where nodes represent positions and costs reflect movement.
- **BFS baseline:** Ensures reachability assessments and establishes a comparison point for path length.
- **A* search:** Employs Manhattan distance to remaining pellets, extending to multi-goal contexts to minimize total travel.
- **Obstacle handling:** Discusses trap avoidance and cost penalties for dangerous tiles.

### Results & Discussion
A* significantly reduces total steps compared with BFS, especially in larger mazes where heuristic guidance prevents redundant exploration. The team outlines future enhancements such as integrating heuristics from ghost prediction or dynamic pellet prioritization.

### Resources & Further Reading
- Report delves into heuristic formulation and code snippets implementing the algorithms.  
- Slide deck provides animations and interface mockups for the Pac-Man agent.
