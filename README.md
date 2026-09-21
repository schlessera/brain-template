# brain-template

> **Placeholder.** This repository is not usable yet. It is here so that the
> work of building it has somewhere to live.

This will be the starting point for your own brain: a GitHub template you
generate from, ending with a private repository of your own markdown that the
`brain` CLI and any coding agent can operate.

```sh
gh repo create my-brain --template schlessera/brain-template --private --clone
cd my-brain && bun install
# then, in a coding agent: /brain-init
```

## What it will contain

Generated from `template/` in [schlessera/brain-kit](https://github.com/schlessera/brain-kit),
pinned to a published release:

- `brain.config.ts` — your taxonomy and settings
- `CLAUDE.md` — the agent contract, importing the rules from `@schlessera/brain`
- `.mcp.json` — the MCP server registration
- `me/`, `notes/`, `context/` — empty, waiting for your content
- `.agents/skills/` and `.claude/skills/` — the workflow skills

**It ships no taxonomy of its own.** `/brain-init` interviews you and builds
one that fits what you actually keep. That is the feature — a knowledge base
that arrives with somebody else's filing system is a knowledge base you fight.

## What it will not contain

**Hosting.** Running the optional chat UI needs a container, a compose file and
a reverse proxy, and those belong in their own repository so that infrastructure
arrives by version bump and your content stays yours. A separate hosting
template will cover that.

## Where the work is tracked

In [schlessera/brain-kit](https://github.com/schlessera/brain-kit/issues) until
this repository has enough shape to carry its own. Issues about what this
template should contain can be opened here.

## License

MIT
