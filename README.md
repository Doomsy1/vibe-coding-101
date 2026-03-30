# Agentic Engineering 101: AI Coding Tools for Students

A guide to AI-assisted coding tools, specifically for university students who get ridiculous amounts of free credits and trials. Seriously, take advantage of this while you can.

## Quick Reference

| Tool | Credits/Limits | Best For | Student Perk |
|------|----------------|----------|--------------|
| **OpenAI Codex** | Practically unlimited | Best overall | [$100 student credits](https://developers.openai.com/community/students) |
| **Claude Code** | $5-15 every 5 hours | Precise edits, planning | [Campus program](https://claude.com/programs/campus) |
| **Cursor** | ~$45/month in API credits | Quick, precise edits | [1 year free](https://cursor.com/en-US/students) |
| **OpenCode** | Free models available | Great UX, parallel | Free |
| **GitHub Copilot** | ~$80/month in usage | IDE integration | [Free with Pack](https://education.github.com/pack) |
| **Antigravity** | Good limits | Planning | Free (Google, data concerns) |
| **Gemini CLI** | ~$20/day | Backup option | Free Year (w/ Pro) |
| **AI Studio** | Basically unlimited | General use | Free |
| **Perplexity** | Pro features | Research + coding | [1 month + referrals](https://www.perplexity.ai/help-center/en/articles/12162294-how-to-verify-your-student-status) |
| **Gemini Pro** | Hard to hit limits | General use | [1 month trial](https://gemini.google/students/) |

---

## Tier 1: Worth Paying for

### [OpenAI Codex](https://openai.com/codex/)
This is the best tool right now. Not "one of the best." Just the best. If you're serious about agentic coding, this is what I'd recommend first. The limits are insanely hard to hit, to the point that they feel basically unlimited. GPT-5.4 is also the best model overall for coding right now. The one place it still kinda sucks is UI and front-end. It gets sloppy fast, so if I care about how something looks, I'd much rather use Claude 4.6 Opus or Gemini 3.1 Pro.

### [Claude Code](https://claude.com/product/claude-code)
Claude Code is still really, really good. Its planning mode is awesome, and for precise edits it's still one of my favorites. I also trust it way more than GPT-5.4 for front-end work when I actually want the result to look good. The annoying part is the credit cycle. You get $5-15 every 5 hours, which sounds great until you actually start using it hard and suddenly you're rationing messages. If you want free access as a student, that usually comes through a campus program, ambassador, or builder-style initiative, not some automatic perk that everybody gets.

### [Cursor](https://cursor.com/)
You get around $45/month in API credits, and eligible university students can get [one free year of Cursor Pro](https://cursor.com/en-US/students). I still like it for random vibe-coding experiments and quick edits inside the editor. It's not my main thing anymore, but it's still very nice to have around.

---

## Tier 2: Good because it's free

### [GitHub Copilot](https://github.com/features/copilot)
You get around $80/month of usage. The annoying part is that it isn't measured like normal API credits, so you can't be quite as reckless with it. Still, verified students get Copilot's premium features for free through the [GitHub Student Developer Pack](https://education.github.com/pack), which is a pretty absurd deal.

### [OpenCode](https://opencode.ai/)
Another CLI tool, and honestly still one of the best user experiences of any of them. If you want free models, my current recommendations are Nemotron 3 Super and Minimax M2.5. Obviously they'll use your data for whatever they want, but it feels very similar to Claude Code, maybe even more polished. The UI has some finicky behaviors, but overall very solid. You can also plug in other providers like Google to use their API credits, which is nice.

### Codex Student Note
Codex still isn't just straight-up free for students forever, which is unfortunate. But OpenAI did recently add [$100 in free API credits for eligible students](https://developers.openai.com/community/students), which is enough to get started without immediately paying. After that, though, if you're going to spend money on one thing, this is the one I would spend it on.

---

## Tier 3: Other Free Options

### [Antigravity](https://antigravity.google/) (Google)
Free for everyone, which is a little concerning because they probably munch on your data. Pretty good usage limits though. Not exactly sure how much, but it works well for planning. The UX isn't great, but it's definitely usable.

### [Gemini CLI](https://github.com/google-gemini/gemini-cli)
Not a good user experience at all. Feels very clunky. But you get credits, around $20 a day, so it's a solid backup.

### [AI Studio](https://aistudio.google.com/)
Not really for coding, but great for chatting. Usage limits? They basically don't exist. Pretty much unlimited.

### [Perplexity](https://www.perplexity.ai/)
Perplexity changed the student deal, so it's not the crazy free-year thing anymore. Right now it's more like [student verification](https://www.perplexity.ai/help-center/en/articles/12162294-how-to-verify-your-student-status), one month of Pro, and then extra months through referrals. Still useful though, especially since you can bounce between a bunch of frontier models. Here's my [referral link](https://plex.it/referrals/8N3ELADE) if you want to help me out.

### [Gemini Pro](https://gemini.google/)
Google's older student offer was better. The current [Gemini for Students](https://gemini.google/students/) has a one month Google AI Pro trial in some regions instead of the old year-long deal. Still, if you already have it, the limit is weirdly hard to hit in practice.

---

## Pro Tips

### Use LSP
LSP stands for Language Server Protocol. Basically, it lets the AI see real-time errors from your editor, like type errors, missing imports, and syntax issues. So instead of spitting out broken code that you have to fix yourself (or wait for it to rerun), it catches mistakes as it writes. Seriously, turn this on.

### Use Subagents & Skills
These are basically really good prompts that the model can decide to use. They make a huge difference.

**Subagent Resources:**
- [Claude Code Subagents Docs](https://code.claude.com/docs/en/sub-agents)
- [Awesome Claude Code Subagents](https://github.com/VoltAgent/awesome-claude-code-subagents)

**Skills Resources:**
- [Claude Code Skills Docs](https://code.claude.com/docs/en/skills)
- [Official Anthropic Skills](https://github.com/anthropics/skills)
- [Awesome Claude Skills](https://github.com/ComposioHQ/awesome-claude-skills)

### OpenCode Parallel Sessions
Cool trick: you can start multiple sessions and have them running in parallel, all from one terminal window. No need to open multiple terminals.

### Use Agent Apps for Multi-Tasking
If you're juggling multiple tasks or running a bunch of agents at once, an app can honestly be way nicer than having twelve terminal windows open like a maniac. Tools like [T3 Chat / T3 Code](https://t3.codes/) and the [Codex app](https://developers.openai.com/codex/app) are not separate providers, they're just cleaner interfaces for using the same agents. T3 also gives you Claude Code, which is nice.

### Use Voice Dictation
[Wispr Flow](https://wisprflow.ai) is a voice dictation tool that actually understands code. You can speak naturally and it formats everything correctly, including syntax, file names, and code structure. It has deep integrations with Cursor, and VS Code. If you want to support me, here's my [referral link](https://wisprflow.ai/r?ARIO16).

---

## My Workflow

Here's how I actually use these tools:

| Situation | Tool |
|-----------|------|
| Most coding tasks | **OpenAI Codex** |
| Starting from scratch, need to plan carefully | **OpenAI Codex** or **Claude Code** |
| Quick, precise edits | **Claude Code** |
| Random vibe coding experiments | **Cursor** |
| UI or front-end that needs to actually look good | **Claude Code (Opus 4.6)** or **Gemini 3.1 Pro** |
| Don't want to burn credits on something | See below |

### Credit Management Strategy
When I don't want to use my good credits on something less important:
1. Use **OpenAI Codex** for the main task
2. Switch to **Claude Code** if I want more precise edits or better planning
3. Use **Cursor** for experiments
4. Fall back to **OpenCode**, **Copilot**, **Antigravity**, or **Gemini CLI** when I want to save money

For most things, though, I just use Codex now because it's that good.

---

## Why This Guide?

University students get absurd benefits from these companies: free trials, massive credit allowances, the works. This guide is specifically about maximizing those perks while you still have your university email.

Happy coding!
