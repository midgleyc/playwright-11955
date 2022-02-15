Running

```bash
npm run types
```

shows the erroring output:

```
> types
> tsc -p jsconfig.json
                                                                                                                                                                                                                   
a.mjs:3:36 - error TS2694: Namespace '"/home/chris/temp/playwright-11955/node_modules/playwright/index"' has no exported member 'Page'.
                                                                                                                                                                                                                   
3 /** @typedef {import("playwright").Page} Page */
                                     ~~~~
                                                                                                                                                                                                                   
b.mts:1:15 - error TS2614: Module '"playwright"' has no exported member 'Page'. Did you mean to use 'import Page from "playwright"' instead?
                                                                                                                                                                                                                   
1 import type { Page } from "playwright";
                ~~~~
                                                                                                                                                                                                                   
                                                                                                                                                                                                                   
Found 2 errors in 2 files.

Errors  Files
     1  a.mjs:3
     1  b.mts:1
```
