# Figures

Every figure in the paper and appendices, named in reading order. Each entry lists what the figure
shows and the script that produces it. Filenames are prefixed so they sort in the order the paper
uses them.

> The scripts named below belong to the analysis pipeline, which will be released as a replication
> package with the journal version of the paper. They are not part of this public repository yet.

## Body figures (in the paper)

| File | Paper | Shows | Produced by |
|---|---|---|---|
| `figure_01_modularity_trend.png` | Figure 1 | Quarterly whole-chamber modularity, with the crisis window and the detected change-points | `04_analysis/72_modularity_qstar.R`, `20_changepoint_detection.R` |
| `figure_02_reelected_crossing.png` | Figure 2 | Community-crossing rates among reelected deputies, by transition | `04_analysis/18_within_deputy_fe_reeleitos.R` |
| `figure_03_falsification_panel.png` | Figure 3 | Falsification panel: within-55L phase split, permutation-corrected Q\*, and the null dose-response | `04_analysis/90_figure_options.R` (composed from `28`, `72`, `40`) |
| `figure_04_community_alluvial.png` | Figure 4 | Party paths across coordinating communities over time (PT, PMDB, Centrão) | `04_analysis/34_test17_community_composition.R`, `35_test18_centrao_stability.R` |
| `figure_05_centrao_concentration_continuity.png` | Figure 5 | Centrão concentration and dyad-continuity, dated membership scheme | `04_analysis/35_test18_centrao_stability.R`, `46_centrao_canonical_rerun.R` |
| `figure_06_pivot_membership.png` | Figure 6 | Share of each party in the largest coordinating community, 52L to 57L | `04_analysis/43_pivotality.R`, `73_largest_community_validation.R` |
| `figure_07_decisiveness_migration.png` | Figure 7 | Vote-level decisiveness on competitive roll-calls, net of the president's party | `04_analysis/54_decisiveness_presidente.R`, `69_pivotal_votes_ex_pres.R` |

## Appendix figures

| File | Appendix | Shows | Produced by |
|---|---|---|---|
| `figure_B1_subject_placebo.png` | Figure B1 | Subject-matter placebo: crossing by domain at the 54L to 55L break | `04_analysis/22_materia_placebo_3way.R` |
| `figure_F1_thresholds.png` | Figure F1 | Crossing under the twelve-cell grid of edge and shared-vote thresholds | `04_analysis/24_robustness_thresholds.R` |
| `figure_F2_weighting.png` | Figure F2 | Crossing under alternative projection weightings (Jaccard, resource-allocation, Newman) | `04_analysis/36_robustness_weighting.R` |
| `figure_F3_algorithms.png` | Figure F3 | Crossing and label-free ARI/NMI across four community-detection algorithms | `04_analysis/37_robustness_algorithm.R` |
| `figure_F4_centrao_sensitivity.png` | Figure F4 | Centrão concentration and continuity under six membership schemes | `04_analysis/38_centrao_classification_sensitivity.R` |
| `figure_G1_community_heatmap.png` | Figure G1 | Community composition heatmap (companion to Figure 4) | `04_analysis/34_test17_community_composition.R` |
| `figure_G2_pivot_heatmap.png` | Figure G2 | Largest-community membership heatmap (companion to Figure 6) | `04_analysis/43_pivotality.R` |

## Notes

- Figures are referenced from `paper/paper.md` and `paper/appendices.md` with relative paths
  (`../figures/...`), so the paper renders correctly from within this repository.
- To regenerate a figure, run its script from the project root after the pipeline has produced the
  derived data it reads. See `../scripts/README.md`.
