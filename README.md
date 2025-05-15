# nuxt-module-npmrc-comment-error-repro

```bash
$ npm i
$ npx nuxi module add pinia
[2:16:01]  ERROR  [GET] "https://registry.npmjs.org # test comment/@pinia/nuxt": <no response> Failed to parse URL from https://registry.npmjs.org # test comment/@pinia/nuxt

    at async $fetchRaw2 (node_modules/nuxi/dist/shared/nuxi.BzZJv2UC.mjs:371:14)
    at async $fetch2 (node_modules/nuxi/dist/shared/nuxi.BzZJv2UC.mjs:417:15)
    at async resolveModule (node_modules/nuxi/dist/chunks/add2.mjs:315:22)
    at async Promise.all (index 0)
    at async Object.setup (node_modules/nuxi/dist/chunks/add2.mjs:150:34)
    at async runCommand$1 (node_modules/nuxi/dist/shared/nuxi.BlFGnQYG.mjs:1739:5)
    at async runCommand$1 (node_modules/nuxi/dist/shared/nuxi.BlFGnQYG.mjs:1758:11)
    at async runCommand$1 (node_modules/nuxi/dist/shared/nuxi.BlFGnQYG.mjs:1758:11)
    at async runMain$1 (node_modules/nuxi/dist/shared/nuxi.BlFGnQYG.mjs:1896:7)

  [cause]: Failed to parse URL from https://registry.npmjs.org # test comment/@pinia/nuxt

      at node:internal/deps/undici/undici:13510:13
      at async $fetchRaw2 (node_modules/nuxi/dist/shared/nuxi.BzZJv2UC.mjs:359:26)

    [cause]: Invalid URL

        at new URL (node:internal/url:818:25)
        at new Request (node:internal/deps/undici/undici:9586:25)
        at fetch (node:internal/deps/undici/undici:10315:25)
        at fetch (node:internal/deps/undici/undici:13508:10)
        at fetch (node:internal/bootstrap/web/exposed-window-or-worker:75:12)
        at node_modules/nuxi/dist/shared/nuxi.BzZJv2UC.mjs:451:58
        at $fetchRaw2 (node_modules/nuxi/dist/shared/nuxi.BzZJv2UC.mjs:359:32)
        at onError (node_modules/nuxi/dist/shared/nuxi.BzZJv2UC.mjs:280:16)
        at $fetchRaw2 (node_modules/nuxi/dist/shared/nuxi.BzZJv2UC.mjs:371:20)
        at async $fetch2 (node_modules/nuxi/dist/shared/nuxi.BzZJv2UC.mjs:417:15) 



[2:16:01]  ERROR  [GET] "https://registry.npmjs.org # test comment/@pinia/nuxt": <no response> Failed to parse URL from https://registry.npmjs.org # test comment/@pinia/nuxt
```