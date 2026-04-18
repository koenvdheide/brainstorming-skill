# brainstorming-skill

A Claude Code plugin that walks ideas through a structured brainstorming and spec-writing workflow, with an External Review Round that dispatches the `reviewer` subagent and `/codex:codex` red-team.

Invokes as `/brainstorming:brainstorming` once installed.

This is a modified fork of the `brainstorming` skill from [obra/superpowers](https://github.com/obra/superpowers) (MIT-licensed, Copyright © 2025 Jesse Vincent). See `LICENSE-UPSTREAM` and `NOTICE` for attribution.

## Install

Via the review-plugins marketplace:

```text
/plugin marketplace add koenvdheide/review-plugins
/plugin install brainstorming@review-plugins
```

Or directly from this repo:

```text
/plugin marketplace add koenvdheide/brainstorming-skill
/plugin install brainstorming@brainstorming-skill
```

## Dependencies

The External Review Round dispatches the `reviewer` subagent and invokes `/codex:codex`. Install those plugins first:

```text
/plugin install claude-reviewer@review-plugins
/plugin install codex@review-plugins
```

If either is unavailable, the skill falls back to self-review with a flagged caveat.

## License

MIT (own code) + MIT (upstream fork). See [`LICENSE`](LICENSE), [`LICENSE-UPSTREAM`](LICENSE-UPSTREAM), and [`NOTICE`](NOTICE).
