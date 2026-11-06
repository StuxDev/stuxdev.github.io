# Changelog

All notable changes to Stux.Dev GitHub Pages Redirect (stuxdev.github.io) are documented here.

Each release's sections come in this order: Added, Changed, Fixed, Removed, Security, Deprecated. This project uses [Date Versioning](https://datevers.ing) since v26.10.23 (`YY.MM.DD`, the UTC release date, with `-1`, `-2`… for later releases the same day); earlier releases used [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## v26.11.06

### Changed

- The README and CONTRIBUTING call this template by its full name, Stux.Dev GitHub Pages Redirect, as services.stux.dev
  does, and their logos follow GitHub's light or dark theme.
- The README's Configuration section shows the lines actually in `index.html` (which redirect to github.com/StuxDev),
  and says the visitor's path isn't carried over. The feature list no longer claims it is.
- The README's footer matches the other Stux.Dev repositories, and its License section gives the copyright holder,
  Stux.Group.
- This changelog's intro gives the house section order instead of citing Keep a Changelog, whose order differs.

## v26.10.23

### Added

- `tests/version.sh`, which checks that `VERSION.md` is a valid Date Version, a real calendar date not in the future, and the same as the newest entry in this changelog

### Changed

- Switched from Semantic Versioning to [Date Versioning](https://datevers.ing): releases are numbered by their UTC release date as `YY.MM.DD`, with `-1`, `-2`… for later releases the same day. This release follows v1.0.1
- `commit.sh` and `commit.bat` refuse a `VERSION.md` that isn't a valid Date Version or is dated in the future (UTC), and warn when it's dated before today
- `README.md` and `CONTRIBUTING.md` describe Date Versioning and the release steps

## v1.0.1

### Fixed
- GitHub Pages was using the legacy branch-deploy build system, which can silently stop auto-deploying with no error recorded anywhere (discovered on SeasonalOverlaysLibrary — its live site served stale content for over an hour with no visible failure). Switched to GitHub Actions-based Pages deployment (`.github/workflows/pages.yml`), making every deploy an ordinary, observable CI run instead.

## v1.0.0

### Added
- Initial GitHub Pages redirect repo for Stux.Dev, redirecting `stuxdev.github.io` to `github.com/StuxDev` — `VERSION.md`/`CHANGELOG.md`/`CONTRIBUTING.md`/`commit.sh`+`commit.bat` added, following the standard release-flow convention used across other Stux.Group family repos.
