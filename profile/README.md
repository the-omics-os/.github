<div align="center">
  <img alt="Omics-OS Banner" src="https://raw.githubusercontent.com/the-omics-os/lobster/main/docs/assets/banner.png" width="700">
</div>

<br/>

<div align="center">
  <strong>Multi-omics data infrastructure for foundation models & biotech</strong>
  <br/><br/>
  <a href="https://omics-os.com"><img src="https://img.shields.io/badge/omics--os.com-000000?style=for-the-badge&logo=globe&logoColor=white" alt="Website"></a>
  <a href="https://docs.omics-os.com"><img src="https://img.shields.io/badge/docs-omics--os.com-1a1a2e?style=for-the-badge&logo=readthedocs&logoColor=white" alt="Docs"></a>
  <a href="https://app.omics-os.com"><img src="https://img.shields.io/badge/cloud-Omics--OS-0066cc?style=for-the-badge&logo=googlecloud&logoColor=white" alt="Cloud"></a>
  <a href="https://pypi.org/project/lobster-ai/"><img src="https://img.shields.io/badge/PyPI-lobster--ai-3775A9?style=for-the-badge&logo=pypi&logoColor=white" alt="PyPI"></a>
</div>

<br/>

---

We build the **data infrastructure layer** that sits between raw multi-omics experiments and downstream AI/ML models. Our tools handle the hardest part of computational biology: gathering heterogeneous datasets, preprocessing them correctly, harmonizing across platforms, and tracking provenance — so scientists can focus on discovery.

<br/>

## Our Stack

<table width="100%">
  <thead>
    <tr>
      <th align="left" width="200">Project</th>
      <th align="left">Description</th>
      <th align="center" width="100">Status</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td><a href="https://github.com/the-omics-os/lobster"><b>Lobster AI</b></a></td>
      <td>Open-source multi-agent bioinformatics engine — 22 specialist agents across 10 packages, orchestrated by LangGraph. Handles scRNA-seq, bulk RNA-seq, proteomics, genomics, metabolomics, and more via natural language.</td>
      <td align="center"><img src="https://img.shields.io/badge/-public-2ea44f?style=flat-square" alt="public"></td>
    </tr>
    <tr>
      <td><b>Omics-OS Cloud</b></td>
      <td>Managed platform with LLM gateway, cloud compute, and team collaboration. Same Lobster engine, zero infrastructure to manage. Deploy on AWS with a single CDK stack.</td>
      <td align="center"><img src="https://img.shields.io/badge/-private-6c757d?style=flat-square" alt="private"></td>
    </tr>
    <tr>
      <td><b>BioVault</b></td>
      <td>Decision-grade evidence cards for wet-lab scientists. Ask a biological question, get a structured answer backed by curated data — gene functions, disease associations, pathway context.</td>
      <td align="center"><img src="https://img.shields.io/badge/-private-6c757d?style=flat-square" alt="private"></td>
    </tr>
    <tr>
      <td><b>Omics-OS Docs</b></td>
      <td>Full documentation — architecture, tutorials, API reference, case studies. 111 MDX pages powered by Fumadocs.</td>
      <td align="center"><img src="https://img.shields.io/badge/-private-6c757d?style=flat-square" alt="private"></td>
    </tr>
  </tbody>
</table>

<br/>

## What Lobster AI Does

```bash
pip install lobster-ai && lobster init && lobster chat
```

Then describe your analysis in plain language:

```text
> Search PubMed for single-cell CRISPR screens in T cells from 2023–2024,
  download the most cited dataset, run QC, integrate batches with Harmony,
  cluster the cells, annotate cell types, and export a reproducible notebook.
```

Every step produces **W3C-PROV provenance** and can be exported as a **reproducible Jupyter notebook**.

<br/>

## Domains Covered

| Domain | Key Capabilities |
|--------|-----------------|
| **Single-Cell RNA-seq** | QC, doublet detection, batch integration (Harmony/scVI), clustering, cell type annotation, trajectory inference |
| **Bulk RNA-seq** | Normalization, differential expression (PyDESeq2), GSEA, publication-ready export |
| **Clinical Genomics** | VCF/PLINK, GWAS, variant annotation (VEP), pathogenicity scoring |
| **Mass Spec Proteomics** | MaxQuant/DIA-NN/Spectronaut, PTM analysis, batch correction, biomarker panel selection |
| **Affinity Proteomics** | Olink NPX/SomaScan ADAT/Luminex MFI, LOD quality, bridge normalization |
| **Metabolomics** | LC-MS/GC-MS/NMR, PCA/PLS-DA/OPLS-DA, m/z annotation (HMDB/KEGG) |
| **Machine Learning** | Feature selection, survival analysis, cross-validation, SHAP, multi-omics integration (MOFA) |
| **Literature & Data** | PubMed/GEO/PRIDE/MetaboLights search, dataset download, metadata harmonization |

<br/>

## For AI Coding Agents

Install skills that give Claude Code, Cursor, or Gemini CLI deep knowledge of the Lobster architecture:

```bash
curl -fsSL https://skills.lobsterbio.com | bash
```

This installs `lobster-use` (analysis workflows) and `lobster-dev` (agent development). Your coding agent understands the full 10-package structure, tool patterns, and AQUADIF contract — without reading source code manually.

<br/>

## Architecture

<div align="center">
  <img alt="Ecosystem Topology" src="https://raw.githubusercontent.com/the-omics-os/lobster/main/docs/assets/architecture-topology.svg" width="85%">
</div>

<br/>

## Links

| | |
|---|---|
| **Website** | [omics-os.com](https://omics-os.com) |
| **Documentation** | [docs.omics-os.com](https://docs.omics-os.com) |
| **Cloud Platform** | [app.omics-os.com](https://app.omics-os.com) |
| **PyPI** | [pypi.org/project/lobster-ai](https://pypi.org/project/lobster-ai/) |
| **Coding Agent Skills** | [skills.lobsterbio.com](https://skills.lobsterbio.com) |
| **Contact** | kevin.yar@omics-os.com |

<br/>

<div align="center">
  <sub>Built in Switzerland by <a href="https://omics-os.com">Omics-OS</a> — saving the world, one dataset at a time.</sub>
</div>
