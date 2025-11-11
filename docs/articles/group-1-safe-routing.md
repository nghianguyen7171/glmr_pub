---
layout: article
title: Safe Routing Under Traffic Incidents
hero_title: Safe Routing Under Traffic Incidents
hero_lead: "Group 1 contrasts Greedy and A* search to preserve commuter safety across Hanoi when roads become disrupted."
hero_badge: Issue 1 · GLMR
hero_subtitle: Searching Strategy and Its Application
group: "Group 1"
authors:
  - "Nguyen Thuy Quynh"
  - "Nguyen Ho Nhat Minh"
  - "Nguyen Quang Minh"
  - "Le Duc Minh"
instructor: "PhD. Nguyen Trong Nghia"
presentation_score: 8.0
report_score: 9.1
weighted_score: 8.66
tags:
  - "Route Planning"
  - "A* Search"
  - "Greedy Search"
pdf_read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%201%20Topic%204/INTRO_AI%20(1).pdf"
pdf_download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%201%20Topic%204/INTRO_AI%20(1).pdf"
presentation_links:
  - label: "Presentation Deck"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/MIDTERM_GROUP%201.pptx.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/MIDTERM_GROUP%201.pptx.pdf"
highlights:
  - "Implements a blocked-edge simulation engine to stress-test routing resiliency under random incidents."
  - "Benchmarks Greedy against A* with empirical metrics on path optimality, node expansion, and response time."
  - "Translates experimental findings into actionable guidelines for daily commuters navigating Hanoi’s congestion."
feedback_positive:
  - "Applicability is a big strength with intensive experiments rooted in real-world motivation."
  - "Random block generation function and validation strategy were clearly explained."
feedback_focus:
  - "Method section would benefit from richer visualizations of the proposed workflow."
  - "Slide narrative should trim heavy theory text and provide more commentary on code listings."
---

### Abstract
The team frames everyday commuting in Hanoi as a dynamic route-search problem, comparing Greedy and A* algorithms while accounting for disrupted roads. Their system ingests OpenStreetMap data, assigns safety-weighted edges, and simulates random blockages to discover resilient paths that minimize risk.

### Methodology Snapshot
- **Graph preparation:** Coordinates normalized and haversine heuristics computed for each node-to-goal pair.
- **Search engines:** Greedy Best-First Search prioritizes minimal heuristic distance, while A* combines path cost and heuristic to guarantee optimal detours.
- **Scenario testing:** Three levels of incident severity (one, two, or three blocked edges) evaluate adaptability to disruptions.
- **Metrics tracked:** Expanded nodes, travel cost, execution time, and success rate across multiple randomized trials.

### Results & Discussion
A* consistently produced shorter and more reliable paths when congestion shattered the primary route, especially once three adjacent edges were disabled. Greedy, although faster, struggled to recover from misleading heuristics and sometimes failed to find viable alternatives. The authors highlight the trade-off between rapid dispatch decisions and risk-aware routing, positioning A* as the dependable foundation for urban trip planning tools.

### Resources & Further Reading
- Data pipeline, heuristics, and simulation scripts are documented in the linked PDF report.  
- Slides offer a concise visualization of the incident workflow and node expansion comparisons.

### Related Presentations
- [Scoring summary entry](../scoring-summary.html) provides evaluation context and overall ranking.
