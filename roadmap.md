# Roadmap

This document outlines the planned development of the **Sound, Resonance & Acoustic Violence Taxonomy**. It is a living, community‑driven roadmap – priorities and timelines may shift based on contributor interest, funding, and world events. Check marks indicate completed milestones.

---

## Version 2.1 – Scientific Rigour & Citations

**Goal:** Transform the glossary into a citable reference work.

- [ ] **Citation database**  
  Link each term to at least one authoritative source:
  - ISO standards (e.g., ISO 1996, ISO 9612)
  - WHO Environmental Noise Guidelines
  - Peer‑reviewed journals (Journal of the Acoustical Society of America, Noise & Health, etc.)
  - Official government reports (NIOSH, OSHA, EU‑OSHA, CTBTO)
  - Legal cases and treaties (ECHR rulings, ICC evidence)
  - Implement as a machine‑readable `citations.json` with DOI, title, and relevance fields.

- [ ] **Confidence level tagging for all entries**  
  Formalise the existing informal tags (e.g., “weak evidence”, “active investigation”) using a simple schema:
  - ✅ **Established** – robust, replicated evidence
  - ⚠️ **Plausible** – some evidence, but not conclusive
  - ❌ **Unsubstantiated** – widely circulated but scientifically unsupported
  - 🔍 **Under investigation** – active research or official inquiry

---

## Version 2.2 – Case Studies & Real‑World Context

**Goal:** Ground abstract concepts in documented incidents.

- [ ] **Case study snapshots**  
  Mini‑essays (500–1000 words) embedded in the `resources/case-studies/` directory, covering:
  - Havana Syndrome timeline and scientific investigations
  - LRAD deployment at protests (e.g., G20 Pittsburgh 2009, Ferguson 2014)
  - Low‑frequency hum complaints (Bristol, Taos, Windsor)
  - Use of noise/music as torture (Abu Ghraib, Guantánamo)
  - Stuka dive bomber Jericho trumpets as psychological warfare
  - Each snapshot includes cross‑links to taxonomy terms and citation references.

- [ ] **Timeline of acoustic weapon development**  
  An interactive timeline (later) or a static markdown chronology from ancient sound‑based intimidation to modern directed energy research.

---

## Version 2.3 – Usability & Interconnection

**Goal:** Make the taxonomy faster to navigate and easier to contribute to.

- [ ] **Glossary aliases & synonyms**  
  Support multiple common terms (e.g., “sound cannon” → Sonic Cannon, “vibroacoustic disease” → Vibroacoustic Disease). Implement in a `aliases.yaml` and integrate into a search index.

- [ ] **Auto‑generated connections mind map**  
  Use Mermaid or Graphviz to produce a visual graph of all cross‑links between terms, updated on each commit. Embeddable in the repository README.

- [ ] **Contribution‑friendly templates**  
  Add issue templates and a pull request checklist that guide new contributors to provide definitions, evidence levels, and references.

---

## Version 2.5 – Web Exploration & Interactivity

**Goal:** Make the taxonomy accessible to non‑technical users, journalists, and policymakers.

- [ ] **Interactive web explorer**  
  A single‑page application (or static site) allowing users to:
  - Filter terms by category, frequency range, evidence level
  - See immediate connections and related terms
  - Toggle between a glossary and a frequency‑spectrum overlay

- [ ] **Frequency spectrum visualisation**  
  A horizontal axis from 0 Hz to >20 kHz, with coloured bands indicating perception thresholds, health risk zones, weapon effects, and animal hearing ranges. Terms like “Infrasound”, “Ultrasound”, “Tinnitus induction” placed appropriately.

- [ ] **API endpoint**  
  Serve the taxonomy as a RESTful JSON API:
  - `GET /terms` with query parameters
  - `GET /terms/:id`
  - Auto‑generated OpenAPI documentation

---

## Version 3.0 – Global Reach & Accessibility

**Goal:** Translate the resource and create derivative works for different audiences.

- [ ] **Multilingual translations**  
  Community‑validated translations to Spanish, French, Arabic, Chinese, and others. Translation files in `i18n/` with CI checks for completeness.

- [ ] **Simplified “Quick Guide”**  
  A 2‑page PDF/HTML primer for journalists, human rights defenders, and legal aid groups, covering:
  - Basic definitions of acoustic violence and harassment
  - Health effects summary
  - Legal frameworks in plain language
  - What to do if you’re targeted

- [ ] **Audio examples library**  
  Short, safe‑to‑listen clips (<15s, level‑limited) demonstrating:
  - Beating frequencies
  - Shepard tone illusion
  - Infrasonic hum (safe levels)
  - White/pink noise and masking
  - Sound of an LRAD alert tone (attenuated)
  - All examples accompanied by clear warnings and context.

---

## Ongoing & Long‑Term Initiatives

These are evergreen tasks, not tied to a single release.

### Research & Monitoring
- [ ] **Living systematic review**  
  Automated search (via RSS, PubMed, Scopus) for new publications on:
  - Acoustic weapons
  - Infrasound health effects
  - Low‑frequency noise syndrome
  - Havana Syndrome updates
  New findings are triaged and added to the citation database and case studies.

- [ ] **Havana Syndrome reference hub**  
  A dedicated, updated timeline collecting all government reports, peer‑reviewed papers, and media investigations. Maintained as a sub‑project.

### Policy & Advocacy
- [ ] **Model legislation comparison**  
  A table tracking noise ordinances, sonic weapon regulations, and acoustic privacy laws across jurisdictions (federal, state, international). Useful for policy research and advocacy.

- [ ] **Human rights documentation toolkit**  
  Guidelines for documenting sound‑based harassment or torture for use in legal proceedings and human rights reports.

---

## How to Contribute to the Roadmap

We welcome proposals for new features, re‑prioritisations, or even entirely new roadmap items. Open a discussion in the repository’s **Issues** tab with the label `roadmap`. Please describe the problem your idea solves and, if possible, suggest how it could be implemented.

The roadmap will be reviewed quarterly by maintainers, with community input gathered via polls and discussions.
