# Original research recovery ledger

**Status: PARTIAL SOURCE-ARTIFACT RECOVERY — 2026-10-29**

The repository previously contained research content that was subsequently removed. Its visible GitHub history currently begins with a documentation-only commit on 2026-10-29; this is **not** proof that earlier research never existed. This ledger records positively located legacy study artifacts in the PI's private Google Drive. It does **not** claim recovered executable original source code.

## Located original results (private Drive, not redistributed)

| Workflow | Located source artifact | Recoverability |
|---|---|---|
| M3 discovery | `M3_GE_D_scores_by_endpoint_after_AIDO_h.csv` | Original endpoint-discriminability result table located |
| M3 discovery | `M3_highD_BP_panel_top_demo_after_AIDO_h.csv` | Original selected-panel table located |
| M12 survival | `M12_OS_D_weighted_risk_aligned_BP_burden_PASS_OS_median_groups.csv` | Patient-level TCGA score, survival time, event, median group located |
| M12 survival | `M12_OS_D_weighted_risk_aligned_BP_burden_PASS_OS_tertile_groups.csv` | Corresponding tertile groups located |
| M12 survival | `M12_patient_profiles_with_clinical_and_enhanced_burden.csv` | Historical mechanism/burden and clinical profile data located |
| M12 statistics | `M12_preferred_manuscript_candidate_tests.csv`, `M12_patient_level_statistical_validation_summary.csv`, `M12_bootstrap_HR_stability.csv` | Historical statistical summaries located |
| M12 figure outputs | `M12plus_KM_OS_D_weighted_risk_aligned_BP_burden_PASS_median_OS.png`, `M12plus_KM_OS_D_weighted_risk_aligned_BP_burden_PASS_tertiles_OS.png` | Original figure images located |

Source folders in Drive: `M3_GE_highD_selection` and `M12_patient_level_statistical_validation`. Their raw outputs remain private; this ledger does not grant a license or authorization to republish patient-level files.

## Patient-level checks already performed

For the located TCGA M12 PASS median and tertile CSVs, the same 518 patient IDs and the same survival times/event indicators were found in both sources. The total was 64 OS events. Median groups: low 259 patients / 18 events, high 259 / 46 events. Tertile groups: low 174 / 13 events, middle 171 / 14, high 173 / 37. These support source-bound reconstruction of those descriptive KM plots and censor/risk-table calculations; they do not remove original outcome-selection leakage.

## Not recovered or not independently certified

- Original executable M3/M12 preprocessing, selection and model-fitting source scripts; exact dependencies and run environment.
- Historical original 20-process D-weighted frozen METABRIC patient-level score export and fully locked transfer pipeline.
- Original 300-replicate Cox bootstrap coefficient series, source contrast and complete resampling code; historical medians 11.05 and 10.1481 remain discordant.
- Fully resolved TCGA GE+CN+clinical 1,073-versus-1,078 matching lineage.
- Leakage-safe nested GE+CN+MU versus matched GE-only model ablation.

## Recovery protocol

Reconstruct the archive from the **original** backed-up scripts and dependency manifests if found. Preserve paths, execution provenance and content hashes, and do not fabricate source files using descriptions of past outputs. Before publishing any underlying dataset, verify distribution rights and remove personally sensitive or nonredistributable material. Distinguish source-artifact recovery, executable reproducibility and scientific validation as three separate milestones.

**Current conclusion:** Original study result artifacts have been located in private Drive; original execution code has **not** yet been recovered or restored to this GitHub repository.
