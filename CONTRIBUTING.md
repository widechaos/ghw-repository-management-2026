# Contributing

I maintain this personal GitHub Skills exercise. The fictional Mergington school application and sample records come from the MIT-licensed upstream template; do not upload real student information or credentials.

## Propose a change

Search existing issues, then use the bug or feature template for a focused proposal. Security vulnerabilities belong in the private reporting channel described in SECURITY.md.

Create a branch from main, keep changes small, and open a pull request explaining the problem, resulting behavior and validation. Direct pushes, branch deletion and force pushes to main are blocked. Code-owner review is requested for the application, database, authentication and frontend paths. I review changes before merging.

## Local development

Use a disposable local environment. Install requirements.txt in a Python virtual environment and supply a local MongoDB instance as required by src/backend/database.py. Start the API with `python -m uvicorn src.app:app --reload`, then open the local URL reported by Uvicorn. Never use production or employer data.

For documentation-only contributions, check links, filenames and rendered Markdown. For application changes, exercise the affected API or UI and describe the observed result in the pull request. Do not claim tests that you did not run. Keep local configuration and secrets out of Git.

Follow CODE_OF_CONDUCT.md. Preserve upstream licensing and credit reused material.
