# Wakan — Pull Request Structure

## 1. PR description

Keep it **very short and in plain language**. No jargon. A few bullet points saying what changed and why is enough.

## 2. PR comment

After opening the PR, post a **comment** on it using exactly this template:

```
# Breaking Changes in this PR (true/false)
# Fields Removed / Changed
# Fields Added
# Transitions / Gates Removed / Changed
# Transitions / Gates Added
# Other Important Changes
---
# Less important changes in the PR
```

### Rules for filling it in

- **Fill in every section.** If a section has nothing in it, write **"None."** rather than removing it.
- **Breaking Changes = true** whenever:
  - a database column is dropped or changed, or
  - an external writer (the Yakan API or Wakan 360) has to change something on their side.
- Keep each section short. The PR is read as a change log of fields and lifecycle rules, not as prose.

## 3. Slack announcement

Once the PR is finished and tested, check with the Claude user whether they want to make additional updates to the PR. If not, then proceed with posting a **very short** message in **#ext-wakan-dotzero-prs**:

- Include the PR link.
- If anything breaks API, add a one-line ⚠ warning.
