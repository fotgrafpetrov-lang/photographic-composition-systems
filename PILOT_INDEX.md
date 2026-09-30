# Pilot index / Индекс экспериментов

This index is intentionally conservative. If a historical detail is not present in the compact record, it is marked incomplete rather than invented.

## Pilot 180
Legacy pilot in the composition research sequence.

**Compact record:** incomplete.  
Do not reconstruct missing details from guesswork.

## Pilot 218 — local piece vs global frame
Key real frames:
- 4219 — stool in left niche, shifted right relative to local piece; user: insufficient left space.
- 4221 — narrow vertical zone works; visible divider is not necessarily a limiter.
- 4224 — subject pressed to door; “места нет.”

Importance: early evidence that local system position can differ from global-frame position.

## Pilot 272
Late pre-316 stage involving compensation, visual mass, weak versus strong counterweights, and generator behaviour.

Stable carry-forward:
- weak compensation can fill empty volume;
- counterweight should not become the target;
- equal mass is unnecessary;
- gradients repeatedly acted as strong generator compensation;
- geometric/outlined shapes can become more distracting than soft/fragmented forms.

Detailed provenance is partial in this compact snapshot.

## Pilot 316 — real 26-frame series
Input: 26 real photographs, multiple recurring scenes.

Main value:
- forced analysis away from isolated synthetic cues;
- generated hypotheses about system-scale structure, large empty regions, subject extension, reflections, field/path structures;
- later exposed the danger of explaining real frames too quickly with one mechanism.

Current lesson: use real series primarily to identify **large systems and their relations**, then validate local corrections with the user.

Media note:
- Pilot 316 images are retained in the local research package but are not mirrored in this GitHub snapshot yet.

## Pilot 324 — global vs local
Synthetic G/H/I comparison.

User:
- G — normal
- H — more or less, but needs adjustment
- I — centre on local piece

Carry-forward: local and global systems can impose different demands simultaneously.

## Pilot 325 — local-system strength
Same geometry, increasing local contrast/strength.

User responses:
- normal
- normal
- adjust
- shift

Carry-forward: a local structure may become compositionally relevant as its contrast/system strength increases. No universal threshold claimed.

## Pilot 326 — local-system offset
Fixed subject; local piece increasingly shifted.

User:
- normal
- centre on piece
- centre on piece
- move to connection line
- move to connection line

Historical interpretation: two stable positional targets.  
Current correction: do not generalize; response depends on the whole large-system context.

## Pilot 327 — centre-to-boundary sweep
Fixed local system; move subject from local centre toward boundary.

User responses included:
- normal
- slight shift
- shift to centre
- put on line
- seems normal

Useful as local evidence only.

## Pilot 328 — denser transition sweep
User: “так тоже самое скажу.”

Outcome: experiment added little. Triggered the methodological question “зачем это?” and led to abandoning micro-threshold mapping as the main direction.

## Post-328 methodological correction
User:
The answer depends on contrast of the piece, overall frame contrast relative to the subject, and many other factors.

Current direction:
**break frame into large systems first; after that perform fine tuning by balancing compromises.**

## Pilot 329 — generator as composition-correction operator

Goal: stop asking whether the generator merely “makes images prettier” and instead record **which large-system operations it performs** when transforming a frame.

### 329-001 — person in harvested field: active sky suppression
Working sequence: real frame → first generation → second generation.

Observed first-step operation:
- large upper sky system becomes substantially calmer;
- fine cloud activity/local contrast is reduced;
- the subject becomes more isolated against the upper system;
- the lower field remains comparatively textured.

Second-step observation:
- the large-system arrangement changes much less, suggesting provisional stabilization after G1.

Current operation class:
**suppress active system / reduce competing background activity**

Important confound:
fine cloud detail can also be lost through generative reconstruction, so this case is strong evidence of a transformation pattern, not proof of its perceptual mechanism.

### 329-002 — stool at wall/grass boundary: weak structuring of a large wall field
Working identification: first image real, second generated. **This identity has not yet been explicitly confirmed by the user.**

Observed generated changes:
- broad low-frequency tonal structure appears in the wall;
- wall/grass tonal relation strengthens;
- the stool stays small near the system boundary;
- the large wall remains visually empty but less structurally uniform.

