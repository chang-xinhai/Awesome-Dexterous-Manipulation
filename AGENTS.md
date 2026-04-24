# AGENTS.md

## Mission

This repository is a curated **Awesome-Dexterous-Manipulation** list for the robotics ecosystem around dexterous hands, tactile sensing, hand-centric manipulation tasks, learning/control methods, benchmarks, datasets, and infrastructure.

The goal is not to be a generic robot-manipulation bibliography. The goal is to organize the most relevant resources for:
- dexterous hands, multi-finger grippers, tactile sensors, and multimodal hardware
- hand-centric manipulation capabilities such as in-hand manipulation, non-prehensile manipulation, dynamic dexterity, bimanual dexterity, and deformable-object skills
- robot learning and control methods that materially advance dexterous manipulation
- data collection pipelines, teleoperation systems, simulation stacks, benchmarks, and datasets
- surveys, reviews, and taxonomy resources that help structure the field

## Single-file content policy

All curated content lives in `README.md`.

Do **not** create `contents/` pages for paper organization.
Do **not** split the awesome list into multiple markdown content files unless the user explicitly requests it.

Allowed root-level files:
- `README.md` - the canonical awesome list
- `AGENTS.md` - governance and maintenance rules
- `LICENSE`
- `.gitignore`
- optional static assets under `assets/` or `imgs/` when they improve presentation

## Canonical section layout

`README.md` should use this top-level structure:
1. `Hardware & Sensor Systems`
2. `Dexterity Capabilities & Tasks`
3. `Methodology`
4. `Infrastructure`
5. `Surveys & Reviews`

Use `About`, `Must Read`, `News`, and `Contents` near the top of the README. Keep subsection anchors stable.

## Section definitions

### Hardware & Sensor Systems

Include resources about the physical interface layer for dexterous manipulation:
- dexterous hands and anthropomorphic hand platforms
- non-anthropomorphic hands and multi-finger grippers
- tactile sensors, robotic skin, force sensing, and visuo-tactile fingertips
- multimodal setups combining vision, touch, proprioception, force/torque, audio, or wearable capture

### Dexterity Capabilities & Tasks

Include work primarily defined by the manipulation capability or task family:
- prehensile manipulation: in-hand reorientation, rotation, finger gaiting, regrasping, tool use, extrinsic dexterity
- non-prehensile manipulation: pushing, sliding, flipping, rolling, pivoting
- dynamic and agile manipulation: catching, throwing, juggling, pen spinning, high-frequency object motion
- complex and specialized tasks: bimanual dexterous manipulation and deformable object manipulation

Do **not** turn this section into a broad manipulation task dump. The hand-centric dexterity connection should be clear.

### Methodology

Include learning, planning, control, and data-pipeline methods that are important for dexterous manipulation:
- reinforcement learning and sim-to-real
- imitation learning, behavior cloning, action chunking, and diffusion policies
- VLA/foundation models used for dexterous or fine-grained manipulation
- trajectory optimization, MPC, kinematics, and motion planning
- teleoperation, glove/exoskeleton capture, robot-free teaching, passive video, and internet data extraction

### Infrastructure

Include reusable infrastructure:
- simulators and physics engines
- benchmark suites and datasets
- robot descriptions, assets, environments, data formats, and training/evaluation stacks

### Surveys & Reviews

Include survey papers, tutorials, taxonomies, and review-style resources that help readers understand dexterous manipulation, tactile sensing, grasping, or robot manipulation more broadly.

## Inclusion policy

The repository uses **core + strong adjacent** scope.

### Include first
- canonical dexterous manipulation papers and projects
- widely used dexterous hands, tactile sensors, and open hardware/software platforms
- datasets and benchmarks designed for hand-centric grasping, dexterous manipulation, tactile manipulation, or dexterous teleoperation
- methods demonstrated on dexterous hands, in-hand manipulation, bimanual dexterity, visuo-tactile manipulation, or contact-rich fine manipulation

### Include selectively
- general robot-learning policies when they are commonly used as dexterous manipulation baselines or infrastructure
- broad manipulation benchmarks when they include important dexterous-hand, tactile, deformable, or fine manipulation components
- humanoid manipulation work when dexterous-hand manipulation is a central contribution

### Usually exclude
- generic pick-and-place manipulation with weak dexterity relevance
- broad robot planning/control work that does not materially help dexterous manipulation
- unrelated industrial gripper resources without a clear dexterous or multi-finger angle
- unverified papers, rumor-like projects, or entries without a reliable public source

## Source priority

