# Meet DeployAnyway 0.4.0

**Tools for developers who probably should know better.**

Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

Dallas and Benji, Todd's fun-loving, high-energy huskies, inspire the mindset: stay curious, bring some joy, and make room for play while doing the work. Developers deserve that too. A good joke can make a frustrating afternoon easier; useful behavior, tests and clear documentation make the tool worth keeping.

**[Explore all five live demos](https://deployanyway.github.io/)**. Every tool has discoverable choices, output previews, copyable examples, documentation and feedback links. Inputs stay in your browser.

| Tool                                                                 | What you can use                                                                                              | Personality included                        |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- | ------------------------------------------- |
| [bro-say](https://github.com/DeployAnyway/bro-say)                   | 13 characters, 20 moods, six themes, 48 message presets, say/think, Unicode wrapping and stdin                | Emotional support for production.           |
| [error-translator](https://github.com/DeployAnyway/error-translator) | 46 curated errors, likely causes, next checks, batches and structured catalogs                                | The stack trace has chosen violence.        |
| [excuse-js](https://github.com/DeployAnyway/excuse-js)               | 132 original excuses across eleven categories, seeded batches, full catalogs and honest next steps            | Finally, a dependency that takes the blame. |
| [doggo-log](https://github.com/DeployAnyway/doggo-log)               | Six levels, JSON, request context, child loggers and 48 optional rotating commentary lines                    | Good logs. Very good logs.                  |
| [ship-it-meter](https://github.com/DeployAnyway/ship-it-meter)       | Twelve evidence scenarios, explainable scores, release gates and prioritized plans with verification criteria | Confidence is not a build artifact.         |

## Try them in your terminal

Bring Node 22.13+ or Node 24. All five packages are published at 0.4.0:

```sh
npx @deployanyway/bro-say@0.4.0 --preset husky --seed dallas --mood dallas
npx @deployanyway/error-translator@0.4.0 EACCES --mode rubber-duck
npx @deployanyway/excuse-js@0.4.0 testing --report --seed launch
npx @deployanyway/doggo-log@0.4.0 info "Request complete" --bark --bark-mode rotate --seed benji --json
npx @deployanyway/ship-it-meter@0.4.0 --scenario ready --plan
```

## Go beyond the first joke

bro-say can render your own text or select original presets. Use --list-characters, --list-moods, --list-themes and --list-presets to explore. Say and think accept stdin; renderBro returns structured data. --plain and --box provide legacy layouts; see its migration guide.

error-translator supports --list and --catalog, plain or rubber-duck explanations, and ordered JSON batches. errorCatalog() exposes the same definitions as the CLI. Unknown errors stay explicitly unknown; suggested checks are guidance, not automatic fixes.

excuse-js provides --list and category --catalog. Seeded batches exhaust twelve phrases before repeating; excuseReport adds a practical next step. listExcuses returns a fresh array for your own interfaces.

doggo-log defaults to classic behavior. Opt into bark commentary and barkMode: 'rotate' for eight distinct lines per level before repetition. Child loggers carry copied request context; filtering, JSON, timestamps and custom writers remain available. Failed writes do not consume a bark. Never use logs as secret redaction.

ship-it-meter offers --list-scenarios, --scenario and --plan, alongside --gate, --checklist and JSON stdin. Plans expose prioritized tasks and observable verification criteria, including rollback and monitoring. A blocked plan/gate exits 1; invalid input exits 2. Scores are heuristics based on supplied evidence, not deployment guarantees.

All packages include typed ESM/CommonJS APIs, MIT licenses, migration notes, tests, coverage gates and cross-platform CI. bro-say has two direct runtime dependencies; the others have none. Pin package versions when seeded output must remain identical across catalog changes.

## Tell us what happened

[Feedback for each tool](https://deployanyway.github.io/#feedback-title) · [Original character ideas](https://github.com/DeployAnyway/bro-say/issues/new?template=character.md)

Include your package version, OS, terminal/font where relevant, expected behavior and a small reproduction. Original workplace-safe contributions are welcome; read the repository's CONTRIBUTING.md first.

[Code and documentation](https://github.com/DeployAnyway) · [Copyable launch post](LAUNCH-POST.md)
