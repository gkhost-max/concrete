---
name: concrete-paper-writing
description: Write publication-ready papers for concrete transport, pumping, extrusion, and shotcrete / sprayed concrete research. Use when drafting, restructuring, polishing, or reviewing manuscripts about concrete rheology, pumpability, pipeline pressure loss, lubrication layers, nozzle/spray process parameters, rebound, buildability, accelerator effects, fibre-reinforced shotcrete, 3D concrete printing, field trials, laboratory pumping loops, or Chinese-language requests about 混凝土输送、泵送、喷射混凝土、湿喷、干喷、可泵性、回弹率、喷射工艺. Also use for citation verification, figure/table planning, reviewer-response preparation, and journal-specific manuscript adaptation in civil engineering, cementitious materials, and construction automation.
---

# Concrete Paper Writing for CCR / CCC / CBM

Use this skill to help write rigorous papers in concrete transport, pumping, extrusion, and shotcrete / sprayed concrete research. The goal is a manuscript that a civil engineering, construction materials, or construction automation reviewer can evaluate and reproduce.

The original folder name is `ml-paper-writing`, but this skill now targets concrete delivery and spraying domains. Do not default to ML conference templates, GPU/seed reporting, algorithm baseline language, or NeurIPS/ICML-style checklists unless the user explicitly asks for a machine-learning paper in this domain.

## Core Stance

Be proactive, but do not invent experimental facts.

- Draft concrete text when the user's notes, data, figures, or manuscript are sufficient.
- Ask only targeted questions when a missing detail affects scientific validity, such as mixture proportions, pump/nozzle geometry, measurement method, sample size, curing age, or target journal.
- Mark unresolved items plainly as `AUTHOR INPUT NEEDED`, `DATA NEEDED`, or `CITATION NEEDED`.
- Preserve units, test conditions, material names, standard numbers, and measurement methods exactly as provided.
- Never fabricate mix designs, pressure values, rheological parameters, strength values, rebound rates, statistical significance, standards, citations, or field-trial conditions.

## Domain Scope

Use this skill for papers involving one or more of these topics:

- Concrete pumpability, transportability, pressure loss, blockage risk, segregation, bleeding, or lubrication layer formation.
- Rheology of cementitious materials: yield stress, plastic viscosity, thixotropy, structural build-up, static/dynamic yield stress, flow retention, and temperature effects.
- Wet-mix or dry-mix shotcrete, sprayed concrete linings, tunnel support, slope protection, repair layers, and fibre-reinforced shotcrete.
- Nozzle process parameters: air pressure, flow rate, nozzle angle, nozzle distance, spray velocity, accelerator dosage, layer thickness, and deposition quality.
- Rebound, dust, adhesion, buildability, surface quality, compaction, porosity, and anisotropy after spraying or extrusion.
- Laboratory pumping loops, full-scale pumping lines, field spraying trials, extrusion rigs, printable concrete, and 3D concrete printing when the main issue is material delivery or deposition.
- Numerical or hybrid modelling: CFD, DEM, SPH, FEM, Bingham/Herschel-Bulkley models, lubrication-layer models, pressure-loss equations, and data-driven prediction, when tied to concrete transport or spraying.

## Domain-Specific Intake

Before drafting a full manuscript, build a compact evidence map. If the user has not provided information, infer only safe structure and mark details as missing.

```
Evidence Map:
- Target journal or article type:
- Main application: pumping / wet shotcrete / dry shotcrete / extrusion / 3D printing / field support
- Main contribution in one sentence:
- Material system: cement, SCMs, aggregate grading, fibres, admixtures, accelerator, water-to-binder ratio
- Mixture table available: yes/no
- Equipment: pump type, line length/diameter, bends, nozzle, compressor, mixer, rheometer, sensors
- Process variables: flow rate, pressure, nozzle angle/distance, air pressure, accelerator dosage, layer thickness
- Measured responses: pressure loss, flow/slump/spread, rheology, rebound, buildability, strength, bond, durability, microstructure
- Replicates/statistics:
- Standards or protocols used:
- Key figures/tables already available:
- Citations already verified:
- Missing details that affect validity:
```

