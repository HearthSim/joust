# Joust Changelog
All notable changes to this project will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [Unreleased]
### Added
- Show Prince Malchezaar at game start (#142, @azeier)
- Show C'Thun stats in opponent hand (#133, @azeier)
- Show C'Thun as a minion during ritual (#137, @azeier)
- Highlight Hero Power when it's played (#140, @azeier)
- Add golden hero power and hero frame (#155, @andburn)
- Add golden inplay weapons (#159, @andburn)

### Changed
- Update dependencies
- Improve skip back behaviour when replay is paused
- Replace react-dimensions with a custom implementation (#121)
- Show error to user when fullscreen entering fails (#123)

### Fixed
- Malchezaar causing delay before Mulligan (#136, @azeier)
- Fix Mulligan X loading in late

## [0.7.0] - 2016-09-19
### Added
- Add C'Thun Rituals (@azeier)
- Add `Joust.destroy()`
- Add `Launcher.onFullscreen(callback:(fullscreen:boolean) => void)`
- Add `Launcher.onReady(ready:() => void)`
- Add `Launcher.fullscreen(fullscreen: boolean)`
- Shrinkwrap dependencies
- Add `gulp sentry:release`
- Add ES2015 polyfills using `babel-polyfill`
- Hide statistics for minions with HIDE\_STATS (#128, @jleclanche)
- Add `Launcher.enableKeybindings()` and `Launcher.disableKeybindings()`
- Add golden inplay frames (#134, @andburn)
- Add class borders for golden cards (#134, @andburn)

### Changed
- Replace own HearthstoneJSON implementation with common one
- Tweak scrubber tooltips
- Keybindings no longer have priority over non-joust HTML inputs
- Rescale speeds by a factor of 1.5
- Improve card description formatting
- HSReplay: Don't bail when encountering unknown tags

### Fixed
- Fix Shifter Zerus in hidden hand
- Improve Scrubber performance
- Fix minions being asleep when they shouldn't be

## [0.6.0] - 2016-08-21
### Added
- Add loading screen messages
- Show Hero Power and Weapon details on mouse over
- Various loading screen strings
- Add locale support
- Defer metadata fetching to hearthstonejson on npm
- Add Launcher.metadataSource to override HearthstoneJSON

### Fixed
- Show current stats when hovering entities
- Fix launcher example in README.md
- Fix default card art endpoint
- Fix GameStateScrubber.percentageWatched returning +/-Infinity

### Changed
- Don't unexhaust hero powers when hovering
- Update README.md
- Switch to Typescript 2.0.0

### Deprecated
- `Launcher.metadata` is now obsolete

## [0.5.0] - 2016-08-13
### Added
- Save replay speed preference in cookie
- Save ignore browser warning in cookie
- Unexhaust weapons and hero powers when hovering

### Changed
- Tweak text positioning
- Change timeline cursor (graphical)
- Improve performance when resizing applet horizontally

### Removed
- Remove proprietary fonts from source

### Fixed
- Changelog formatting
- Fix error when skipping back during Mulligan

## [0.4.0] - 2016-08-07
### Added
- Display keybindings in scrubber tooltips
- `Launcher.cardArt()` and `.assets()` can now accept a callback
- Ensure fullscreen does not error on unsupported devices (#123)
- Launcher: Add `.duration`, `.secondsWatched` and `.percentageWatched`

## [0.3.1] - 2016-08-01
### Fixed
- Fix minion hovering region for full card

## [0.3.0] - 2016-07-31
### Added
- Highlight cards that are swapped during Mulligan
- Display full card when hovering minions
- Show warning to users of IE/Edge due to clip-path not being supported
- Automatically run `typings install` on `npm install`
- Add Node v6.3 to supported versions

### Changed
- Reduce the pause after card is drawn
- Tweak tooltips
- Remove the pause between cards played by Yogg-Sarron
- Increase width of play/pause button
- Automatically download enums.d.ts on `npm install`

### Fixed
- Fix release URLs in Changelog

## [0.2.0] - 2016-07-28
### Added
- Metrics now contain a release tag
- Add tooltip when hovering secrets
- Add custom tooltips for scrubber buttons
- Lock screen orientation to landscape in fullscreen (#46)
- Display player concedes (#114)
- Add Changelog

### Changed
- Fully rework timings, greatly improving playback
- `Joust.release()` now reports a Semver string
- Prevent context menu in most places
- Reorder scrubber buttons

### Fixed
- Fix graphical glitch in timeline when Mulligan was very short

## 0.1.0 - 2016-07-25
### Added
- Code for initial development release

[Unreleased]: https://github.com/HearthSim/joust/compare/0.7.0...HEAD
[0.7.0]: https://github.com/HearthSim/joust/compare/0.6.0...0.7.0
[0.6.0]: https://github.com/HearthSim/joust/compare/0.5.0...0.6.0
[0.5.0]: https://github.com/HearthSim/joust/compare/0.4.0...0.5.0
[0.4.0]: https://github.com/HearthSim/joust/compare/0.3.1...0.4.0
[0.3.1]: https://github.com/HearthSim/joust/compare/0.3.0...0.3.1
[0.3.0]: https://github.com/HearthSim/joust/compare/0.2.0...0.3.0
[0.2.0]: https://github.com/HearthSim/joust/compare/0.1.0...0.2.0
