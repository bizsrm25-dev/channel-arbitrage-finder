# Channel Arbitrage Finder

An AI agent skill that finds a video format you can win with: one where more people want to watch than creators currently make well.

It interviews you about your interests, goals, platforms and resources, and asks how you want to make videos: **faceless with AI**, **faceless but human-made**, **on camera**, or a **hybrid**. Then it researches live YouTube, Shorts, TikTok or Reels data and gives you up to three channel plans. Each plan comes with evidence, names, titles, thumbnails, a ready-to-record first episode, art direction for your production mode, a cost and time budget, and a 30-day test.

The skill is plain Markdown with no code to run and no paid analytics account. It follows the open [Agent Skills specification](https://agentskills.io/specification), so it works in Claude (Claude.ai and Claude Code) and in OpenAI Codex.

## The idea behind it

Niches are industries and formats are markets. The signal to look for is **small accounts repeatedly breaking out far beyond their following in the same format**, while few creators deliver that format well. Once you've found the gap, you can enter it three ways:

1. **Serve the same market better.** Improve what viewers of a working format actually value.
2. **Transfer a proven format.** Bring a viewing mechanic that works elsewhere to a niche where it's missing.
3. **Scale through creators.** Brief several creators on a format that's already working.

The method comes from a short lecture on content arbitrage. [`references/method.md`](channel-arbitrage-finder/references/method.md) summarises it with timestamps and marks clearly which research settings (thresholds, windows, scoring) the skill adds on top.

## Install

Download `channel-arbitrage-finder.zip` from the [latest release](../../releases/latest), or clone this repo.

- **Claude.ai:** go to **Customize → Skills → + → Create skill → Upload a skill**, select the ZIP and enable it. Code execution and file creation must be turned on. ([guide](https://support.claude.com/en/articles/12512180-use-skills-in-claude))
- **Claude Code:** copy the `channel-arbitrage-finder` folder into `~/.claude/skills/` (or `.claude/skills/` inside a project), then type `/channel-arbitrage-finder`. ([docs](https://code.claude.com/docs/en/skills))
- **Codex:** copy the folder into `~/.agents/skills/` (or `.agents/skills/` in a project), then type `$channel-arbitrage-finder`. ([docs](https://developers.openai.com/codex/skills/))

The research stage needs live web search and browsing.

## Use

Say something like *"Find a YouTube channel idea I can make on weekends"* or *"I want to test a faceless history channel."* Answer the short interview and confirm your profile. The skill saves your profile as `channel-profile.md` so you can come back later and ask it to check whether the window is still open.

## What's in the repo

```
channel-arbitrage-finder/        the installable skill
├── SKILL.md                     entry point and workflow
├── references/
│   ├── method.md                the source method, with timestamps
│   ├── intake-questions.md      interview script and branching
│   ├── research-playbook.md     searches, evidence rules, outlier screen
│   ├── scoring-rubric.md        weighted 7-factor ranking
│   ├── production-modes.md      faceless-AI / faceless-human / on-camera / hybrid
│   └── art-styles.md            16 visual styles with prompts
└── templates/
    ├── opportunity-report.md    the report you receive
    └── user-profile.md          reusable creator profile
examples/                        two full test runs (19 Nov 2026)
├── history-and-technology.md    faceless + AI, 10 h/week, $50/month
├── fitness-coach.md             on-camera coach with a home studio
├── research-ledger.md           every query and public metric behind them
├── self-check.md                maps each step of the method to the skill
└── sample-profiles/
```

The example creators are simulated. The channels and numbers in the examples are public YouTube observations from the run date, and they will change.

## Honest limits

- The skill reports what it can verify, and marks everything else **unverified**. It won't invent statistics, and it stops if it has no web access.
- Results are hypotheses to test with a 30-day pilot, not income predictions.
- Check current platform policies on AI-generated and reused content before you publish. The skill links to them in each report.

## License

[MIT](LICENSE)
