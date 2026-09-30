# START HERE

## 1. What this research is trying to do

The project is looking for a **working structural model of photographic composition in real scenes**, especially ordinary urban / overcast / non-spectacular scenes where sunset, fog, dramatic color, texture, or other obvious attractions cannot be relied upon to save the frame.

The working direction is not “discover one magic placement rule.” The latest state is hierarchical:

> **First: decompose the frame into large compositional systems.  
> Second: understand relations among those systems.  
> Third: tune the subject and local structure inside them by balancing compromises.**

The term “large system” is a project working term, not a standard established photography term.

## 2. Canonical analysis order (current)

When analysing a frame, do not begin with the exact position of the subject.

1. **Identify the subject / goal of the frame.**
2. **Identify large systems** at frame scale: large fields, planes, connected masses, regions, or structures that function as coherent units.
3. **Identify relations between large systems:** separation, overlap, continuity, common boundary, dominance, contrast, open/closed edges, upper/lower interaction.
4. **Identify which system(s) carry the subject.**
5. Only then analyse the **reserve around the subject**, local centering, attachment to boundaries/intersections, crop, compensators, and other fine adjustments.
6. Treat the final position as a **compromise among several simultaneous systems**, not as the output of one universal rule.

## 3. What “large system” does NOT mean

It is not simply:
- one physical object;
- one semantic category;
- one large shape;
- one tonal blob;
- foreground / middle ground / background by default.

Several physical objects may act as one system. One physical surface may split into several systems if its structure, boundary, contrast, or role changes.

The exact operational segmentation criteria are still an open problem.

## 4. Central current correction

A recurring mistake in previous pilots was trying to isolate one variable too early: “line versus centre,” “effective centre,” “nearest attractor,” “strong boundary,” etc.

The user’s correction is central:

> The answer changes with the contrast of the local piece, the total contrast of the frame relative to the subject, and many other interacting factors. The useful reduction is to operate first with **large systems**, then do finer tuning through compromise.

Therefore:
- do not assign a fixed “weight” to a line, patch, gradient, or object outside the frame context;
- do not expect a universal winner between “centre of empty area” and “intersection line”;
- do not infer a universal threshold from a few synthetic frames.

## 5. Stable vocabulary in one paragraph

The **subject (предмет / цель кадра)** is the target around which the frame is being solved. It requires a usable **reserve of space**. “Оптималка” means an optimal reserve, often with the subject appropriately centred inside its effective local area; “максималка” is deliberately enlarged homogeneous space that can strengthen isolation of the subject. **Continuous structures / lines** can glue otherwise separate regions, but continuity alone is not a universal law. **Limiters / boundaries** can close a plane. **Compensators** occupy excessive empty volume without becoming a rival subject. Their visual mass is contextual. Upper and lower parts of the frame often behave as different systems rather than one symmetric container.

## 6. Status labels used in this repository

- `repeated_observation` — occurred repeatedly across real/synthetic work and survived discussion.
- `working_principle` — useful current rule of analysis, not claimed universal.
- `pilot_specific` — observed in a specific experiment; do not generalize automatically.
- `hypothesis` — proposed mechanism requiring testing.
- `rejected_or_oversimplified` — path that was useful historically but should not be carried forward as a law.
- `open` — unresolved.

## 7. How another LLM should enter the project

Do not begin by teaching photography. Begin by reading the current state, then analyse new material using the large-system hierarchy. Preserve uncertainty. If a new observation contradicts the model, update the model rather than explaining the contradiction away.


---

# Core model / Текущее ядро модели

## A. Coarse-to-fine architecture

The current research architecture is:

**frame → large systems → system relations → subject-bearing system → local reserve / boundaries / compensation → fine balance of compromises**

This hierarchy is more important than any single micro-rule discovered in synthetic pilots.

### Stage 1 — Large-system segmentation

Find the few largest units that actually organize the frame. Candidate cues include:
- continuous or common boundaries;
- coherent plane / field;
- tonal or contrast organization;
- common texture or repeated structure;
- connectedness;
- open versus closed continuation toward the frame edge;
- overlap and occlusion;
- whether multiple elements act as one mass;
- whether an area has its own internal organization relative to neighbouring areas.

