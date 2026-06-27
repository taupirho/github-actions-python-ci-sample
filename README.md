# GitHub Actions Python CI Sample

This is a small public sample for setting up a basic GitHub Actions workflow on a Python project.

It checks three things:

- Python dependencies install cleanly.
- Ruff can lint and check formatting.
- Pytest can run the test suite.

The workflow is intentionally small. It is a good starting point before adding deployment jobs, environment-specific secrets, branch protection, or release gates.

## Files

- `.github/workflows/python-ci.yml` - GitHub Actions workflow.
- `pyproject.toml` - ruff and pytest configuration.
- `src/sample_app/` - tiny example package.
- `tests/` - tiny pytest example.

## Run Locally

```bash
python -m pip install --upgrade pip
pip install ruff pytest
ruff check .
ruff format --check .
pytest
```

## Full Starter Pack

The full GitHub Actions CI/CD Starter Pack for Python includes the workflow templates plus a release gate, readiness checklist, troubleshooting notes, pre-commit config, and two walkthrough PDFs.

Full pack:
https://thomasreid4.gumroad.com/l/pafvzf?utm_source=github&utm_medium=sample_repo&utm_campaign=github_actions_pack_launch&utm_content=readme

