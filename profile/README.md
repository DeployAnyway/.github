# DeployAnyway

![DeployAnyway husky developer badge](https://deployanyway.github.io/assets/deployanyway-husky.png)

**Tools for developers who probably should know better.**

Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

small open-source tools for expressing yourself, debugging, regrouping, logging and deciding what to ship. Choose the one(s) that helps your day.

Dallas and Benji, Todd's fun-loving, high-energy huskies, inspire the mindset: stay curious, bring some joy, and make room for play while doing the work. Developers deserve that too. A good joke can make a frustrating afternoon easier; useful behavior, tests and clear documentation make the tool worth keeping.

**[Try every tool and explore its options →](https://deployanyway.github.io/)** No signup or API keys. Demo inputs stay in your browser.

## One toolbox. Plenty of questionable confidence.

| Tool                                                                 | What you can use                                                                                              | Personality included                        |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| [bro-say](https://github.com/DeployAnyway/bro-say)                   | 13 characters, 20 moods, six themes, 48 message presets, say/think, Unicode wrapping and stdin                | Emotional support for production.           |
| [error-translator](https://github.com/DeployAnyway/error-translator) | 46 curated errors, likely causes, next checks, batches and structured catalogs                                | The stack trace has chosen violence.        |
| [excuse-js](https://github.com/DeployAnyway/excuse-js)               | 132 original excuses across eleven categories, seeded batches, full catalogs and honest next steps            | Finally, a dependency that takes the blame. |
| [doggo-log](https://github.com/DeployAnyway/doggo-log)               | Six levels, JSON, request context, child loggers and 48 optional rotating commentary lines                    | Good logs. Very good logs.                  |
| [ship-it-meter](https://github.com/DeployAnyway/ship-it-meter)       | Twelve evidence scenarios, explainable scores, release gates and prioritized plans with verification criteria | Confidence is not a build artifact.         |

All five are [published on npm at 0.4.0](https://www.npmjs.com/org/deployanyway), MIT licensed, with CLIs, ESM/CommonJS APIs and TypeScript declarations. bro-say has two direct runtime dependencies for terminal text; the other four have none. CI covers Linux Node 22/24 and Windows/macOS Node 24, coverage gates and installed-package checks.

With Node 22.13+ or Node 24:

```sh
npx @deployanyway/bro-say@0.4.0 --preset husky --seed dallas --mood dallas
npx @deployanyway/error-translator@0.4.0 EACCES --mode rubber-duck
npx @deployanyway/excuse-js@0.4.0 testing --report --seed launch
npx @deployanyway/doggo-log@0.4.0 info "Request complete" --bark --bark-mode rotate --seed benji --json
npx @deployanyway/ship-it-meter@0.4.0 --scenario ready --plan
```

npx may ask to install on first use. Each repository includes full API examples, a changelog, migration notes and contribution guidance. Expanded catalogs can change seeded selections between versions; pin versions for reproducible output.

## Make the next release useful

[Bugs and ideas for all five tools](https://deployanyway.github.io/#feedback-title) · [Original character ideas](https://github.com/DeployAnyway/bro-say/issues/new?template=character.md) · [Meet the toolbox](https://github.com/DeployAnyway/.github/blob/main/MEET-DEPLOYANYWAY.md) · [Copyable launch post](https://github.com/DeployAnyway/.github/blob/main/LAUNCH-POST.md)

These are focused libraries: terminal fonts can disagree on emoji width; error explanations are curated; logs do not redact secrets; release scores use supplied evidence and do not run your CI. Humor is optional where it would obscure facts. The tools should earn a place in your workflow.
