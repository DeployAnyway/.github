# DeployAnyway 1.0: bring joy, bring receipts

Tools for developers who probably should know better. Software nobody requested, built with questionable priorities, and shipped with absolute confidence!

Dallas and Benji supply the energy. The code supplies something worth keeping: build summaries that preserve failure, cause-chain diagnostics, honest incident drafts, isolated request logging with redaction, and release policies that ask for actual reports. All five tools share the spotlight.

[Try every tool and its options](https://deployanyway.github.io/). MIT, Node22.13+/24, CLI + ESM/CommonJS APIs + TypeScript declarations.

Copy into sh/bash:

```sh
printf '%s' '{"exitCode":1,"tests":{"passed":42,"failed":1}}' | npx @deployanyway/bro-say@1.0.0 --summary --plain
printf '%s' '{"message":"Startup failed","cause":{"code":"ENOENT","message":"Missing config.json"}}' | npx @deployanyway/error-translator@1.0.0 --diagnose
printf '%s' '{"service":"API","status":"investigating","impact":"Some requests fail","action":"Checking the deployment","owner":"On-call","nextUpdate":"2026-10-09T09:15:00Z"}' | npx @deployanyway/excuse-js@1.0.0 --incident --require-complete
npx @deployanyway/doggo-log@1.0.0 info 'Request complete' --context '{"requestId":"42","authorization":"private"}' --json
npx @deployanyway/ship-it-meter@1.0.0 --report-file receipts.json --policy '{"minCoverage":90}' --json
```

The last command requires real receipts from your pipeline; [the collector example](https://github.com/DeployAnyway/ship-it-meter/blob/main/examples/collect-receipts.mjs) records fresh Node/c8/build results. bro-say renders facts; your script must preserve the underlying build exit. Incident updates are drafts; no message is sent.

For async requests:

```js
import { createRequestLogger } from "@deployanyway/doggo-log/context";
const log = createRequestLogger({ json: true });
await log.run({ requestId: "benji-42", authorization: "private" }, async () => {
  await Promise.resolve();
  log.child("database").info("Query complete");
});
log.dispose(); // after all service work has finished
```

[Bugs, original character ideas and feature requests](https://deployanyway.github.io/#feedback-title) are welcome. Tell us what made your real work easier.
