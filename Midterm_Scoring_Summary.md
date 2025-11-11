# Midterm Scoring Summary

## Methodology
- Converted presentation `rank` values from `presentation_raking.csv` to a 10-point scale (1 → 9, 2 → 8, 3 → 7). Blank ranks were treated as 8.
- Combined presentation scores with report evaluations (0–10 scale) using weights: 60% report + 40% presentation.
- Evaluated reports available for Groups 1–8 in `Midterm_AI_Project`; Groups 9 and 10 did not submit reports and are excluded.

## Overall Results

| Group | Topic | Presentation Score | Report Score | Weighted Total | Highlights |
|-------|-------|--------------------|--------------|----------------|------------|
| 6 | Thoát khỏi mê cung | 9.0 | 9.2 | **9.12** | Extensive benchmarking across 100 randomized mazes per size with runtime, memory, and path-length metrics supporting evacuation insights. |
| 1 | Tìm đường đi an toàn khi có sự cố giao thông | 8.0 | 9.1 | **8.66** | Dynamic incident simulations with blocked-edge scenarios and comparative analysis showing A* robustness. |
| 4 | Tìm đường đi cho 2 robots không va chạm | 7.0 | 9.3 | 8.38 | Detailed joint-state modeling and comparison of BFS, independent A*, and Joint A*. |
| 2 | Thu gom rác tối ưu | 7.0 | 9.0 | 8.20 | Strong TSP formulation, MST-based heuristic analysis, and comprehensive experiments. |
| 7 | Kế hoạch tham quan Hà Nội trong 1 ngày | 7.0 | 8.7 | 8.02 | Clear problem framing, data visualization, and discussion of real-world applicability. |
| 8 | Game Pac-Man tìm thức ăn | 8.0 | 8.0 | 8.00 | Solid A* walkthrough with BFS comparison; presentation praised for structure though long. |
| 3 | Giải toán N-Queens | 8.0 | 7.3 | 7.58 | Algorithms explained with DFS/Hill-Climbing/Beam Search; report missing some quantitative metrics. |
| 5 | Giao hàng trong thành phố Hà Nội | 7.0 | 6.8 | 6.88 | Report still high-level with placeholders; needs fuller comparative evaluation. |

## Top 2 Reports

### 1. Group 6 – Maze Pathfinding
- Report: Detailed experiments across multiple maze sizes with 100-run averages for runtime, memory, and path optimality.
- Presentation: Praised for strong motivation and clear literature review; minor request to add explicit cost metrics for the BM function.

### 2. Group 1 – Safe Routing Under Incidents
- Report: Comprehensive workflow, randomized blocked-edge simulations, and comparative evaluation of Greedy vs. A* under dynamic constraints.
- Presentation: Highlighted for real-world relevance, intensive experiments, and clear motivation; recommended to add workflow visualizations and code explanations.

## Notes on Other Groups
- **Group 4**: Joint A* work is excellent; presentation should better connect theory to concrete warehouse scenarios.
- **Group 2**: Technically strong, but slides would benefit from consistent labeling of geographic nodes.
- **Group 8**: Add quantitative comparisons to support narrative claims about A* performance.
- **Group 5**: Prioritize completing experiments and comparative analysis in the report.

## Recommended Follow-ups
- Share this summary with students and emphasize feedback for the top teams.
- Encourage Groups 4 and 2 to tighten application-story alignment in final deliverables.
- Check in with Groups 5 and 3 on expanding experimental evidence if required for final grading.
