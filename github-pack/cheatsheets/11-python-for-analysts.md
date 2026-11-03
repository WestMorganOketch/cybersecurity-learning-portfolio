# Python Automation for Analysts

Purpose: use small, auditable Python scripts to reduce repetitive analysis work.

Useful patterns
- `python -m venv <ENV_DIR>` — create an isolated environment.
- `python -m pip install -r <REQUIREMENTS_FILE>` — install pinned dependencies from a trusted requirements file.
- `with open(<INPUT_FILE>, encoding='utf-8') as f:` — read text with explicit encoding and automatic file closure.
- Use `json.loads()` or `csv.DictReader` to parse structured input after validating its source and format.

Good practices
Validate inputs, handle missing fields, set file-size limits, use clear exceptions, and avoid executing data as code. Keep secrets out of source files and logs. Prefer small functions with predictable inputs and outputs. Test with synthetic examples before processing real evidence.

Defensive notes
Run scripts with the minimum permissions required, use trusted dependencies, review package provenance, and protect output files containing investigative data. Avoid uploading logs or samples to public services without approval.

Standard reference knowledge added: general Python practices for defensive analysis; no room flags or answers are included.
