# Claude Code Changelog

[![Status](https://status.marckrenn.dev/api/badge/3/status)](https://status.marckrenn.dev/status/cchbot)
[![Uptime](https://status.marckrenn.dev/api/badge/3/uptime)](https://status.marckrenn.dev/status/cchbot)

This repository tracks changes to [Claude Code](https://docs.anthropic.com/en/docs/claude-code)'s system prompt and feature flags across versions.

## What's Tracked

### System Prompts (`cc-prompt.md`)
The internal system prompt that shapes how Claude behaves in the CLI. This is the instruction set that defines Claude Code's capabilities, safety guidelines, tool usage patterns, and behavioral constraints.

### Feature Flags (`cc-flags.md`)
Statsig feature flags embedded in Claude Code, revealing:
- Experimental features being tested
- Feature gates and rollout status
- Dynamic configurations
- A/B test experiments

## How It Works

Each version's files are tagged (e.g., `v2.0.76`). This enables easy diffing between any two versions using GitHub's compare view:

```
https://github.com/marckrenn/claude-code-changelog/compare/v2.0.70...v2.0.76
```

## What Powers [@ClaudeCodeLog](https://x.com/ClaudeCodeLog)

This repo is the backbone of the [@ClaudeCodeLog](https://x.com/ClaudeCodeLog) Twitter/X account, which automatically:

1. Detects new Claude Code releases
2. Extracts system prompts and feature flags
3. Analyzes changes using AI-powered diff generation
4. Posts threaded summaries with deep-links to specific diff sections

The diff URLs include line-specific anchors (e.g., `#diff-...R105-R117`) that link directly to the relevant changes.

## Structure

- `cc-prompt.md` — System prompt (updated with each release)
- `cc-flags.md` — Feature flags (updated with each release)
- Tags (`v1.0.x`, `v2.0.x`) — Version snapshots for diffing

## Example Thread

When a new version is released, [@ClaudeCodeLog](https://x.com/ClaudeCodeLog) posts:

1. **Announcement** — Version number with change counts
2. **CLI Changelog** — Official changelog from Anthropic
3. **Flag Changes** — Added/removed feature flags
4. **Prompt Summary** — Overview of system prompt changes
5. **Detailed Changes** — Individual changes with screenshots and diff links

## Related

- [@ClaudeCodeLog on X](https://x.com/ClaudeCodeLog) — Automated changelog posts
- [cchistory](https://github.com/badlogic/cchistory) — Tool used for system prompt extraction
- [How cchistory works](https://mariozechner.at/posts/2025-08-03-cchistory/) — Technical deep-dive
- [Claude Code Documentation](https://docs.anthropic.com/en/docs/claude-code)
- [Claude Code on npm](https://www.npmjs.com/package/@anthropic-ai/claude-code)
