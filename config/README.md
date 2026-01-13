# Configuration

## Purpose

This directory contains configuration files that specify evaluation parameters, model settings, and experimental conditions for FSISP evaluations.

## Configuration Types

### Evaluation Configurations
- Specify which prompts to use
- Define evaluation sessions and groupings
- Set procedural parameters

### Model Configurations
- Document model identifiers and versions
- Record relevant model parameters (temperature, max tokens, etc.)
- Note any model-specific settings

### Environment Configurations
- Specify software versions and dependencies
- Document runtime environment details
- Record relevant system information

## File Formats

Configurations can be stored in:

- **YAML** (`.yaml`, `.yml`): Human-readable, supports comments
- **JSON** (`.json`): Strict format, widely supported
- **TOML** (`.toml`): Clear syntax, good for nested configs

Choose the format that best fits your workflow and tooling.

## Guidelines

Configuration files should:

1. **Be Self-Documenting**: Include comments explaining parameters
2. **Be Version-Controlled**: Track changes to configurations
3. **Be Reproducible**: Contain all information needed to replicate setup
4. **Be Validated**: Check for completeness and correctness
5. **Be Isolated**: Separate concerns (model config vs. evaluation config)

## Example Structure

```
config/
├── README.md                    # This file
├── models/                      # Model-specific configurations
│   ├── model_a.yaml
│   └── model_b.yaml
├── evaluations/                 # Evaluation session configs
│   ├── session_001.yaml
│   └── session_002.yaml
└── templates/                   # Configuration templates
    └── template.yaml
```

## Configuration Template

A basic configuration might include:

```yaml
# Evaluation Session Configuration
session:
  id: "session_001"
  date: "2026-01-13"
  description: "Brief description of evaluation focus"

model:
  identifier: "model-name-version"
  parameters:
    temperature: 0.7
    max_tokens: 1000

prompts:
  - id: "prompt_001"
    source: "prompts/basic/prompt_001.md"

evaluation:
  rubric: "eval/rubric_basic.md"
  observers: ["researcher_1"]
```

## Best Practices

1. **Document Defaults**: Explicitly state default values
2. **Validate Inputs**: Check configurations before use
3. **Track Provenance**: Link configs to specific evaluation sessions
4. **Maintain Consistency**: Use consistent naming and structure
5. **Include Metadata**: Add dates, versions, and descriptions