## Contribution Framing

Frame the paper around a material-process-performance chain:

```
Material design or model
  -> transport / pumping / spraying mechanism
  -> measurable process response
  -> hardened or field performance consequence
```

A strong contribution usually answers at least one of these questions:

- What material parameter controls transport or spray behaviour, and under what boundary conditions?
- What process parameter reduces pressure loss, rebound, blockage, dust, or quality variability?
- What mechanism links fresh-state rheology to sprayed-layer build-up, adhesion, compaction, or hardened properties?
- What validated model predicts pressure loss, rebound, layer stability, or pumpability beyond one mixture?
- What field-scale evidence shows that a laboratory metric transfers to actual pumping or spraying?

Avoid claiming novelty from a single new mixture unless the mechanism, process window, field validation, or predictive framework is clear.

## Manuscript Workflow

### 1. Define The Claim Ledger

Create a claim ledger before writing results.

```
Claim Ledger:
- Claim C1:
  Evidence: figure/table/test
  Boundary condition: mixture, flow rate, pipe/nozzle, age, temperature
  Risk: confounder, missing replicate, scale-up limit
- Claim C2:
  Evidence:
  Boundary condition:
  Risk:
```

Every paragraph in Results and Discussion should trace back to a claim in this ledger.

### 2. Plan Figures Before Prose

Concrete transport papers live or die on figure clarity. Plan the evidence sequence first:

1. System schematic: material, pump/pipe/nozzle/spray setup, sensors, and variables.
2. Mixture/protocol table: proportions, admixtures, fibres, aggregate grading, test ages.
3. Fresh-state response: slump flow, flow table, V-funnel, rheology, setting, thixotropy, or build-up.
4. Transport/spray response: pressure-time curves, pressure gradient, blockage, spray deposition, rebound, layer build-up.
5. Hardened or durability response: strength, bond, toughness, permeability, porosity, microstructure.
6. Mechanism or model validation: predicted vs measured, sensitivity analysis, process window.

### 3. Draft The Abstract

Use a civil/materials abstract structure:

1. Practical problem: why pumping/spraying/deposition currently fails or remains difficult.
2. Knowledge gap: what relationship, mechanism, scale, or process window is not established.
3. Approach: material system, apparatus, variables, and methods.
4. Main quantitative findings: only numbers supported by data.
5. Mechanistic or engineering implication: what design, model, or process choice becomes possible.

Avoid generic openings such as "Concrete is the most widely used construction material" unless the paper specifically needs that scale framing.

### 4. Draft The Introduction

Use a funnel suited to concrete technology:

- Field or engineering need: tunnel support, high-rise pumping, repair, underground construction, automated spraying, printable construction, or quality control.
- Technical bottleneck: blockage, high pressure loss, rebound, poor build-up, segregation, early-age instability, fibre dispersion, durability trade-off.
- Prior approaches: rheology control, admixture design, accelerator control, nozzle optimization, modelling, field monitoring.
- Gap: missing scale transfer, missing mechanism, limited process parameter space, unclear material-process coupling, insufficient validation.
- Present study: concise contribution list, with each contribution tied to a measured outcome.

Contribution bullets should be specific:

```
This study:
1. Quantifies how [material/process variable] changes [pressure loss/rebound/buildability] under [defined conditions].
2. Identifies [mechanism] using [rheology/microstructure/model/field data].
3. Provides [model/process window/design rule] validated by [independent mixtures or field trial].
```

### 5. Draft Materials And Methods

Methods must enable reproduction. Include enough detail for another lab or contractor to repeat the work.

Required details when applicable:

