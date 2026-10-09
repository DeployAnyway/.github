# DeployAnyway

![DeployAnyway husky developer badge](https://deployanyway.github.io/assets/deployanyway-husky.png)

**Tools for developers who probably should know better.**

Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

small open-source tools for expressing yourself, debugging, regrouping, logging and deciding what to ship. Choose the one(s) that helps your day.

Dallas and Benji, Todd's fun-loving, high-energy huskies, inspire the mindset: stay curious, bring some joy, and make room for play while doing the work. Developers deserve that too. A good joke can make a frustrating afternoon easier; useful behavior, tests and clear documentation make the tool worth keeping.

**[Try every tool and explore its options →](https://deployanyway.github.io/)** No signup or API keys. Demo inputs stay in your browser.

## One toolbox. Plenty of questionable confidence.

| Tool                                                                 | What you can use                                                                                           | Personality included                        |
| -------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| [bro-say](https://github.com/DeployAnyway/bro-say)                   | Measured build/test summaries, unknown/failure states, original characters, say/think and Unicode wrapping | Emotional support for production.           |
| [error-translator](https://github.com/DeployAnyway/error-translator) | Error/cause diagnostics, cycle/depth bounds, 46 curated codes, likely causes and concrete next checks      | The stack trace has chosen violence.        |
| [excuse-js](https://github.com/DeployAnyway/excuse-js)               | Factual incident drafts, owners/next updates/missing facts, public-safe defaults and 132 seeded jokes      | Finally, a dependency that takes the blame. |
| [doggo-log](https://github.com/DeployAnyway/doggo-log)               | Isolated async request scopes, context/literal redaction, child loggers and optional husky commentary      | Good logs. Very good logs.                  |
| [ship-it-meter](https://github.com/DeployAnyway/ship-it-meter)       | Node/Jest/Istanbul report policies, failed/stale/wrong-commit blockers and prioritized repair plans        | Confidence is not a build artifact.         |

All five are [published on npm at 1.0.0](https://www.npmjs.com/org/deployanyway), MIT licensed, with CLIs, ESM/CommonJS APIs and TypeScript declarations. bro-say has two direct runtime dependencies for terminal text; the other four have none. CI covers Linux Node 22/24 and Windows/macOS Node 24, coverage gates and installed-package checks.

With Node 22.13+ or Node 24:

```sh
npx @deployanyway/bro-say@1.0.0 --preset husky --seed dallas --mood dallas
npx @deployanyway/error-translator@1.0.0 EACCES --mode rubber-duck
npx @deployanyway/excuse-js@1.0.0 testing --report --seed launch
npx @deployanyway/doggo-log@1.0.0 info "Request complete" --bark --bark-mode rotate --seed benji --json
npx @deployanyway/ship-it-meter@1.0.0 --scenario ready --plan
```

npx may ask to install on first use. Each repository includes full API examples, a changelog, migration notes and contribution guidance. Expanded catalogs can change seeded selections between versions; pin versions for reproducible output.

## Make the next release useful

[Bugs and ideas for all five tools](https://deployanyway.github.io/#feedback-title) · [Original character ideas](https://github.com/DeployAnyway/bro-say/issues/new?template=character.md) · [Meet the toolbox](https://github.com/DeployAnyway/.github/blob/main/MEET-DEPLOYANYWAY.md) · [Copyable launch post](https://github.com/DeployAnyway/.github/blob/main/LAUNCH-POST.md)

These are focused libraries: terminal fonts can disagree on emoji width; error explanations are curated; logs do not redact secrets; release scores use supplied evidence and do not run your CI. Humor is optional where it would obscure facts. The tools should earn a place in your workflow.

## Worth keeping in your codebase

Useful facts first; personality around them. V1 adds measured build summaries, error cause diagnostics, accountable incident drafts, request scopes/redaction and report-backed release policies. Every package ships runnable examples, stable structured APIs, CLI exit contracts, ESM/CommonJS declarations and migration notes. No telemetry or external API service is needed.

The demo previews actual pure package behavior, with copyable Node examples where processes, files or AsyncLocalStorage are involved. Sample receipts are visibly labeled demonstration data. A gate consumes evidence from your trusted pipeline; it cannot verify an arbitrary submitted artifact or prove a deployment safe. Redaction covers configured context keys and literal secrets, not unknown secrets in arbitrary objects.

We have tested release contracts and integrations; we have not proved community adoption, retention, or superiority to mature tools. Use it in a real workflow and [tell us what helped or got in the way](https://github.com/DeployAnyway/.github/issues).
