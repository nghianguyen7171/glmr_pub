---
layout: article
permalink: /articles/group-7-tourism.html
title: One-Day Hanoi Tourism Route Planning
hero_title: One-Day Hanoi Tourism Route Planning
hero_lead: "Group 7 blends Greedy and A* search to curate visitor itineraries that respect opening times and travel budgets."
hero_badge: Issue 1 · GLMR
hero_subtitle: Searching Strategy and Its Application
group: "Group 7"
authors:
  - "Nguyen Thanh Lan"
  - "Trinh Duc Thanh"
  - "Vu Ngoc Hai"
  - "Do Quang Trung"
instructor: "Nghia"
presentation_score: 7.0
report_score: 8.7
weighted_score: 8.02
tags:
  - "Itinerary Planning"
  - "Travel Optimization"
  - "A* Search"
pdf_read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%207%20Topic%202/NATIONAL%20ECONOMICS%20UNIVERSITY_FIXING_FINAL.pdf"
pdf_download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_AI_Project/Group%207%20Topic%202/NATIONAL%20ECONOMICS%20UNIVERSITY_FIXING_FINAL.pdf"
presentation_links:
  - label: "Presentation Deck – Part 1"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Gr7_Tour_Part1.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Gr7_Tour_Part1.pdf"
  - label: "Presentation Deck – Part 2"
    read: "https://rawcdn.githack.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Gr7_Tour_Part2.pdf"
    download: "https://raw.githubusercontent.com/nghianguyen7171/glmr_pub/main/Midterm_presentation/Gr7_Tour_Part2.pdf"
highlights:
  - "Constructs a state-space formulation that respects location opening hours and cumulative time budgets."
  - "Leverages admissible heuristics to ensure A* finds maximal-coverage itineraries."
  - "Visualizes route decisions through dashboards that support traveler exploration."
feedback_positive:
  - "Excellent visualization with clear data storytelling and meaningful conclusions."
  - "Problem definition and application motivation were well-delivered."
feedback_focus:
  - "Presentation pacing should be tightened and literature review streamlined."
  - "Consider adding more visuals when explaining algorithms instead of raw code."
---

### Abstract
Aiming to maximize tourist satisfaction during a single day in Hanoi, the authors measure how Greedy and A* search balance travel overhead against attraction coverage. The study demonstrates how search heuristics can personalize itineraries for cultural excursions.

### Methodology Snapshot
- **State representation:** Tracks current location, visited set, and time-of-day to enforce opening-hour constraints.
- **Greedy baseline:** Chooses the closest feasible attraction at each step, minimizing immediate travel time.
- **A* planner:** Employs a heuristic combining remaining attraction count and average visit time to ensure optimal coverage.
- **Scenario testing:** Dataset of seven attractions includes travel matrices, visit durations, and ratings to evaluate different visitor priorities.

### Results & Discussion
Greedy produced fast, intuitive itineraries but occasionally skipped high-value locations. A* validated the Greedy path in this data set yet required substantially more node expansions, highlighting the trade-off between assurance and efficiency. The report advocates for hybrid approaches that display the Greedy plan instantly while A* confirms optimality in the background.

### Resources & Further Reading
- Interactive dashboards and heuristics are documented in the PDF report.  
- Two-part slide deck showcases the visualization system and comparative charts.
