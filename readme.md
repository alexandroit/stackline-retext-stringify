# @stackline/retext-stringify

> retext plugin to serialize prose.

[![npm version](https://img.shields.io/npm/v/@stackline/retext-stringify.svg?style=flat-square)](https://www.npmjs.com/package/@stackline/retext-stringify)
[![license](https://img.shields.io/npm/l/@stackline/retext-stringify.svg?style=flat-square)](https://github.com/alexandroit/stackline-retext-stringify)
[![GitHub repository](https://img.shields.io/badge/GitHub-repository-181717?style=flat-square&logo=github)](https://github.com/alexandroit/stackline-retext-stringify)
[![Docs](https://img.shields.io/badge/docs-alexandro.net-0f766e?style=flat-square)](https://alexandro.net/docs/vanilla/retext-stringify/)
[![Reddit community](https://img.shields.io/badge/community-r%2FStackline-ff4500?style=flat-square&logo=reddit&logoColor=white)](https://www.reddit.com/r/Stackline/)

**[Documentation](https://alexandro.net/docs/vanilla/retext-stringify/)** | **[npm](https://www.npmjs.com/package/@stackline/retext-stringify)** | **[Issues](https://github.com/alexandroit/stackline-retext-stringify/issues)** | **[Repository](https://github.com/alexandroit/stackline-retext-stringify)**

**Current package version:** `1.0.2`

---

## Why this package?

`@stackline/retext-stringify` is the Stackline-maintained distribution of `retext-stringify@3.1.0`. It is an independent continuation of [retext-stringify](https://github.com/retextjs/retext); original authors and licenses remain credited below.

## Compatibility

| Item | Value |
| :--- | :--- |
| Package | `@stackline/retext-stringify@1.0.2` |
| API target | `retext-stringify@3.1.0` |
| Supported Node.js | `See supported framework requirements` |
| License | `MIT` |
| Module type | `module` |
| Main entry | `index.js` |
| Types | `index.d.ts` |
| Runtime dependencies | `unified, @types/nlcst, nlcst-to-string` |

## Installation

```bash
npm install @stackline/retext-stringify
```

Preserve existing imports and plugin resolution with an npm alias:

```bash
npm install retext-stringify@npm:@stackline/retext-stringify
```

## Usage and API reference

### retext-stringify


[**retext**][retext] plugin to serialize natural language.
[Compiler][] for [**unified**][unified].
Serializes [**nlcst**][nlcst] syntax trees.

## Sponsors

Support this effort and give back by sponsoring on [OpenCollective][collective]!



<table>
<tr valign="middle">
<td width="20%" align="center" colspan="2">
  <a href="https://www.gatsbyjs.org">Gatsby</a> 🥇<br><br>
  <a href="https://www.gatsbyjs.org"><img src="https://avatars1.githubusercontent.com/u/12551863?s=256&v=4" width="128"></a>
</td>
<td width="20%" align="center" colspan="2">
  <a href="https://vercel.com">Vercel</a> 🥇<br><br>
  <a href="https://vercel.com"><img src="https://avatars1.githubusercontent.com/u/14985020?s=256&v=4" width="128"></a>
</td>
<td width="20%" align="center" colspan="2">
  <a href="https://www.netlify.com">Netlify</a><br><br>
  
  <a href="https://www.netlify.com"><img src="https://images.opencollective.com/netlify/4087de2/logo/256.png" width="128"></a>
</td>
<td width="10%" align="center">
  <a href="https://www.holloway.com">Holloway</a><br><br>
  <a href="https://www.holloway.com"><img src="https://avatars1.githubusercontent.com/u/35904294?s=128&v=4" width="64"></a>
</td>
<td width="10%" align="center">
  <a href="https://themeisle.com">ThemeIsle</a><br><br>
  <a href="https://themeisle.com"><img src="https://avatars1.githubusercontent.com/u/58979018?s=128&v=4" width="64"></a>
</td>
<td width="10%" align="center">
  <a href="https://boosthub.io">Boost Hub</a><br><br>
  <a href="https://boosthub.io"><img src="https://images.opencollective.com/boosthub/6318083/logo/128.png" width="64"></a>
</td>
<td width="10%" align="center">
  <a href="https://expo.io">Expo</a><br><br>
  <a href="https://expo.io"><img src="https://avatars1.githubusercontent.com/u/12504344?s=128&v=4" width="64"></a>
</td>
</tr>
<tr valign="middle">
<td width="100%" align="center" colspan="10">
  <br>
  <a href="https://opencollective.com/unified"><strong>You?</strong></a>
  <br><br>
</td>
</tr>
</table>

## Install

This package is [ESM only](https://gist.github.com/sindresorhus/a39789f98801d908bbc7ff3ecc99d99c):
Node 12+ is needed to use it and it must be `import`ed instead of `require`d.

[npm][]:

```sh
npm install @stackline/retext-stringify
```

## Use

```js
import {unified} from 'unified'
import {stream} from 'unified-stream'
import retextEnglish from 'retext-english'
import retextStringify from '@stackline/retext-stringify'
import retextEmoji from 'retext-emoji'

const processor = unified()
  .use(retextEnglish)
  .use(retextEmoji, {convert: 'encode'})
  .use(retextStringify)

process.stdin.pipe(stream(processor)).pipe(process.stdout)
```

## API

This package exports no identifiers.
`retextStringify` is the default export.

### `unified().use(retextStringify)`

Serialize [**nlcst**][nlcst] syntax trees.
There is no configuration.

## Contribute

See [`contributing.md`][contributing] in [`retextjs/.github`][health] for ways
to get started.
See [`support.md`][support] for ways to get help.
Ideas for new plugins and tools can be posted in [`retextjs/ideas`][ideas].

A curated list of awesome retext resources can be found in [**awesome
retext**][awesome].

This project has a [code of conduct][coc].
By interacting with this repository, organization, or community you agree to
abide by its terms.

## License

[MIT][license] © [Titus Wormer][author]



[build-badge]: https://github.com/retextjs/retext/workflows/main/badge.svg

[build]: https://github.com/retextjs/retext/actions

[coverage-badge]: https://img.shields.io/codecov/c/github/retextjs/retext.svg

[coverage]: https://codecov.io/github/retextjs/retext

[downloads-badge]: https://img.shields.io/npm/dm/retext-stringify.svg

[downloads]: https://www.npmjs.com/package/retext-stringify

[size-badge]: https://img.shields.io/bundlephobia/minzip/retext-stringify.svg

[size]: https://bundlephobia.com/result?p=retext-stringify

[sponsors-badge]: https://opencollective.com/unified/sponsors/badge.svg

[backers-badge]: https://opencollective.com/unified/backers/badge.svg

[collective]: https://opencollective.com/unified

[chat-badge]: https://img.shields.io/badge/chat-discussions-success.svg

[chat]: https://github.com/retextjs/retext/discussions

[health]: https://github.com/retextjs/.github

[contributing]: https://github.com/retextjs/.github/blob/main/contributing.md

[support]: https://github.com/retextjs/.github/blob/main/support.md

[coc]: https://github.com/retextjs/.github/blob/main/code-of-conduct.md

[ideas]: https://github.com/retextjs/ideas

[awesome]: https://github.com/retextjs/awesome-retext

[license]: https://github.com/retextjs/retext/blob/main/license

[author]: https://wooorm.com

[npm]: https://docs.npmjs.com/cli/install

[unified]: https://github.com/unifiedjs/unified

[compiler]: https://github.com/unifiedjs/unified#processorcompiler

[retext]: https://github.com/retextjs/retext

[nlcst]: https://github.com/syntax-tree/nlcst

## Credits and original authors

- Original project: [retext-stringify](https://github.com/retextjs/retext).
- Titus Wormer.
- Copyright (c) 2014 Titus Wormer <tituswormer@gmail.com>.
- Stackline maintenance: [Alexandro Paixao Marques](https://www.linkedin.com/in/aleinfo/) and [Stackline contributors](https://github.com/alexandroit).

Original copyright, license notices and contributor acknowledgements remain part of this distribution. Stackline maintenance does not replace authorship of the original work.

## Community and Links

- [Stackline website](https://alexandro.net/)
- [GitHub projects](https://github.com/alexandroit)
- [npm packages](https://www.npmjs.com/~alex360qc)
- [Reddit community — r/Stackline](https://www.reddit.com/r/Stackline/)
- [Maintainer LinkedIn](https://www.linkedin.com/in/aleinfo/)

Use this repository's issue tracker for reproducible bugs and feature requests. Join r/Stackline for examples, usage questions and release discussions.