- Binder composition, SCMs, cement type, aggregate source/grading, fibre type/length/dosage, admixture and accelerator type/dosage.
- Mix proportions by mass or volume, water-to-binder ratio, sand-to-binder ratio, aggregate moisture correction, mixing sequence, rest time, and temperature.
- Rheology protocol: instrument geometry, shear history, pre-shear/rest, shear-rate sweep, fitting model, calibration, and time after mixing.
- Fresh concrete tests: standard used, timing, temperature, replicates, and acceptance/measurement criteria.
- Pumping setup: pump type, pipe diameter, total length, bends, vertical lift, flow rate, pressure sensor locations, sampling frequency, and cleaning/blockage protocol.
- Shotcrete setup: wet/dry process, nozzle type, nozzle distance/angle, air pressure, material flow, accelerator injection point/dosage, substrate condition, panel geometry, operator/robot control mode.
- Hardened tests: curing regime, specimen extraction direction, age, loading rate, number of specimens, and relevant standard.
- Statistics: replicate count, reported dispersion, test used, significance threshold, and outlier policy.

When citing standards, verify the current version and local equivalent. Examples of commonly relevant families include ASTM C143/C143M, ASTM C1611/C1611M, ASTM C39/C39M, ASTM C109/C109M, ASTM C1609/C1609M, EN 12350, EN 12390, ACI 506 guidance, EFNARC sprayed concrete guidance, and RILEM recommendations. Do not cite a standard unless the user or a verified source confirms it applies.

### 6. Draft Results

Organize Results by claim, not by lab chronology.

Effective result subsection patterns:

- "Rheological evolution controls pressure loss during pumping"
- "Nozzle distance and accelerator dosage jointly determine rebound"
- "A lubrication layer explains the observed reduction in pressure gradient"
- "Buildability improves at the cost of interlayer bond beyond the optimum window"
- "The pressure-loss model transfers from laboratory loop to field line within [verified error]"

For each subsection:

1. State the tested claim in the first sentence.
2. Point to the exact figure/table and describe what readers should see.
3. Report quantitative changes with units and uncertainty.
4. Name the mechanism only after evidence is shown.
5. State boundary conditions and avoid overgeneralization.

### 7. Draft Discussion

The Discussion should answer "what does this change for concrete delivery or spraying practice?"

Cover:

- Mechanistic interpretation: rheology, particle migration, lubrication, air entrainment, hydration/setting, fibre orientation, compaction, or substrate interaction.
- Engineering implication: mixture design rule, allowable flow-rate range, nozzle control window, acceptance test, field monitoring strategy, or model use case.
- Comparison with literature: explain agreement or disagreement through material, equipment, scale, or test-protocol differences.
- Scale and boundary limits: lab-to-field transfer, pipe/nozzle geometry, operator effects, ambient conditions, material variability.
- Trade-offs: pumpability vs buildability, rebound vs early strength, accelerator dosage vs durability, fibre content vs blockage risk, flowability vs segregation.

### 8. Draft Conclusions

Conclusions should be numbered or compact paragraphs. Each item must connect:

```
variable or mechanism -> measured evidence -> practical implication -> boundary condition
```

Avoid unsupported universal claims such as "this method solves shotcrete rebound". Prefer bounded claims such as "under the tested wet-mix conditions and nozzle distance range, increasing [X] reduced rebound by [Y] while maintaining [Z]."

## Citation Workflow

Never generate references from memory.

Use available tools such as Zotero, CrossRef, publisher pages, DOI resolvers, Google Scholar, Web of Science, Scopus, PubMed for biomedical-cement contexts, or domain databases when available. For every citation:

1. Verify that the paper, standard, report, or guideline exists.
2. Verify bibliographic metadata from a primary or reliable source.
3. Verify that the cited source actually supports the claim.
4. Fetch or export BibTeX/RIS/ENW programmatically when possible.
5. Mark unverified items as `CITATION NEEDED` or `VERIFY STANDARD VERSION`.

High-value literature categories for this domain:

- Rheology and pumpability of cementitious materials.
- Shotcrete rebound, adhesion, accelerator, fibre-reinforced sprayed concrete, and tunnel support.
- Lubrication layer and pressure-loss modelling in concrete pumping.
- Extrusion and 3D concrete printing buildability / open time / interlayer bond.
- Standards, RILEM/ACI/EFNARC guidance, and field practice reports.
- Review papers in Cement and Concrete Research, Cement and Concrete Composites, Construction and Building Materials, Materials and Structures, Automation in Construction, Tunnelling and Underground Space Technology, ACI Materials Journal, ASCE Journal of Materials in Civil Engineering, and related journals.

