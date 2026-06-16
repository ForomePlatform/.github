<!--
  BOOK URL — single source of truth.
  The book is linked everywhere through the [book] reference label defined on
  the line below. To switch to your custom vanity URL later, change ONLY that
  one line. (This works because every book link in this file is Markdown, not
  raw HTML, so the [book] label resolves everywhere.)
-->
[book]: https://link.springer.com/book/10.1007/978-3-032-21032-6

# Forome Platform

## About the Forome Association

We are a team of experts in data management, governance, engineering, and
bioinformatics. We founded the **Forome Open Genomics** community to accelerate
Mendelian disease diagnostics and have since expanded our focus to making
research data trustworthy and verifiable for the age of AI. Our work spans
reproducible data engineering, data governance, population and environmental
health, clinical genomics, and semantic models of scientific evidence — and
everything we build is open source.

Learn more at the [Forome Association home page](https://forome.org/).

---

## Contents

On this page:

- [Dorieh](#dorieh) — an open-source platform for building reproducible,
  verifiable data pipelines — the foundation for trustworthy data in the age of AI.
- [Research Data that Can Be Trusted](#research-data-that-can-be-trusted) — our
  SpringerBriefs book that introduces the provenance framework behind Dorieh and
  applies it to healthcare claims data.
- [AnFiSA](#anfisa) — a fully open-source platform for variant curation in rare
  genetic disease, built for contributions from clinicians, researchers, and
  developers.
- [Research projects](#research-projects) — open research that underpins and
  extends our platforms, including a **semantic model of genetic evidence (GEM)**
  and **synthetic healthcare claims datasets** for testing provenance and
  data-quality methods.
---


---

## Dorieh

*Evidence-based data for evidence-based AI.*

[![PyPI version of the dorieh package](https://img.shields.io/pypi/v/dorieh)](https://github.com/ForomePlatform/dorieh)
[![Dorieh documentation](https://img.shields.io/badge/docs-foromeplatform.github.io-blue)](https://foromeplatform.github.io/dorieh/)

**[Dorieh](https://github.com/ForomePlatform/dorieh)** is our open-source
platform for building **reproducible, verifiable data pipelines** — the
foundation for trustworthy data in the age of AI.

As AI increasingly writes pipelines and models, the old basis for trust — having
a human read and understand the code — no longer scales. Dorieh shifts that
basis from *explain → understand* to *formalize → validate*: it makes
**what was actually done to the data** something a machine can check, on every
run.

It does this through **actionable provenance**:

- **Provenance** — structured, queryable records of what happened to the data,
  captured automatically as workflows execute (not static narrative PDFs).
- **Rules** — formal, machine-checkable predicates over those records, written to
  be read by clinicians, regulators, and governance experts, not only engineers.
- **Actions** — compliance attestations, audit trails, quality assertions, and
  drift alerts produced as outputs of the pipeline itself. Compliance stops being
  a document and becomes a query.

Under the hood, Dorieh runs portable workflows using the
[Common Workflow Language (CWL)](https://www.commonwl.org/) and Infrastructure
as Code, so results can be reproduced on confidential data by sharing
infrastructure rather than the data itself. It ships with production pipelines
for population and environmental health — CMS Medicare & Medicaid claims (via
ResDAC) and climate and air-pollution data — with built-in cleansing,
deduplication, and quality control.

**Explore:** [Documentation](https://foromeplatform.github.io/dorieh/) ·
[Repository](https://github.com/ForomePlatform/dorieh)

---

## Research Data that Can Be Trusted

*Our new book in the SpringerBriefs in Computer Science series (Springer
Nature, © 2026).*

[![Springer Nature banner for the book "Research Data that Can Be Trusted", showing the cover and title](images/SM_Image_Horizontal_978-3-032-21032-6.png)][book]

The [book behind Dorieh][book], by Michael Bouzinier, Dmitry Etin, Naeem
Khoshnevis, Max Shad, and Scott Yockel:

- argues for the need for a new approach to **data provenance**;
- introduces the concept of **descriptive dataflow operators**; and
- applies the framework to analyze **healthcare claims data quality**, revealing
  insights into inconsistencies and deficiencies.

[**Read it on Springer**][book] ·
[Download the flyer (PDF)](https://raw.githubusercontent.com/ForomePlatform/.github/main/profile/pdf/Flyer_978-3-032-21032-6.pdf)

*ISBN 978-3-032-21032-6 · DOI 10.1007/978-3-032-21032-6*

---

## AnFiSA

*Variant curation for rare genetic disease.*

**AnFiSA** is an established, fully open-source computational platform for the
analysis of sequencing data for **rare genetic disease** — a variant curation
tool designed to invite and accept contributions from clinicians, researchers,
and professional software developers.

Its design rests on three architectural principles:

- a **multidimensional DBMS** for genomic data to support reproducibility;
- **curated decision trees** adaptable to changing clinical rules; and
- a **crowdsourcing-friendly interface** for difficult-to-diagnose cases.

Read our research article in the *Journal of Biomedical Informatics*:

[![Graphical abstract of the AnFiSA research article in the Journal of Biomedical Informatics](https://ars.els-cdn.com/content/image/1-s2.0-S153204642200185X-ga1_lrg.jpg)](https://www.sciencedirect.com/science/article/abs/pii/S153204642200185X)

**Start using AnFiSA.** The [deploy repository](https://github.com/ForomePlatform/deploy)
is your starting point; the easiest way is to
[use docker-compose](https://github.com/ForomePlatform/deploy/blob/main/docker-compose/README.md).

**Key repositories:**
[Backend & REST API](https://github.com/ForomePlatform/anfisa) ·
[Frontend](https://github.com/ForomePlatform/Anfisa-React-Client) ·
[Deployment](https://github.com/ForomePlatform/deploy)

**Documentation:**
[User documentation](https://foromeplatform.github.io/documentation/anfisa-user.v0.7/) ·
[Development documentation](https://foromeplatform.github.io/documentation/anfisa-dev.v0.7/index.html)

---

## Research projects

Open research that underpins and extends our platforms:

**[genetic-evidence-model](https://github.com/ForomePlatform/genetic-evidence-model)**
— *A Semantic Model of Genetic Evidence.* A framework — SHACL shapes, a curated
annotation corpus, and versioned protocols — for representing genetic evidence
from the biomedical literature in a form suitable for variant interpretation,
automated reasoning, and AI-ready clinical infrastructure. Paper in submission.

**[synthetic-resdac-claims](https://github.com/ForomePlatform/synthetic-resdac-claims)**
(`synthmed`) — generates synthetic ResDAC / Medicare claims (MEDPAR, MBSF) as
FTS-conformant fixed-width files, rolling a synthetic beneficiary cohort forward
year by year with realistic data-quality errors injected. This allows Dorieh
pipelines to be developed and tested without confidential CMS data. Companion
dataset on [Zenodo](https://doi.org/10.5281/zenodo.18915558) (CC-BY-4.0);
methods paper in submission.

---

## Contribute or provide feedback

If you would like to participate in our projects, please reach out. We welcome
contributions from clinicians, researchers, and professional software
developers — including source code, documentation, Frequently Asked Questions,
and proposals for new use cases. We also value feedback on existing
functionality: please open a GitHub issue or contact us directly.

---

## Sponsors

Forome software development has been sponsored by a number of organizations,
including **Harvard University**, **IBM Cognitive Cloud** and the **IBM Chicago
Center for Advanced Studies**, **Quantori**, and others.

When developing Java code, we use the
[JProfiler Java profiler](https://www.ej-technologies.com/products/jprofiler/overview.html).
