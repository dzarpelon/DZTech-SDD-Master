# TASK — bootstrap-repo

## Purpose

Create the initial repository foundation only.

Use this task only when the repository does not already exist locally or on GitHub.

---

## Inputs

You MUST read and follow:

- `master-spec/dztech-sdd-master-spec-v1.md`
- `master-spec/dztech-sdd-master-operational-workflow-spec-v1.md`
- `AGENTS.md`

---

## Execution Model

Treat the repository as not yet created.

You MUST:

1. Create the local repository folder
2. Initialize git
3. Create the GitHub repository
4. Create the required minimal repository structure
5. Add the source-of-truth files
6. Create the GitHub Actions baseline
7. Commit and push the initial repository state

---

## Requirements

You MUST:

- Create a structured, minimal repository
- Keep the repository aligned to the source-of-truth files
- Include workflow representation in repository files
- Include GitHub Actions CI
- Stop after the repository foundation is complete

---

## Constraints

You MUST NOT:

- Use this task for an already existing repository
- Add features not defined by the specifications
- Over-engineer the implementation
- Continue past the initial foundation state

---

## Success Criteria

Repository state is valid when:

- The repository exists locally and on GitHub
- Required structure exists
- Source-of-truth files are present
- GitHub Actions baseline exists
- Initial commit and push are complete
