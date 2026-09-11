# webpack Working Groups

A repository for all working groups and documentation.

Working groups are self-organizing teams within the webpack organization that own a
specific area of the project — security, documentation, design, and so on. Every group's
charter, member list, and documentation lives in this repository, under
[`working-groups/`](working-groups), one folder per group.

## Active working groups

| Working group | Scope |
| --- | --- |
| [Security Working Group](working-groups/security-wg/README.md) | Security policies and procedures, security triage, vulnerability disclosure, and ecosystem security guidance. |
| [Documentation Working Group](working-groups/docs-wg/README.md) | [webpack.js.org](https://webpack.js.org) content and infrastructure, documentation reviews, style and terminology conventions. |

The Security Working Group also keeps its
[incident response plan](working-groups/security-wg/INCIDENT_RESPONSE_PLAN.md),
[packages in scope](working-groups/security-wg/docs/packages-in-scope.md), and
[threat model](working-groups/security-wg/docs/threat-model.md) here.

## Archived working groups

| Working group | Status |
| --- | --- |
| [Design Working Group](working-groups/design-wg/README.md) | Archived — replaced by individual contributions and help from the OpenJS Foundation. |
| [Performance Working Group](working-groups/performance-wg/README.md) | Archived — this work is now covered by the core working group. |

## Issues and pull requests

Every issue and pull request that belongs to a working group must be prefixed with the
name of that working group in square brackets:

```
[docs-wg] Document the new asset modules API
[security-wg] Add a triage checklist to the incident response plan
```

> [!NOTE]
> Shorthands such as `SEC`, `CORE`, `DOCS` within the working group trackers are also okay.


The prefix is the working group's short name — the same name as its folder under
[`working-groups/`](working-groups) and its `@webpack/<name>` team, for example
`[security-wg]` or `[docs-wg]`. It applies here and in any tracker a working group uses,
so that work can be attributed to a group at a glance and filtered with a simple search.

Use a single prefix per issue or pull request. If a change genuinely spans two groups,
prefix it with the group that owns the change and mention the other group in the body.

## Starting a new working group

1. Copy [`template/README.md`](template/README.md) as the starting point for the new
   group's `README.md`, and fill in the name, purpose, goals, members, and communication
   channel. The upstream copy lives in [webpack/wg-template](https://github.com/webpack/wg-template).
2. Open a proposal with the webpack [TSC](https://github.com/webpack/tsc) describing the
   group's charter and the initial members.
3. Once approved, a `@webpack/<topic>-wg` team is created in the webpack organization.
4. Open a pull request against this repository adding `working-groups/<topic>-wg/` with the
   group's documentation, and a row for it in the table above.

## Template

The working group template is mirrored in [`template/`](template):

- [`template/README.md`](template/README.md) — the working group README template.
- [`template/LICENSE`](template/LICENSE) — the MIT license shipped with the template.

## Code of Conduct

The [webpack Project's Code of Conduct](https://github.com/webpack/webpack/blob/main/CODE_OF_CONDUCT.md)
applies to this repository and to every working group listed here.
