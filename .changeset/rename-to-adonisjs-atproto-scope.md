---
'@adonisjs-atproto/tap': major
---

Rename package to `@adonisjs-atproto/tap`

The package has moved from the personal `@thisismissem` scope to the shared
`@adonisjs-atproto` org scope, dropping the now-redundant `adonisjs-atproto-`
prefix from the basename. The old `@thisismissem/adonisjs-atproto-tap` package is
deprecated and will receive no further updates.

To migrate, reinstall under the new name and update your imports:

```sh
node ace add @adonisjs-atproto/tap
```

```diff
-import { defineConfig } from '@thisismissem/adonisjs-atproto-tap'
-import tap from '@thisismissem/adonisjs-atproto-tap/services/tap'
-import indexer from '@thisismissem/adonisjs-atproto-tap/services/indexer'
+import { defineConfig } from '@adonisjs-atproto/tap'
+import tap from '@adonisjs-atproto/tap/services/tap'
+import indexer from '@adonisjs-atproto/tap/services/indexer'
```

Also update the provider entry in `adonisrc.ts` from
`@thisismissem/adonisjs-atproto-tap/provider` to `@adonisjs-atproto/tap/provider`.
There are no API changes — only the package name has changed.
