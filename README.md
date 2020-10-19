# node-hypixel

[![npm](https://img.shields.io/npm/v/@zikeji/hypixel)][npm]
[![npm bundle size](https://img.shields.io/bundlephobia/min/@zikeji/hypixel)][npm]
[![visit docs](https://img.shields.io/badge/docs-VuePress-green)][docs]
[![Snyk Vulnerabilities for npm package version](https://img.shields.io/snyk/vulnerabilities/npm/@zikeji/hypixel)][npm]
[![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/npm/@zikeji/hypixel)][npm]
[![GitHub license](https://img.shields.io/github/license/zikeji/node-hypixel)](https://github.com/zikeji/node-hypixel/blob/master/LICENSE)
[![GitHub last commit](https://img.shields.io/github/last-commit/zikeji/node-hypixel)][github]
[![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/zikeji/node-hypixel)][github]
[![GitHub issues](https://img.shields.io/github/issues/zikeji/node-hypixel)](https://github.com/zikeji/node-hypixel/issues)
[![Coveralls](https://img.shields.io/coveralls/github/zikeji/node-hypixel)](https://coveralls.io/github/zikeji/node-hypixel)
[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/zikeji/node-hypixel/release)][github]

[npm]: https://www.npmjs.com/package/@zikeji/hypixel
[github]: https://github.com/zikeji/node-hypixel
[docs]: https://node-hypixel.zikeji.com
[hypixel]: https://api.hypixel.net/

An unopinionated async/await API wrapper for [Hypixel's Public API][hypixel] developed in TypeScript complete with [documentation][docs], typed interfaces for all API responses, rate-limit handling, a few helpers, and support for undocumented endpoints.

The library aims to replicate the [Hypixel API][hypixel] as closely as possible, and as such won't alter the results, merely offering intellisense suggestions, rate-limit handling, and helpers.

## Project Status

`ALPHA` - this project is not ready for production use, expect breaking changes that do not follow semver. semantic-releaser bumped me to 1.0.0, I had intended to stay on 0.X.X, and use 1.0.0 as my release, but it didn't pan out. 2.0.0 will be my release once all necessary features are completed.

### Roadmap

- [x] Add rate limiting support
- [ ] Add method, typing, testing, and documentation for:
  - [ ] Boosters
  - [ ] Find Guild
  - [ ] Friends
  - [ ] Game Counts
  - [ ] Guild
  - [ ] Key
  - [ ] Leaderboards
  - [ ] Player
  - [ ] Player Count
  - [ ] Recent Games
  - [ ] **Resources**
    - [ ] Achievements
    - [ ] Challenges
    - [ ] **Guilds**
      - [ ] Achievements
      - [ ] Permissions
    - [ ] **SkyBlock**
      - [x] Collections
      - [ ] Skills
    - [ ] Quests
  - [ ] **SkyBlock**
    - [x] News
    - [ ] Profile
    - [ ] Profiles
    - [ ] Auction
    - [ ] Auctions
    - [ ] Bazaar
  - [ ] Status
  - [x] Watchdog Stats

## Installation

Use [npm](https://www.npmjs.com) to install this library.

```bash
npm i --save @zikeji/hypixel
```

## Usage

```javascript
import { Client as Hypixel } from "@zikeji/hypixel";
const client = new Hypixel("API_KEY");
```

## Contributing
If some API result isn't documented / typed out fully, please open an issue and I can add it ASAP. Otherwise, pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

All changes must ensure they pass eslint, tests, and that testing is updated to meet or exceed the previous coverage.

## License
[MIT](https://choosealicense.com/licenses/mit/)