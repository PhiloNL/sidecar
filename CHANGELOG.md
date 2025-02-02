# Changelog
## Unreleased 

## 0.3.5 - 2022-01-09

### Added

- Add Package method to include strings as files.
- Add Package method to include files with more explicit path control ([#41](https://github.com/hammerstonedev/sidecar/pull/41))

### Fixed

- Wait for the function to update before updating environment variables.
- Be more clear when deleting keys

## 0.3.4 - 2022-01-02

### Fixed

- Add method to ensure function is updated before we try to do anything else. Should hopefully fix [#32](https://github.com/hammerstonedev/sidecar/issues/32)  


## 0.3.3 - 2021-11-01

### Added
- Added runtime constants ([#33](https://github.com/hammerstonedev/sidecar/pull/33))
- Add event invocation support ([#36](https://github.com/hammerstonedev/sidecar/pull/36))
 
### Fixed
- Docs typo ([#31](https://github.com/hammerstonedev/sidecar/pull/31)) 
- Update package documentation to include note for shipping node_modules ([#34](https://github.com/hammerstonedev/sidecar/pull/34))

## 0.3.2 - 2021-08-13

### Added
- Support for Container Images. [#29](https://github.com/hammerstonedev/sidecar/pull/29)

## 0.3.1 - 2021-07-31

### Fixed
- Cast Memory and Timeout to integers. Fixes [#28](https://github.com/hammerstonedev/sidecar/issues/28)

## 0.3.0 - 2021-07-20

### Added
- Support for Lambda environment variables ([#25](https://github.com/hammerstonedev/sidecar/pull/25))

## 0.2.0 - 2021-07-12 

### Added
- New `sidecar.env` config option to separate Sidecar environment from application environment. Useful mostly for teams who have multiple developers that all have an app env of `local` and don't want to be constantly overwriting each other's functions.
- New `sidecar:warm` command ([#6](https://github.com/hammerstonedev/sidecar/pull/6))
- Better error reporting when `sidecar:deploy` is called and there are no functions.
- Better error reporting when a function is not found. 
- Implemented sweeping to remove old, unused function versions ([#15](https://github.com/hammerstonedev/sidecar/pull/15))
- `--pre-warm` options to `sidecar:deploy` and `sidecar:active` commands ([Commit](https://github.com/hammerstonedev/sidecar/commit/4794e6d4bfc5ddb4976c4686939ca1ee0c0ae979))
- `latestVersionHasAlias` method to the LambdaClient ([Commit](https://github.com/hammerstonedev/sidecar/commit/a54f4e59aef9bfeac57ced7fb50b0c25ff268ab9))

### Changed
- Warming is now opt-in. 0 instances are configured by default. ([Commit](https://github.com/hammerstonedev/sidecar/commit/ba53467368bcb253034fdbae7726fb0916b28de2))
- Moved some methods into the Sidecar\LambdaClient ([#15](https://github.com/hammerstonedev/sidecar/pull/15))
- Break out logging & environment concerns from the Lambda Client. ([Commit](https://github.com/hammerstonedev/sidecar/commit/20e368c9773c4aae2262021c7682cf72737af270))

### Fixed
- Allow spacing in `APP_NAME` [#17](https://github.com/hammerstonedev/sidecar/pull/17)  

## 0.1.4 - 2021-06-05

- Added `*` option to include the entire base directory in the package. 

## 0.1.3 - 2021-05-24

- Fix more `sidecar:configure` AWS errors.

## 0.1.2 - 2021-05-24

- Fix other `sidecar:configure` AWS errors. ([#8](https://github.com/hammerstonedev/sidecar/issues/8) & ([#9](https://github.com/hammerstonedev/sidecar/issues/9))

## 0.1.1 - 2021-05-24

- Fix undefined `choice` ([#7](https://github.com/hammerstonedev/sidecar/issues/7))

##  v0.1.0 - May 15th, 2021.

First release.