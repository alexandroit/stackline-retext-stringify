# Upstream and maintenance review

Independent maintenance of `retext-stringify@3.1.0` as `@stackline/retext-stringify`.

- Source history: https://github.com/retextjs/retext/tree/95fd8db44198fe306380d5a5f1f2df17bb290a4f
- Original npm integrity: `sha512-767TLOaoXFXyOnjx/EggXlb37ZD2u4P1n0GJqVdpipqACsQP+20W+BNpMYrlJkq7hxffnFk+jc6mAK9qrbuB8w==`.
- Issues checked: 2026-09-29T00:22:06.618077+00:00.
- Original authors, notices and license are retained. Published runtime and declaration file hashes are recorded in `.stackline/upstream.json`; reviewed differences are explicitly listed there.
- Original functional suites run against both source and the extracted final tarball. Type checks and the complete development/runtime audit must pass.

This maintenance branch selects the npm package from the upstream monorepo into the repository root and retains the upstream Git history. Shared tests are narrowed to this package and wired to its local implementation. Other monorepo products are not published by this repository.

The npm metadata omits gitHead. The retained source commit was found in upstream history by matching every published runtime JavaScript file byte-for-byte. Generated declaration files were recovered from the integrity-verified npm artifact.

## Issue triage

The bounded open-issue query returned no issue entries. This is not evidence that the upstream is abandoned or bug-free. No upstream runtime bug fix is claimed.

The evidence query fetched the latest 100 open and 30 closed issue/PR entries and removed PRs. This is a bounded review, not a claim of exhaustive issue history or resolution of every issue.

## Release verification

GitHub Actions publishes the reviewed passing-CI tarball. Release completion requires exact source identity, zero open CodeQL alerts, npm provenance and tarball identity, normal and aliased installs, and matching immutable GitHub release assets. Existing versions are never replaced.
