# Meet DeployAnyway

Tools for developers who probably should know better.

Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

DeployAnyway makes small JavaScript and Node.js tools for the parts of development that deserve both a useful answer and a mildly irresponsible joke. All five packages are available on npm, with a CLI, an ES module API, zero production dependencies, and an MIT license.

Bring Node 22 or later. We brought tests.

## Five tools. Several questionable decisions.

**[error-translator](https://www.npmjs.com/package/@deployanyway/error-translator)** explains common Node.js errors in plain English, with likely causes and debugging steps. Because the stack trace has chosen violence.

```sh
npx @deployanyway/error-translator ECONNREFUSED
```

**[excuse-js](https://www.npmjs.com/package/@deployanyway/excuse-js)** generates developer excuses for bugs, builds, deployments, and more. Use a seed for repeatable output. Finally, a dependency that takes the blame.

```sh
npx @deployanyway/excuse-js deployment --seed demo
```

**[doggo-log](https://www.npmjs.com/package/@deployanyway/doggo-log)** logs messages with levels, optional JSON, and dog emojis. Good logs. Very good logs.

```sh
npx @deployanyway/doggo-log info "Server started"
```

**[ship-it-meter](https://www.npmjs.com/package/@deployanyway/ship-it-meter)** turns supplied test, coverage, and build evidence into an explainable readiness score. It is a heuristic, not a deployment guarantee; it does not inspect your CI.

```sh
npx @deployanyway/ship-it-meter --tests 125 --coverage 82 --build pass
```

**[bro-say](https://www.npmjs.com/package/@deployanyway/bro-say)** formats terminal messages in six developer moods. Your build output has a hype person now.

```sh
npx @deployanyway/bro-say "Tests passed!" --mood hype
```

`npx` may ask to install a package on the first run. Prefer a library? Install any package with `npm install @deployanyway/<package>` and follow its repository's API examples.

Browse the code and documentation at [github.com/DeployAnyway](https://github.com/DeployAnyway). Try a tool, report a bug, or contribute an original workplace-safe joke. The priorities are questionable. The tools have tests.
