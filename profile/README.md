<!--
  BOOK URL — single source of truth.
  The book is linked everywhere through the [book] reference label defined on
  the line below. To switch to your custom vanity URL later, change ONLY that
  one line. (This works because every book link in this file is Markdown, not
  raw HTML, so the [book] label resolves everywhere.)
-->
[book]: https://link.springer.com/book/10.1007/978-3-032-21032-6

# Forome Platform

*Evidence-based data for evidence-based AI — open-source platforms for research data you can trust and verify.*

---

## About the Forome Association

We are a team of data management experts and bioinformaticians who founded the
**Forome Open Genomics** community to accelerate Mendelian disease diagnostics.
Our work spans reproducible data engineering, population and environmental
health, and clinical genomics — and everything we build is open source.

Learn more at the [Forome Association home page](https://forome.org/).

---

## Dorieh — evidence-based data for evidence-based AI

[![PyPI version of the dorieh package](https://img.shields.io/pypi/v/dorieh)](https://github.com/ForomePlatform/dorieh)
[![Dorieh documentation](https://img.shields.io/badge/docs-foromeplatform.github.io-blue)](https://foromeplatform.github.io/dorieh/)

**[Dorieh](https://github.com/ForomePlatform/dorieh)** is our open-source platform
for building **reproducible, verifiable data pipelines** — the foundation for
trustworthy data in the age of AI.

As AI increasingly writes the pipelines and the models, the old basis for trust —
a human reads the code and understands it — no longer scales. Dorieh shifts the
basis of trust from *explain → understand* to *formalize → validate*: it makes
**what was actually done to the data** something a machine can check, on every run.

It does this through **actionable provenance**:

- **Provenance** — structured, queryable records of what happened to the data,
  captured automatically as workflows execute (not narrative PDFs).
- **Rules** — formal, machine-checkable predicates over those records, written to
  be read by clinicians, regulators, and governance experts, not only engineers.
- **Actions** — compliance attestations, audit trails, quality assertions, and
  drift alerts produced as outputs of the pipeline itself. Compliance stops being
  a document and becomes a query.

Under the hood, Dorieh runs portable workflows on the
[Common Workflow Language (CWL)](https://www.commonwl.org/) with an
Infrastructure-as-Code deployment, so results can be reproduced on confidential
data by sharing infrastructure rather than data. It ships production pipelines for
population and environmental health — CMS Medicare & Medicaid claims (via ResDAC),
climate and air-pollution data — with built-in cleansing, deduplication, and
quality control.

**Explore:** [Documentation](https://foromeplatform.github.io/dorieh/) ·
[Repository](https://github.com/ForomePlatform/dorieh) ·
[synthetic-resdac-claims](https://github.com/ForomePlatform/synthetic-resdac-claims)
— synthetic CMS/ResDAC claims data to test pipelines without real PHI.

---

## Featured book — Research Data that Can Be Trusted

[![Springer Nature banner for the book "Research Data that Can Be Trusted", showing the cover and title](images/SM_Image_Horizontal_978-3-032-21032-6.png)][book]

***[Research Data that Can Be Trusted][book]*** (SpringerBriefs in Computer
Science, Springer Nature, 2026) is the book behind Dorieh, by Michael Bouzinier,
Dmitry Etin, Naeem Khoshnevis, Max Shad, and Scott Yockel. It:

- argues for the need for a new approach to **data provenance**;
- introduces the novel approach of **descriptive dataflow operators**; and
- applies the framework to analyze **healthcare claims data quality**, revealing
  insights into inconsistencies and deficiencies.

[**Read it on Springer**][book] ·
[Download the flyer (PDF)](https://raw.githubusercontent.com/ForomePlatform/.github/main/profile/pdf/Flyer_978-3-032-21032-6.pdf)

*ISBN 978-3-032-21032-6 · DOI 10.1007/978-3-032-21032-6*

---

## AnFiSA — variant curation for rare genetic disease

**AnFiSA** is an established, fully open-source computational platform for the
analysis of sequencing data for **rare genetic disease** — a variant curation
tool built to invite and accept contributions from clinicians, researchers, and
professional software developers.

Its design rests on three architectural principles:

- a **multidimensional DBMS** for genomic data, to address reproducibility;
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

## Contribute or provide feedback

If you would like to participate in our projects, please reach out. We invite and
accept contributions from clinicians, researchers, and professional software
developers — as source code, documentation, Frequently Asked Questions, and
proposals for new use cases. We also value feedback on existing functionality —
please open a GitHub issue or contact us directly.

---

## Sponsors

Forome software development has been sponsored by a number of organizations,
including **Harvard University**, **IBM Cognitive Cloud** and the **IBM Chicago
Center for Advanced Studies**, **Quantori**, and others.

When developing Java code, we use the
[JProfiler Java profiler](https://www.ej-technologies.com/products/jprofiler/overview.html).
