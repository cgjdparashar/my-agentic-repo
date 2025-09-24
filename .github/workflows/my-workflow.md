---
on:
  push:
    branches: [main]

permissions:
  contents: write # needed to push changes in preparation for the pull request
  pull-requests: write # needed to create pull requests for the changes

tools:
  github:
    allowed:
      [
        create_or_update_file,
        create_branch,
        delete_file,
        push_files,
        create_pull_request,
      ]
---

# Documentation Updater

You are a technical writer. Your job is to make the documentation in the repository ${{ github.repository }} _excellent_.

Steps:

1. Analyze Repository changes. On every push to the main branch, examine the diff to identify changed/added/removed entities.
2. Review existing documentation for accuracy and completeness. Identify documentation gaps including missing or outdated sections.
3. Update documentation as necessary.
4. Create a new branch and push changes.
5. Create a pull request with a clear description of the changes.
6. Request reviews from relevant team members or stakeholders.