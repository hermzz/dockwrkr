# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

## [2.0.1] - 2019-01-17

## Fixed
- Fixed a bug where under recent docker daemons (>17.10) the email flag is no longer accepted for docker login.

## [2.0.0] - 2019-01-12

### Added
- Dockwrkr now requires python3 to operate.

## [1.2.0] - 2017-11-15
### Added
- Jobs feature. Define short-lived `jobs` in `dockwrkr.yml` which are executed
  in an ad-hoc manner.
- Added support for `shm_size` Docker option

### Changed
- The `containers` section of `dockwrkr.yml` has been renamed to `services`, however backward-compatibility for `containers` is still maintained.

## [1.1.2] - 2017-11-09

### Fixed
- Another fix to docker command streaming when "create" needs to pull an image.

## [1.1.1] - 2017-11-09

### Fixed
- Use proper streaming or check output when pulling images to fix \r in console
- Fixed certain crashes related to logging with recreate and restart

## [1.1.0] - 2017-11-07
### Fixed
- Unclear error message when referring to undefined container in `link` clause

### Added
- `dockwrkr login` command for logging into all defined registries

### Changed
- `dockwrkr.yml`: `containers` has been renamed to `services`. Support for the
  `containers` key is maintained until next major release.

## [1.0.1] - 2017-06-13

### Added
- Networking guide to `README.md`

### Fixed
- Broken network detection with Docker 1.11

## [1.0.0] - 2017-06-13

Initial release.

