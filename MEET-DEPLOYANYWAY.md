# Meet DeployAnyway 0.3.0

**Tools for developers who probably should know better.**

Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

Five useful Node.js tools. Original developer humor. CLIs, typed ESM/CommonJS APIs, cross-platform CI and installed-package checks. Bring Node 22.13+ or Node 24. We brought tests.

**[Try the flagship playground](https://deployanyway.github.io/candidate/)**. No signup or API keys. Inputs stay in your browser. [Explore all five tools](https://deployanyway.github.io/).

## bro-say: emotional support for production

13 original terminal characters, 12 personas and six themes. Say or think, wrap Unicode text, pipe a build log, or request seeded random choices and structured JSON. The husky supplies an LGTM sign; your message stays yours.

```sh
npx @deployanyway/bro-say@0.3.0 "Deploy anyway." --character husky --mood corporate
echo "Build failed" | npx @deployanyway/bro-say@0.3.0 --think --mood panic
npx @deployanyway/bro-say@0.3.0 "こんにちは 👋 café" --width 24 --theme neon
```

Install globally for bro-say and bro-think, or use the typed brosay, brothink and renderBro APIs. Default artwork/wrapping changed in 0.3.0; [migration options](https://github.com/DeployAnyway/bro-say/blob/main/MIGRATION.md) include --plain and --box. Fonts/emulators may disagree on emoji width.

## Four more useful questionable decisions

**[error-translator](https://www.npmjs.com/package/@deployanyway/error-translator)** explains common errors, likely causes and debugging steps. Now with ordered batches, stdin and a supported-error catalog. The stack trace has chosen violence.

```sh
echo '["ENOENT","ECONNREFUSED"]' | npx @deployanyway/error-translator@0.3.0 --batch --json
```

**[excuse-js](https://www.npmjs.com/package/@deployanyway/excuse-js)** pairs a seeded excuse with a useful next action. Joke, then fix the thing.

```sh
npx @deployanyway/excuse-js@0.3.0 testing --report --seed launch --json
```

**[doggo-log](https://www.npmjs.com/package/@deployanyway/doggo-log)** supplies levels, JSON and copied scalar context. Child loggers carry request context without mutating their parent. Good logs. Very good logs.

```sh
npx @deployanyway/doggo-log@0.3.0 info "Request complete" --context '{"requestId":"launch-42"}' --json
```

**[ship-it-meter](https://www.npmjs.com/package/@deployanyway/ship-it-meter)** turns supplied evidence into a score, actions and a gate with blockers. Blocked gates exit 1; malformed input exits 2. Confidence is not a build artifact.

```sh
npx @deployanyway/ship-it-meter@0.3.0 --gate --tests 125 --coverage 92 --build pass --json
```

npx may ask to install on first use. All packages are MIT licensed. bro-say has two direct runtime dependencies for display width/wrapping; the others have none. The error catalog is curated, logging is not secret redaction, and release scores do not inspect your CI or authorize deployment.

## Tell us what happened

[Report a flagship bug](https://github.com/DeployAnyway/bro-say/issues/new?template=bug_report.md) · [Pitch an original character](https://github.com/DeployAnyway/bro-say/issues/new?template=character.md) · [Suggest a feature](https://github.com/DeployAnyway/bro-say/issues/new?template=feature_request.md)

For another tool, open its repository's issue chooser. Include your version, OS, terminal/font and a small reproduction when relevant.

[Code and documentation](https://github.com/DeployAnyway) · [Copyable launch post](LAUNCH-POST.md)
