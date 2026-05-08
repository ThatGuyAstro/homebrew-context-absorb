# homebrew-context-absorb

Homebrew tap for [`context-absorb`](https://github.com/ThatGuyAstro/context-absorb), a cross-CLI session transfer tool for parallel AI coding sessions (Claude Code + Codex).

## Install

```bash
brew install ThatGuyAstro/context-absorb/context-absorb
```

After install, run the post-install hook to wire up the runtime, shell command, and skill wrappers:

```bash
context-absorb install --repo-root "$(brew --prefix context-absorb)/libexec"
```

## What this gets you

The shared `session-absorb` CLI plus seven Claude Code slash commands:

- `/absorb` - click picker for browsing sessions and choosing actions
- `/session-absorb` - canonical alias of `/absorb`
- `/handoff` - structured cross-session work transfer
- `/inbox` - pending handoffs targeted at this session
- `/ack <id>` - mark a handoff absorbed

See the [main repo](https://github.com/ThatGuyAstro/context-absorb) for full docs, command reference, and use cases.

## License

MIT, same as the parent project. Formula source is in this repo at `context-absorb.rb`.
