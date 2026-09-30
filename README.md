# Photographic Composition as Large Systems

## Abstract

This repository documents an ongoing empirical research program on **photographic composition as a hierarchy of large interacting visual systems**. Instead of beginning with isolated rules such as the rule of thirds, golden ratio, leading lines, or fixed visual weight, the method first decomposes a photograph into large compositional systems, studies the relations among those systems, identifies the system carrying the subject, and only then performs local adjustment of subject reserve, boundaries, crop, compensation, and other compromises.

The project combines real-photo analysis, synthetic pilot experiments, explicit failure logs, and machine-readable research notes. Its main goal is to develop a transferable structural model that can be used by photographers, researchers, computer-vision systems, and language/vision models without repeating the same exploratory path.

**Research keywords:** photographic composition, visual composition, image aesthetics, photography research, large compositional systems, global-local composition, visual balance, subject placement, negative space, visual mass, Gestalt, pictorial organization, image aesthetic assessment, computer vision, multimodal models.

**Public reuse:** textual and machine-readable research content is licensed under CC BY-NC-ND 4.0; see `LICENSE.md`. Media/images are excluded unless explicitly marked.

## Ongoing research notebook / Рабочая база исследования композиции фотографии

**Version:** 0.1  
**Snapshot date:** 2026-09-30  
**Primary language:** Russian, with English keywords for searchability and LLM handoff.

This repository is a compact transfer package for an ongoing empirical investigation of photographic composition. Its purpose is to let another language model, researcher, or future session enter the work near the current state instead of restarting from generic photography rules.

Это не учебник по композиции и не набор «правил хорошей фотографии». Центральная рабочая идея исследования: **сначала анализировать кадр на уровне крупных взаимодействующих систем, затем выполнять более тонкую локальную подстройку и балансировку компромиссов.**

### Read first

1. `START_HERE.md`
2. `CORE_MODEL.md`
3. `TERMINOLOGY.md`
4. `FINDINGS.md`
5. `FAILED_PATHS.md`
6. `PILOT_INDEX.md`
7. `OPEN_QUESTIONS.md`
8. `HOW_TO_CONTINUE_WITH_AN_LLM.md`

For machine ingestion:
- `machine/state.json`
- `machine/principles.json`
- `machine/terminology.json`
- `machine/experiments.jsonl`

A short transfer prompt is in `PROMPT_FOR_OTHER_LLM.txt`.

### Status

This is an **ongoing working theory**, not peer-reviewed science. Statements are explicitly labeled as repeated observation, working principle, pilot-specific result, hypothesis, or rejected/over-simplified path. Do not silently upgrade a hypothesis into a law.

### Important negative instruction

Do **not** reset the discussion to rule of thirds, golden ratio, generic leading-line advice, or generic “visual weight” explanations unless the actual frame requires them. Those frameworks are not the starting point of this research.
