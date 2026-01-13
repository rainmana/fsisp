# Scripts

## Purpose

This directory contains helper scripts for organizing evaluations, managing configurations, and processing documentation in the FSISP framework.

## Scope

Scripts in this directory support:

- Organizing and validating configuration files
- Generating documentation templates
- Processing and formatting evaluation data
- Automating repetitive tasks
- Maintaining consistency across the framework

## Guidelines

Scripts should:

1. **Be Documented**: Include clear usage instructions and examples
2. **Be Tested**: Validate scripts before adding to repository
3. **Be Portable**: Minimize dependencies and document requirements
4. **Be Focused**: Each script should have a single, clear purpose
5. **Be Safe**: Include appropriate error handling and validation

## Languages

Common languages for scripts include:

- **Python**: Data processing, validation, formatting
- **Bash/Shell**: File operations, automation
- **JavaScript/Node.js**: JSON processing, web integration
- **R**: Statistical analysis, qualitative data processing

Choose the language that best fits the task and available expertise.

## Example Structure

```
scripts/
├── README.md                    # This file
├── requirements.txt             # Python dependencies (if applicable)
├── package.json                 # Node.js dependencies (if applicable)
├── validate_config.py           # Validate configuration files
├── generate_template.sh         # Generate documentation templates
├── format_results.py            # Format evaluation documentation
└── utils/                       # Shared utilities
    └── common.py
```

## Common Script Types

### Validation Scripts
Verify that configurations and documentation follow expected formats:

```python
# Example: validate_config.py
# Validates YAML configuration files against schema
```

### Template Generators
Create consistent documentation templates:

```bash
# Example: generate_template.sh
# Generates evaluation session template with metadata
```

### Processing Scripts
Format and organize evaluation documentation:

```python
# Example: format_results.py
# Formats observation notes according to style guidelines
```

### Utility Scripts
General-purpose helpers for common tasks:

```python
# Example: check_structure.py
# Verifies directory structure is complete
```

## Documentation Standards

Each script should include:

1. **Header Comment**: Purpose, usage, and author
2. **Dependencies**: Required libraries or tools
3. **Usage Examples**: Command-line examples
4. **Error Handling**: Graceful failure modes
5. **Help Text**: Built-in usage information

Example Python script header:

```python
#!/usr/bin/env python3
"""
Script Name: validate_config.py
Purpose: Validate FSISP configuration files against schema
Usage: python validate_config.py <config_file>
Dependencies: pyyaml, jsonschema
Author: FSISP Contributors
"""

import sys
import argparse

def main():
    parser = argparse.ArgumentParser(
        description='Validate FSISP configuration files'
    )
    parser.add_argument('config_file', help='Path to configuration file')
    # ... rest of script
```

## Best Practices

1. **Version Control**: Track script changes with meaningful commits
2. **Testing**: Test scripts with various inputs
3. **Error Messages**: Provide clear, actionable error messages
4. **Logging**: Add logging for debugging and audit trails
5. **Documentation**: Keep README updated with new scripts
6. **Portability**: Use virtual environments for Python, lock files for Node.js

## Dependencies

If scripts require external dependencies:

### Python
Create `requirements.txt`:
```
pyyaml>=6.0
jsonschema>=4.0
markdown>=3.0
```

Install with: `pip install -r requirements.txt`

### Node.js
Create `package.json`:
```json
{
  "name": "fsisp-scripts",
  "version": "1.0.0",
  "dependencies": {
    "js-yaml": "^4.1.0",
    "ajv": "^8.0.0"
  }
}
```

Install with: `npm install`

## Security Considerations

When writing scripts:

1. **Validate Inputs**: Sanitize and validate all user inputs
2. **Avoid Shell Injection**: Use proper subprocess handling
3. **Limit Permissions**: Request only necessary file system access
4. **Review Dependencies**: Audit third-party libraries
5. **Handle Secrets**: Never hardcode credentials or API keys

## Contributing Scripts

When adding new scripts:

1. Ensure they align with framework principles
2. Document thoroughly
3. Test with various inputs
4. Update this README
5. Consider edge cases and error conditions
