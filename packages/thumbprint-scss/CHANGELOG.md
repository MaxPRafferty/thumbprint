# Changelog

## Unreleased

## 1.0.0 - 2019-04-08

### Changed

-   [Patch] Replace `$tp-spacer__unit` in `textarea.scss` with hardcoded pixel value.

### Removed

-   [Major] Remove `function.scss` that contained the `tp-spacer` function which used a unit of `8` to output a pixel value. To upgrade, first replace any instances of `tp-spacer(*)` that have an equivalent [space token](https://thumbprint.design/tokens/scss/#section-space). Then replace any remaining instances with a hardcoded pixel value. For example, `tp-spacer(1)` would be `$tp-space__2`, `tp-spacer(1.5)` would be `12px` as it has no equivalent space token.

## 0.3.1 - 2019-04-02

### Changed

-   [Patch] Update version of dependencies. This doesn't affect the outputted code.

## 0.3.0 - 2019-03-28

### Changed

-   [Patch] Convert all `tp-spacer` instances to `tp-space__*` or hardcoded values. (#159)

### Added

-   [Minor] Add `tertiary` theme that is the same as our `secondary` style. `secondary` will soon be redesigned to have blue text. Consumers should replace `tp-button--secondary` with `tp-button--tertiary` to avoid and visual changes. (#89)

## 0.2.0 - 2019-03-25

### Changed

-   [Patch] Replace deprecated `tp-font__text` tokens with new values. (#171)
-   [Minor] Change `tp-alert--warning` background color to `$tp-color__yellow-200` and text color to `$tp-color__yellow-600` for better readability.

## 0.1.3 - 2019-03-11

### Changed

-   [Patch] Update version of dependencies. This doesn't affect the outputted code.

## 0.1.2 - 2019-02-20

### Changed

-   [Patch] Replaced Sass placeholder and `@extend` with class. (#107)
-   [Patch] Use a red border in the `caution` button focus state. (#116)

### Deprecated

-   [Patch] Indicate that the "wrap snap" class and mixin are deprecated. (#17)

## 0.1.1 - 2019-02-08

### Changed

-   [Patch] Change name of the CSS dist from `css.css` to `components.css`.
-   [Patch] Use tilde imports in Node Sass with `node-sass-tilde-importer`.

## 0.1.0 - 2019-02-07

### Added

-   [Minor] Created package for Thumbprint SCSS. (#38)
