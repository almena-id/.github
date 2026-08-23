# `.github` (organization)

**GitHub-facing metadata for the Almena Network organization** — the narrative shown on the
org profile, and, over time, whatever templates or policies are genuinely shared by every
repository. See [organization repository conventions](https://docs.github.com/en/organizations/collaborating-with-groups-in-your-organization/customizing-your-organizations-profile).

| Path | Purpose |
| --- | --- |
| [`profile/README.md`](profile/README.md) | The organization profile: what Almena is, the principles it is measured against, and one row per repository. It describes each repository on its own — never an aggregate checkout or a hub layout. |

Nothing else lives here yet. **Workflows, issue templates and `CODEOWNERS` belong in the
repository they apply to**, under that repository's own CI and governance conventions; a copy
kept here would be one nobody edits when the repository it describes changes.

A repository added, renamed or retired is a change to `profile/README.md` in the same breath.
That table is worth exactly as much as its last update.