These are **candidate cues**, not yet a finished segmentation algorithm.

### Stage 2 — Relations among systems

Analyse:
- relative scale;
- relative contrast and visual mass;
- upper/lower asymmetry;
- whether systems are glued or independent;
- whether a boundary closes an area or continues “to infinity”;
- whether one system supports, competes with, or destabilizes the subject-bearing system.

### Stage 3 — Subject inside a system

Only after the large structure is understood:
- available reserve around subject;
- whether reserve is too small / optimal / excessive;
- local centering relative to the effective area;
- position on or away from meaningful intersections/boundaries;
- interaction with crop;
- whether subject crosses, closes, or is contained by a system boundary.

There is no universal rule that centre is always better than boundary, or boundary better than centre. The answer depends on the whole system.

### Stage 4 — Compensation and fine tuning

If a large region feels excessive, it does not necessarily need a new object. It may be stabilized by:
- weak edge elements;
- fragmented forms;
- soft tonal changes;
- gradients;
- reflections/shadows/continuations;
- texture;
- other low-dominance structures.

A useful compensator should normally **fill or structure volume without becoming the new subject**.

### Stage 5 — Compromise

Real frames rarely satisfy every local relation simultaneously. Fine composition is treated as **balancing several imperfectly compatible demands** after the large systems are established.

This is why trying to derive one exact placement rule from one cue usually fails.

---

## B. System-level principles currently worth carrying forward

### 1. Visual mass is contextual

A black rectangle, line, gradient, plant, reflection, or bright patch does not possess one fixed composition weight. Its effect depends on:
- frame-scale systems;
- subject contrast;
- neighbouring contrast;
- geometry;
- degree of connectedness;
- whether it becomes an independent recognizable object;
- whether it closes or opens a region.

### 2. Large empty volume can be useful

Large empty space is not automatically an error. Its success depends on the surrounding system:
- the subject may occupy/extend into it;
- weak structures may stabilize it;
- surrounding boundaries may close it;
- repetition/texture may make it part of a coherent field;
- the subject may remain dominant despite large reserve.

### 3. A “bad” frame is not guaranteed to become good by cropping

Cropping can expose or alter system relations, but the project explicitly rejects the assumption that every bad frame contains a good crop.

### 4. Top and bottom are often different systems

Upper and lower regions should not automatically be treated as symmetric reserves around the subject. Light sky, dark ground, active vegetation, reflections, horizon bands, etc. can create distinct systems with different visual effects.

### 5. Continuous structures can glue regions

A physical continuous line, shadow, reflection, or repeated connected structure can help multiple regions read together. But:
- this is not sufficient by itself;
- semantic/physical connection may confound the effect;
- do not turn “continuity” into a universal placement rule.

### 6. Boundaries matter through function, not just contrast

A visible line can be:
- a real separator between systems;
- an internal line inside one system;
- an edge limiter;
- an independent accent.

Equal contrast does not guarantee equal compositional function.

---

## C. What is NOT currently claimed

The project does **not** currently claim:
- a numeric universal “visual weight” formula;
- a universal optimal percentage of empty space;
- that the subject should always be centred in its local area;
- that the subject should always sit on a boundary/intersection;
- that the nearest structural “attractor” wins;
- that continuous contact automatically makes an area belong to the subject;
- that one local system simply overrides the global system;
- that micro-threshold findings from synthetic tests generalize to real photographs.

---

## D. Research direction

The strongest next problem is not another micro-threshold experiment. It is:

> **Operationally define how to segment a frame into large compositional systems, then test whether that segmentation improves prediction of real composition corrections on unseen photographs.**

That would turn the current expert practice into an explicit analysis pipeline.


---

# Failed paths, over-simplifications, and confounds

This file exists specifically so another model does **not** repeat the same path.

## 1. Searching for one universal placement rule
**Status:** rejected_or_oversimplified

Examples:
- “centre of local piece beats boundary”
- “boundary beats centre”
- “nearest stable position wins”
- “effective centre determines subject position”