Current operation class:
**structure quiet volume / redistribute contrast between large systems**

Status:
useful candidate, but source identity must be confirmed before treating it as a clean case.

### 329-003 — legacy stool/empty-volume generation series
Across earlier synthetic/img2img attempts with deliberately excessive empty space, generators repeatedly introduced:
- gradients;
- texture;
- light streaks;
- foliage/leaves;
- weak edge structures.

These additions often occupied the excessive empty region without becoming an equally dominant subject.

Current operation class:
**add weak compensator / structure quiet volume**

Limitation:
those historical tests were not clean paired balanced-vs-unbalanced controls, so the next version of 329 must explicitly compare matched pairs.
### Quantitative check of 329-001

A first image-statistics check changes the interpretation slightly.

Using normalized regions of the three supplied frames:

- upper-sky high-frequency RMS: ~0.0342 in the likely real frame → ~0.0173 and ~0.0161 in the two generated versions;
- mid-field high-frequency RMS: ~0.0991 → ~0.0711 and ~0.0618.

So generation smooths **both** sky and field. This means ordinary generative reconstruction/smoothing is a genuine confound.

However, the relative reduction is stronger in the sky:
- sky: about **49–53%** reduction in high-frequency residual;
- field: about **28–38%** reduction.

Mean gradient shows the same direction:
- sky: ~0.0108 → ~0.0037 / ~0.0027;
- field: ~0.0484 → ~0.0318 / ~0.0276.

Therefore the corrected reading is:

> 329-001 is **not evidence of sky-only compositional cleanup**. It is global smoothing with a substantially stronger suppression of the upper sky system.

This keeps the system-level hypothesis alive, but it also gives Pilot 329 its first explicit null/confound control: future cases must distinguish **ordinary reconstruction smoothing** from **disproportionate correction of the compositionally problematic system**.
### Quantitative check of 329-002

The stool/wall pair gives a cleaner result than 329-001.

Assuming the first supplied image is the real frame and the second the generated reconstruction:

**Upper wall**
- low-frequency residual structure: ~0.00484 → ~0.00715 (**+48%**);
- mid-scale structure: ~0.00594 → ~0.00887 (**+49%**);
- high-frequency texture: ~0.03364 → ~0.01749 (**−48%**);
- mean gradient magnitude: ~0.03019 → ~0.01360 (**−55%**).

**Mid wall**
- low/mid-frequency structure rises by roughly **13%**;
- high-frequency structure falls by roughly **39%**;
- mean gradient falls by roughly **53%**.

**Mid grass**
- low-frequency structure changes only about **−5%**;
- high-frequency structure about **−12%**;
- mean gradient about **−13%**.

This is important because the wall does not show simple uniform smoothing. It shows a **scale transfer**:

> fine wall texture is suppressed while broader weak tonal structure increases.

The grass does not undergo an equally strong transformation.

Current interpretation:
**structure quiet volume by replacing fine texture with low-frequency tonal organization.**

This is a substantially cleaner match to the compensator hypothesis than 329-001, though the real/generated identity still needs explicit user confirmation.

### 329-004 — clean L/C/R position control

The user regenerated the three prepared inputs in separate fresh contexts using a neutral request to reproduce each photograph closely.

Measured normalized stool x-position:

- **L:** input 0.21765 → generated 0.21313
- **C:** input 0.49773 → generated 0.49629
- **R:** input 0.77678 → generated 0.78849

So the generator **did not recenter the stool**. Subject position was preserved very closely.

Visual observations:

- **C:** no strong new compensating element is obvious.
- **L:** several new dark, low-contrast tonal marks appear along the lower wall to the **right** of the stool, inside the large empty wall volume. They are absent in the prepared input.
- **R:** no equally obvious mirror-image structure appears on the left.

Important structural caveat:
the background is not left-right symmetric. A vertical wall seam already exists on the right. The R stool sits close to that seam; the L stool leaves a long open interval between subject and seam.

Therefore the L/R asymmetry is potentially informative rather than a failed mirror control:

> the generator may respond to the **system context** of the empty volume, not simply to raw geometric distance from the frame center.

Current status:
strong clean candidate, but it should be repeated over multiple generations/seeds before treating the compensator pattern as stable.

