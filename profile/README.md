# DeployAnyway

**Tools for developers who probably should know better.**

Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

We make small JavaScript and Node.js developer tools that do something useful and then make a joke about it. Debug an error. Log a message. Check your deployment evidence. Prepare an explanation for the meeting you are about to have.

The priorities are questionable. The tools have tests.

## Meet the dependencies you can explain later

| Package                                                              | What it does                                             | Why it exists                                |
| -------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------- |
| [error-translator](https://github.com/DeployAnyway/error-translator) | Plain-English error explanations and debugging tips      | The stack trace has chosen violence.         |
| [excuse-js](https://github.com/DeployAnyway/excuse-js)               | Developer excuse generator with repeatable seeded output | Finally, a dependency that takes the blame.  |
| [doggo-log](https://github.com/DeployAnyway/doggo-log)               | Console logger with levels, JSON, and dog emojis         | Good logs. Very good logs.                   |
| [ship-it-meter](https://github.com/DeployAnyway/ship-it-meter)       | Explainable deployment readiness scoring                 | Turns questionable confidence into a number. |
| [bro-say](https://github.com/DeployAnyway/bro-say)                   | Terminal message formatter with six moods                | Your build output has a hype person now.     |

All five are available on [npm under @deployanyway](https://www.npmjs.com/org/deployanyway). They use ES modules, require Node 22 or later, have zero production dependencies, and are MIT licensed.

## Try one before the meeting starts

Run these in a terminal with Node 22 or later. `npx` may ask to install the package the first time.

### Translate the error that ruined your morning

```sh
npx @deployanyway/error-translator ECONNREFUSED
```

Get an explanation, likely causes, and practical next steps for a refused connection.

### Give the deployment a spokesperson

```sh
npx @deployanyway/excuse-js deployment --seed demo
```

Get the same original, workplace-safe excuse each time with the same seed in this version. Includes categories for bugs, builds, databases, deadlines, and more.

### Put a good dog in your logs

```sh
npx @deployanyway/doggo-log info "Server started"
```

Print an INFO log with a dog emoji. Add `--json` for structured output or `--no-emoji` when the incident report gets serious.

### Measure the confidence before someone says ship it

```sh
npx @deployanyway/ship-it-meter --tests 125 --coverage 82 --build pass
```

Get a score, verdict, and reasons based on the evidence you supply. This is an illustrative heuristic, not a deployment guarantee; it does not inspect your CI.

### Give your terminal a hype person

```sh
npx @deployanyway/bro-say "Tests passed!" --mood hype
```

```text
BRO! THE TERMINAL IS APPLAUDING!

Tests passed!
```

## Use them in JavaScript too

Every tool exports a small API as well as a CLI. For example:

```sh
npm install @deployanyway/doggo-log
```

```js
import { createDogLogger } from "@deployanyway/doggo-log";

const log = createDogLogger({ json: true, prefix: "api" });
log.info("Server started on port %d", 3000);
```

```json
{ "level": "info", "message": "Server started on port 3000", "prefix": "api" }
```

Use an ES module project (`"type": "module"` in `package.json`) or save the example as `.mjs`. Each repository has API documentation, CLI options, examples, and a contribution guide.

## Contribute something we probably should have thought of

Bug reports, clearer explanations, useful features, documentation fixes, and original workplace-safe jokes are welcome. Open an issue in the relevant repository and read its `CONTRIBUTING.md` before sending a pull request.

Small tools. Clear behavior. Funny output. Absolute confidence, supported by at least some evidence.
