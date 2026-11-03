---
title: 'LexiCan: Lexicographic Canonicalization of Point Clouds for Machine Learning Applications'

authors:
  - Daniel Sanchez
  - Djordje Mihajlovic
  - Federica Valeau
  - Luka Benić
  - me
  - Soutrik Sarangi
  - Snir Hordan

date: '2026-10-10T00:00:00Z'
publishDate: '2026-10-10T00:00:00Z'

publication_types: ['article']

publication: '*arXiv preprint arXiv:2610.15171*'
publication_short: '*arXiv*'

abstract: 'Canonicalization resolves the rotational and permutation ambiguity of 3D point clouds by selecting a unique orbit representative, maintaining their geometric information while allowing standard architectures, such as Transformers, to operate on them. Existing canonicalizations, however, exhibit discontinuity jumps on molecular configurations and non-trivial invariance errors in popular molecular datasets, which lead to ambiguity in their representation. To bridge this gap, we introduce LexiCan, a canonicalization that is provably invariant under either $O(3)$ or $SO(3)$, empirically invariant to rotations to within $\sim 10^{-6}$ angstroms on the QM9 and QM-sym molecular datasets, and mitigates discontinuity jumps on QM-sym, while running orders of magnitude faster than an existing canonicalization. Finally, non-invariant models perform better on QM9 property prediction and ModelNet40 shape classification with LexiCan than with that canonicalization.'

summary: 'LexiCan is a fast, provably O(3)/SO(3)-invariant canonicalization of 3D point clouds. It lets standard, non-invariant architectures such as Transformers work on molecules and shapes without rotation or permutation ambiguity.'

tags:
  - Geometric Deep Learning
  - Canonicalization
  - Point Clouds
  - Molecular Machine Learning

featured: true

hugoblox:
  ids:
    arxiv: 2610.15171
    doi: 10.48550/arXiv.2610.15171

links:
  - type: preprint
    provider: arxiv
    id: 2610.15171
  - type: pdf
    url: https://arxiv.org/pdf/2610.15171

projects: []
slides: ''
---

## About the paper

A 3D point cloud, such as a molecule or a scanned shape, has no preferred orientation or point ordering. Rotate it or shuffle its points and it is still the same object. *Canonicalization* handles this by mapping every rotated and permuted copy to one unique representative. All the geometric information is kept, and standard architectures such as Transformers can then be used directly, with no need for specially built invariant networks.

**The problem.** Existing canonicalizations are not as clean as they should be. On molecular configurations they show *discontinuity jumps*, where a tiny change to the input causes a large change to the canonical form. They also show non-trivial invariance errors on popular molecular datasets. As a result, the "unique" representation is not actually unambiguous.

**LexiCan.** We introduce a lexicographic canonicalization that:

- is **provably invariant** under either O(3) or SO(3),
- is **empirically invariant** to rotations to within about 10⁻⁶ ångströms on the QM9 and QM-sym molecular datasets,
- **mitigates discontinuity jumps** on QM-sym,
- runs **orders of magnitude faster** than an existing canonicalization.

**Results.** Non-invariant models do better with LexiCan than with that existing canonicalization, both on QM9 molecular property prediction and on ModelNet40 shape classification.
