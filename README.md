# 🌍 **Fractal Time Community**

![GAL-2 API Status](https://img.shields.io/endpoint?url=https://gal-2-technologies.github.io/fractal-time-community/status.json&label=GAL-2%20API&color=brightgreen)

### *Powered by GAL-2™ — Global Alignment Layer | Fractal Time*

[![FTS DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.17467893.svg)](https://doi.org/10.5281/zenodo.17467893)

---

## Current GAL-2 Implementation Status

**Fractal Time Community** preserves the public research lineage behind GAL-2™ and the Fractal Time thesis.

The current GAL-2 implementation separates the protected mathematical engine from the application-facing product surface:

**Reference inputs → Protected Core → GAL-2 Time → GAL-2 API → GAL-2 Node → Time Contract → enrolled application**

The **Protected Core** creates the GAL-2 Time trajectory.  
The **GAL-2 API** delivers GAL-2 Time.  
**GAL-2 Node** makes GAL-2 Time locally consumable.  
The **Time Contract** governs whether an enrolled application should consume it.

The current technical evaluation release is:

**GAL-2 Node v1.0.0-rc11**

Supported evaluation platforms:

- Linux ARM64
- macOS Apple Silicon

Founder-operated, real-duration **72-hour upstream-outage endurance runs** have been completed on both platforms.

Across the two runs, observed application-facing behavior included:

**LIVE → HOLDOVER → DEGRADED → FAIL_CLOSED → recovery to LIVE**

At hard-policy exhaustion, safe consumption was denied and the Provider refused GAL-2 Time consumption rather than silently falling back to raw host time.

No application-visible backward GAL-2 Time steps were observed in the tested trajectories.

### RC11 Public Evidence

**GAL-2 Node v1.0.0-rc11: Real-Duration 72-Hour Upstream-Outage Endurance Evidence on macOS Apple Silicon and Linux ARM64**

https://doi.org/10.5281/zenodo.22164457

This is founder-operated engineering evidence, not independent third-party validation, metrology certification, or a UTC-traceability claim.

Independent technical evaluators are invited to reproduce the RC11 failure scenario on hardware operated outside GAL-2 Technologies.

---

## Public Dataset & Verification

The full **7-day Solstice Run** dataset is publicly archived and citable.

Zenodo DOI:

https://doi.org/10.5281/zenodo.18018704

This dataset includes:

- 7-day uninterrupted software-only time continuity
- No GNSS, no atomic clocks, no PTP in the declared test configuration
- Raw CSVs, manifests, hashes, and methodology
- 508,548 observed samples
- No backward steps observed in the tested GAL-2 trajectory

Zenodo is the canonical source of record.

This repository references the dataset without duplicating it.

---

## 🚀 **Fractal Time Research**

**Fractal Time Community** is the public research hub for documenting, testing, discussing, and extending the **Fractal Time Standard (FTS)** research lineage behind GAL-2™.

The original Fractal Time thesis explores whether digital time can maintain a continuous mathematical relationship with the natural Earth-Sun temporal cycle while remaining useful to modern software systems.

Developed by **GAL-2 Technologies LLC** in Puerto Rico, this research later evolved into the current GAL-2 architecture, where the Protected Core, GAL-2 API, GAL-2 Node, and Time Contract have distinct operational roles.

The Fractal Time research thesis and the current GAL-2 product architecture should not be treated as interchangeable claims.

---

## 🧭 **Mission**

To investigate and develop a digital temporal framework that can remain connected to the natural Earth-Sun relationship while supporting continuity, resilience, and explicit application-side governance.

The broader research objective is to explore how software can consume time without treating every delivered timestamp as automatically safe application state.

In the current GAL-2 implementation, this operational idea is exposed through the **Time Contract**.

---

## 🕰️ **Why It Matters**

Modern digital infrastructure depends on time for:

- transaction ordering
- distributed-system coordination
- authentication and expiration
- logs and audit trails
- databases and committed state
- telecommunications
- financial systems
- blockchain and distributed ledgers
- AI and automated workflows
- industrial and critical infrastructure

Existing technologies such as UTC, GNSS, PTP, NTP, chrony, atomic clocks, grandmasters, timing receivers, and operating-system clocks remain essential parts of modern timing infrastructure.

GAL-2 does not claim to replace them.

The GAL-2 research and product thesis addresses a different question:

**What should an application do when delivered time can no longer be safely trusted or consumed under declared policy?**

GAL-2 adds an application-facing temporal governance boundary between delivered time and committed software state.

**Keep your timing stack. GAL-2 governs whether applications should consume time.**

---

## 🧬 **Fractal Time Thesis**

The original Fractal Time research explores a mathematical approach to digital time that is intended to remain connected to the natural duration and progression of the Earth-Sun temporal relationship.

Among the research questions explored by the project are:

- continuous digital-time progression
- long-duration temporal stability
- solar alignment
- behavior across civil-time discontinuities
- leap-second handling
- application-safe temporal consumption
- resilient behavior during upstream loss

These remain distinct research and engineering questions.

Public experiments and datasets should be interpreted according to the scope and methodology declared in each individual record.

The proprietary mathematical implementation used by the GAL-2 Protected Core is **not published in this repository**.

---

## 📜 **Core Documents**

| Document | Description |
|-----------|-------------|
| **RFC-FTS-0001.txt** | *Fractal Time Standard (FTS), Public Draft v1.0* — [DOI: 10.5281/zenodo.17467893](https://doi.org/10.5281/zenodo.17467893) |
| **PUBLIC_DISCLOSURE_NOTICE.txt** | *Public disclosure notice for the material contained in this repository* |
| **24h Public Metrics** | [DOI: 10.5281/zenodo.17522023](https://doi.org/10.5281/zenodo.17522023) |
| **Historical 72h Stability Evidence** | [DOI: 10.5281/zenodo.17450086](https://doi.org/10.5281/zenodo.17450086) |
| **Solstice 7D Dataset** | [DOI: 10.5281/zenodo.18018704](https://doi.org/10.5281/zenodo.18018704) |
| **5-Day Time Contract Adversarial Characterization** | [DOI: 10.5281/zenodo.20357131](https://doi.org/10.5281/zenodo.20357131) |
| **RC4 120-Hour Time Contract Characterization** | [DOI: 10.5281/zenodo.20582981](https://doi.org/10.5281/zenodo.20582981) |
| **RC5.1 Public Evaluator Evidence** | [DOI: 10.5281/zenodo.20646973](https://doi.org/10.5281/zenodo.20646973) |
| **RC11 Cross-Platform 72h Endurance Evidence** | [DOI: 10.5281/zenodo.22164457](https://doi.org/10.5281/zenodo.22164457) |

---

## 🧪 **Validation & Research**

GAL-2 maintains a growing public evidence lineage covering different parts of the research and product architecture.

### Historical 72-Hour Experiment

The historical 72-hour record reports **0.000 ms deviation over 259,200 seconds** under its declared experiment and measurement method on macOS / Python 3.13.

That result should be interpreted within the methodology and claim boundary of the archived record rather than as a universal metrology guarantee.

Evidence:

https://doi.org/10.5281/zenodo.17450086

### Solstice 7D

The Solstice 7D run observed **508,548 samples across seven days** and recorded no backward steps in the tested GAL-2 trajectory.

Evidence:

https://doi.org/10.5281/zenodo.18018704

### Time Contract Evidence

Later public work expanded beyond trajectory continuity into application-facing temporal governance, including:

- `safe_to_consume`
- bounded HOLDOVER
- DEGRADED operation
- controlled recovery
- FAIL_CLOSED
- monotonic publication
- source lineage
- explicit refusal instead of silent raw host-time fallback

Relevant public records include:

- 5-Day Adversarial Characterization  
  https://doi.org/10.5281/zenodo.20357131

- RC4 120-Hour Time Contract Characterization  
  https://doi.org/10.5281/zenodo.20582981

### GAL-2 Node RC11

The current GAL-2 Node v1.0.0-rc11 has completed founder-operated real-duration 72-hour upstream-outage endurance runs on:

- macOS Apple Silicon
- Linux ARM64

The public record includes machine-readable datasets, controller events, integrity material, observer/fault-injection tooling, platform evidence, and cryptographic hashes.

Evidence:

https://doi.org/10.5281/zenodo.22164457

These results are **founder-operated engineering evidence**.

The next evidence step is independent reproduction by operators using hardware and environments outside GAL-2 Technologies.

---

## 🧠 **How to Contribute**

Fractal Time Community remains open to reproducibility work, technical discussion, comparative experiments, and independently generated evidence.

Possible contributions include:

1. Fork this repository.
2. Review the public research documents and datasets.
3. Run independent continuity or comparative timing experiments using clearly documented methodology.
4. Publish raw results, environment details, hashes, and methodology.
5. Submit a Pull Request under `/community_results` where appropriate.
6. Clearly distinguish independently reproduced results from GAL-2 founder-operated results.

For GAL-2 Node RC11 evaluation, use the current product and evaluator information available through the official GAL-2 site.

Accepted community submissions may be referenced in the public validation lineage when their methodology and provenance are sufficiently documented.

---

## 🔐 **Protected Core and IP Boundary**

This repository does **not** publish the proprietary GAL-2 Protected Core, Fractal Time formula, private production source code, API credentials, signing secrets, or other protected implementation material.

The public research record is intended to make claims, interfaces, datasets, methodologies, and observable behavior inspectable without requiring disclosure of the Protected Core.

Publication of evidence does not imply publication of the underlying proprietary mathematical implementation.

---

## 🌐 **Connect**

🌎 **Official Site:** [https://www.gal-2.com](https://www.gal-2.com)

🧩 **GAL-2 Node:** [https://www.globalalignmentlayer.com/evaluate](https://www.globalalignmentlayer.com/evaluate)

📚 **Documentation:** [https://www.globalalignmentlayer.com/documentation](https://www.globalalignmentlayer.com/documentation)

🧪 **Public Validation:** [https://www.globalalignmentlayer.com/validation](https://www.globalalignmentlayer.com/validation)

🔬 **RC11 72h Evidence:** [https://doi.org/10.5281/zenodo.22164457](https://doi.org/10.5281/zenodo.22164457)

📘 **Historical Zenodo Evidence:** [https://zenodo.org/records/17450086](https://zenodo.org/records/17450086) | [https://zenodo.org/records/17522023](https://zenodo.org/records/17522023) | [https://zenodo.org/records/18018704](https://zenodo.org/records/18018704)

📧 **Contact:** support@gal-2.com

💠 **Repository:** [github.com/gal-2-technologies/fractal-time-community](https://github.com/gal-2-technologies/fractal-time-community)

---

## ⚖️ **License and Intellectual Property**

Materials in this repository that are expressly distributed under the **MIT License** are governed by the terms of that license.

The MIT License applies only to material actually included in this repository and covered by that license.

No license is granted by this repository to:

- GAL-2™ trademarks
- patents or patent applications
- trade secrets
- the GAL-2 Protected Core
- the proprietary Fractal Time formula
- proprietary algorithms not published here
- GAL-2 Node or other software not expressly distributed under the repository license
- commercial services or production infrastructure operated by GAL-2 Technologies LLC

Use of GAL-2 products, services, protected technology, or separately licensed software may require separate authorization or commercial terms from **GAL-2 Technologies LLC**.

---

## 🪐 **Vision**

> “We are not changing time —  
> we are restoring its harmony.”  
>
> — **Francisco E. Torres Alvarado (El 5 Viviente)**  
> *Founder & Creator of GAL-2™*

---

© 2025–2026 **GAL-2 Technologies LLC** — All Rights Reserved.  
*Global Alignment Layer | Fractal Time*

---

## 📖 **Citation**

For the original Fractal Time Standard public draft, cite:

**Torres Alvarado, Francisco E. (2025).**  
*RFC-FTS-0001 — Fractal Time Standard (FTS) v1.0 — Powered by GAL-2™.*  
**GAL-2 Technologies LLC**, San Juan, Puerto Rico.  
Version DOI: [10.5281/zenodo.17467893](https://doi.org/10.5281/zenodo.17467893)

For the current GAL-2 Node RC11 endurance evidence, cite the corresponding Zenodo record:

**GAL-2 Node v1.0.0-rc11: Real-Duration 72-Hour Upstream-Outage Endurance Evidence on macOS Apple Silicon and Linux ARM64**

DOI: [10.5281/zenodo.22164457](https://doi.org/10.5281/zenodo.22164457)

> “We’re not changing time — we’re realigning it with creation.”  
> — *Francisco E. Torres Alvarado (El 5 Viviente)*
