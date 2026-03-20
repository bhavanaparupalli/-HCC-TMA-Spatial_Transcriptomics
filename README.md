#README — CosMx 1K TMA Ligand-Receptor Preliminary Analysis

Date: March 19, 2026
Analyst: Bhavana Parupalli
Dataset: hcc_tmas_final.RDS — HCC CosMx 1K TMA, 23 patients
Location:- /gpfs/data/franses-lab/Cosmx/1k/1k_whole_tma/RDS/

Analysis Description:
Patients were stratified into High and Low groups based on mean gene expression per patient. Cell type composition was compared between High and Low groups. Spearman correlation was used to test ligand-receptor relationships.

Figures Generated:

1. LGALS9_grant.pdf — LGALS9 tumor expression, High vs Low patients + cell composition
2. JAG1_grant.pdf - JAG1 tumor expression, High vs Low patients + cell composition
3. NOTCH1_final7.pdf - NOTCH1 endothelial expression, High vs Low patients + cell composition
4. NOTCH3_final.pdf - NOTCH3 endothelial expression, High vs Low patients + cell composition
5. JAG1_NOTCH1_clean.pdf - JAG1 tumor vs NOTCH1 endothelial side by side + cell composition
6. JAG1_NOTCH3_clean.pdf - JAG1 tumor vs NOTCH3 endothelial side by side + cell composition
7. LR_pairs_summary.pdf - Spearman correlation scatter plots for LGALS9-HAVCR2, IGF1-IGF1R, TNFSF14-LTBR

Key Results:

| LR Pair | rho | p-value |
|---------|-----|---------|
| LGALS9 - HAVCR2 (CD8 T cells) | 0.26 | 0.27 |
| IGF1 - IGF1R | 0.15 | 0.49 |
| TNFSF14 - LTBR | -0.09 | 0.67 |
| JAG1 - NOTCH1 (endothelial) | 0.26 | 0.24 |
| JAG1 - NOTCH3 (endothelial) | 0.17 | 0.45 |

Genes Not in CosMx 1K Panel:
- ANGPTL4 (from ANGPTL4-CDH5 pair)
- EFNA2 (from EFNA2-EPHA2 pair)

Next Steps:
Run COMMOT spatial LR analysis at single-cell level with distance weighting for more powerful spatial detection of these interactions.

