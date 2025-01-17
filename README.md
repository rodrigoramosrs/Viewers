<!-- prettier-ignore-start -->
<!-- markdownlint-disable -->
<div align="center">
  <h1>ohif-viewer</h1>
  <p><strong>ohif-viewer</strong> is a zero-footprint medical image viewer provided by the <a href="http://ohif.org/">Open Health Imaging Foundation (OHIF)</a>. It is a configurable and extensible progressive web application with out-of-the-box support for image archives which support <a href="https://www.dicomstandard.org/dicomweb/">DICOMweb</a>.</p>
</div>


<div align="center">
  <a href="https://docs.ohif.org/"><strong>Read The Docs</strong></a> |
  <a href="https://github.com/OHIF/Viewers/tree/master/docs/latest">Edit the docs</a>
</div>
<div align="center">
  <a href="https://docs.ohif.org/demo">Demo</a> |
  <a href="https://ohif.canny.io/">Roadmap</a> |
  <a href="https://react.ohif.org/">Component Library</a>
</div>


<hr />

[![CircleCI][circleci-image]][circleci-url]
[![codecov][codecov-image]][codecov-url]
[![All Contributors](https://img.shields.io/badge/all_contributors-7-orange.svg?style=flat-square)](#contributors)
[![code style: prettier][prettier-image]][prettier-url]
[![semantic-release][semantic-image]][semantic-url]

[![NPM version][npm-version-image]][npm-url]
[![NPM downloads][npm-downloads-image]][npm-url]
[![Pulls][docker-pulls-img]][docker-image-url]
[![MIT License][license-image]][license-url]
<!-- markdownlint-enable -->
<!-- prettier-ignore-end -->

> ATTENTION: If you are looking for Version 1 (the Meteor Version) of this
> repository, it lives on
> [the `v1.x` branch](https://github.com/OHIF/Viewers/tree/v1.x)

## Why?

Building a web based medical imaging viewer from scratch is time intensive, hard
to get right, and expensive. Instead of re-inventing the wheel, you can use the
OHIF Viewer as a rock solid platform to build on top of. The Viewer is a
[React][react-url] [Progressive Web Application][pwa-url] that can be embedded
in existing applications via it's [packaged source
(ohif-viewer)][ohif-viewer-url] or hosted stand-alone. The Viewer exposes
[configuration][configuration-url] and [extensions][extensions-url] to support
workflow customization and advanced functionality at common integration points.

If you're interested in using the OHIF Viewer, but you're not sure it supports
your use case [check out our docs](https://docs.ohif.org/). Still not sure, or
you would like to propose new features? Don't hesitate to
[create an issue](https://github.com/OHIF/Viewers/issues) or open a pull
request.

## Getting Started

This readme is specific to testing and developing locally. If you're more
interested in production deployment strategies,
[you can check out our documentation on publishing](https://docs.ohif.org/).

Want to play around before you dig in?
[Check out our LIVE Demo](https://viewer.ohif.org/)

### Setup

_Requirements:_

- [NodeJS & NPM](https://nodejs.org/en/download/)
- [Yarn](https://yarnpkg.com/lang/en/docs/install/)

_Steps:_

1. Fork this repository
2. Clone your forked repository (your `origin`)

- `git clone git@github.com:YOUR_GITHUB_USERNAME/Viewers.git`

3. Add `OHIF/Viewers` as a `remote` repository (the `upstream`)

- `git remote add upstream git@github.com:OHIF/Viewers.git`

### Developing Locally

In your cloned repository's root folder, run:

```js
// Restore dependencies
yarn install

// Stands up local server to host Viewer.
// Viewer connects to our public cloud PACS by default
yarn start
```

For more advanced local development scenarios, like using your own locally
hosted PACS and test data,
[check out our Essential: Getting Started](https://docs.ohif.org/essentials/getting-started.html)
guide.

### Contributing

> Large portions of the Viewer's functionality are maintained in other
> repositories. To get a better understanding of the Viewer's architecture and
> "where things live", read
> [our docs on the Viewer's architecture](https://docs.ohif.org/advanced/architecture.html#diagram)

It is notoriously difficult to setup multiple dependent repositories for
end-to-end testing and development. That's why we recommend writing and running
unit tests when adding and modifying features. This allows us to program in
isolation without a complex setup, and has the added benefit of producing
well-tested business logic.

1. Clone this repository
2. Navigate to the project directory, and `yarn install`
3. To begin making changes, `yarn run dev`
4. To commit changes, run `yarn run cm`

When creating tests, place the test file "next to" the file you're testing.
[For example](https://github.com/OHIF/Viewers/blob/master/src/utils/index.test.js):

```js
// File
index.js

// Test for file
index.test.js
```

As you add and modify code, `jest` will watch for uncommitted changes and run
your tests, reporting the results to your terminal. Make a pull request with
your changes to `master`, and a core team member will review your work. If you
have any questions, please don't hesitate to reach out via a GitHub issue.

## Issues

_Looking to contribute? Look for the [Good First Issue][good-first-issue]
label._

### 🐛 Bugs

Please file an issue for bugs, missing documentation, or unexpected behavior.

[**See Bugs**][bugs]

### 💡 Feature Requests

Please file an issue to suggest new features. Vote on feature requests by adding
a 👍. This helps maintainers prioritize what to work on.

[**See Feature Requests**][requests-feature]

### ❓ Questions

For questions related to using the library, please visit our support community,
or file an issue on GitHub.

[Google Group][google-group]

## Roadmap

If you want to know what's planned for the very near future,
[check out our roadmap](https://ohif.canny.io/). The best way to influence when
and what is worked on is to contribute to the conversation by creating GitHub
issues, and contributing code through pull requests. OHIF's high level
priorities for the near future are:

- Feature parity with version 1
- Extension and configuration improvements with key integration partners
- Continued Developer Experience Improvements
- Segmentation Tools, and improved VTK.js support

More granular information will make it's way to the backlog as these items
become scoped for development by core maintainers.

> Don't hesitate to ask questions, propose features, or create pull requests.
> We're here, we're listening, and we're ready to build the best open source
> medical imaging viewer on the web.

#### Roadmap Generously Powered by Canny.io

<a href="https://ohif.canny.io/">
  <img height="30" src="docs/latest/assets/img/canny-full.png" />
</a>

## Contributors

Thanks goes to these wonderful people
([emoji key](https://allcontributors.org/docs/en/emoji-key)):

<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
<!-- prettier-ignore -->
<table><tr><td align="center"><a href="https://github.com/swederik"><img src="https://avatars3.githubusercontent.com/u/607793?v=4" width="100px;" alt="Erik Ziegler"/><br /><sub><b>Erik Ziegler</b></sub></a><br /><a href="https://github.com/OHIF/Viewers/commits?author=swederik" title="Code">💻</a></td><td align="center"><a href="https://github.com/evren217"><img src="https://avatars1.githubusercontent.com/u/4920551?v=4" width="100px;" alt="Evren Ozkan"/><br /><sub><b>Evren Ozkan</b></sub></a><br /><a href="https://github.com/OHIF/Viewers/commits?author=evren217" title="Code">💻</a></td><td align="center"><a href="https://github.com/galelis"><img src="https://avatars3.githubusercontent.com/u/2378326?v=4" width="100px;" alt="Gustavo André Lelis"/><br /><sub><b>Gustavo André Lelis</b></sub></a><br /><a href="https://github.com/OHIF/Viewers/commits?author=galelis" title="Code">💻</a></td><td align="center"><a href="http://dannyrb.com/"><img src="https://avatars1.githubusercontent.com/u/5797588?v=4" width="100px;" alt="Danny Brown"/><br /><sub><b>Danny Brown</b></sub></a><br /><a href="https://github.com/OHIF/Viewers/commits?author=dannyrb" title="Code">💻</a></td><td align="center"><a href="https://github.com/all-contributors/all-contributors-bot"><img src="https://avatars3.githubusercontent.com/u/46843839?v=4" width="100px;" alt="allcontributors[bot]"/><br /><sub><b>allcontributors[bot]</b></sub></a><br /><a href="https://github.com/OHIF/Viewers/commits?author=allcontributors" title="Documentation">📖</a></td><td align="center"><a href="https://www.linkedin.com/in/siliconvalleynextgeneration/"><img src="https://avatars0.githubusercontent.com/u/1230575?v=4" width="100px;" alt="Esref Durna"/><br /><sub><b>Esref Durna</b></sub></a><br /><a href="#question-EsrefDurna" title="Answering Questions">💬</a></td><td align="center"><a href="https://github.com/diego0020"><img src="https://avatars3.githubusercontent.com/u/7297450?v=4" width="100px;" alt="diego0020"/><br /><sub><b>diego0020</b></sub></a><br /><a href="https://github.com/OHIF/Viewers/commits?author=diego0020" title="Code">💻</a></td></tr></table>

<!-- ALL-CONTRIBUTORS-LIST:END -->

This project follows the
[all-contributors](https://github.com/all-contributors/all-contributors)
specification. Contributions of any kind welcome!

## License

MIT © [OHIF](https://github.com/OHIF)

## Acknowledgments

To acknowledge the OHIF Viewer in an academic publication, please cite

> _LesionTracker: Extensible Open-Source Zero-Footprint Web Viewer for Cancer
> Imaging Research and Clinical Trials_
>
> Trinity Urban, Erik Ziegler, Rob Lewis, Chris Hafey, Cheryl Sadow, Annick D.
> Van den Abbeele and Gordon J. Harris
>
> _Cancer Research_, November 1 2017 (77) (21) e119-e122 DOI:
> [10.1158/0008-5472.CAN-17-0334](https://www.doi.org/10.1158/0008-5472.CAN-17-0334)

**Note:** If you use or find this repository helpful, please take the time to
star this repository on Github. This is an easy way for us to assess adoption
and it can help us obtain future funding for the project.

This work is supported primarily by the National Institutes of Health, National
Cancer Institute, Informatics Technology for Cancer Research (ITCR) program,
under a
[grant to Dr. Gordon Harris at Massachusetts General Hospital (U24 CA199460)](https://projectreporter.nih.gov/project_info_description.cfm?aid=8971104).

<!--
Links:
-->

<!-- prettier-ignore-start -->
<!-- ROW -->
[all-contributors-image]: https://img.shields.io/badge/all_contributors-0-orange.svg?style=flat-square
[contributing-url]: https://github.com/OHIF/Viewers/blob/react/CONTRIBUTING.md
[circleci-image]: https://circleci.com/gh/OHIF/Viewers.svg?style=svg
[circleci-url]: https://circleci.com/gh/OHIF/Viewers
[codecov-image]: https://codecov.io/gh/OHIF/Viewers/branch/react/graph/badge.svg
[codecov-url]: https://codecov.io/gh/OHIF/Viewers/branch/react
[prettier-image]: https://img.shields.io/badge/code_style-prettier-ff69b4.svg?style=flat-square
[prettier-url]: https://github.com/prettier/prettier
[semantic-image]: https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg
[semantic-url]: https://github.com/semantic-release/semantic-release
<!-- ROW -->
[npm-url]: https://npmjs.org/package/ohif-viewer
[npm-downloads-image]: https://img.shields.io/npm/dm/ohif-viewer.svg?style=flat-square
[npm-version-image]: https://img.shields.io/npm/v/ohif-viewer.svg?style=flat-square
[docker-pulls-img]: https://img.shields.io/docker/pulls/ohif/viewer.svg?style=flat-square
[docker-image-url]: https://hub.docker.com/r/ohif/viewer
[license-image]: https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square
[license-url]: LICENSE
<!-- DOCS -->
[react-url]: https://reactjs.org/
[pwa-url]: https://developers.google.com/web/progressive-web-apps/
[ohif-viewer-url]: https://www.npmjs.com/package/ohif-viewer
[configuration-url]: https://docs.ohif.org/essentials/configuration.html
[extensions-url]: https://docs.ohif.org/advanced/extensions.html
<!-- Misc. -->
[react-viewer]: https://github.com/OHIF/Viewers/tree/react
<!-- Issue Boilerplate -->
[bugs]: https://github.com/OHIF/Viewers/labels/bug
[requests-feature]: https://github.com/OHIF/Viewers/labels/enhancement
[good-first-issue]: https://github.com/OHIF/Viewers/labels/good%20first%20issue
[google-group]: https://groups.google.com/forum/#!forum/cornerstone-platform
<!-- prettier-ignore-end -->
