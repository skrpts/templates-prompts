---
type: prompt
id: prompt-comparison
title: "Comparison"
description: "Produces a structured comparison of items across defined dimensions"
tags: [Production, Template]
connections: []
metadata:
  template_category: "Prompt Pattern"
---

## Purpose

Compare the provided items across defined criteria. Produce a structured, balanced analysis.

## Prompt

Compare the following items:

{{input.items}}

### Criteria to evaluate:
{{input.criteria}}

### Output Format

1. **Comparison matrix** — table with items as columns, criteria as rows
2. **Analysis per criterion** — which item excels and why
3. **Trade-offs** — what you gain and lose with each option
4. **Recommendation** — which item fits which use case

### Rules

- Be balanced — every item has strengths and weaknesses
- Use specific evidence, not vague judgements
- Acknowledge when items are too close to call on a criterion
- Note any criteria where the comparison is unfair (different categories)
