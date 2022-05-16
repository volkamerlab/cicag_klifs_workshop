# RCS CICAG workshop &mdash; KLIFS: making kinase structures work

Albert J. Kooistra, University of Copenhagen, Dominique Sydow & Andrea Volkamer, Charité – Universitätsmedizin Berlin

This repository contains the notebook shown in the context of the 2-hour hands-on RCS CICAG workshop on KLIFS, OpenCADD-KLIFS, and KiSSim.

- KLIFS &mdash; [website](https://klifs.net) and [paper](https://doi.org/10.1093/nar/gkaa895)
- OpenCADD-KLIFS &mdash; [code](github.com/volkamerlab/opencadd) and [paper](https://joss.theoj.org/papers/10.21105/joss.03951)
- KiSSim &mdash; [code](github.com/volkamerlab/kissim) and [paper](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.2c00050)

## Workshop

- [Event link](https://www.rsc.org/events/detail/73782/open-source-tools-for-chemists)
- When? 2022-05-19
- Where? Online

## Material

1. KLIFS database (Albert Kooistra): Presentation
2. KLIFS application (Andrea Volkamer): Presentation
3. KLIFS application (Dominique Sydow): [Notebook (Google Colab)](https://colab.research.google.com/github/volkamerlab/cicag_klifs_workshop/blob/main/klifs_workshop.ipynb)

If you prefer to run the notebook locally (instead of using Google Colab), follow these instructions:

```
git clone git@github.com:volkamerlab/cicag_klifs_workshop.git
cd cicag_klifs_workshop
mamba env create -f environment.yaml
conda activate cicag
jupyter lab
```

The notebook is a mix of the following TeachOpenCADD notebooks:
- [T012 · Data acquisition from KLIFS](https://projects.volkamerlab.org/teachopencadd/talktorials/T012_query_klifs.html)
- [T025 · Kinase similarity: Kinase pocket (KiSSim fingerprint)](https://projects.volkamerlab.org/teachopencadd/talktorials/T025_kinase_similarity_kissim.html)
- [T026 · Kinase similarity: Interaction fingerprints](https://projects.volkamerlab.org/teachopencadd/talktorials/T026_kinase_similarity_ifp.html)
- [T028 · Kinase similarity: Compare different perspectives](https://projects.volkamerlab.org/teachopencadd/talktorials/T028_kinase_similarity_compare_perspectives.html)

## Abstract

Over the past three decades, six thousand structures of the catalytic kinase domain have been made publicly available via the Protein Data Bank. But to what extent are we making use of this wealth of information? In order to harness this data in a better way and to make it readily available for all to use in their research, KLIFS was constructed. KLIFS, i.e. the Kinase–Ligand Interaction Fingerprints and Structures database, is a structural kinase database that systematically collects and processes all structures of the catalytic kinase domain. With the database, you can - for example - easily get a complete overview of all structures, search for ligands with a specific binding mode, identify analogs or your ligands of interest, collect data for your data mining and machine learning applications.

For this workshop, the developers of KLIFS have teamed up with the [Volkamer Lab](https://volkamerlab.org/) and therefore the workshop will be divided into two segments. First, Albert J. Kooistra will give an introduction to KLIFS and demonstrate different functionalities of the KLIFS website and the integration of KLIFS in KNIME via the [3D-e-Chem](https://dx.doi.org/10.1002%2Fcmdc.201700754) nodes. In the second half, Andrea Volkamer and Dominique Sydow will demonstrate, based on their new kinase-focused [TeachOpenCADD](https://projects.volkamerlab.org/teachopencadd/talktorials.html#kinase-similarity) workflow, how to assess kinase similarity from different data perspectives. They will emphasize their Python package [KiSSim](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.2c00050) – a KLIFS-based kinase structural similarity fingerprint, and [OpenCADD-KLIFS](https://joss.theoj.org/papers/10.21105/joss.03951) – a Python module to facilitate the integration of KLIFS data into kinase research workflows.