# OV-CIL-PCB Research

PhD research repository: **Open-Vocabulary Continual Learning Framework for Domain-Adaptive PCB Defect Detection**

## Contents

| Path | Description |
|---|---|
| `docs/OV_CIL_PCB_v2_Study_Guide.docx` | Framework v2 architecture design and annotated research reference guide (Aug 2026). Covers the updated 2025-2026 landscape (DitHub, COVD, ODOV), gap analysis, LoRA module library design, Board-as-Branch domain organisation, NDA-driven unlearning mechanism, migration plan, benchmark strategy, publication plan, and a 17-entry annotated reading list. |

## Key concepts (v2 framework)

- **Base model:** YOLOE-26s (CNN backbone, open-vocabulary embedding head, real-time edge deployment)
- **Adaptation:** LoRA module library, one module per **board design** (domain-incremental)
- **Privacy stack:** input-side masking (barcodes / QR / logos / serial numbers) + output-side **module-level unlearning** (W' = W - a*BA) for NDA compliance
- **Pipeline:** zero-shot -> few-shot -> full continual learning, plus unlearning as the symmetric removal operation

## Tier-1 reading (before next semester)

1. DitHub — arXiv:2503.09271 (NeurIPS 2025)
2. COVD — arXiv:2605.27116 (2026)
3. ODOV benchmark — CVPR 2026
4. LoRA — arXiv:2106.09685 (ICLR 2022)
5. YOLOE — arXiv:2503.07465 (2025)

Full annotated list with study notes guidance is in the study guide, Section 10.
