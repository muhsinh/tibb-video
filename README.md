# Scenic Constraint Benchmark (No Humans / No Animals)

You want a quick, auditable benchmark of T2I/T2V models under strict constraints:
- NO humans (even silhouettes)
- NO animals (even tiny birds)
- NO text/logos/watermarks (unless you plan to crop/regenerate)

## Folder Guide
- 01_raw/        All outputs (images/videos). Keep everything.
- 02_top_picks/  Only compliant, best-scoring outputs.
- 03_fail/       Hard fails (humans/animals/text/etc.).
- 04_notes_scores/  Settings screenshots + notes.

## Files
- prompts.md     Prompt pack and scene list
- models.md      Model inventory + what to record (licensing flags as UNKNOWN until verified)
- scorecard.csv  One row per output (scores + pass/fail + notes)
- runlog.md      Free-form notes, weird failures, UI settings

## Naming Convention
MODALITY_MODEL_SCENE_PROMPTv##_RUN##_YYYYMMDD.ext

Examples:
- T2I_FLUX1_S2_Promptv01_RUN01_20260204.png
- T2V_LumaRay314_S4_Promptv02_RUN02_20260204.mp4
