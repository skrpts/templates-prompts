---
type: prompt
id: prompt-summarisation
title: "Summarisation"
description: "Summarises long-form content into a concise overview with key points"
tags: [Production, Template]
connections: []
metadata:
  template_category: "Prompt Pattern"
---

## Purpose

Summarise the provided text into a concise overview. Preserve the most important information and key arguments.

## Prompt

Summarise the following text. Produce:

1. **Executive summary** (2-3 sentences)
2. **Key points** (bulleted list, 5-8 points)
3. **Notable quotes or data** (if any)
4. **What's missing** (important context not covered)

### Text to Summarise

{{input.text}}

### Rules

- Preserve the original meaning — do not editorialise
- Include specific numbers, dates, and names
- Note any claims that lack supporting evidence
- Keep the summary under 20% of the original length
