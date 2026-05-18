# amlmarketplaces/deepseek

Claude Code marketplace federating all `@amlplugins/deepseek-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-deepseek": {
      "source": { "source": "github", "repo": "amlmarketplaces/deepseek" }
    }
  },
  "enabledPlugins": {
      "deepseek-chat@aml-deepseek": true,
      "deepseek-reasoner@aml-deepseek": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/deepseek`, cached under `~/.claude/plugins/cache/aml-deepseek/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (2 total)

- `deepseek-chat` — [@amlplugins/deepseek-chat](https://github.com/amlplugins/deepseek-chat)
- `deepseek-reasoner` — [@amlplugins/deepseek-reasoner](https://github.com/amlplugins/deepseek-reasoner)

## Related

- npm packages: `@amlplugins/deepseek-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
