# Changelog

All notable changes in the [thekingoffamily/OpenDots](https://github.com/thekingoffamily/OpenDots) fork.

Format based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Changed

- Default model provider in `.env.example` is DeepSeek (`OPENAI_BASE_URL=https://api.deepseek.com/v1`, `OPENAI_MODEL=deepseek-chat`) so local setup only needs `OPENAI_API_KEY` (plus `INTELLIGENCE_API_KEY` for CopilotKit).
- `npm run dev` no longer sets `NODE_ENV=development` via Unix shell syntax (broken on Windows `cmd`). Use `NODE_ENV=development` in `.env` instead (documented in `.env.example`).

### Notes

- Slack and Voice remain optional; empty `INTELLIGENCE_API_KEY` still blocks conversation setup in the UI.
- Upstream remote for syncing: `https://github.com/CopilotKit/OpenDots.git`.
