---
type: prompt
id: prompt-rewriting
title: "Rewriting"
description: "Rewrites content for a different audience, tone, or reading level"
tags: [Production, Template]
connections: []
metadata:
  template_category: "Prompt Pattern"
---

## Purpose

Rewrite the provided text for a different audience, tone, or reading level while preserving the core message.

## Prompt

Rewrite the following text according to these parameters:

- **Target audience:** {{input.target_audience}}
- **Desired tone:** {{input.tone}}
- **Reading level:** {{input.reading_level}}

### Original Text

{{input.text}}

### Rules

- Preserve all factual content and key arguments
- Adapt vocabulary and sentence complexity for the target audience
- Maintain the original structure unless a different structure serves the audience better
- Flag any content that cannot be simplified without losing meaning
