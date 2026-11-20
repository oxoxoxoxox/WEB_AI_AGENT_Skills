# Agent guidelines

This repository is a reusable guide library for personal web projects. Its primary language is Korean.

## Select the relevant guide

- Planning and scope: `plan/README.md`.
- UI, visual direction, and reusable components: `design/design-guide.md`.
- Implementation: `development/README.md`.
- Bugs or unexpected behavior: `debugging/README.md`.
- Review and completion: `review/README.md`.
- Session handoff: `memory/README.md`.

Read only the guides relevant to the request. When working on another project, read that project's own instructions and current code first. Explicit user direction and applicable higher-priority instructions take precedence over library guidance.

## Source boundaries

`references/superpowers/` is vendored third-party source material. It is not an automatically installed plugin. Do not treat all of its instructions as globally active merely because the files exist. Read a specific upstream skill when needed or requested, and report material workflow requirements before applying them. Do not install plugins, run upstream scripts or hooks, or launch subagents merely to browse this library.

Do not modify the upstream snapshot for routine guide edits. Change the curated guides instead. For an upstream refresh, follow `references/README.md` and update `references/SUPERPOWERS_SOURCE.md`.

## Editing and verification

- Keep reusable guides separate from personal project facts.
- Preserve source attribution and third-party license notices.
- Distinguish templates, proposals, and verified facts.
- Keep relative Markdown links valid.
- Verify only what the change requires. For documentation changes, check links, paths, whitespace, and repository status. Do not run upstream test suites merely because a reference snapshot is present.
- Do not claim installation, tests, deployment, or publication without checking the actual result.
