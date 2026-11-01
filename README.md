# skills

Agent skills I use while building and shipping my own apps. I'm a product engineer in Hamburg: I run [Baby Phone](https://apps.apple.com/sa/app/baby-phone-abc-123-games/id6823124937) (iOS), [SellEazyy](https://selleazyy.com/) (Shopify apps StockPing and OrderPing) and [B1 Atlas](https://b1atlas.com/). Each skill here came out of a step I kept repeating, such as checking a Shopify app idea, writing the App Store listing, designing a paywall or reviewing a draft. They follow the [Agent Skills](https://agentskills.io) format, so they work in Claude Code, Cursor, Codex and other agents that read `SKILL.md`.

Each skill lives in its own repo. This page is the index.

## Shopify

Taken in order, these cover an app from idea to App Store submission.

| Skill | What it does | Install |
|---|---|---|
| [shopify-app-idea-validator](https://github.com/ratul0/shopify-app-idea-validator) | Checks a Shopify app idea against merchant complaints, competitors and revenue potential, scores it on 8 dimensions and gives a verdict from "build it" to "don't build this". Starts from skepticism. | `npx skills add ratul0/shopify-app-idea-validator` |
| [shopify-app-factory](https://github.com/ratul0/shopify-app-factory) | Builds a Shopify app in 7 phases, from discovery and Reddit research to deployment on Fly.io. Shopify code is validated through the Shopify Dev MCP. | `npx skills add ratul0/shopify-app-factory` |
| [shopify-app-listing](https://github.com/ratul0/shopify-app-listing) | Walks through all 14 App Store submission form fields, checks Shopify's wording rules and writes a copy-paste-ready `app-store-listing.md`. | `npx skills add ratul0/shopify-app-listing` |
| [shopify-app-release-assistant](https://github.com/ratul0/shopify-app-release-assistant) | Guides you through the 14 deliverables for submission: name, description, screenshots shot list, privacy and GDPR notes, review instructions, compliance checklist. | `npx skills add ratul0/shopify-app-release-assistant` |
| [shopify-icon-forge](https://github.com/ratul0/shopify-icon-forge) | Takes an app icon from questions to concepts to a clean SVG, then exports PNGs at the sizes the App Store, admin and social previews need. | `npx skills add ratul0/shopify-icon-forge` |

## iOS

Both repos cover SwiftUI app design: screens, onboarding, paywalls, microcopy and review. They hold the same material in two shapes.

| Skill | What it does | Install |
|---|---|---|
| [ios-app-design](https://github.com/ratul0/ios-app-design) | One skill for designing and reviewing SwiftUI screens: layout, onboarding, paywalls and pricing, microcopy, polish and a Must/Should/Could critique. Detail loads on demand from `references/`. | `npx skills add ratul0/ios-app-design` |
| [ios-ux-skills](https://github.com/ratul0/ios-ux-skills) | The same ground split into 19 separate skills (home screen, onboarding, paywall, motion, dark mode, App Store pages and more), for when you want to load one topic at a time. | `npx skills add ratul0/ios-ux-skills` |

If you're not sure which to pick, start with `ios-app-design`.

## Writing

| Skill | What it does | Install |
|---|---|---|
| [depth-writing](https://github.com/ratul0/depth-writing) | Writes and audits persuasive text (articles, landing pages, emails) with a five-layer model from conscious thought down to identity. Audit mode scores a draft 0–3 per layer and names the deepest layer that fails. | `npx skills add ratul0/depth-writing` |

## Install in Claude Code, Cursor or Codex

The [`skills` CLI](https://github.com/vercel-labs/skills) installs a skill into the agent you pick:

```bash
npx skills add ratul0/shopify-app-listing
```

It asks which agents to install for. To skip the prompt, name the agent:

```bash
npx skills add ratul0/shopify-app-listing --agent claude-code
npx skills add ratul0/shopify-app-listing --agent cursor
npx skills add ratul0/shopify-app-listing --agent codex
```

Replace `shopify-app-listing` with any repo name from the tables above. Start a new session afterwards; skills trigger from their description, and you can also ask for one by name.

**Without the CLI**, clone a repo into your agent's skills directory:

```bash
# Claude Code
git clone https://github.com/ratul0/depth-writing.git ~/.claude/skills/depth-writing

# Codex
git clone https://github.com/ratul0/depth-writing.git ~/.codex/skills/depth-writing
```

`ios-ux-skills` holds its skills in a `skills/` folder, so copy the folders you want from there rather than cloning the whole repo into one directory.

## Feedback

If a skill gives you a bad result, open an issue on that skill's repo with the prompt you used and what you got back.
