# Meet DeployAnyway. We shipped it anyway.

Tools for developers who probably should know better.

Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

We built five small, useful JavaScript and Node.js tools, added original workplace-safe humor, and somehow remembered the tests:

- **error-translator:** explains common errors and debugging steps. Rubber-duck mode adds commentary from the only teammate who has never broken main.
- **excuse-js:** generates seeded developer excuses, now in batches for the meeting you are about to have. Finally, a dependency that takes the blame.
- **doggo-log:** console logging with levels, JSON, nested scopes, and optional dog commentary. Good logs. Very good logs.
- **ship-it-meter:** explainable deployment readiness scores and an actionable preflight checklist. Confidence is not a build artifact.
- **bro-say:** six moods for terminal announcements, now with ASCII boxes. Your build output has a hype person.

Try them in your browser: **https://deployanyway.github.io/**

No signup. No API keys. Inputs stay in your browser. Prefer the terminal? With Node 22 or later:

```sh
npx @deployanyway/error-translator ECONNREFUSED --mode rubber-duck
npx @deployanyway/excuse-js deployment --count 3 --seed demo
npx @deployanyway/doggo-log success "Migration complete" --bark
npx @deployanyway/ship-it-meter --tests 125 --coverage 82 --build pass --day friday --checklist
npx @deployanyway/bro-say "Tests passed!" --mood hype --box
```

All five have a CLI and an ES module API, zero production dependencies, and an MIT license. The readiness score uses supplied evidence, not your actual CI; it is a heuristic, not permission to skip release checks.

Code, docs, and contributions: https://github.com/DeployAnyway

The priorities are questionable. The tools have tests.
