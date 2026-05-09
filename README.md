# @dngnguyen/paperclip-adapter-utils

Mirror of `@paperclipai/adapter-utils` (workspace `0.3.1`) from the [paperclipai/paperclip](https://github.com/paperclipai/paperclip) monorepo, republished under the `@dngnguyen` scope to GitHub Packages.

## Why this exists

The npm registry namespace `@paperclipai/adapter-utils` is owned by an unrelated party and exposes a different API. The Paperclip workspace package is private. External plugins (e.g. `@dngnguyen/paperclip-adapter-qwen-local`) need a published copy of the workspace surface — that's what this package is.

## Sync

Source-of-truth is `paperclip/packages/adapter-utils/src/`. Sync via the same pattern as the qwen-local plugin (manual sync script + drift CI). On every paperclip release that bumps the workspace version, bump this package's version to match (`0.3.x → 0.3.x`), tag, and let the publish workflow ship.

## Install

```bash
# .npmrc
@dngnguyen:registry=https://npm.pkg.github.com
//npm.pkg.github.com/:_authToken=<your-PAT-with-read:packages>

npm install @dngnguyen/paperclip-adapter-utils
```

## License

MIT (matches upstream).
