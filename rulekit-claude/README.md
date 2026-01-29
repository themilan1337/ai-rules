# Vue.js RuleKit

> Vibe code Vue applications with confidence 🧑‍💻

## Installation

### 1. Copy Rules

Copy `PROJECT/CLAUDE.md` to your project root:

```sh
cp PROJECT/CLAUDE.md ~/my-project/
```

> [!TIP]
> **Fill the name and description** of your project in the root `CLAUDE.md`/`AGENTS.md` file. Add any project-specific workflow like creating PRs, using a specific MCP server, etc.

**Claude Code only:** Copy global commands from `HOME/` to `~/`—see `HOME/README.md` for instructions.

**Linking (testing only):**

```sh
ln -s <absolute-path-to-vue-rulekit>/PROJECT/CLAUDE.md ~/my-project/CLAUDE.md
```

### 2. Install Skills

```sh
pnpx skills add git@github.com:posva/vue-rulekit.git
```

> [!NOTE]
> SSH required (private repo, HTTPS won't work).

## Other Agents

For non-Claude agents, rename `CLAUDE.md` to `AGENTS.md`. Supported: Codex, Jules, Cursor, Windsurf, Devin, GitHub Copilot, Gemini CLI, VS Code, Zed, Warp, Aider, and [more](https://agents.md/).

## Recommended Tools

### Command Line

- [`magick`](https://imagemagick.org/) - Image manipulation: `brew install imagemagick`
- [`cwebp`](https://developers.google.com/speed/webp) - WebP format: `brew install webp`

### MCP Servers

Keep MCP servers **per project**—they can bloat context and shorten sessions.

#### Nuxt UI

If using [`@nuxt/ui`](https://ui.nuxt.com), [add their MCP server](https://ui.nuxt.com/docs/getting-started/ai/mcp#claude-code).

#### Browser Automation

- [agent-browser](https://github.com/vercel-labs/agent-browser): Simple, light, effective (used in `HOME/.claude/CLAUDE.md`)
- [Playwright MCP](https://github.com/microsoft/playwright-mcp): Powerful but heavy on context, I personally avoid it

## Resources

Read these fully (no AI summaries):

- [Claude best practices](https://www.anthropic.com/engineering/claude-code-best-practices): Rules organization, custom commands, prompt improvement
- Use `/clear` often—larger context leads to hallucinations and rule drift. Split tasks into smaller ones.

## Roadmap

- [x] Vue Components best practices
- [ ] Composables best practices
- [x] Vue Router + file based routing best practices
- [x] Support for Cursor
- [ ] Pinia Colada best practices
- [ ] Nuxt best practices
- [x] Nuxt UI (use the mcp server)
- [x] Testing Components best practices
- [ ] VueUse most used composables
