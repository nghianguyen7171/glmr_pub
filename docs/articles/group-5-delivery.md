---
layout: article
title: Urban Delivery with Classical Search Heuristics
hero_title: Urban Delivery with Classical Search Heuristics
hero_lead: "Group 5 prototypes a Hanoi delivery planner by contrasting BFS, Greedy, and A* across real map segments."
hero_badge: Issue 1 · GLMR
hero_subtitle: Searching Strategy and Its Application
group: "Group 5"
authors:
  - "Tran Tuan Anh"
  - "Hoang Thi Ngoc Han"
  - "Nguyen Phung Hoa"
  - "Nguyen Hoang Tuan"
instructor: "Nguyen Trong Nghia"
presentation_score: 7.0
report_score: 6.8
weighted_score: 6.88
tags:
  - "Last-mile Delivery"
  - "Greedy Search"
  - "A* Search"
pdf_read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%205%20topic%201/Introduction_to_AI.pdf"
pdf_download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%205%20topic%201/Introduction_to_AI.pdf"
presentation_links:
  - label: "Presentation Deck"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Nho%CC%81m%205.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Nho%CC%81m%205.pdf"
highlights:
  - "Structures the delivery problem as weighted graph traversal with admissible heuristics for A*."
  - "Compares path optimality, search depth, and runtime across representative districts."
  - "Discusses integration of heuristic routing into smart city logistics."
feedback_positive:
  - "Problem stays grounded in realistic delivery challenges and ties back to smart-city scenarios."
  - "Clear definition of algorithms and reference to practical applications."
feedback_focus:
  - "Slides should condense theory-heavy sections and tighten time management."
  - "Report would benefit from deeper comparative evaluation tables and conclusions."
---

### Abstract
Positioning delivery logistics as a path-search problem, the authors explore how classical AI algorithms support route optimization when real-time traffic data is limited. The project underscores the role of admissible heuristics in balancing efficiency with solution quality.

### Methodology Snapshot
- **Graph modeling:** Major roads mapped as nodes and edges with travel costs reflecting distance and conditions.
- **Algorithm comparison:** BFS verifies shortest paths in unweighted contexts, Greedy accelerates dispatch through heuristic choices, and A* blends both approaches for optimal results.
- **Evaluation:** Focused case studies demonstrate improvements in fuel usage and travel time when heuristics are tuned to the urban grid.

### Results & Discussion
A* consistently outperforms Greedy by avoiding detours, while Greedy remains appealing for low-latency decisions. BFS serves as a baseline but scales poorly. The report encourages combining A* with higher-level meta-heuristics to handle multi-stop itineraries.

### Resources & Further Reading
- Annotated pseudo-code and comparative charts live in the linked PDF.  
- Slide deck highlights visual explanations of BFS, Greedy, and A* traversal.
