# Changelog

All notable changes to this project will be documented in this file.

## [1.2.2](https://github.com/SpotOnInc/renovate-config/compare/v1.2.1...v1.2.2) (2023-03-30)


### Bug Fixes

* Removal `v` prefix in `_VERSION` now support `X.Y.Zany.thing` tags ([#66](https://github.com/SpotOnInc/renovate-config/issues/66)) ([e808761](https://github.com/SpotOnInc/renovate-config/commit/e808761abc0ceb98b255c5c5d6b1378168dff20e))

## [1.2.1](https://github.com/SpotOnInc/renovate-config/compare/v1.2.0...v1.2.1) (2023-03-24)


### Bug Fixes

* Remove `v` prefix in Dockerfile and Github Action `_VERSION` variables ([#64](https://github.com/SpotOnInc/renovate-config/issues/64)) ([5910fc0](https://github.com/SpotOnInc/renovate-config/commit/5910fc0e8cfca02521dd00cf64aad842529dcbef))

# [1.2.0](https://github.com/SpotOnInc/renovate-config/compare/v1.1.0...v1.2.0) (2023-02-27)


### Features

* Remove `v` prefix in Dockerfile `_VERSION` variables ([#54](https://github.com/SpotOnInc/renovate-config/issues/54)) ([0090822](https://github.com/SpotOnInc/renovate-config/commit/0090822746015f84522cc382aa28e6c07909d147))


### Reverts

* Revert "chore(deps): update jossef/action-latest-release-info action to v1.2.2" (#53) ([f52e989](https://github.com/SpotOnInc/renovate-config/commit/f52e989d7fa4734db4a880e7098c0fb73cfb0c02)), closes [#53](https://github.com/SpotOnInc/renovate-config/issues/53)

# [1.1.0](https://github.com/SpotOnInc/renovate-config/compare/v1.0.0...v1.1.0) (2023-01-23)


### Bug Fixes

* Point in Dependency dashboard Header ([7a0cf25](https://github.com/SpotOnInc/renovate-config/commit/7a0cf257fab713a459f621098f63fe6270e80a97))


### Features

* Simplify logs location search by adding link to Dashboard ([#37](https://github.com/SpotOnInc/renovate-config/issues/37)) ([ac2fcde](https://github.com/SpotOnInc/renovate-config/commit/ac2fcdebd4bbe0c12d153f85b52fa327cee952a4))

# 1.0.0 (2023-01-17)


### Features

* Pin Terraform versions as Digests, and init SemVer ([#28](https://github.com/SpotOnInc/renovate-config/issues/28)) ([f3c33a5](https://github.com/SpotOnInc/renovate-config/commit/f3c33a522e1b3cebd7b2dc3e1d0ff2e0697ae5f5))
