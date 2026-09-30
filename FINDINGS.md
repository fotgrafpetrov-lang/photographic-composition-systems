# Findings / Накопленные результаты

## I. Repeated observations worth retaining

### F1. Start with systems, not micro-rules
**Status:** working_principle

The most useful reduction of the many interacting factors is to first operate with **large systems of the frame**. Fine placement comes later as balancing compromises.

### F2. Local and global organization can disagree
**Status:** repeated_observation

A subject may look acceptable relative to the whole frame but badly positioned inside its local piece, or vice versa.

This was present in real pilot 218 and later isolated synthetically in pilots 324–327.

### F3. Visual mass is not fixed
**Status:** repeated_observation

The same class of element can act as:
- counterweight,
- boundary,
- accent,
- weak filler,
- structural connector,
depending on the rest of the frame.

### F4. Weak compensation can stabilize large empty volume
**Status:** repeated_observation

A large empty region does not necessarily need a second object. Weak gradients, fragmented forms, reflections, edge elements, or soft structures can make the region participate in the frame while the subject remains dominant.

### F5. A compensator should not become the new target
**Status:** repeated_observation

In synthetic tests, a filled black rectangle was maximally heavy; outlined/geometric shapes could become distracting. A soft light gradient without hard edges often worked better as a counterweight. Fragmented shapes tended to stop the eye less strongly.

### F6. Equal mass is not required
**Status:** repeated_observation

The subject should normally remain the dominant target. The counterweight/compensator does not need to match the subject in visual mass.

### F7. Upper and lower regions behave differently
**Status:** repeated_observation

Many real-frame corrections involved “top too much,” “bottom too active,” “dark bottom pulls,” “upper gradient pulls,” etc. Treating top/bottom as symmetric empty margins was repeatedly inadequate.

### F8. Continuous structures can glue dissimilar areas
**Status:** repeated_observation with caveats

Lines, shadows, reflections, and continuous structures can connect regions. However the exact mechanism may mix perceptual continuity, semantic recognition, and system boundaries. Do not generalize to “any continuous line improves composition.”

### F9. Generative editors tend to repair intentionally bad empty space
**Status:** repeated_observation

Attempts to ask a generative model to create “too much space” without compensating texture/structure repeatedly produced balancing gradients, texture, light lines, leaves, etc. This makes synthetic generation a poor source of naturally unbalanced controls unless the compensation is explicitly suppressed.

### F10. “Bad” is not guaranteed to contain “good” by crop
**Status:** explicit project constraint

Do not assume a bad frame becomes good through cropping. Cropping must be evaluated as a new system, not as a guaranteed repair.

---

## II. Pilot-specific observations

### Blur / patch thresholds
Some synthetic series suggested blur/softening effects becoming perceptible around roughly a few percent, with user comments such as ~3% beginning to work and 5–7% being a useful range in that setup. Other pixel-size patch experiments had 2 px / 20 px / 35 px observations.

**Status:** pilot_specific  
**Do not generalize.** The user repeatedly objected to tests that sat at the limit of visibility.

### Pilot 218
Real local-versus-global examples:
- `4219`: stool in left niche but shifted right relative to local piece; user: “левого пространства не хватает.”
- `4221`: narrow vertical zone works; divider is “не ограничитель.”
- `4224`: no room; subject pressed to door.

This is one of the strongest early sources for local-system analysis.

### Pilot 324
Synthetic global/local structure:
- G (global only): user — “нормально”
- H (global + local): “более менее, но надо куда-то крутить по кадру”
- I (local only): “центрировать по куску”

Useful conclusion: global and local systems can coexist and conflict; one does not simply switch the other off.

### Pilot 325
Increasing strength of a local system:
- weak: “нормально”
- next: “нормально”
- stronger: “крутить”
- strongest: “смещать”

Useful only as evidence that the relevance of a local system can change with its contrast/strength. Do not infer a universal threshold.

### Pilot 326
Increasing offset of a local piece relative to a fixed subject:
- 0: “нормально”
- moderate offsets: “смещать по центру куска”
- large offsets: “смещать на линию соединения”

Initially interpreted as two positional attractors. Later corrected: this cannot be treated as a universal mechanism because the answer depends on contrast of the piece, total frame contrast relative to the subject, and many other interacting factors.

### Pilots 327–328
Dense sweep between centre of local piece and boundary produced responses such as:
- “нормально”
- “чуть сместить”
- “сместить в центр”
- “поставить на линию”
- “вроде норм”

The denser 328 test was judged redundant (“так тоже самое скажу”). The user then challenged the purpose of the branch. Final lesson: do not spend effort mapping micro-thresholds before establishing what system-level problem is being solved.

---

## III. Current high-level result

The most important current synthesis is:

> **Many low-level variables can be compacted by first parsing the frame into large interacting systems. After that, composition becomes finer adjustment and balancing of compromises inside and between those systems.**

This is the direction to preserve in future work.
