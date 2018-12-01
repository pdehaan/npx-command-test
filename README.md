# npx-command-test

Testing multiple commands in npx package.

This dummy module has 2 separate commands specified in the package.json `bin` field:

```js
  "bin": {
    "commandA": "cmdA.js",
    "commandB": "cmdB.js"
  },
```

You can invoke them by specifying the `-p` (aka `--package`) and `-c` (aka "command") flags in [**npx**](https://github.com/zkat/npx).

```sh
$ npx -p pdehaan/npx-command-test -c commandA

command A from /Users/pdehaan/.npm/_npx/65556/lib/node_modules/npx-command-test/cmdA.js

$ npx -p pdehaan/npx-command-test -c commandB

command B from /Users/pdehaan/.npm/_npx/65675/lib/node_modules/npx-command-test/cmdB.js
```
