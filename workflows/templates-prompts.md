---
type: workflow
id: templates-prompts
title: "Prompt Templates"
description: "Prompt patterns — system prompts, few-shot, chain-of-thought, extraction, and more"
tags: [Production, Templates]
connections:
  - target: prompt-system
    type: uses
  - target: prompt-few-shot
    type: uses
  - target: prompt-cot
    type: uses
  - target: prompt-extraction
    type: uses
  - target: prompt-classification
    type: uses
  - target: prompt-conversational
    type: uses
  - target: prompt-summarisation
    type: uses
  - target: prompt-rewriting
    type: uses
  - target: prompt-comparison
    type: uses
  - target: prompt-code-generation
    type: uses
  - target: llm-service
    type: runs_on
metadata:
  estimated_duration: "1 minute"
  trigger: manual
  template: true
output_step: "prompt-system"
composite_steps:
  - "prompt-system"
  - "prompt-few-shot"
  - "prompt-cot"
  - "prompt-extraction"
  - "prompt-classification"
  - "prompt-conversational"
  - "prompt-summarisation"
  - "prompt-rewriting"
  - "prompt-comparison"
  - "prompt-code-generation"
execution:
  - skill: "prompt-system"
    step_type: "generation"
---

## Overview

This skrpt contains 10 prompt templates for use when creating new prompt nodes. Import this skrpt to add these templates to your template picker.

## Templates

### Prompt Pattern

- **System Prompt** — Role definition with constraints and output format
- **Few-Shot Prompt** — System message with example input/output pairs
- **Chain-of-Thought** — Step-by-step reasoning before final answer
- **Extraction Prompt** — Extract structured data from unstructured input
- **Classification Prompt** — Categorise input into predefined classes
- **Conversational Prompt** — Persona-based conversational agent with tone and rules
- **Summarisation** — Summarise long text into key points
- **Rewriting** — Rewrite text for a different audience or tone
- **Comparison** — Compare multiple items across defined criteria
- **Code Generation** — Generate code from a specification

