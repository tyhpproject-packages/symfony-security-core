<!-- tyhp-readme:start -->
# tyhpdef/symfony-security-core

Tyhp type definitions for `symfony/security-core` `7.4.18`.

```bash
composer require --dev tyhpdef/symfony-security-core:7.4.18
```

This is a metapackage. Composer also installs `tyhpdef/symfony-security-core-impl` (type files).
Require **this** name, not `tyhpdef/symfony-security-core-impl`.

See https://tyhplang.com.

## Maintain `symfony/security-core`? Ship the types yourself

If you are a Packagist maintainer of `symfony/security-core`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/symfony-security-core-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `symfony/security-core` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/symfony-security-core": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `symfony/security-core` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `symfony/security-core` with a real constraint,
   `"replace": { "tyhpdef/symfony-security-core": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `symfony/security-core` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/symfony-security-core` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
