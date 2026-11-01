# Topics and homepages

Suggested GitHub topics and homepage for each skill repo. Homepage is the repo's [skills.sh](https://skills.sh) page. Nothing here has been applied yet.

`--add-topic` only adds, so `shopify-app-release-assistant` keeps the topics it already has (`agent-skill`, `ai-agent`, `app-submission`, `claude-code`, `cursor`, `shopify`, `shopify-app`, `shopify-app-store`, `shopify-development`, `skills-sh`). The others have none today.

GitHub allows 20 topics per repo, lowercase, hyphens only.

## Topics

| Repo | Homepage | Topics |
|---|---|---|
| shopify-app-idea-validator | https://skills.sh/ratul0/shopify-app-idea-validator | `agent-skills`, `claude-code`, `skills-sh`, `shopify`, `shopify-app`, `idea-validation`, `market-research`, `competitive-analysis` |
| shopify-app-factory | https://skills.sh/ratul0/shopify-app-factory | `agent-skills`, `claude-code`, `skills-sh`, `shopify`, `shopify-app`, `react-router`, `prisma`, `polaris`, `fly-io` |
| shopify-app-listing | https://skills.sh/ratul0/shopify-app-listing | `agent-skills`, `claude-code`, `cursor`, `codex`, `skills-sh`, `shopify`, `shopify-app`, `shopify-app-store`, `app-store-listing` |
| shopify-app-release-assistant | https://skills.sh/ratul0/shopify-app-release-assistant | `codex`, `app-store-listing`, `gdpr` (adds to the existing set) |
| shopify-icon-forge | https://skills.sh/ratul0/shopify-icon-forge | `agent-skills`, `claude-code`, `cursor`, `codex`, `skills-sh`, `shopify`, `shopify-app`, `app-icon`, `svg` |
| ios-app-design | https://skills.sh/ratul0/ios-app-design | `agent-skills`, `claude-code`, `cursor`, `codex`, `skills-sh`, `ios`, `swiftui`, `ui-design`, `ux-design`, `paywall`, `human-interface-guidelines` |
| ios-ux-skills | https://skills.sh/ratul0/ios-ux-skills | `agent-skills`, `claude-code`, `cursor`, `codex`, `skills-sh`, `ios`, `swiftui`, `ux-design`, `onboarding`, `paywall`, `human-interface-guidelines` |
| depth-writing | https://skills.sh/ratul0/depth-writing | `agent-skills`, `claude-code`, `codex`, `skills-sh`, `copywriting`, `writing`, `persuasion` |
| skills (this repo) | none | `agent-skills`, `claude-code`, `cursor`, `codex`, `skills-sh`, `shopify`, `ios`, `swiftui`, `writing`, `product-engineering` |

## Commands

Run only after approval. The `skills` repo command needs the repo to exist first.

```bash
gh repo edit ratul0/shopify-app-idea-validator --homepage "https://skills.sh/ratul0/shopify-app-idea-validator" \
  --add-topic agent-skills --add-topic claude-code --add-topic skills-sh --add-topic shopify \
  --add-topic shopify-app --add-topic idea-validation --add-topic market-research --add-topic competitive-analysis

gh repo edit ratul0/shopify-app-factory --homepage "https://skills.sh/ratul0/shopify-app-factory" \
  --add-topic agent-skills --add-topic claude-code --add-topic skills-sh --add-topic shopify \
  --add-topic shopify-app --add-topic react-router --add-topic prisma --add-topic polaris --add-topic fly-io

gh repo edit ratul0/shopify-app-listing --homepage "https://skills.sh/ratul0/shopify-app-listing" \
  --add-topic agent-skills --add-topic claude-code --add-topic cursor --add-topic codex --add-topic skills-sh \
  --add-topic shopify --add-topic shopify-app --add-topic shopify-app-store --add-topic app-store-listing

gh repo edit ratul0/shopify-app-release-assistant --homepage "https://skills.sh/ratul0/shopify-app-release-assistant" \
  --add-topic codex --add-topic app-store-listing --add-topic gdpr

gh repo edit ratul0/shopify-icon-forge --homepage "https://skills.sh/ratul0/shopify-icon-forge" \
  --add-topic agent-skills --add-topic claude-code --add-topic cursor --add-topic codex --add-topic skills-sh \
  --add-topic shopify --add-topic shopify-app --add-topic app-icon --add-topic svg

gh repo edit ratul0/ios-app-design --homepage "https://skills.sh/ratul0/ios-app-design" \
  --add-topic agent-skills --add-topic claude-code --add-topic cursor --add-topic codex --add-topic skills-sh \
  --add-topic ios --add-topic swiftui --add-topic ui-design --add-topic ux-design --add-topic paywall \
  --add-topic human-interface-guidelines

gh repo edit ratul0/ios-ux-skills --homepage "https://skills.sh/ratul0/ios-ux-skills" \
  --add-topic agent-skills --add-topic claude-code --add-topic cursor --add-topic codex --add-topic skills-sh \
  --add-topic ios --add-topic swiftui --add-topic ux-design --add-topic onboarding --add-topic paywall \
  --add-topic human-interface-guidelines

gh repo edit ratul0/depth-writing --homepage "https://skills.sh/ratul0/depth-writing" \
  --add-topic agent-skills --add-topic claude-code --add-topic codex --add-topic skills-sh \
  --add-topic copywriting --add-topic writing --add-topic persuasion

# after `gh repo create ratul0/skills --public ...`
gh repo edit ratul0/skills --description "Agent skills for Shopify app builders, SwiftUI designers and writers. Index of my skill repos." \
  --add-topic agent-skills --add-topic claude-code --add-topic cursor --add-topic codex --add-topic skills-sh \
  --add-topic shopify --add-topic ios --add-topic swiftui --add-topic writing --add-topic product-engineering
```

## Notes

- skills.sh status on 2026-11-01: 200 for `shopify-app-idea-validator`, `shopify-app-factory`, `shopify-app-release-assistant` and `ios-app-design`. 404 for `shopify-app-listing`, `shopify-icon-forge`, `ios-ux-skills` and `depth-writing`. Those four are probably not indexed yet; I haven't confirmed what triggers indexing. Either leave their homepage unset for now or set it and re-check later.
- Repo descriptions are fine as they are, except `shopify-icon-forge`, which ends with the install command; trim it if you like.
