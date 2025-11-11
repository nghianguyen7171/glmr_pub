---
layout: article
permalink: /articles/group-3-nqueens.html
title: Applying AI Search Algorithms to Solve the N-Queens Problem
hero_title: Applying AI Search Algorithms to Solve the N-Queens Problem
hero_lead: "Group 3 benchmarks DFS, Hill-Climbing, and Beam Search to illuminate search trade-offs in the iconic N-Queens puzzle."
hero_badge: Issue 1 · GLMR
hero_subtitle: Searching Strategy and Its Application
group: "Group 3"
authors:
  - "Group 3 Team"
instructor: "PhD. Nguyen Trong Nghia"
presentation_score: 8.0
report_score: 7.3
weighted_score: 7.58
tags:
  - "Constraint Search"
  - "Hill-Climbing"
  - "Beam Search"
pdf_read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%203%20Topic%208/AI-report.pdf"
pdf_download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%203%20Topic%208/AI-report.pdf"
presentation_links:
  - label: "Presentation Deck"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/GROUP%203%20-%20Applying%20AI%20search%20algorithms%20to%20solve%20the%20N-Queens%20problem.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/GROUP%203%20-%20Applying%20AI%20search%20algorithms%20to%20solve%20the%20N-Queens%20problem.pdf"
highlights:
  - "Frames N-Queens as a watchtower placement challenge to motivate real-world relevance."
  - "Contrasts solution completeness versus speed by juxtaposing DFS backtracking with local search methods."
  - "Provides pseudo-code and experimental logs for varying board sizes."
feedback_positive:
  - "Explanation of algorithms was clear with intuitive illustrations."
  - "Experimental design and comparative discussion were well-received."
feedback_focus:
  - "Report and presentation leaned heavily into theory; more metrics are encouraged."
  - "Allocate time to build motivation and empirical depth during the talk."
---

### Abstract
Leveraging the N-Queens problem as a benchmark, the team explores how classical search techniques behave under escalating complexity. DFS ensures completeness, Hill-Climbing emphasizes speed with local refinements, and Beam Search offers a balanced heuristic approach.

### Methodology Snapshot
- **State representation:** Arrays encapsulate queen placements, simplifying conflict detection across rows and diagonals.
- **Algorithm suite:** DFS backtracking enumerates full solution sets, Hill-Climbing performs steepest ascent with random restarts, and Beam Search prunes to the top-k successors each depth.
- **Evaluation metrics:** Success rate, explored states, and runtime measured across boards of size 4, 6, and 8.
- **Heuristic design:** Conflict-count heuristics inform both hill-climbing moves and beam prioritization.

### Results & Discussion
DFS reliably delivers all valid configurations but its exponential explosion becomes apparent beyond N=8. Hill-Climbing excels on small boards yet stalls in local optima without restarts. Beam Search mediates between both extremes, offering faster convergence at the expense of completeness. The authors recommend combining DFS for verification with heuristic methods for rapid candidate generation.

### Resources & Further Reading
- Report appendices include pseudocode listings for each algorithm.  
- Slides distill algorithm intuition with animated board traces.