## CCR / CCC / CBM Journal Targeting

Default to the three Elsevier journal families most relevant to concrete transport and sprayed concrete manuscripts:

- `CCR` = Cement and Concrete Research.
- `CCC` = Cement and Concrete Composites.
- `CBM` = Construction and Building Materials.

When the user does not name a journal, first infer whether the manuscript is closer to CCR, CCC, or CBM, then state the fit and draft accordingly.

### Cement and Concrete Research (CCR)

Choose CCR when the paper makes a fundamental materials-science contribution. CCR favours major results on cementitious materials, novel experimental or analytical methods, modelling, diagnosis of real cement/concrete systems, and improved material performance with broad scientific assimilation.

For concrete pumping or spraying, frame the manuscript for CCR only if the work explains a mechanism such as:

- rheology, thixotropy, hydration, flocculation, setting, or admixture interaction;
- lubrication layer formation, particle migration, pore structure, or microstructure-property coupling;
- validated modelling that links material structure to fresh or hardened performance;
- digital fabrication or rheology control with a fundamental cementitious-materials question.

CCR risk filter: if the paper only optimizes a mixture or process setting without mechanism, it is probably not CCR-ready. Strengthen the paper by adding mechanistic evidence, a transferable model, or a clear structure-property-performance argument.

### Cement and Concrete Composites (CCC)

Choose CCC when the paper focuses on cement-based composites and links material-scale properties to engineering performance. CCC is a strong fit for fibre-reinforced sprayed concrete, polymer or blended cement composites, special aggregates, waste inclusions, fracture, durability, composite mechanics, fabrication, modelling, and practical applications, provided the material-scale connection is explicit.

For pumping or shotcrete, frame for CCC when the work shows:

- fibre type, fibre orientation, dispersion, toughness, bond, fracture, or anisotropy effects;
- microstructure as it relates to engineering properties;
- durability or serviceability effects of sprayed, pumped, extruded, or repaired cement composites;
- field or component behaviour that is connected back to material-scale properties.

CCC risk filter: do not present a field application alone. Tie in situ behaviour, repair performance, sustainability, or serviceability to measured material properties.

### Construction and Building Materials (CBM)

Choose CBM when the paper is an innovative construction-materials study with a practical laboratory campaign, experimental breadth, repair/new-work relevance, or construction technology implication. CBM is a good default for applied pumping, wet/dry shotcrete, rebound reduction, process optimization, practical mix design, monitoring, NDT, and repair/maintenance materials.

For pumping or shotcrete, frame for CBM when the work shows:

- original laboratory experiments or experimental campaigns with clear construction-material application;
- practical mixture design, process parameter windows, quality-control metrics, or repair/new-work relevance;
- comparison across binders, aggregates, admixtures, fibres, accelerators, or process settings;
- performance evidence useful to engineers, contractors, or material suppliers.

CBM risk filter: avoid drifting into pure structural engineering, pure materials chemistry, geotechnics, mining/backfill, soil/rock mechanics, or unbound road/railway bed layers unless the manuscript has a clear construction-materials focus.

### Elsevier Submission Checks For CCR / CCC / CBM

Before finalizing a manuscript for these journals, check:

- Article type: research paper by default; use review/communication/discussion only when the journal permits that article type for the case.
- Single-anonymized review: do not assume double-blind formatting unless the journal or special issue explicitly asks.
- Highlights: prepare short, result-specific highlights when required by the submission system.
- Graphical abstract: prepare only if useful or required; it must convey the material-process-performance chain.
- Data statement: include a data availability statement and repository link when data are shared.
- Research data: recommend trusted repositories for pressure logs, rheology data, mixture tables, image sets, scripts, and model data.
- Declaration of competing interests and funding: include standard Elsevier declarations.
- Declaration of generative AI use: if AI tools helped draft, organize, or edit the manuscript, tell the user to include the required disclosure statement; do not list AI tools as authors.
- Units and nomenclature: use SI units, define all mixture codes, and keep symbols consistent.
- Figures and tables: ensure captions stand alone and include sample size, error bars, and test conditions.
- References: use the target journal's Elsevier reference style or a verified reference manager export; never invent metadata.

