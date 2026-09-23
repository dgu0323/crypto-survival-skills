# Crypto Survival Skills

Workflow skills for Grok. They locate you in the Web3 / crypto food chain. They do not pick tokens.

- Pack version: 1.5 (2026-09-23)
- Skill versions: decode 1.4 · triage 1.4 · niche 1.4 · profit-system 1.5
- Install into the Grok user skills directory (`.grok/skills/`)
- Languages: [Chinese README](./README.md) · [English README](./README.en.md)

Skill bodies are written in Chinese. **Output follows the user's language.** Do not install a second English-only copy.

User prompts carry source material only. Output format lives in `SKILL.md`. Do not restate the template in chat.

## Source and disclaimer

Distilled from:

- Author: ZTZZ (X: [@ZTZZBTC](https://x.com/ZTZZBTC))
- Essay: [Slow Is Fast / 慢就是快](https://x.com/ztzzbtc/status/2102374831119610291) (2026-09-22)

This pack is a **third-party workflow wrapper**, not an official ZTZZ release and not a reprint of the essay.

**Not investment advice.** No token lists, targets, size, or leverage. Keep the source link if you redistribute. Do not rebrand this as official or as a guaranteed profit system.

## The four skills

| Directory | Version | Use when | You provide |
|---|---|---|---|
| `crypto-incentive-decode` | 1.4 | Posts, chats, KOLs, "bullish long term" | Skill name + link or paste |
| `crypto-project-triage` | 1.4 | Protocols, airdrops, TGEs, buy vs use vs work | Skill name + ticker or CA |
| `crypto-niche-builder` | 1.4 | Income beyond buying tokens; 90-day plan | Skill name + optional skills / hours / narrative |
| `crypto-profit-system` | 1.5 | Joining a team, full-time, adding size, token salary, FOMO | Skill name + what you are about to do |

Routing:

```
New narrative / new post     -> incentive-decode
Still want to participate    -> project-triage
Want to earn in the industry -> niche-builder
About to spend time or cash  -> profit-system
```

## Install

```text
/home/workdir/.grok/skills/<skill-name>/
```

One folder per skill. Folder name must match `name` in `SKILL.md`. Keep `references/`. Start a **new conversation** after install.

### A. Drop the zip on Grok

```text
Install these 4 skills into /home/workdir/.grok/skills/
Keep the original folder names. Each folder must include SKILL.md and references/.
Ask before overwriting same-name folders. Then list dirs and check name matches folder.
```

### B. Copy files

```bash
cp -R crypto-incentive-decode crypto-project-triage crypto-niche-builder crypto-profit-system \
  /home/workdir/.grok/skills/
```

### C. GitHub

```text
Install the skill from https://github.com/<owner>/<repo>/tree/main/crypto-incentive-decode
```

Existing same-name folders abort the install. Private repos need `GITHUB_TOKEN` or `GH_TOKEN`.

## Use (short triggers)

```text
Use crypto-incentive-decode
https://x.com/……
```

```text
Use crypto-project-triage on $BP
```

```text
Use crypto-niche-builder
Java backend, about 8 hours a week, looking at Backpack $BP
```

```text
Use crypto-profit-system
$BP doubled this week, the group wants me to add at 0.84, I have no airdrop
```

Combined:

```text
Decode this post first. If it is still worth a look, run triage. I am a retail buyer.
```

```text
Use niche-builder to pick the work, then profit-system to keep rent money off the same narrative.
```

## Confirm and edit

```text
List my current user skills only.
```

Decode must fetch verification itself and list sources. Triage must split three columns. Niche must include a this-week action. Profit-system must open with a default action.

When editing files:

- `name` equals the folder name (lowercase, digits, single hyphens)
- `description` is one unquoted line; do not use `: ` (colon-space)
- Triggers belong in `description`
- Validate: `bash /root/.grok/skills/skill-creator/scripts/validate-skill.sh /home/workdir/.grok/skills/<skill-name>`

## Do not use this pack to

- Call direction, list tokens, or set targets
- Treat the food chain as proof of collusion
- Merge the four skills into one file
- Share skills next to keys, exchange APIs, or seed phrases

## License and credit

The essay belongs to ZTZZ. This pack is a structured excerpt for personal learning and agent workflows. Keep the original link when you share it.
