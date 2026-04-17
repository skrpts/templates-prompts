---
type: prompt
id: prompt-few-shot
title: "Few-Shot Prompt"
description: "Few-shot prompt with example pairs for consistent output"
tags: [Production, Template]
connections: []
metadata:
  template_category: "Prompt Pattern"
---

## System Message
You are a {{ROLE}}. Follow the examples below to understand the expected output format.

## Examples

### Example 1
**Input:** {{EXAMPLE_INPUT_1}}
**Output:** {{EXAMPLE_OUTPUT_1}}

### Example 2
**Input:** {{EXAMPLE_INPUT_2}}
**Output:** {{EXAMPLE_OUTPUT_2}}

### Example 3
**Input:** {{EXAMPLE_INPUT_3}}
**Output:** {{EXAMPLE_OUTPUT_3}}

## Task
Now process the following input using the same format:

**Input:** {{USER_INPUT}}
