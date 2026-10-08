# DeployAnyway

**Tools for developers who probably should know better.**

Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

We make useful JavaScript and Node.js tools with original developer humor. The priorities are questionable. The tools have tests.

## Meet the flagship: bro-say 0.3.0

13 original terminal friends, including a husky developer with an LGTM sign. 12 personas, six themes, speech and thoughts, Unicode-aware wrapping, stdin and seeded choices. Emotional support for production, without pretending to repair production.

**[Try the flagship and all five tools in your browser →](https://deployanyway.github.io/candidate/)** No signup or API keys. Inputs stay in your browser.

With Node 22.13+ or Node 24:

```sh
npx @deployanyway/bro-say@0.3.0 "Deploy anyway." --character husky --mood corporate
echo "Build failed" | npx @deployanyway/bro-say@0.3.0 --think --mood panic
```

## Five tools. One questionable organization.

| Package                                                              | Useful behavior in 0.3.0                                                 | Questionable confidence                     |
| -------------------------------------------------------------------- | ------------------------------------------------------------------------ | ------------------------------------------- |
| [bro-say](https://github.com/DeployAnyway/bro-say)                   | Original characters, say/think, wrapping, stdin and structured rendering | Your terminal deserves emotional support.   |
| [error-translator](https://github.com/DeployAnyway/error-translator) | Error explanations, debugging steps, ordered batches and stdin           | The stack trace has chosen violence.        |
| [excuse-js](https://github.com/DeployAnyway/excuse-js)               | Seeded excuses paired with an honest next action                         | Finally, a dependency that takes the blame. |
| [doggo-log](https://github.com/DeployAnyway/doggo-log)               | Levels, JSON and copied request context with child loggers               | Good logs. Very good logs.                  |
| [ship-it-meter](https://github.com/DeployAnyway/ship-it-meter)       | Evidence-based scores, preflight actions and gates with blockers         | Confidence is not a build artifact.         |

All five are [on npm at 0.3.0](https://www.npmjs.com/org/deployanyway), MIT licensed, with CLIs, ESM/CommonJS APIs and TypeScript declarations. bro-say uses two direct runtime dependencies for terminal text; the other four have none. CI covers Linux Node 22/24 and Windows/macOS Node 24, with coverage and installed-package checks.

[Meet DeployAnyway and try the examples](https://github.com/DeployAnyway/.github/blob/main/MEET-DEPLOYANYWAY.md) · [Launch post](https://github.com/DeployAnyway/.github/blob/main/LAUNCH-POST.md)

## Help us make 0.3.1 useful

[Report a bro-say bug](https://github.com/DeployAnyway/bro-say/issues/new?template=bug_report.md) · [Pitch an original character](https://github.com/DeployAnyway/bro-say/issues/new?template=character.md) · [Suggest a feature](https://github.com/DeployAnyway/bro-say/issues/new?template=feature_request.md)

For other tools, use their repository's issue templates. Terminal/font feedback and original workplace-safe contributions are welcome. Read CONTRIBUTING.md before sending a PR.

Fonts can disagree on emoji width. Error explanations are curated; jokes are not incident evidence; readiness scores use supplied data and are not deployment authorization. bro-say's default output changed in 0.3.0—see its migration guide for --plain and --box compatibility options.
