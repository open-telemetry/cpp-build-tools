# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Guideline to update the version

Increment the:

* MAJOR version when you make incompatible API/ABI changes,
* MINOR version when you add functionality in a backwards compatible manner, and
* PATCH version when you make backwards compatible bug fixes.

## [Unreleased]

## [0.24] 2025-07-20

* Bump actions/checkout from 3 to 4
  [#2](https://github.com/open-telemetry/cpp-build-tools/pull/2)

* Bump docker/login-action from 2 to 3
  [#3](https://github.com/open-telemetry/cpp-build-tools/pull/3)

* docker user for cpp_format_tools
  [#4](https://github.com/open-telemetry/cpp-build-tools/pull/4)

* [DOC] Cleanup after migration from build-tools
  [#5](https://github.com/open-telemetry/cpp-build-tools/pull/5)

* bump alpine to 3.19
  [#6](https://github.com/open-telemetry/cpp-build-tools/pull/6)

* [CI] Upgrade to clang-format-18
  [#8](https://github.com/open-telemetry/cpp-build-tools/pull/8)

* [FORMAT] Do not format .diff and .patch
  [#10](https://github.com/open-telemetry/cpp-build-tools/pull/10)

* Add FOSSA scanning workflow
  [#11](https://github.com/open-telemetry/cpp-build-tools/pull/11)

* [ADMIN] Add FOSSA badges
  [#12](https://github.com/open-telemetry/cpp-build-tools/pull/12)

* Add ossf-scorecard scanning workflow
  [#13](https://github.com/open-telemetry/cpp-build-tools/pull/13)

* Update community member listings
  [#14](https://github.com/open-telemetry/cpp-build-tools/pull/14)

* Fix outdated community membership link
  [#16](https://github.com/open-telemetry/cpp-build-tools/pull/16)

* Add minimum token permissions for all github workflow files
  [#17](https://github.com/open-telemetry/cpp-build-tools/pull/17)

* Don't rely on github team links which aren't visible to external contributors
  [#15](https://github.com/open-telemetry/cpp-build-tools/pull/15)

* Important note:

  * The last release from repository https://github.com/open-telemetry/build-tools,
    which generated a cpp_format_tools docker image,
    uses tag v0.23
  * To ensure continuity for generated docker images:
    https://hub.docker.com/r/otel/cpp_format_tools/tags
    the first release for this repository uses tag v0.24

## [0.0] 2024-02-16

* Migrated from https://github.com/open-telemetry/build-tools
