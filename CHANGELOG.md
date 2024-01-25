# Change Log
Important changes to Instructions will be documented in this file.
Instructions follows [Semantic Versioning](http://semver.org/).

## [2.3.0](https://github.com/ephread/Instructions/releases/tag/2.3.0)
Released on 2023-09-13.

### Added
- Support for Xcode 15 / Swift 5.9

### Changed
- Changed `FlowManager.currentIndex` to be public get, private set [#298]

[#298]: https://github.com/ephread/Instructions/issues/298

## [2.2.0](https://github.com/ephread/Instructions/releases/tag/2.2.0)
Released on 2022-05-25.

### Added
- Emulate coach mark skipping when stopping the flow from code [#265]
- Expose Instructions' root window [#268]
- Add a new delegate method triggered when tapping a coach mark [#185]
- Add new position options for the default coach mark views' "next" label [#273]

[#265]: https://github.com/ephread/Instructions/issues/265
[#268]: https://github.com/ephread/Instructions/issues/268
[#185]: https://github.com/ephread/Instructions/issues/185
[#273]: https://github.com/ephread/Instructions/issues/273

## [2.1.1](https://github.com/ephread/Instructions/releases/tag/2.1.1)
Released on 2021-11-16.

### Fixed
- Fix [#258] - Fix documentation comments in CoachMarkHelper
- Fix [#259] - Quick fix regarding no cutout area use
- Fix [#261] - Fix iOS 15 Layout for CoachMarkBodyDefaultView

[#258]: https://github.com/ephread/Instructions/issues/258
[#259]: https://github.com/ephread/Instructions/issues/259
[#261]: https://github.com/ephread/Instructions/issues/261

## [2.1.0](https://github.com/ephread/Instructions/releases/tag/2.1.0)
Released on 2021-06-06.

### Added
- New helper methods to:
    - deal with cutout paths that aren't anchored to a specific view;
    - update all coach mark properties at once.

## [2.0.1](https://github.com/ephread/Instructions/releases/tag/2.0.1)
Released on 2021-02-07.

### Fixed
- Fix [#229] - Blur Effect not working when used with .controller context
- Fix [#247] - Fix for Mac Catalyst
- Fix [#248] - Update README.md
- Fix [#250] - Fix Spelling Mistakes

[#229]: https://github.com/ephread/Instructions/issues/229
[#247]: https://github.com/ephread/Instructions/issues/247
[#248]: https://github.com/ephread/Instructions/issues/248
[#250]: https://github.com/ephread/Instructions/issues/250

### Changed
- Moved all error messages into their own structs.

## [2.0.0](https://github.com/ephread/Instructions/releases/tag/2.0.0)
Released on 2020-05-14.

### Fixed
- Fix [#205] - Safe area insets ignored by coach mark layout system
- Fix [#231] - Support iOS 13's `WindowScene`
- Fix incorrect window bounds while multitasking on iPad

[#205]: https://github.com/ephread/Instructions/issues/205
[#231]: https://github.com/ephread/Instructions/issues/231

### Changed
- Move from Travis to Github Actions
- Refactor example project
- Change return type in `coachMarkViewsAt` to enforce the type through protocol
  composition
- Unify the naming conventions for exposed properties

### Added
- Full dark mode support
- Customizable default Coachmark
- Support of Swift Package Manager
- Let overlay forward touch events with a new option [#212]

[#212]: https://github.com/ephread/Instructions/issues/212

### Removed
- Asset Bundles

## [1.4.0](https://github.com/ephread/Instructions/releases/tag/1.4.0)
Released on 2019-05-04.

### Fixed
- Fix [#218] - Division by zero during layout phase

### Changed
- Turn runtime checks into compile time checks (protocol composition)
- Improve error message when `numberOfCoachMarks <= 0`

### Removed
- Remove deprecated methods
- Remove LFS in snapshot submodule

[#218]: https://github.com/ephread/Instructions/issues/218

## [1.3.1](https://github.com/ephread/Instructions/releases/tag/1.3.1)
Released on 2019-10-05.

### Fixed
- Fix [#204] - `spec.swift_version` set to 5 instead of 5.0

[#204]: https://github.com/ephread/Instructions/issues/204

## [1.3.0](https://github.com/ephread/Instructions/releases/tag/1.3.0)
Released on 2019-04-11.

### Fixed
- Fix [#187] - Wrong index reported by `didHide`

### Added
- Add previous coach mark functionality ([#182])

### Changed
- Migrated to Swift 5

[#182]: https://github.com/ephread/Instructions/issues/182
[#187]: https://github.com/ephread/Instructions/issues/187

## [1.2.2](https://github.com/ephread/Instructions/releases/tag/1.2.2)
Released on 2018-12-06.

## [1.2.1](https://github.com/ephread/Instructions/releases/tag/1.2.1)
Released on 2018-12-05. ⚠️ Defective version

### Fixed
- Fix [#160] - CoachMark misplaced on iPad

### Added
- Add support for coach marks placed over cutout paths. ([#152])
- Add support for presentation contexts. ([#84])
- Add support for animated coach marks.

### Changed
- Change willSHow and didShow coachmark delegate methods to discriminate between
  different configuration changes.

[#84]: https://github.com/ephread/Instructions/issues/84
[#152]: https://github.com/ephread/Instructions/issues/152
[#160]: https://github.com/ephread/Instructions/issues/160

## [1.2.0](https://github.com/ephread/Instructions/releases/tag/1.2.0)
Released on 2018-06-04.

### Changed
- Migrated to Swift 4.1 (PR [#159])

### Fixed
- Fix [#163] - Silly weak modifier in protocol property.
- Fix [#166] - `UIApplication.networkActivityIndicatorVisible` called from background queue.
- Fix [#90] - Crash occurring infrequently if the view controller is dismissed too quickly. (PR [#161])

### Added
- Add supports for ornaments on the overlay.
- Add (partially implemented by [#131]).
- Add status bar style customization (PR [#164], PR [#139]).
- Add proper support for iPhone X.

[#90]: https://github.com/ephread/Instructions/issues/90
[#131]: https://github.com/ephread/Instructions/pull/131
[#139]: https://github.com/ephread/Instructions/pull/139
[#159]: https://github.com/ephread/Instructions/pull/159
[#161]: https://github.com/ephread/Instructions/pull/161
[#163]: https://github.com/ephread/Instructions/issues/163
[#164]: https://github.com/ephread/Instructions/pull/164
[#166]: https://github.com/ephread/Instructions/issues/166

## [1.1.0](https://github.com/ephread/Instructions/releases/tag/1.1.0)
Released on 2017-08-09.

### Added
- Add a new delegate method to handle tap on the overlay ([#100]).

### Fixed
- Fix [#127] & [#132] by retrieve configuration from parent controller.

[#100]: https://github.com/ephread/Instructions/issues/100
[#127]: https://github.com/ephread/Instructions/issues/127
[#132]: https://github.com/ephread/Instructions/issues/132

## [1.0.0](https://github.com/ephread/Instructions/releases/tag/1.0.0)
Released on 2017-07-05.

No changes.

## [1.0.0-beta.1](https://github.com/ephread/Instructions/releases/tag/1.0.0-beta.1)
Released on 2017-06-04.

### Added
- Support for Swift 3.
- Ability to choose the `UIWindowLevel` for the overlay.
- Ability to prepare Instructions for frame changes manually.

### Changed
- Renamed a number of methods to make them conform to the [API Design Guidelines]

### Fixed
- Fix [#74] possible build failure on Carthage due to unneeded build dependency (PR [#76]).
- Fix inability to detect if user has skipped the flow (PR [#81]).
- Fix blur effect on iOS 10 [#80].

[API Design Guidelines]: https://swift.org/documentation/api-design-guidelines/
[#74]: https://github.com/ephread/Instructions/issues/74
[#76]: https://github.com/ephread/Instructions/issues/76
[#81]: https://github.com/ephread/Instructions/issues/81
[#80]: https://github.com/ephread/Instructions/issues/80

## [0.5.0](https://github.com/ephread/Instructions/releases/tag/0.5.0)
Released on 2016-09-06.

### Fixed
- Fix [#63] dataSource methods wrongly called during idle state.
- Fix [#58] inability to restart the flow.

[#63]: https://github.com/ephread/Instructions/issues/63
[#58]: https://github.com/ephread/Instructions/issues/58

### Changed
- Deprecate calling helper methods directly from `CoachMarkController`, methods are now available through the `CoachMarkController.helper` object.
- Deprecate calling flow state properties directly from `CoachMarkController`, properties are now available through the `CoachMarkController.flow` object.
- Deprecate settings overlay parameters directly from `CoachMarkController`, properties are now available through the `CoachMarkController.overlay` object.

### Added
- Full support of App Extensions.

## [0.4.3](https://github.com/ephread/Instructions/releases/tag/0.4.3)
Released on 2016-08-10.

### Fixed
- Fix [#57], [#60] – Duplicated coach marks on rotation.
- Fix crash occurring on index 0 when `coachMarkWillLoadForIndex` returns false.

[#57]: https://github.com/ephread/Instructions/issues/57
[#60]: https://github.com/ephread/Instructions/issues/60

## [0.4.2](https://github.com/ephread/Instructions/releases/tag/0.4.2)
Released on 2016-07-07.

### Fixed
- Fix an issue where the `skipped` parameter was not set properly on `didFinishShowingAndWasSkipped`.
- Fix most timing issues, leading to multiple coach marks being displayed.

## [0.4.1](https://github.com/ephread/Instructions/releases/tag/0.4.1)
Released on 2016-07-04.

### Removed
- Remove partial support for App Extensions (will be added back in full for 0.5.0).

### Fixed
- Fix a bug caused by always-enabled touch inside the cutout path.
- Fix a crash occurring during background fetches.
- Fix the shift of cutout paths occurring when toggling the in-call status bar.

### Changed
- Change completion method signature in delegate; it now provides a boolean notifying whether the flow was skipped by the user.

## [0.4.0](https://github.com/ephread/Instructions/releases/tag/0.4.0)
Released on 2016-02-21.

### Changed
- Change `datasource` to `dataSource`.

### Added
- Add ability to manually specify where the coach should sit.
- Add ability to pilot the transitions/the flow from the code.
- Add ability to skip coach marks.

## [0.3.0](https://github.com/ephread/Instructions/releases/tag/0.3.0)
Released on 2015-10-31.

### Added
- Add ability to skip a tour.

## [0.2.1](https://github.com/ephread/Instructions/releases/tag/0.2.1)
Released on 2015-10-03.

### Fixed
- Wrap unavailable method into `if #available` block.

## [0.2.0](https://github.com/ephread/Instructions/releases/tag/0.2.0)
Released on 2015-10-03. ⚠️ Defective version

### Added
- Add full size transition support
- Add full right-to-left language support

## [0.1.2](https://github.com/ephread/Instructions/releases/tag/0.1.2)
Released on 2015-10-01.

### Added
- Add Carthage support

## [0.1.1](https://github.com/ephread/Instructions/releases/tag/0.1.1)
Released on 2015-10-01.

### Added
- Add CocoaPods support

## [0.1.0](https://github.com/ephread/Instructions/releases/tag/0.1.0)
Released on 2015-10-01.

### Added
- Initial release of Instructions.
