# AIDO Multi-Omics I 5.0

**Research repository — Informatics and Health major-revision work in progress (29 October 2026).**

This repository documents a modular biological-process analysis of breast-cancer multi-omics observations. The manuscript describes TCGA-BRCA discovery, MSigDB Hallmark observation-readiness and endpoint-informed process selection, followed by curated cancer-gene and STRING network evidence and exploratory survival analyses. **This repository is not yet an independently executable reproduction package.** No source scripts, raw cohort data, locked models, or patient-level tables have been committed in this initial documentation-only revision.

## Scientific evidence boundaries

- **Discovery and multiplicity:** 50 Hallmark processes were evaluated against overall survival and stage (100 process–endpoint tests). The selected 20 processes were ranked by maximum nominal `D = −log10(p)`. Joint Benjamini–Hochberg adjustment retained only two OS process–endpoint tests at `q < 0.05`; selection is outcome-informed.
- **Original 20-process D-weighted score:** Process selection, weighting and risk-direction construction reused TCGA outcome information. Survival separation in the same TCGA cohort (`n = 518`, 64 OS events) is exploratory, **not held-out prognostic validation**. Historical bootstrap median HR `11.05` conflicts with a recovered 300-replicate summary median `10.1481` (empirical percentiles `3.02597–37.05408`); the original model contrast and replicate-level lineage remain unresolved.
- **Distinct GE-only out-of-fold sensitivity:** Five-fold TCGA analysis yielded C-index `0.551`, conditional bootstrap interval `0.459–0.658` (`n = 518`, 64 OS events). Upstream full-cohort expression normalization means this is **not** asserted to be completely preprocessing-isolated or a nested revalidation of the original D-weighted model.
- **Distinct frozen GE-only METABRIC comparator:** C-index `0.473`; continuous-score HR `1.039` (95% CI `0.763–1.415`, `p = 0.808`; `n = 1,979`, 1,143 events). Its frozen high-risk cutoff assigned **zero** high-risk patients, so a binary Kaplan–Meier comparison and binary HR are not estimable. These results concern the five-process GE-only comparator, **not** the historical 20-process D-weighted model.
- **Historical D-weighted METABRIC analysis:** Original patient-level scores and fully frozen-model transfer have not been independently reconstructed. Historical median-group counts `989 + 991 = 1,980` disagree with stated `n = 1,979`; tertile counts also sum to 1,980. Historical external significance must not be treated as verified fixed-score external validation.
- **TCGA harmonization:** Historical GE+CN+clinical sample counts differ (`1,073` in narrative versus `1,078` in an archived table/figure), pending unique-patient source reconciliation.
- **Multi-omics incremental value:** A leakage-safe, matched, fully nested GE-only versus GE+CN+MU ablation has **not** established additional prognostic value from CN/MU.

## Scope and availability

The contribution under revision is **auditable organization of biological-process and supporting molecular/biological evidence**. Clinical prognostic deployment, independent validation of the original integrated score, and reproducible fixed-score transfer are **not established**.

The manuscript, Supplementary Information, point-by-point reviewer responses, and figure reconstructions are undergoing quality and provenance review. They are **not represented as a released, submission-approved package** here. Public TCGA-BRCA, METABRIC, GSE96058, MSigDB, curated cancer-gene, and STRING resources have their own provenance and usage requirements. No redistribution of protected or non-redistributable source datasets is implied.

**Reproducibility status:** Documentation only / source-and-version reconciliation ongoing. Exact dataset releases, joins and exclusions, mappings, environment dependencies, fold splits, pretrained objects, historical bootstrap details and complete original D-weighted external-score replay remain to be certified. Do not interpret this README as evidence that raw analyses have been independently rerun.

## Major revision status

- Manuscript: *A modular biological-process multi-omics framework for cancer-gene- and network-anchored breast cancer survival stratification*
- Journal: *Informatics and Health*
- Manuscript ID: `INFOH-D-26-00138`
- Revision deadline: **8 November 2026**
- Status (29 October 2026): **Scientific revision in progress; submission authorization pending**

This page records evidence limits transparently; it does not replace the submitted manuscript, journal correspondence or source-level verification.
