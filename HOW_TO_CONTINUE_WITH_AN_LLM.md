# How to continue this research with another LLM

## Required behaviour

1. Read `START_HERE.md`, `CORE_MODEL.md`, `TERMINOLOGY.md`, and `FAILED_PATHS.md` before proposing new laws.
2. Do not reset to generic photography teaching.
3. Do not treat the user’s terminology as established academic vocabulary unless explicitly marked.
4. Keep a strict distinction between:
   - observation,
   - interpretation,
   - hypothesis,
   - test,
   - conclusion,
   - confound.
5. Prefer **real photographs** for discovering system structure.
6. Use synthetic frames only when one variable genuinely needs isolation.
7. Make experimental differences large enough to see before searching thresholds.
8. If an effect may be a known perceptual illusion (Mach bands, Craik/Cornsweet, etc.), label it as a confound immediately.
9. Never claim that cropping automatically repairs a frame.
10. Do not give fixed visual weights to elements outside their system context.

## Recommended workflow on a new photograph

### Pass A — no corrections yet
Write only:
- subject / goal;
- 2–6 candidate large systems;
- boundaries between them;
- which systems are connected versus independent;
- relative contrast / dominance;
- which system(s) carry the subject.

### Pass B — local analysis
Then write:
- subject reserve;
- local centering or useful boundary attachment;
- open/closed sides;
- top/bottom asymmetry;
- competing accents;
- possible compensators.

### Pass C — prediction
Only now make a concrete prediction:
- keep;
- move;
- crop;
- add/remove/soften a structure.

### Pass D — user calibration
Record user answer without retroactively pretending the model predicted it.

If wrong:
- identify which system segmentation or relation was wrong;
- update the model;
- do not invent a new micro-law merely to save the previous explanation.

## Experiment log template

```yaml
pilot:
frame_or_seed:
question:
large_systems:
controlled_variables:
manipulated_variable:
prediction_before_user_answer:
user_answer:
result:
confounds:
status:
next_test:
```

## What success would look like

Not “the model can explain any frame after the answer.”

Success means:
1. system segmentation is reproducible enough to discuss;
2. the model makes useful pre-registered predictions on unseen frames;
3. wrong predictions reveal systematic missing variables;
4. the number of ad-hoc rules decreases over time.
