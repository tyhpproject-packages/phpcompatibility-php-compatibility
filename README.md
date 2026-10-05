<!-- tyhp-readme:start -->
# tyhpdef/phpcompatibility-php-compatibility

Tyhp type definitions for `phpcompatibility/php-compatibility` `9.3.5`.

```bash
composer require --dev tyhpdef/phpcompatibility-php-compatibility:9.3.5
```

This is a metapackage. Composer also installs `tyhpdef/phpcompatibility-php-compatibility-impl` (type files).
Require **this** name, not `tyhpdef/phpcompatibility-php-compatibility-impl`.

See https://tyhplang.com.

## Maintain `phpcompatibility/php-compatibility`? Ship the types yourself

If you are a Packagist maintainer of `phpcompatibility/php-compatibility`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/phpcompatibility-php-compatibility-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `phpcompatibility/php-compatibility` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/phpcompatibility-php-compatibility": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `phpcompatibility/php-compatibility` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `phpcompatibility/php-compatibility` with a real constraint,
   `"replace": { "tyhpdef/phpcompatibility-php-compatibility": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `phpcompatibility/php-compatibility` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/phpcompatibility-php-compatibility` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
