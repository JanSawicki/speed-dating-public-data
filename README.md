# Speed-dating simulation: saved results

This repository contains saved synthetic outputs and derived results used in the exploratory study “Self-Presentation in LLM-Based Social Simulation: A Controlled Matching Experiment.” The simulation code and configuration are maintained separately in [speed-dating-public-code](https://github.com/JanSawicki/speed-dating-public-code).

The experiment contains 1,080 generated conversations: three model endpoints × ten designed attendee profiles × four instruction levels × three hobby-overlap conditions × three repetitions. All conversations and profiles are synthetic; no human participants or personal records are included. These saved outputs let readers inspect the results without rerunning mutable hosted model endpoints.

## Contents

- data/state/: serialized profiles, conversations, recipient scores, and aggregate claim counts, organized by generating model.
- data/cache/: structured request and response records for recipient scoring and claim coding. These preserve the model inputs and parsed outputs used in the analysis. Redundant raw invocation caches are omitted.
- data/jasss_cross_scoring/: request and response records for the fixed-transcript scoring sensitivity analysis. Gemini and GPT rescored the same 108 sampled transcripts; the requested Claude scorer was unavailable.
- data/charts/: aggregate result tables and figures from the original analysis.
- derived/: conversation-level measures and cell summaries, score-alignment audit, cross-scorer results, and LLM-judge agreement summaries reported in the manuscript.
- config.yaml: experiment prompts, profile definitions, model identifiers, and run settings.

Original compatibility-score identifiers were checked against exact cached requests. This confirms record alignment; it does not validate model judgments. Six malformed participant-model claim checklists are excluded from the LLM-to-LLM agreement summary. Agreement between automated judges is not evidence of human-level accuracy. No human annotation results are included.

## Reproducing the analysis

The source repository contains the simulation and analysis code. Use the saved states and structured caches here as input data. The derived/ directory contains the conversation-level CSV files, cell summaries, and JSON audit records used by the manuscript. Regenerating conversations through hosted APIs is separate from reproducing analyses from saved outputs and may produce different results as model endpoints change.

Model-call collection dates and immutable provider snapshots were not recoverable from the saved records. The additional Gemini/GPT fixed-transcript ratings were generated on 5 November 2026. The Claude cross-scoring endpoint returned a not-found error; no substitute model was used.

## Version and citation

This repository is versioned with Git. The initial public snapshot is release v1.0.0: https://github.com/JanSawicki/speed-dating-public-data/tree/v1.0.0. Cite this release tag or commit used in your analysis alongside the paper citation. The public-code repository contains the implementation; this repository contains saved outputs and derived data.

No separate data license is asserted here. The outputs are generated from third-party model services; consult their applicable terms when reusing them.
