## Changelog 📝

All notable changes to Flightdeck for 11ty will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.2.6] - 2024-05-07

**Full Changelog**: https://github.com/edheltzel/flightdeck-for-11ty-parcel/compare/v0.2.5...v0.2.6

### Changed

- package updates:
  - @aplinejs v3.13.7
  - @aplinejs/persist v3.13.7
  - @biomejs/biome v1.6.0


## [0.2.5] - 2024-03-04

**Full Changelog**: https://github.com/edheltzel/flightdeck-for-11ty-parcel/compare/v0.2.4...v0.2.5

### Adds

- includes AlpineJS for interactive components that need Javascript
- adds `{% Image %}` shortcode for responsive images using @11ty/eleventy-img

## [0.2.4] - 2024-02-27

**Full Changelog**: https://github.com/edheltzel/flightdeck-for-11ty-parcel/compare/v0.2.3...v0.2.4

## [0.2.3] - 2023-12-12

### Chore
- 🧹 Package updates:
  - markdown-it v14.0.0

## [0.2.2] - 2023-12-01

### Chore
- 🧹 Package updates:
  - Parcel v2.10.3
  - Luxon v3.4.4

## [0.2.1] - 2023-11-05

### Chore
- 🧹 Package updates

## [0.2.0] - 2023-10-14

