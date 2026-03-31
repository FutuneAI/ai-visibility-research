# Entity Layer Construction: A Structured Reference

**Document:** `entity-layer-framework.md`  
**Series:** AI Visibility for Chinese Brands — Note 05  
**Status:** Published  
**Last updated:** 2026-03

---

## Abstract

This document provides a structured reference for building an English-language entity layer from a state of Complete Absence or Fragmented Presence. It covers platform selection rationale, content structure requirements, publication sequencing, and the distinct roles of a brand's own website and social media channels.

This document is designed to be read alongside the diagnostic framework in [`ai-visibility-diagnostic.md`](./ai-visibility-diagnostic.md). The diagnostic identifies which state a brand is in; this document provides the construction protocol for brands in Pattern A (Complete Absence) and early Pattern B (Fragmented Presence).

For the analytical narrative version of this content, see: [Medium — Part 05](https://medium.com/@futuneai)

---

## Core Premise

AI systems form entity concepts through pattern recognition across training data — not through real-time retrieval. A brand's visibility in AI-generated answers is determined by whether stable, consistent, independently sourced descriptions of that brand exist in the corpora these systems were trained on.

Building an entity layer is the process of creating that stable, consistent, independently sourced presence in the locations AI training pipelines draw from.

---

## Platform Selection

Not all web content carries equal weight in AI entity formation. The table below reflects observed signal weight based on platform inclusion patterns in major AI training datasets.

| Platform | Signal Weight | Primary Mechanism | Notes |
|----------|--------------|-------------------|-------|
| GitHub (README, reference docs) | High | Structured machine-readable content; high technical trust | Most effective for entity definition documents and structured knowledge |
| Medium (long-form analysis) | High | Above-average training dataset inclusion rates for long-form indexed content | Narrative authority layer; more effective than self-hosted blog |
| Quora (answers) | High | Direct source for retrieval-augmented systems (Perplexity) | Q&A format maps directly to how RAG systems generate recommendations |
| LinkedIn Articles | Medium-High | Indexed as standalone documents; professional-context authority | Distinct from LinkedIn posts — see Social Media section below |
| Third-party editorial | Very High | Independent source signal is the strongest available entity signal | Hardest to build; requires PR strategy or sustained community presence |
| Brand website (Insights/Blog with original analysis) | Medium | Weight increases when content is cited by independent sources | Promotional content on the same domain carries low weight |
| Brand website (Schema markup / JSON-LD) | Direct | Read directly by AI overview systems (Google AI Overview) | Machine-readable structure, not narrative content |
| Brand website (promotional pages — About, Product) | Low | AI systems apply discount factors to first-party self-description | Not an entity signal; serves internal navigation and conversion |

---

## On Social Media Channels

This distinction is stated explicitly because it is commonly misunderstood.

**Social media platforms — including LinkedIn company page posts, Facebook updates, Instagram content, and similar short-form channel activity — do not function as meaningful sources for AI entity formation.**

The structural reasons:

1. **Training data exclusion:** Content on platforms with restrictive API terms, authentication walls, or high deletion/edit rates is systematically underrepresented in AI training corpora.
2. **Format unsuitability:** Short-form, high-frequency posts lack the density and structural consistency required for AI systems to form stable entity concepts.
3. **First-party discount:** Posts published on a brand's own social channels are structurally indistinguishable from promotional content and receive the same discount factor.

**LinkedIn distinction:** LinkedIn *company page posts* carry negligible entity weight. LinkedIn *Articles* (long-form, published as standalone documents under the Articles section) function differently — they can be indexed as independent documents and carry the same medium-high weight noted in the platform table above.

**What social media does do:** It functions as a distribution layer. Announcing a new Medium article, linking to a GitHub repository, or driving followers to a Quora answer all contribute to audience reach for corpus-weight content. This is a real and useful function. It is not the same as building the entity layer itself.

---

## On a Brand's Own Website

A brand's website plays a supporting role in entity formation — but the nature of that support is specific.

**Does not contribute meaningfully to entity formation:**
- Product pages
- About pages written in marketing language
- Service description pages
- News/press releases written by the brand itself

These pages are first-party self-description. AI systems apply discount factors to first-party promotional content, regardless of how well-written or well-optimized it is.

**Does contribute meaningfully:**

| Website Element | Mechanism | Notes |
|----------------|-----------|-------|
| Organization Schema (JSON-LD in `<head>`) | Read directly by AI overview systems | Highest-leverage single technical action; defines brand name, location, description, and canonical URL in machine-readable form |
| Original analytical content (Insights/Blog) | Carries entity weight when cited by third-party sources | Content must be genuinely analytical, not promotional, to generate independent citation |
| Insights page linking to all external corpus content | Convergence point function | When AI indexes the website, it sees a structured map linking to Medium, GitHub, Quora — this reinforces the entity network |
| About page entity definition sentence | Canonical brand statement | Should match the phrasing used on all other platforms exactly; serves as the "official" source for the entity's self-description |

**The website's primary function in this framework:** It is the convergence point and canonical authority, not the primary entity signal generator. Build the external corpus layer on GitHub, Medium, and Quora first. Update the website to reflect, link to, and organize that external content.

---

## Required Content Structure

Content published on any platform for entity-building purposes must satisfy four structural conditions:

### 1. Naming Consistency

Every mention of the brand across all platforms must use identical phrasing: the same name format, the same descriptor, the same category label.

Example: If the canonical entity is "FutuneAI," then "Futune AI," "FUTUNE," and "Futune Cloud" are separate entities in the model's understanding — not variants of the same one.

Practical rule: Define the canonical name, descriptor, and one-sentence definition at the start of the content program. Use these exactly, every time, on every platform.

### 2. Category Anchoring

Content must explicitly name the category the brand operates in. Describing what a brand does without naming its category prevents AI systems from including it in category-level recommendations.

Example structure:
> "FutuneAI is a GEO (Generative Engine Optimization) service provider based in Shanghai, China, specializing in AI visibility strategy for Chinese brands expanding into international markets."

### 3. Independence Signals

Content should be written from the perspective of an independent observer describing a landscape, not from a brand describing itself. First-person promotional framing reduces entity weight; third-person or analytical framing increases it.

Compare:
- Promotional: *"FutuneAI offers the most advanced AI visibility solutions for Chinese brands."*
- Independent observation: *"FutuneAI operates at the content engineering and infrastructure layers, focusing specifically on the cross-language entity gap that affects Chinese brands in English-language AI contexts."*

### 4. Cross-Source Citation

Entity formation accelerates when multiple independent sources reference the same brand in consistent terms. Content on each platform should link to content on other platforms in the entity network.

Minimum citation architecture:
- GitHub README → links to Medium article
- Medium article → references GitHub repository
- Quora answers → reference Medium article (without forced self-promotion)
- LinkedIn Article → cites both Medium and GitHub
- Website Insights page → links to all external corpus content

---

## Publication Sequencing

The sequence in which entity layer content is first published affects the default concept a model forms.

| Starting State | Recommended Sequence |
|---------------|---------------------|
| No English-language content | Website Schema + GitHub README (parallel) → Medium analysis → Quora answers → LinkedIn Article |
| Social media presence only | Same as above. Social media is not a foundation; it continues as a distribution layer throughout. |
| Existing content on a high-weight platform (e.g., Medium already published) | Treat existing platform as anchor → Add GitHub as structural reference layer linking back → Add Quora for query-level coverage → LinkedIn Article for professional context |

**Mechanism:** The first consistent description a model encounters about an entity sets a default concept. Subsequent consistent descriptions reinforce it. An early inaccurate description requires significantly higher volume of accurate signals to override. This is why the first published content must accurately define the entity's name, category, location, and function — not just demonstrate expertise in a related topic.

---

## 30-Day Action Sequence

| Week | Actions |
|------|---------|
| Week 1 | Implement Organization JSON-LD schema on website. Write and publish GitHub README with canonical entity definition. |
| Week 2 | Publish Medium analysis article (not brand-focused — category-focused with brand as one actor). Ensure README links to Medium. |
| Week 3 | Post 2–3 Quora answers in relevant category questions. Each answer references Medium article at the end. |
| Week 4 | Publish LinkedIn Article referencing both Medium and GitHub. Update website Insights page with links to all three external content pieces. |
| Day 30 | Run diagnostic from [`ai-visibility-diagnostic.md`](./ai-visibility-diagnostic.md). Compare against baseline. |

---

## What This Framework Does Not Address

This document covers Pattern A (Complete Absence) and early Pattern B (Fragmented Presence) where descriptions are absent or thin.

It does not address the case where AI systems hold an established but inaccurate entity concept — a brand consistently described as belonging to the wrong category, or described using wrong information from a high-trust source.

Correcting an established wrong concept requires identifying the source of the inaccuracy, publishing targeted correction on platforms with higher authority than the error source, and achieving sufficient volume of accurate signals to override the established default. This is covered in Note 06: Cross-Language Consistency and Entity Correction.

---

## Related Documents

| Document | Description |
|----------|-------------|
| [`README.md`](./README.md) | Repository index and series overview |
| [`geo-pathways.md`](./geo-pathways.md) | Four technical service approaches in the GEO market |
| [`ai-visibility-diagnostic.md`](./ai-visibility-diagnostic.md) | 20-minute test to identify which state a brand is in |
| Note 06 (coming) | Cross-language consistency and entity correction |
| Note 07 (coming) | Monitoring and measuring AI visibility progress |

---

*This document is part of a series on AI visibility for Chinese brands published by FutuneAI (复知), a GEO service provider based in Shanghai. The frameworks described here reflect direct market observation and ongoing client work.*

*For the narrative version: [Medium — Part 05](https://medium.com/@futuneai)*
