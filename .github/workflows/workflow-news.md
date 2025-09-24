---
on:
  workflow_dispatch:

permissions:
  contents: write
  issues: write

tools:
  github:
    allowed: [create_issue]
---

# Name: Hello World AI Workflow

When this workflow is triggered, use AI to generate a simple "Hello, world!" message.

Post the message as a GitHub Issue titled:
"Hello from AI 👋"

The body of the issue should include:
- A friendly greeting
- A fun fact about AI
- A motivational quote
