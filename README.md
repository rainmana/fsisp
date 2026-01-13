# FSISP: Frontier Self-Reference & Inhibition Stability Probe

A research-oriented LLM evaluation framework for qualitative analysis of model behavior under specific prompt conditions.

## Overview

FSISP is a qualitative evaluation harness designed for systematic investigation of language model responses. This framework provides structured prompts, evaluation rubrics, and documentation for conducting rigorous research on model behavior.

**Important:** This is NOT a benchmark or scoring system. FSISP is a qualitative research tool that emphasizes documentation, reproducibility, and systematic observation.

## Repository Structure

```
fsisp/
├── README.md           # This file
├── LICENSE             # License information
├── CITATION.cff        # Citation metadata
├── prelude/            # Background context and methodology
├── prompts/            # Structured prompts for evaluation
├── config/             # Configuration files for evaluations
├── eval/               # Evaluation rubrics and guidelines
├── results/            # Directory for storing evaluation results
└── scripts/            # Helper scripts for running evaluations
```

## Directory Overview

### `prelude/`
Contains background information, research context, and methodological documentation. This provides the foundation for understanding the framework's purpose and approach.

### `prompts/`
Structured prompts used in evaluations. Each prompt is documented with its purpose, expected usage, and relevant context.

### `config/`
Configuration files that specify evaluation parameters, model settings, and experimental conditions.

### `eval/`
Evaluation rubrics and guidelines for systematic qualitative analysis. Includes frameworks for documenting observations and patterns.

### `results/`
Directory for storing evaluation results and observations. Includes templates and documentation guidelines for maintaining consistency.

### `scripts/`
Helper scripts for organizing evaluations, managing configurations, and processing documentation.

## Usage

This framework is designed for researchers conducting qualitative evaluations of language models. It provides structure without imposing quantitative metrics, allowing for nuanced observation and analysis.

1. Review the prelude documentation to understand the research context
2. Select or adapt prompts from the `prompts/` directory
3. Configure evaluation parameters in `config/`
4. Apply evaluation rubrics from `eval/` during analysis
5. Document observations in `results/` following provided templates

## Principles

- **Qualitative Focus**: Emphasizes detailed observation over quantitative scoring
- **Neutrality**: Maintains objective, research-oriented language
- **Reproducibility**: Provides clear documentation for replication
- **Transparency**: Documents methodology and limitations openly

## Contributing

This is a research framework. Contributions should maintain the qualitative, neutral, and research-oriented approach. All additions must avoid anthropomorphic language and should not include invented results or conclusions.

## Citation

If you use this framework in your research, please cite using the information in `CITATION.cff`.
