# Contributing to disease-monograph-app

This repository contains the disease monograph SMART application. Start with [readme.txt](readme.txt), which identifies the separate semantic-service dependency, and distinguish frontend changes from changes that belong in that service.

## Before you start

Search existing issues and pull requests before starting, and discuss substantial changes or new dependencies in an issue. Use an issue template when one is offered. For a bug, include the affected commit or version, environment, a minimal reproduction, and expected versus observed behavior; remove sensitive information from logs and screenshots.

## Development and validation

Review [package.json](package.json), [index.html](index.html), and [launch.html](launch.html) before changing application behavior. The manifest declares a FHIR client dependency but has no npm build, test, or serve scripts. Record the local environment and exact verification steps used, including any unavailable external-service dependency.

Use synthetic records to check affected data mappings, empty or incomplete responses, launch behavior, and rendered content. Keep bundled third-party libraries and their notices separate from project-owned code; avoid unrelated vendor rewrites. For monograph content changes, include traceable sources and explain any terminology or clinical interpretation change. Do not use production credentials or identifiable patient material to reproduce a problem.

## Pull requests

Work on a focused branch from the current default branch. Open a pull request explaining the problem, the resulting behavior, and any compatibility or data-format changes. Link the relevant issue and complete any existing PR template.

Add focused regression coverage for changed behavior and update affected examples or documentation. Describe the checks actually run, their results, and any checks you could not run. For documentation-only changes, verify links, examples, and rendered formatting. Use the repository's existing checks and review/merge process; preserve required checks and resolve actionable feedback without weakening the checks.

## Security and sensitive information

Follow the [account security policy](https://github.com/edithatogo/.github/blob/main/SECURITY.md). Report vulnerabilities privately through the repository's **Report a vulnerability** option if available; otherwise request a private reporting contact without posting exploit details. Never include credentials, personal information, restricted datasets, or confidential records in issues, commits, fixtures, or diagnostic output.

## Licensing and conduct

The repository's [license](LICENSE) continues to apply. Be respectful and constructive, and follow the [account code of conduct](https://github.com/edithatogo/.github/blob/main/CODE_OF_CONDUCT.md). Preserve attribution and third-party notices. Contribute only material you are entitled to share; resolve unclear permissions before adding third-party content. This guide does not change licensing terms or introduce a CLA or DCO requirement.

## References

- [GitHub contribution guideline conventions](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/setting-guidelines-for-repository-contributors)
- [OpenSSF contribution and quality criteria](https://www.bestpractices.dev/en/criteria)
