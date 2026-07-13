# Agentic Engineering 101: AI Coding Tools for Students

A practical guide to AI coding agents, with a focus on the unusually good deals available to university students.

> Last reviewed: July 12, 2026. Pricing, quotas, model access, and student offers change fast. The linked official pages are the source of truth.

## Quick Reference

| Tool | Current access and limits | Best for | Student angle |
|------|---------------------------|----------|---------------|
| **OpenAI Codex** | Included usage depends on your ChatGPT plan | End-to-end engineering, parallel agents, long tasks | [Verified university students in the US and Canada can claim $100 in ChatGPT credits for Codex](https://developers.openai.com/community/students) |
| **Claude Code** | Included with Claude Pro and Max; usage limits apply | Precise edits, planning, front-end work | [Claude for Education](https://claude.com/solutions/education) is institution-wide, and Anthropic is accepting applications for fall 2026 student programs |
| **GitHub Copilot** | Free plan includes 2,000 completions per month; paid plans add agent usage | IDE integration and low-friction autocomplete | [Copilot Student is free for verified students](https://github.com/features/copilot/plans) |
| **Cursor** | Everyone can start free; paid access varies by plan | Editor-first agent workflows and quick experiments | The old blanket one-year student offer is gone; [student promotions now run through campus and online events](https://cursor.com/students) |
| **OpenCode** | Open source, with free models or your own providers | Flexible terminal, IDE, and desktop workflows | Free to install, with provider costs depending on what you connect |
| **Gemini CLI** | Free tier currently lists 60 requests per minute and 1,000 requests per day with a personal Google account | A generous free terminal agent and backup option | No student verification required for the personal-account free tier |
| **Google Antigravity** | Limits vary by Google AI plan | Agent-first IDE workflows | Google AI Pro and Ultra include expanded Antigravity limits |
| **Google AI Studio** | Free and paid access depend on the model and region | Prompting, prototyping, and API experiments | Google AI Pro includes expanded AI Studio limits |
| **Perplexity Education Pro** | Discounted Pro plan for verified students and educators | Research, source discovery, and Learn Mode | Verify through the Education plan |
| **Gemini app** | Free access plus paid Google AI plans | General study, research, and multimodal work | Google's previous student offer ended March 11, 2026 in the current region |

## My Current Picks

### [OpenAI Codex](https://openai.com/codex/)

This is still my first recommendation for serious agentic engineering. It works across ChatGPT, the editor, and the terminal, and it is especially strong when a task needs repository-wide reasoning, testing, pull requests, worktrees, or several agents working in parallel.

The student offer is better than the old wording in this guide suggested: eligible university students in the United States and Canada can claim $100 in ChatGPT credits for Codex. These are not API credits, and they expire 12 months after the grant date.

### [Claude Code](https://claude.com/product/claude-code)

Claude Code remains one of my favorite tools for careful planning, precise edits, and front-end work. Claude Code is included with Claude Pro at $20 monthly, or $17 per month with annual billing. Max plans are currently $100 or $200 per month, and usage limits apply.

There is no universal individual student discount listed. Student access is mainly through institution-wide Claude for Education programs and Anthropic's student programs.

### [GitHub Copilot](https://github.com/features/copilot)

Copilot is the most dependable standing student deal. Its free plan includes 2,000 completions per month, while verified students can use Copilot Student for free. It is a strong default when you want AI directly inside an IDE without adopting a separate agent workflow.

### [Cursor](https://cursor.com/)

Cursor is still great for fast editor-based work and experiments. The important update is that the old one-year-free student offer is no longer a standing benefit. Cursor now points students to promotions at campus and online events, while everyone can start with the free plan.

### [OpenCode](https://opencode.ai/)

OpenCode is the best open and provider-flexible option in this list. It runs in the terminal, IDE, or desktop app, supports LSP integration, can run multiple sessions in parallel, and lets you use included free models or connect other providers.

### [Gemini CLI](https://github.com/google-gemini/gemini-cli)

Gemini CLI is a much stronger free backup than the old "$20 per day" estimate implied. Google's current repository lists a personal-account free tier of 60 requests per minute and 1,000 requests per day. It also includes shell and file tools, web fetching, Google Search grounding, and MCP support.

### [Google Antigravity](https://antigravity.google/) and [Google AI Studio](https://aistudio.google.com/)

Antigravity is Google's agent-first development environment. Exact limits are plan-dependent, so I would not attach a made-up daily dollar value to it. Google AI Pro currently advertises expanded limits in Antigravity, AI Studio, and Jules.

AI Studio is useful for prompt experiments, model comparison, and quick prototypes. It is not a direct replacement for a repository-aware coding agent.

### [Perplexity Education Pro](https://www.perplexity.ai/help-center/en/articles/12590157-what-is-education-pro)

Perplexity is primarily a research tool, not my main coding agent. Education Pro is currently a discounted plan for verified students and educators, with Pro features plus Learn Mode and education-specific guidance. The old free-year and referral-month framing is no longer the main student offer.

## Pro Tips

### Put Instructions in the Repository

Do not rely on a giant prompt you paste into every session. Add an `AGENTS.md` or the tool-specific equivalent with setup commands, test commands, style rules, architectural boundaries, and a clear definition of done.

For Codex, the official docs explain how global and repository-level `AGENTS.md` files are discovered and combined.

### Use LSP

Language Server Protocol support gives the agent live feedback about type errors, missing imports, symbols, and syntax. Turn it on whenever the tool supports it.

### Use Skills and Subagents

Skills package repeatable workflows. Subagents are useful for independent investigation, implementation, and review. Keep their jobs narrow and make the parent agent verify the result.

Useful starting points:

- [Codex skills](https://learn.chatgpt.com/docs/build-skills)
- [Codex subagents](https://learn.chatgpt.com/docs/agent-configuration/subagents)
- [Claude Code subagents](https://code.claude.com/docs/en/sub-agents)
- [Claude Code skills](https://code.claude.com/docs/en/skills)

### Use One Branch or Worktree per Task

Parallel agents are only useful when they do not overwrite each other. Give each task its own branch or worktree, keep the scope small, and merge through pull requests.

- [Codex worktrees](https://learn.chatgpt.com/docs/environments/git-worktrees)

### Require Verification

A good agent should show evidence, not just say it is done. Ask it to run the relevant tests, linters, type checks, builds, or browser checks and summarize the actual output.

### Check Data Policies

"Free" often means a different data-use policy, lower privacy guarantees, or a provider-specific retention setting. Check the current policy before using private coursework, research data, credentials, or company code.

### Parallelize Independent Work

Run agents in parallel for tasks that can be reviewed independently, such as research, test writing, migration planning, or separate bug fixes. Keep one controller responsible for scope, evidence, and integration.

## My Durable Setup: [Compass](https://github.com/ariobarin/compass)

I keep my reviewed, portable agent setup in **Compass**. It contains shared instructions, agents, skills, workflows, install wiring, and verification scripts for Codex and related tools.

Start there if you want the actual setup behind this guide rather than another collection of disconnected prompts.

## My Workflow

| Situation | Tool |
|-----------|------|
| Most coding tasks | **OpenAI Codex** |
| Careful planning or precise edits | **Claude Code** |
| Front-end work where visual quality matters | **Claude Code**, then verify in a browser |
| IDE-first autocomplete and chat | **GitHub Copilot** |
| Fast editor experiments | **Cursor** |
| Open or provider-flexible workflow | **OpenCode** |
| Free terminal backup | **Gemini CLI** |
| Research and source discovery | **Perplexity** |
| Durable agent instructions and workflows | **Compass** |

The exact model matters less than the workflow around it. Give the agent good repository context, isolate its changes, make it verify its work, and review the diff before merging.

## Referral Links

These are optional referral links:

- [Perplexity](https://plex.it/referrals/8N3ELADE)
- [Wispr Flow](https://wisprflow.ai/r?ARIO16)

## Official Sources

- [OpenAI Codex](https://openai.com/codex/)
- [Codex for Students](https://developers.openai.com/community/students)
- [Codex AGENTS.md documentation](https://learn.chatgpt.com/docs/agent-configuration/agents-md)
- [Claude Code](https://claude.com/product/claude-code)
- [Claude for Education](https://claude.com/solutions/education)
- [GitHub Copilot plans](https://github.com/features/copilot/plans)
- [GitHub Student Developer Pack](https://education.github.com/pack)
- [Cursor for Students](https://cursor.com/students)
- [OpenCode](https://opencode.ai/)
- [Gemini CLI](https://github.com/google-gemini/gemini-cli)
- [Google AI plans](https://one.google.com/about/google-ai-plans/)
- [Gemini for Students](https://gemini.google/students/)
- [Perplexity Education Pro](https://www.perplexity.ai/help-center/en/articles/12590157-what-is-education-pro)

Happy coding!
