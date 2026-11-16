# Wingman feedback

This is the public place to report what Wingman can't do yet, what broke, and what you'd like it to do next.
[Wingman](https://ai.locodev.dev) is an AI copilot for Unreal Engine by LocoDev. Its source code is private; this
repository holds reports and discussion only.

Use it wherever you hit the problem: in the Wingman panel inside Unreal, or in an outside AI app (Claude Code,
Codex, Cursor and others) that talks to Wingman over MCP. AI agents can file reports here too, as long as they
follow the privacy rules below.

## How to report

Open a [new issue](../../issues/new/choose) and pick a form:

- **Tool limitation:** a Wingman tool can't do something it should, refuses a valid request, or reports success
  for something that didn't happen.
- **Bug or crash:** something broke, the editor crashed, or the panel misbehaved.
- **Feature idea:** a new tool or workflow you'd like.

Questions, tips and workarounds go in [Discussions](../../discussions).

Before you post, check [KNOWN-ISSUES.md](KNOWN-ISSUES.md) and search the open issues. If yours is already there,
add a thumbs-up or a comment with your versions instead of opening a new one.

## What makes a report useful

- Your Wingman version (Updates page in the panel) and Unreal Engine version.
- Where it happened: the Wingman panel, or an outside AI app over MCP (and which one).
- The tool name and the arguments you sent, with personal details taken out.
- The exact error or reply text.
- What you expected instead.

## Privacy

This repository is public. Never post:

- project files, assets or `.uproject` folders
- API keys, tokens, passwords or emails
- full paths that include your name (replace them with something like `<Project>/Content/...`)
- chat text you don't want public

We never ask for any of these here.

## What happens next

We read every report. When we accept one, we add the `accepted` label and track the work on our side. When the fix
ships, we close the report with the version that has it and replace its details with a short note, so the page
stays as a record that it was fixed. Fixes and new tools are listed on the Updates page in the Wingman panel, and
fixed entries come off [KNOWN-ISSUES.md](KNOWN-ISSUES.md).
