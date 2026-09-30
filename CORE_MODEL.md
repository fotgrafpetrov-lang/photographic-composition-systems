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
