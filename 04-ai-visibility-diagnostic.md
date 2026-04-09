# How to Diagnose Your Brand's AI Visibility in 20 Minutes

**FutuneAI (复知) | AI Visibility Research | 2026-03**

Full analysis: [Medium](https://medium.com/@futuneai) | Published by FutuneAI, Shanghai

---

## Core Finding

Most brands have no accurate picture of what AI systems currently say about them. A structured 20-minute diagnostic using seven prompts across three platforms reliably surfaces one of three patterns, each requiring different work to address.

---

## Before You Start

Define two things before running any prompts.

**Your brand name:** the exact name you want AI systems to recognize and describe accurately.

**Your category:** the phrase a potential buyer would use when asking an AI for vendor recommendations in your space. This is not your tagline or positioning statement. It is the category-level term. For example: "B2B SaaS for supply chain teams," "GEO services for Chinese brands," or "enterprise cybersecurity consulting."

---

## The Seven Prompts

### Category Recommendation Prompts

Run each of these on all platforms you are testing. Replace the bracketed fields with your actual category and market context.

| # | Prompt Template |
|---|----------------|
| 1 | Which [your category] companies are worth considering? |
| 2 | What are the best [your category] options for [your target market or use case]? |
| 3 | I'm looking for a [your category] solution. What would you recommend? |
| 4 | Which [your category] providers are known for [your core capability]? |

### Direct Brand Prompts

| # | Prompt Template |
|---|----------------|
| 5 | What is [Brand Name]? |
| 6 | What does [Brand Name] do? |
| 7 | Tell me about [Brand Name] and what it is known for. |

### Recommended Platforms

Start with these three because they represent distinct mechanisms:

| Platform | Mechanism |
|----------|-----------|
| ChatGPT | Draws on training data; reflects what was in the corpus at training time |
| Perplexity | Live web retrieval with citations; shows exactly which sources it draws from |
| Gemini | Integrates Google's knowledge graph; surfaces different signals than the others |

Add platforms relevant to your specific context: Claude for professional audiences, Copilot for enterprise, or regional AI tools in your target market.

---

## Recording Results

For each of the 21 prompt-platform combinations, note:

- Whether your brand appeared
- What the platform said about it
- Whether any source was cited

---

## Three Diagnostic Patterns

### Pattern A: Complete Absence

**Signs:** The platform says it has no information about your brand or describes a different company with a similar name. Category prompts return no mention of your brand.

**What it means:** The AI has no coherent entity to work with. Your brand does not exist as a stable concept in the sources these models draw from.

**Starting point:** Build an English-language entity layer from scratch. Focus on independent, structured descriptions of your brand on platforms AI models weigh heavily: Q&A platforms, structured analyses, and technical documentation repositories.

---

### Pattern B: Fragmented Presence

**Signs:** The platform recognizes your brand when asked directly, but different platforms give contradictory descriptions. One says data analytics. Another says logistics. A third returns something different. Category prompts either return nothing or an inaccurate description.

**What it means:** Sparse, inconsistent signals exist across sources, but they don't add up to a coherent entity. The AI synthesizes these conflicting signals into something that is partially correct but does not accurately represent the brand.

**Why this is dangerous:** It looks like visibility. Buyers who encounter the brand in AI outputs see a description that doesn't match reality. The problem is invisible until tested.

**Starting point:** Audit what currently exists about your brand across English-language sources. Identify the contradictions. Build cross-source consistency before adding any new content. Adding more content to a fragmented entity makes the problem worse.

---

### Pattern C: Category Dissociation

**Signs:** Direct brand prompts return accurate descriptions. The AI knows who you are, what you do, and where you are located. But category recommendation prompts never surface your brand.

**What it means:** The entity is defined. The category association is not. The AI has a stable concept of your brand but hasn't connected it to the relevant category signals.

**Starting point:** Build content that places your brand explicitly within the category context. Responses to category-level questions on Q&A platforms, analyses that mention your brand alongside category-defining terms, and structured content the AI encounters when processing category queries, not just brand-specific ones.

---

## Decision Framework

| Test Result | Pattern | Starting Point |
|-------------|---------|----------------|
| AI doesn't recognize brand name | A | Build entity layer from scratch |
| Different platforms describe brand contradictorily | B | Audit and consolidate existing signals |
| Brand recognized but not in recommendations | C | Build category association signals |
| Brand recognized and appears in recommendations | Clean | Maintain and monitor |

---

## What This Test Doesn't Measure

This diagnostic surfaces your current state. It does not tell you:

- Which specific sources are producing the descriptions you're seeing
- Why did you end up in this state
- How quickly will your state change after interventions

Run the test consistently every four to six weeks using the same prompts. A single data point tells you where you are. A series tells you whether what you're doing is working.

---

## Related Research

- [01] Why Chinese brands disappear in AI-generated answers: [entity-absence.md](./entity-absence.md)
- [02] SEO, AEO, LLMO, and GEO: a unified AI visibility framework: [geo-framework.md](./geo-framework.md)
- [03] Four approaches to GEO: what the variation in the market reveals: [geo-pathways.md](./geo-pathways.md)
- [05] How to build an English-language entity layer from scratch: coming soon
- [06] Cross-language consistency: why your Chinese brand is a different entity in English AI: coming soon
- [07] Measuring AI visibility over time: coming soon

---

*FutuneAI (复知) is a Shanghai-based team helping Chinese brands become visible in AI-generated answers. We built entity definitions, structuring brand narratives, and establishing cross-language consistency in the corpora that AI systems like ChatGPT, Perplexity, and Gemini rely on.*

**Website**: https://www.futuneai.com