### Added
- Package updates: Parcel v2.10.0
- bun as a package manager support
  - `sharp` added a `trustedDependancies` so Bun will work as a package manager
    - [see issue #35 from flightdeck-for-11ty(esbuild version)](https://github.com/edheltzel/flightdeck-for-11ty/issues/35)
  - includes `bun.lockb` and `pnpm-lock.yaml`
- includes visual guidance system (VGS) modules
  - follow cursor
  - theme toggle

### Changed
- Updated node to version 18.17.1 LTS
- Updated dependencies
- To keep things simple 11ty config uses default `.eleventy.js`
- npm script: `purge` updated to include `bun.lockb`
- keeps flightdeck versions in sync: primary project: [flightdeck for 11ty esbuild version](https://github.com/edheltzel/flightdeck-for-11ty-esbuild).


## [0.1.20] - 2023-08-02
### Changed

- Readme Updates
- blockquote shortcode
- local dictonary changes

## [0.1.17] - 2023-07-02

## Adds

- adds button component

### Changed

- Package updates - Parcel v2.9.1


## [0.1.16] - 2023-05-22

### Changed

- Readme is updated with current usage information
- Updated styles and theme switcher included for Lighthouse 100s

## [0.1.15] - 2023-05-17

### Changed

- Packages upgraded
- Readme is updated with current usage information

## [0.1.14] - 2023-03-28

### Changed
- package.json updated
  - uses ENV variables for 11ty build
  - uses yarn 3.5 instead of pnpm
- updates README.md

## [0.1.13] - 2023-03-14

### Changed
- package.json update
### Adds
Includes the following packages as dependencies:
- adds luxon
- adds markdown-it
## [0.1.12] - 2023-03-07
### Changed

- Packages upgraded
  - includes custom 404 page for 11ty Dev Server.
## [0.1.11] - 2023-02-09
### Changed
- includes 11ty 2.0

## [0.1.10] - 2023-02-04
### Changed
- Autopilot update and revert to original SMACSS scaffold

### TODO:
- better introduce the 7-1 patteren for easier theming
## [0.1.9] - 2023-02-04
### Changed
- fixes all the issues introduced with v0.1.6, v0.1.7, and v0.1.8

### Adds
- adds Collections back
- removes Views directory: clone of FD and push to master in new project caused issues with the releases and fudged up the template.

## [0.1.8] - 2023-01-19
- Removed  see v0.1.9

## [0.1.7] - 2023-01-19
- Removed  see v0.1.9
## [0.1.6] - 2023-01-19
### Changed
- `airframe.css` is now `style.css`, only to keep things universally consistent
- Airframe has been renamed to Autopilot
- updates `head.njk` to reflect new style.css
## [0.1.5] - 2023-01-19

### Changed
- updates Eleventy 2.0 Beta
- updates Parcel to latest

### Adds
- adds `.node-version` with `16.15.0` due to Cloudflare Pages defaulting to version 12
- adds Eleventy Dev Server to Flightdeck `workflow.js`
### Removes
- removes `.npmrc` no longer needed, Parcel handles this natively
- removes browsersync from Flightdeck `workflow.js`
## [0.1.4] - 2022-10-19
### Changed
- usage for copyright
- removes unused/empty files

## [0.1.3] - 2022-10-16
### Adds
- moves index.md to `/src/collections/pages/` to keep `src` clean
- adds permalink to index.md to resolve home page during build

## [0.1.2] - 2022-10-05
### Adds
- includes the 11ty Render plugin
- includes `airframe.css` inside of `head.njk` - was `app.css`
- adds `.npmrc` so that auto install of peer dependencies

### Changed
- readme update
- readme now suggests using pnpm again, if preinstalled all dependencies
- parcel watch/build for images now works for any image format supported by sharpJS.
  - images stored in subdirectory are not optimized also.
  - removed passthrough so parcel watch/build doesn't cause an endless loop
  - sharp config includes only quality option
- `.scrub` is now `.scrub.sh`

## [0.1.1] - 2022-09-30
### Changed
- package.json update
- `.scrub` no includes file extension `.scrub.sh`

## [0.1.1] - 2022-09-26

### Changed
- package.json --> Parcel watch now Globs the img directory correctly.

## [0.1.0] - 2022-09-25

### Adds
- includes an early version of Airframe CSS system
- adds content to include sample collections
- adds `.scrub` script through npm scripts to clean and purge

### Removes
- removes most `.keep` files from empty directories. (except for `src/assets/fonts`)

### Changed
- migrates all Flightdeck configuration to `_flightdeck` and `.manifest.js`
   -  file splitting is more organized
- updates license to WTFPL


## [0.0.4] - 2022-06-30

### Adds

- **Re-adds Parcel2 as the primary asset bundler**
- Sharp handles image compression via Parcel

### Removes

- esbuild and esbuild-sass-plugin are removed - now use [Parcel 2](https://parceljs.org/)

### Changed

- Scss no lives at `assets/styles`
-

## [0.0.3] - 2022-06-22

### Adds

- adds better support for postcss using esbuild-sass-plugin
- adds transforms and workflow
  - workflows are items related to development and eleventy specific settings
    - ie: `addPassthroughCopy`
- shortcodes
  - adds codepen shortcode see `/src/__flightdeck/shortcodes/codepen.js` for usage
  - adds `.vscode/shortcode.code-snippets` to list out all available shortcodes for the project.
- plugins
  - adds [eleventy-plugin-embed-everything](https://github.com/gfscott/eleventy-plugin-embed-everything) plugin - instead of creating shortcodes for media embeds - use the URL instead
- filters
  - (ref: [11ty.rocks](https://11ty.rocks))

### Removes

- parcel2 is on a feature branch
- removed most npm scripts - plan to re-add based on esbuild workflow
- removes un-used files left over from Parcel2

### Changed

- project scaffold moves everything under `src` - in better attempts to keep the project root clean
- config is now working under `src/__flightdeck`

### Deprecated

- all browsersync options will be removed once eleventy's server plugin is released under eleventy `v2.0`

## [0.0.2] - 2022-05-17

### Adds

- organized project scaffolded based on [webstoemp- Structuring Eleventy projects](https://www.webstoemp.com/blog/eleventy-projects-structure/)
- adds esbuild for javascript and sass bundling/processing
- - adds "common" shortcodes
  - (ref: [11ty.rocks](https://11ty.rocks))

### Removes

- parcel2 is on a feature branch
- removed most npm scripts - plan to re-add based on esbuild workflow
- removes `youtube.js` under shortcodes in favor of `eleventy-plugin-embed-everything`

### Changed

- eleventy config is broken up into multiple files, that live under `__flightdeck`

### Deprecated

- all browsersync options will be removed once eleventy's server plugin is released under eleventy `v2.0`

## [0.0.2] - 2022-02-20

Checkout branch `feature/parcel2`

### Added

- includes Parcel2
- adds parcel sass transformer
  - adds sass, postcss, autoprefixer for added support for styles during dev and prod
- includes npm-run-all for better npm scripts
  - run `pnpm run` to see a full list
- includes `flightdeck.manifest.js` for project configuration
  - to prevent the `.eleventy.js` from getting too long

### Removes

- drops `yarn` in favor of `pnpm`

## [0.0.1] - 2020-10-24

### Init

- this is an init and left empty intentionally

Attempting keep a minimal configuration for 11ty while keeping the tools similar to [Flightdeck for Jekyll](https://github.com/flight-deck/Flightdeck-for-Jekyll) and [Flightdeck for Hugo](https://github.com/flight-deck/Flightdeck-for-Hugo)
