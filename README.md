<!-- tyhp-readme:start -->
# tyhpdef/illuminate-support

Tyhp type definitions for `illuminate/support` `13.33.0`.

```bash
composer require --dev tyhpdef/illuminate-support:13.33.0
```

This is a metapackage. Composer also installs `tyhpdef/illuminate-support-impl` (type files).
Require **this** name, not `tyhpdef/illuminate-support-impl`.

See https://tyhplang.com.

## Maintain `illuminate/support`? Ship the types yourself

If you are a Packagist maintainer of `illuminate/support`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/illuminate-support-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `illuminate/support` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/illuminate-support": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `illuminate/support` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `illuminate/support` with a real constraint,
   `"replace": { "tyhpdef/illuminate-support": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `illuminate/support` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/illuminate-support` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
