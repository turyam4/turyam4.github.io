---
title: 'Beyond Homology: Non-Abelian and Orientability Invariants Sensitivity in Cellular Networks'

authors:
  - me
  - George Panagopoulos
  - Jun Pang

date: '2026-10-22T00:00:00Z'
publishDate: '2026-10-22T00:00:00Z'

publication_types: ['article']

publication: '*arXiv preprint arXiv:2610.31234*'
publication_short: '*arXiv*'

abstract: 'Topological deep learning (TDL) architectures are typically evaluated on synthetic complex pairs that differ in a target invariant. Yet, whether a model recovers that invariant or an artifact of the chosen discretization is seldom audited. To examine this, we design and test pairs of complexes that look identical to standard homological and local message-passing tests, have the same Hasse graphs, yet differ in the target invariant. We study two beyond-homology regimes: nonAbelian fundamental-group structure and homotopy-matched orientability. For the former, we construct genus-2 pairs that match homology, cell statistics, local incidence profiles, and rank-colored Hasse 1-WL behavior while differing in their fundamental groups. For the latter, we evaluate punctured torus-Klein bottle pairs and show that distance, boundary, cycle, and spectral signals can confound apparent orientability detection, motivating stronger matched controls. Under the tested settings, subcomplex-lifted architectures separate some pairs beyond the matched homological, local-incidence, and Hasse 1-WL controls, while a depth sweep reveals an empirical depth-dependent trend without establishing a general barrier or direct computation of the target invariants. These results show that claims of topological expressivity must be stated relative to the model representation, explicitly controlled information channels, and the precise scope of the benchmark.'

summary: 'Can topological deep learning models detect invariants beyond homology, such as non-Abelian fundamental groups and orientability? We build matched pairs of cell complexes that look identical to standard homological and local message-passing tests, and audit what these models actually pick up.'

tags:
  - Topological Deep Learning
  - Cellular Networks
  - Algebraic Topology
  - Expressivity

featured: true

hugoblox:
  ids:
    arxiv: 2610.31234
    doi: 10.48550/arXiv.2610.31234

links:
  - type: preprint
    provider: arxiv
    id: 2610.31234
  - type: pdf
    url: https://arxiv.org/pdf/2610.31234

projects: []
slides: ''
---

## About the paper

Topological deep learning (TDL) models are often said to "see" topology. Usually this is shown on synthetic pairs of complexes that differ in some target invariant. But a model that separates such a pair may not be recovering the invariant at all. It may be exploiting an artifact of how the spaces were discretized. This paper sets out to audit that gap.

**The approach.** We build *matched* pairs of cell complexes that look identical to standard tests: they share homology, have the same Hasse graphs, and cannot be told apart by homological or local message-passing checks. Even so, they differ in a topological invariant that goes beyond homology. Two regimes are studied:

- **Non-Abelian fundamental-group structure.** These are genus-2 pairs that match in homology, cell statistics, local incidence profiles and rank-colored Hasse 1-WL behavior, but have different fundamental groups.
- **Homotopy-matched orientability.** These are punctured torus vs. Klein bottle pairs. Here we show that distance, boundary, cycle and spectral signals can create the *appearance* of orientability detection, so stronger matched controls are needed.

**What we find.** Under the tested settings, subcomplex-lifted architectures do separate some pairs beyond the matched homological, local-incidence and Hasse 1-WL controls. A sweep over network depth shows an empirical depth-dependent trend. This result does not establish a general barrier, and it does not mean the models compute the invariants directly.

**Takeaway.** A claim of topological expressivity is meaningful only when stated relative to three things: the model's representation, the information channels that are explicitly controlled, and the precise scope of the benchmark.