When adding or updating entries, use sources in this order:
1. official project page, official code repository, or official dataset page
2. arXiv, conference, journal, OpenReview, or proceedings page
3. lab/author pages
4. high-quality awesome lists named in the README acknowledgements
5. Google Scholar citation graph around canonical dexterous manipulation papers

If multiple sources disagree, prefer the most official public source.

## Verification rule for new entries

Do **not** add an entry unless it has a sufficiently reliable canonical public source.

Minimum bar for inclusion:
- a canonical paper URL such as arXiv / conference page / journal page / OpenReview page,
- and/or an official project page, dataset page, or GitHub repo from the authors / lab / organization.

If a candidate cannot be verified with enough confidence:
- do **not** add it to `README.md`
- do **not** guess missing metadata, URLs, venues, or affiliations
- do **not** include partially confirmed or rumor-like items just because they seem relevant

When in doubt, exclude first and wait for a reliable source.

## Entry format

Each subsection should use the same compact table schema:

| Date | Keywords | Institute (first) | Paper / Resource | Publication | Others |
| :--: | :------: | :---------------: | :--------------- | :---------: | :----: |

### Column rules

- `Date`: use `YYYY-MM-DD` whenever possible; use `YYYY-MM` or `YYYY` only when a canonical precise date is not public.
- `Keywords`: short tags only; keep them scannable.
- `Institute (first)`: first institution / lab / company only, concise and normalized.
- `Paper / Resource`: title linked to the canonical paper or resource URL.
- `Publication`: venue name such as `RSS 2024`, `CoRL 2023`, `arXiv`, `Website`, or `GitHub`.
- `Others`: compact links such as `github`, `project`, `dataset`, `hardware`, `docs`, `survey`.

## Sorting rules

- Sort every subsection by `Date` descending.
- Newer entries must appear above older ones.
- If only month or year is public, place the row consistently relative to other rows with known dates.

## Overlap policy

Controlled duplication is allowed.

Examples:
- a tactile dexterous-hand paper may appear in both `Hardware & Sensor Systems` and `Methodology`
- a method paper with a released benchmark may appear in both `Methodology` and `Infrastructure`
- a bimanual dexterity paper may appear in both task and method sections if both roles are important

When duplicating an entry:
- keep the metadata consistent across placements
- adjust `Keywords` only if needed to explain the local role
- do not create unnecessary variant titles

## Dataset metadata guidance

For dataset and benchmark entries, preserve as much of the following as possible in keywords or compact `Others` links:
- observations: RGB, depth, tactile, force/torque, proprioception, audio, point cloud, egocentric video
- action / embodiment: dexterous hand, bimanual, humanoid hand, multi-finger gripper, mobile manipulator
- format / access: HDF5, Zarr, MP4, LeRobot, HuggingFace, Google Drive, Box, raw logs
- scale: number of demonstrations, objects, tasks, environments, hours, or trajectories when the canonical source makes it explicit

Use compact summaries in the table itself and keep verbose explanation out of the main row.

## Maintenance workflow

When adding entries:
1. decide the primary section first
2. check whether the resource should also appear in a second section
3. normalize the six metadata columns
4. insert in descending date order
5. update the Table of Contents only if headings changed
6. keep the README readable; do not over-tag

When reorganizing:
- prefer adding or refining subsections over inventing many new top-level sections
- keep the user-approved top-level section names unchanged unless explicitly asked

## Commit conventions

Use Conventional Commits.

Recommended types for this repository:
- `docs:` content additions or edits in `README.md` / `AGENTS.md`
- `feat:` meaningful new section or structural capability in the awesome list
- `refactor:` taxonomy reorganization without changing the underlying factual content
- `fix:` broken links, date corrections, venue fixes, naming fixes, anchor fixes
- `chore:` maintenance-only cleanup

Recommended examples:
- `docs(agents): define dexterous manipulation curation rules`
- `docs(readme): add tactile sensors and dexterous hand systems`
- `refactor(readme): organize methods into learning control and data collection`
- `fix(readme): correct dexgraspnet metadata`

## What to avoid

- Do not add back the old UMI-specific scope or UMI-only taxonomy.
- Do not revert to a multi-file `contents/` structure.
- Do not add long prose summaries for every paper.
- Do not turn the repo into a general robot manipulation survey.
- Do not introduce inconsistent table schemas across sections.
- Do not add entries without checking their dexterous manipulation relevance.

## Quick checklist before finishing a change

- Is the entry clearly relevant to dexterous manipulation or strong adjacent infrastructure?
- Is it in the right section?
- Should it also appear in another section?
- Does the row use the six required columns?
- Is the date normalized and ordering reasonable?
- Are `Paper / Resource` and `Others` links canonical and working?
- Does the change preserve the single-README architecture?
