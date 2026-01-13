# Results

## Purpose

This directory is designated for storing evaluation results and observations from FSISP evaluations. It provides structure for maintaining consistent documentation across evaluation sessions.

## Important Note

**This directory should NOT contain invented or speculative results.** Only store actual observations from conducted evaluations.

## Organization

Results should be organized to support:

- Tracking individual evaluation sessions
- Comparing across sessions or conditions
- Maintaining provenance and reproducibility
- Protecting sensitive or preliminary data

## Suggested Structure

```
results/
├── README.md                    # This file
├── .gitignore                   # Exclude sensitive/preliminary data
├── templates/                   # Documentation templates
│   ├── session_template.md
│   └── observation_template.md
├── completed/                   # Finalized evaluations
│   ├── session_001/
│   │   ├── metadata.yaml
│   │   ├── observations.md
│   │   └── artifacts/
│   └── session_002/
└── in_progress/                 # Active evaluations
```

## Documentation Templates

Templates help maintain consistency. A basic session template might include:

```markdown
# Evaluation Session: [ID]

## Metadata
- Date: [YYYY-MM-DD]
- Researcher(s): [Names/IDs]
- Model: [Model identifier and version]
- Configuration: [Link to config file]

## Prompts Used
- [List of prompts with references]

## Observations

### Prompt 1: [ID/Name]
[Documented observations using evaluation rubric]

### Prompt 2: [ID/Name]
[Documented observations using evaluation rubric]

## Notes
[Additional context, limitations, or considerations]

## Artifacts
[References to logs, outputs, or other materials]
```

## Guidelines

When documenting results:

1. **Use Consistent Format**: Follow established templates
2. **Link to Configurations**: Reference exact configs and prompts used
3. **Record Metadata**: Date, model version, researcher, conditions
4. **Document Observations**: Use evaluation rubrics consistently
5. **Note Limitations**: Acknowledge constraints and uncertainties
6. **Protect Preliminary Data**: Use `.gitignore` for work-in-progress

## What to Include

✅ **Include**:
- Structured observations following rubrics
- Metadata about evaluation conditions
- Links to configurations and prompts used
- Notes on methodology or deviations
- Relevant context for interpretation

❌ **Do NOT Include**:
- Invented or speculative results
- Unvalidated conclusions
- Raw model outputs without context (consider privacy/terms)
- Personally identifiable information
- Proprietary or sensitive information

## Version Control Considerations

Consider using `.gitignore` to exclude:

- Preliminary or draft observations
- Raw model outputs (depending on terms of service)
- Large binary files
- Sensitive or confidential data

Example `.gitignore` entries:
```
# Exclude in-progress work
in_progress/

# Exclude raw outputs
*/raw_outputs/

# Exclude large files
*.log
*.jsonl
```

## Privacy and Ethics

When storing results:

1. **Review Terms of Service**: Ensure compliance with model provider terms
2. **Protect Privacy**: Redact any personal information
3. **Consider Sensitivity**: Be mindful of controversial or sensitive content
4. **Document Ethically**: Maintain research ethics standards
5. **Secure Storage**: Protect data appropriately

## Best Practices

1. **Regular Backups**: Maintain backups of evaluation data
2. **Clear Naming**: Use consistent, descriptive naming conventions
3. **Progressive Documentation**: Document as you go, not after
4. **Peer Review**: Have results reviewed by another researcher
5. **Archival Format**: Use text-based formats for long-term preservation
