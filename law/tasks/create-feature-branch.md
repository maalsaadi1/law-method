# Create GitHub Feature Branch Task
## Purpose
To create a new feature branch in the project's GitHub repository based on standard conventions.
## Inputs
- Feature name/identifier.
- Base branch (e.g., `develop`, `main`).
- Target repository.
## Instructions
1. Confirm parameters with Composer.
2. Construct branch name (e.g., `feature/[feature-name]`).
3. Use MCP/GitHub tool to:
    a. Fetch latest from base branch.
    b. Create new branch from base branch.
    c. Push new branch to remote.
4. Report success and new branch name to Composer.