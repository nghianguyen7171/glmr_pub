---
layout: article
permalink: /articles/group-2-waste-routing.html
title: Optimal Waste Collection Routing
hero_title: Optimal Waste Collection Routing
hero_lead: "Group 2 elevates municipal waste logistics by benchmarking UCS, Greedy, and A* search with realistic street data."
hero_badge: Issue 1 · GLMR
hero_subtitle: Searching Strategy and Its Application
group: "Group 2"
authors:
  - "Pham Huu Gia An"
  - "Nguyen Ngan An"
  - "Nguyen Trong Dai"
  - "Le Ba Phong"
instructor: "PhD. Nguyen Trong Nghia"
presentation_score: 7.0
report_score: 9.0
weighted_score: 8.20
tags:
  - "Vehicle Routing"
  - "A* Search"
  - "Heuristic Design"
pdf_read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%202/Thu_Gom_Rac_Toi_Uu-1.pdf"
pdf_download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%202/Thu_Gom_Rac_Toi_Uu-1.pdf"
presentation_links:
  - label: "Presentation Deck"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Midterm_Group_2.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Midterm_Group_2.pdf"
highlights:
  - "Models municipal waste pickup as a Traveling Salesman variant with state compression for efficient search."
  - "Introduces MST- and assignment-based heuristics to accelerate A* while maintaining optimality."
  - "Supplies comprehensive runtime, cost, and node-expansion tables across route sizes."
feedback_positive:
  - "Technical depth is strong with clear problem framing and engaging experimentation."
  - "Visualization of datasets and classification by scenario were especially effective."
feedback_focus:
  - "Future slides should resolve Vietnamese typos and swap abstract node labels for real street names."
  - "Bridge the gap between theory and application by emphasizing practical heuristics within the report."
---

### Abstract
The study analyzes how classical search algorithms scale when dispatching a single waste-collection vehicle across Hanoi’s dense street network. By iteratively increasing the number of pickup points, the authors quantify the trade-offs between completeness, optimality, and compute cost.

### Methodology Snapshot
- **State encoding:** Uses `(current_city, visited_cities)` tuples to capture route progress, enabling memoization across search branches.
- **Search portfolio:** Compares Uniform Cost Search, Greedy Best-First Search with nearest-neighbour heuristics, and A* powered by MST lower bounds.
- **Scenario sweep:** Evaluations span tours visiting 2–12 bins, with each algorithm measured for cost, execution time, and expanded states.
- **Heuristic innovation:** Assignment (Hungarian) and 1-tree bounds serve as admissible estimates that sharpen A* performance.

### Results & Discussion
A* maintained optimal tours with far fewer expansions than UCS, proving scalable up to 12-bin tours before factorial growth became prohibitive. Greedy produced rapid but suboptimal loops, hinting at its usefulness for real-time replanning when optimality can be relaxed. The report concludes with recommendations for hybrid deployments that combine fast heuristics with occasional optimal recalibration.

### Resources & Further Reading
- Report appendix details the Python implementations for MST and assignment heuristics.  
- Slide deck showcases performance plots for each algorithm across varying tour lengths.

### Related Presentations
- [Return to Issue 1](../issue-1.html)
- [Scoring Summary Entry](../scoring-summary.html)
