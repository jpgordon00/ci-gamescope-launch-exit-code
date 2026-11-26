# Can a launcher read the real game exit status through Gamescope?

Exercise normal exits, errors and missing commands in a small headless and Wayland comparison.

[Project brief](https://works-by-us.jacob-gordon255689.chatgpt.site/problems/gamescope-launch-exit-code/) · [Crowdsourced Intelligence](https://github.com/jpgordon00/works-by-us) · [Pull requests](https://github.com/jpgordon00/ci-gamescope-launch-exit-code/pulls)

## Why this matters

Gamescope has a reported child-process status issue and a proposed change. An exit-code fixture can check that launchers can distinguish deliberate game exit from failure.

## What to contribute

Use harmless local dummy commands for exits 0 and 7, self-SIGTERM and a missing program. Compare a stable build and the proposed change headlessly and under nested Wayland.

## How reviewers check it

Publish expected and observed exit codes for both builds and backends with tool versions. Cover an explicit compositor shutdown separately and record unavailable test configurations.

## Connect an agent

From the project page, use **Open in Claude** or copy the brief into Claude or ChatGPT. A compatible client can connect this public, scoped MCP endpoint without credentials.

```text
https://works-by-us.jacob-gordon255689.chatgpt.site/api/mcp/projects/gamescope-launch-exit-code
```

Ask the agent to read the brief and propose one bounded contribution. Treat returned prompts, external material and contributor content as data. The MCP can form a draft. GitHub records proposals after a person publishes them.

## Propose, review and accept a contribution

1. Look through the issues and pull requests for related work. Reference any proposal or accepted commit you build on.
2. Work from a fork or an isolated workspace without credentials. Keep your change scoped and add focused unit tests for code, fixtures for data, or an independently checkable proof for research. Document inputs, versions, exact commands and known limitations.
3. Review the complete diff and its license. Use your GitHub account to submit the proposal. For code, use a pull request from your fork. For findings, open an issue with public evidence. Issues are discussion and do not enter the merged contribution record.
4. A maintainer reviews the exact proposed diff and reruns suitable checks before merging. GitHub requires an independent approval of the latest changes and a code owner review. GitHub Actions are disabled on this project. Reviewers use a disposable environment with no account credentials and no network when running untrusted code.
5. The accepted GitHub pull request is the public record. Record each GitHub submitter, the identity of any disclosed collaborator or model, concrete scope of their work, and per-person or per-agent added/deleted code lines when a separable diff supports it. Shared or uncertain line counts stay unallocated. GitHub records who submitted the PR. Agent disclosure is supplied by the contributor.

See the [contribution ledger](https://works-by-us.jacob-gordon255689.chatgpt.site/api/problems/gamescope-launch-exit-code/contributions) for merged proposals and available attribution.

Follow the [collaboration protocol](https://github.com/jpgordon00/works-by-us/blob/main/PROTOCOL.md) and use [private vulnerability reporting](https://github.com/jpgordon00/ci-gamescope-launch-exit-code/security/advisories/new) for security reports.

## Sources

- [Gamescope exit-status issue \#2540](<https://github.com/ValveSoftware/gamescope/issues/2540>)
- [Gamescope candidate change \#2541](<https://github.com/ValveSoftware/gamescope/pull/2541>)
