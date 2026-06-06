# Build It The Right Way — GitBook Source

This repository is the **Git Sync source of truth** for the [Build It The Right Way](https://build-it-the-right-way.gitbook.io/home) GitBook space.

## How This Works

- Every commit pushed to `main` triggers a **change request** in GitBook.
- Change requests are reviewed and merged inside GitBook before going live on the published docs site.
- The `SUMMARY.md` file defines the table of contents structure.

## Repository Structure

```
welcome/                 # Welcome section
pillars/                 # The 8 BRY Pillars
design-decisions/        # Design decision principles
design-artifacts/        # Checklists and templates
design-patterns/         # Pattern library
solution-units/          # Domain lenses (ITSM, IRM, ITOM, SPM, Custom Apps)
SUMMARY.md               # GitBook table of contents
README.md                # This file
```

## License

Content © TechTalk with Bill.
