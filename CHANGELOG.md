# Changelog

All notable changes to this project will be documented in this file. See [commit-and-tag-version](https://github.com/absolute-version/commit-and-tag-version) for commit guidelines.

## [3.0.1](https://github.com/tonylea/helm-chart-lidarr/compare/v3.0.0...v3.0.1) (2026-11-21)

### Bug Fixes

* let Lidarr's first-run screen set the login ([5e85aaf](https://github.com/tonylea/helm-chart-lidarr/commit/5e85aafb620b8ba6ee9449163656047f46781708))

### Documentation

* say the kind test is a fresh install ([3a71e21](https://github.com/tonylea/helm-chart-lidarr/commit/3a71e21d8ef30e107c4b0065aba61308725644ff))

## [3.0.0](https://github.com/tonylea/helm-chart-lidarr/compare/v2.0.0...v3.0.0) (2026-11-21)

### ⚠ BREAKING CHANGES

* persistence.data is now a list of named mounts, each at
  /data/<name>, with at least one required.

### Features

* mount each data volume at /data/<name> ([48fd966](https://github.com/tonylea/helm-chart-lidarr/commit/48fd9665fa4c2a5325696af66d5c720f2552c82b))

### Documentation

* show the chart's download count ([7fc0763](https://github.com/tonylea/helm-chart-lidarr/commit/7fc07632345c4eb5a231c01ee88a134bf68180da))

## [2.0.0](https://github.com/tonylea/helm-chart-lidarr/compare/v1.0.0...v2.0.0) (2026-11-21)

### ⚠ BREAKING CHANGES

* postgres.database is now postgres.databases.main,
  and Lidarr needs a log database, postgres.databases.log.

### Features

* keep Lidarr's log in its own Postgres database ([9dbe1bd](https://github.com/tonylea/helm-chart-lidarr/commit/9dbe1bd581791f858e684791d0c67e8694feac33))

### Bug Fixes

* leave resource requests to whoever deploys the chart ([1178d3e](https://github.com/tonylea/helm-chart-lidarr/commit/1178d3e93338c5d6ba7c1e035af692a742adb4b7))

### Documentation

* keep only the comments that record a decision ([dc54552](https://github.com/tonylea/helm-chart-lidarr/commit/dc545521c957fbd44138337a5b010365145b543c))
* keep the README to the fixed settings and what the chart needs ([7543621](https://github.com/tonylea/helm-chart-lidarr/commit/7543621614e74df84ed656f0a24d9af496990394))

## 1.0.0 (2026-11-21)

### Features

* deploy Lidarr on Postgres, with a fixed API key, a required login and claims for /config and /data ([e3761d9](https://github.com/tonylea/helm-chart-lidarr/commit/e3761d99b23bfc091852b0c92041f8644f138d46))

### Documentation

* describe the chart, its values and how to contribute ([2701d83](https://github.com/tonylea/helm-chart-lidarr/commit/2701d8307672df97ac60956cca7265b68a841563))