Why rejected:
The answer changes with local contrast, whole-frame contrast relative to subject, system strength, neighbouring structures, scale, and many other factors. These variables should first be organized at the large-system level.

## 2. Treating visual weight as a fixed scalar
**Status:** rejected_or_oversimplified

A black patch, line, gradient, plant, or reflection does not have one context-free weight. Its role can change completely with system structure.

## 3. Physical continuity = ownership of space
**Status:** rejected_or_oversimplified

A line/rail/edge may be continuous yet remain independent of the subject. Reflection/shadow can appear strongly attached for semantic/physical reasons. “Connected” is not sufficient as a law.

## 4. Terminal-point theory
**Status:** hypothesis not established

An exploratory branch proposed that a spatial region works when it “terminates” at the subject. Real examples 016/019 motivated this, but it was not cleanly validated and should not be elevated to the core model.

## 5. Micro-threshold hunting too early
**Status:** methodological failure mode

Repeated tests near visibility thresholds produced ambiguous answers and user frustration. Rule:
**first establish a large, obvious effect; only then test thresholds if the threshold itself matters.**

## 6. Using generative models to manufacture bad composition
**Status:** methodological limitation

The generator frequently repairs intended imbalance by adding:
- gradient,
- texture,
- light streak,
- foliage,
- other compensators.

Generated controls must therefore be inspected for hidden balancing cues.

## 7. Cropping as guaranteed repair
**Status:** rejected

Project rule: `bad` does not automatically become `good` by crop.

## 8. Treating known low-level visual illusions as discoveries
**Status:** avoid

Mach bands, Craik/Cornsweet-like brightness effects and similar artifacts should be labeled as known perceptual confounds if they appear. Do not inflate them into new composition laws.

## 9. Over-reading pilot 316 before user calibration
**Status:** caution

The 26-frame real series generated useful hypotheses, but several early assistant explanations were made before enough user correction. Keep the images and hypotheses, but do not treat those interpretations as validated laws.

## 10. Confusing human automatic perception with the proposed analytical method
**Status:** corrected

Humans automatically group visual input, but the project claim is not “people consciously divide photographs into large systems.” The explicit large-system decomposition is a proposed/used analytical method, not standard conscious photographic practice.


---

# Open questions / Что ещё не решено

## 1. Operational segmentation
How can a frame be reproducibly segmented into **large compositional systems**?

Questions:
- What makes two regions one system rather than two?
- Which cues dominate when tone, geometry, texture, and continuity disagree?
- Can a physical surface split into two systems?
- Can separate physical objects form one system?
- At what scale should segmentation stop?

## 2. System hierarchy
Do global and local systems form a strict hierarchy, or do several scales act simultaneously with different strengths?

Current evidence favours simultaneous influence rather than simple override.

## 3. System descriptors
Can hundreds of low-level variables be compacted into a small set of system-level descriptors such as:
- system scale;
- contrast relative to subject;
- closure/openness;
- connectedness;
- internal fragmentation;
- subject reserve;
- competition with neighbouring systems;
- upper/lower role?

These categories are provisional.

## 4. Prediction on unseen real frames
Can the model predict the user’s correction **before** seeing the user’s answer on new photographs?

The useful target is not only “good/bad” but:
- keep;
- crop top/bottom;
- move subject left/right/up/down;
- centre inside local system;
- attach to a boundary/intersection;
- add/remove/soften a compensator.

## 5. Annotation protocol
How should a dataset represent:
- polygons/masks of large systems;
- subject mask;
- system boundaries;
- open/closed edges;
- relation graph between systems;
- user correction;
- confidence / ambiguity?

## 6. Synthetic versus real controls
How can synthetic experiments isolate variables without introducing hidden generator compensation?

## 7. Quantification
Only after system-level categories are stable:
- can reserve be normalized by subject scale?
- can boundary strength be measured?
- can compensation be measured without collapsing into generic saliency?
- are there robust thresholds, or mostly context-dependent transitions?

## 8. Relation to existing theory
Nearest neighbouring concepts include Gestalt grouping, pictorial organization, visual masses, and spatial organization, but the exact coarse-to-fine “large systems → local compromise” method has not been located as a standard photographic framework in the current search.
