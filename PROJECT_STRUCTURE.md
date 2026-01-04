# Project Structure

This document outlines the organization of the LLM Training Toolkit repository.

## Repository Layout

```
llm-training-toolkit/
├── README.md              # Main project documentation
├── .gitignore            # Git ignore rules for Python/ML projects
├── requirements.txt      # Python dependencies
├── PROJECT_STRUCTURE.md  # This file
├── src/                  # Source code package
│   └── __init__.py      # Package initialization
├── notebooks/            # Jupyter notebooks (to be created)
├── experiments/          # Experimental code (to be created)
├── configs/             # Configuration files (to be created)
└── docs/                # Documentation (to be created)
```

## Branch Organization

The repository uses multiple branches for parallel development:

### Main Branch (`main`)
- **Purpose**: Stable, production-ready code
- **Contains**: Core project structure, documentation, and shared utilities
- **Workflow**: Protected branch, requires pull request reviews

### Feature Branches
1. **`qwen-integration`**
   - Experiments with Qwen model training
   - Qwen-specific configurations and notebooks
   - Integration with QwenLM/Qwen repository resources

2. **`starcoder-integration`**
   - Experiments with StarCoder model training
   - StarCoder-specific configurations and notebooks
   - Integration with bigcode-project/starcoder repository resources

3. **`documentation`**
   - Project documentation and guides
   - Tutorials and learning materials
   - API documentation

## Development Workflow

1. **Start from `main`**: Always create feature branches from `main`
2. **Work in feature branches**: Develop specific features in their respective branches
3. **Create pull requests**: Submit changes via PRs for review
4. **Merge to `main`**: After review and approval, merge to main
5. **Keep branches updated**: Regularly rebase/merge from `main`

## External Resources Integration

This project learns from and integrates with:
- **Qwen**: Files from `QwenLM/Qwen` repository
- **StarCoder**: Files from `bigcode-project/starcoder` repository

When copying external resources:
1. Always preserve original directory structure
2. Add attribution comments
3. Document any modifications made
4. Follow original project licenses

## Next Steps

1. Set up the `notebooks/` directory for Jupyter notebooks
2. Create experiment templates in `experiments/`
3. Add configuration templates in `configs/`
4. Develop comprehensive documentation in `docs/`
