---
source_path: /Users/kim/.claude/skills/browser-automation
generated: 2025-12-01T13:30:00Z
git_sha: b75fd51d2702e678b15ef7ce28cf6993a31edb62
git_branch: master
status: complete
files_count: 3
subdirs_count: 0
---

# browser-automation

## Overview

A Claude Code skill for browser automation using Microsoft's Playwright MCP server. Activates when WebFetch fails due to JavaScript-heavy content, access restrictions, or forbidden responses. Provides configuration guidance for headless mode, Chrome profile reuse (for authenticated sessions), and profile setup on new machines. Includes comprehensive research documentation comparing Playwright vs Puppeteer for modern web scraping.

## Key Files

| File | Purpose |
|------|---------|
| SKILL.md | Skill definition with activation trigger, allowed tools (`mcp__playwright__*`, Bash), and configuration instructions for headless mode and Chrome profile setup |
| research-playwright-puppeteer-mcp.md | Detailed research comparing Playwright and Puppeteer for JS-heavy site scraping, covering Chrome profile reuse, auto-wait features, MCP integration, and practical forum scraping patterns |
| .gitignore | Excludes the `chrome-profile/` directory from version control (contains sensitive session data) |

## Subdirectories

None.

## Search Tags

browser-automation playwright puppeteer mcp web-scraping javascript spa chrome-profile authentication headless webfetch fallback forum-scraping network-interception auto-wait locator-api
