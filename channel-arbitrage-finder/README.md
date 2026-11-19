# Channel Arbitrage Finder

This skill helps you choose a repeatable video series you can afford to make. It interviews you, looks up real channels and videos, and gives you up to three channel plans with a first episode and a 30-day test. Allow live web search and browsing for the research stage. No paid analytics subscription is required. The skill is a folder of Markdown files with no code to run or accounts to connect.

## Install once

- **Claude.ai.** Keep the download zipped. Open **Customize → Skills → + → Create skill → Upload a skill**, select `channel-arbitrage-finder.zip` and enable it. Claude requires code execution and file creation to be enabled for custom skills. [Claude's installation guide](https://support.claude.com/en/articles/12512180-use-skills-in-claude)
- **Claude Code.** Unzip the download. Copy the entire `channel-arbitrage-finder` folder into `~/.claude/skills/` for personal use, or `.claude/skills/` inside a project. Open a chat and type `/channel-arbitrage-finder`. [Claude Code skill locations](https://code.claude.com/docs/en/skills)
- **Codex.** Unzip the download. Put the entire folder in `~/.agents/skills/` for personal use, or `.agents/skills/` in your project. Open Codex and type `$channel-arbitrage-finder`. Restart Codex if the skill has not appeared yet. [Codex skill locations](https://developers.openai.com/codex/skills/)

On a Mac, use **Finder → Go → Go to Folder** and paste the destination such as `~/.agents/skills/`. If it is missing, create the enclosing folders in your home folder. On Windows, the personal folder begins inside your user folder, for example `%USERPROFILE%\.agents\skills\`. After copying, opening the skill folder should show `SKILL.md`, `references` and `templates` immediately. The format follows the [Agent Skills specification](https://agentskills.io/specification).

## Start a run

Try “Find a YouTube channel idea I can make on weekends” or “I want to test a faceless history channel.” Answer the short interview and confirm your profile. The agent searches the selected platform and shows what the evidence supports. You can bring a saved `channel-profile.md` next time and say “Use this profile and check whether the window is still open.”

The sample research settings are author additions. The source video teaches a qualitative signal: smaller accounts repeatedly reach far beyond their following in the same format while relatively few creators meet the need well. The report labels unverified data and separates proposed pilots from opportunities that pass the evidence check. Pick a finalist to continue with 30 titles, scripts for the first three episodes, or a brand kit.
