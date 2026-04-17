---
type: prompt
id: prompt-code-generation
title: "Code Generation"
description: "Generates implementation code from a functional specification or description"
tags: [Production, Template]
connections: []
metadata:
  template_category: "Prompt Pattern"
---

## Purpose

Generate code that implements the described functionality. Focus on correctness, readability, and following best practices.

## Prompt

Implement the following:

{{input.specification}}

### Language/framework: {{input.language}}

### Requirements

- Follow the language's idiomatic patterns and conventions
- Include error handling for edge cases
- Add brief inline comments for non-obvious logic
- Use meaningful variable and function names

### Output

Return the complete implementation. If the code spans multiple files, clearly separate them with file path headers.

### Rules

- Prioritise correctness over cleverness
- Handle edge cases explicitly
- Do not include unnecessary dependencies
- Follow SOLID principles where applicable
