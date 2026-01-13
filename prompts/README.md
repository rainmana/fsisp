# Prompts

## Purpose

This directory contains structured prompts used in FSISP evaluations. Each prompt is documented with its purpose, context, and usage guidelines.

## Organization

Prompts should be organized by:

- Category or research focus
- Complexity level
- Evaluation context

## Prompt Documentation

Each prompt file or section should include:

1. **Prompt Text**: The exact text to be used
2. **Purpose**: What aspect of model behavior this prompt investigates
3. **Context**: When and how this prompt should be used
4. **Variations**: Alternative formulations if applicable
5. **Considerations**: Relevant factors for interpretation

## Guidelines

When working with prompts:

- Document prompts exactly as used in evaluations
- Avoid embedding assumptions about model responses
- Use neutral language that doesn't suggest expected outcomes
- Note any dependencies or required context
- Track versions if prompts are modified over time

## Format

Prompts can be stored as:

- Individual text files (`.txt`)
- Markdown documents with annotations (`.md`)
- JSON files with metadata (`.json`)
- YAML files for structured data (`.yaml`)

Choose the format that best supports documentation and reproducibility for your use case.

## Example Structure

```
prompts/
├── README.md                    # This file
├── basic/                       # Foundational prompts
│   ├── prompt_001.md
│   └── prompt_002.md
├── structured/                  # Multi-part prompts
│   └── series_a.yaml
└── templates/                   # Prompt templates
    └── template_guidelines.md
```

## Best Practices

1. **Reproducibility**: Document exact wording and formatting
2. **Versioning**: Track changes to prompts over time
3. **Context**: Include necessary setup or prerequisite information
4. **Neutrality**: Avoid leading or biased language
5. **Clarity**: Make instructions unambiguous