For all three journals, adapt the same evidence into different lead arguments:

- CCR lead: mechanism first, application second.
- CCC lead: composite material-property-performance coupling first.
- CBM lead: practical construction-material innovation and validated application first.

## Common Reviewer Risks

Watch for these failure modes:

- Novelty is only a new mixture, with no mechanism or transferable rule.
- Pumpability is inferred from slump/spread alone without pressure, rheology, or transport evidence.
- Shotcrete rebound is reported without nozzle distance, angle, flow rate, air pressure, accelerator dosage, substrate, or collection method.
- Rheology is reported without shear history, timing after mixing, temperature, or fitting details.
- Lab results are generalized to field-scale pumping without scale discussion.
- Fibre effects are discussed without fibre distribution, orientation, blockage risk, or toughness/bond implications.
- Accelerator improves early strength but durability, setting time, or long-term strength trade-offs are ignored.
- Numerical models are fitted but not validated on independent conditions.
- Photographs are used as evidence without quantitative metrics.
- Statistical dispersion, replicate count, or specimen geometry is missing.
- Standards are cited generically or with outdated/inapplicable versions.

## Tables And Figures

Use SI units consistently. Keep figures readable after journal reduction.

Recommended tables:

- Mix proportions with all units, moisture correction, and admixture dosages.
- Material properties: cement/SCM chemistry, particle size, aggregate grading, fibre properties.
- Test matrix: variables, levels, specimens, ages, replicates.
- Model parameters and validation errors.

Recommended figures:

- Apparatus schematic with dimensions and sensor/nozzle positions.
- Pressure-time and pressure-gradient plots with flow-rate annotations.
- Rheology curves with fitted model and parameter table.
- Rebound/buildability/process-window maps.
- Layer geometry, cross-sections, porosity, fibre distribution, or microstructure images.
- Predicted-vs-measured model validation.

Figure captions must stand alone: define mixture codes, process settings, sample size, and error bars.

## Writing Style

Write for domain reviewers who care about reproducibility and constructability.

- Use concrete nouns: "pressure gradient", "static yield stress", "rebound mass fraction", "nozzle distance", "accelerator dosage".
- Keep terminology stable. Do not alternate between pumpability, transportability, and flowability unless each is defined.
- Separate observation from mechanism: report measured trends first, then interpret.
- Use bounded language: "under the tested conditions", "for the investigated mixture range", "within the measured flow-rate interval".
- Avoid unsupported causality. Use "is consistent with", "suggests", or "may indicate" when mechanism is indirect.
- Avoid vague claims such as "good workability", "excellent performance", or "significant improvement" without metrics.

## Output Expectations

When helping the user, produce directly usable manuscript material:

- Full section drafts when enough evidence exists.
- Structured outlines when key data are missing.
- Claim ledgers, figure plans, table shells, and reviewer-risk audits.
- Polished English from Chinese technical notes while preserving experimental meaning.
- Explicit missing-information lists for facts that cannot be inferred.
- Verified citations or clearly marked citation placeholders.

## Existing References In This Skill Folder

Some bundled reference files were originally written for ML paper writing. Use them cautiously:

- `references/citation-workflow.md`: use only for general citation-verification discipline.
- `references/writing-guide.md`: use only for general clarity and sentence-level writing principles.
- `references/checklists.md`, `references/reviewer-guidelines.md`, and `templates/`: treat as legacy ML resources unless the user explicitly asks for ML/AI conference formatting.

For concrete transport and shotcrete manuscripts, prioritize the domain rules in this `SKILL.md` and verified civil-engineering/materials sources supplied by the user or found through reliable search.

