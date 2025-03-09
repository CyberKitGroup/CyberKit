# CyberKit

CyberKit is a backport of WebKit to older iOS.

## Installation
Please visit [the releases](https://github.com/UInt2048/CyberKit/releases).

## Official OS support & FAQ

Please visit the [CyberKit wiki](https://github.com/UInt2048/CyberKit/wiki).

## Development Branch History

You can clone just the current development branch with `git clone -b safari-7619.1.26.31-branch --single-branch https://github.com/UInt2048/CyberKit.git`

* [safari-7619.1.26.31-branch](https://github.com/UInt2048/CyberKit/tree/safari-7619.1.26.31-branch): 22 October 2024 - present (used in v0.0.9 nightly - present)
   * _Diverged 13 July 2024; built in Xcode 16.0_
* [safari-7617.1.4-branch](https://github.com/UInt2048/CyberKit/tree/safari-7617.1.4-branch): 9 December 2023 - 21 October 2024 (not used in release)
   * _Diverged 6 August 2023; built in Xcode 13.7_
* [safari-7616.1.27.211-branch](https://github.com/UInt2048/CyberKit/tree/safari-7616.1.27.211-branch): 2 October 2023 - 19 October 2024 (used in v0.0.9 alpha)
   * _Diverged 7 July 2023; built in Xcode 13.7_
* [safari-7616.1.12-branch](https://github.com/UInt2048/CyberKit/tree/safari-7616.1.12-branch): 11 May 2023 - 2 October 2023 (used in v0.0.7 alpha - v0.0.8 nightly)
    * _Diverged 22 April 2023; built in Xcode 14.3 before [688c678](https://github.com/UInt2048/CyberKit/commit/688c678f5a3204926f6e005f75f23433bf565153) (committed 31 July 2023), 13.7 starting with 688c678_
* [safari-7616.1.7-branch](https://github.com/UInt2048/CyberKit/tree/safari-7616.1.7-branch): 24 March 2023 - 11 May 2023 (used in v0.0.1 alpha - v0.0.6 alpha)
    * _Diverged 19 March 2023; built in Xcode 14.2 before [fa2170c](https://github.com/UInt2048/CyberKit/commit/fa2170c3604b4ccacbc4f2475f91c0638ac7a2a0) (committed 7 April 2023), 14.3 starting with fa2170c_
* [safari-7616.1.4-branch](https://github.com/UInt2048/CyberKit/tree/safari-7616.1.4-branch): 5 March 2023 - 24 March 2023 (not used in release)
    * _Diverged 25 February 2023; built in Xcode 14.2_
* [safari-7616.1.4pre-branch](https://github.com/UInt2048/CyberKit/tree/safari-7616.1.4pre-branch): 25 February 2023 - 5 March 2023 (not used in release)
    * _Diverged 25 February 2023; built in Xcode 14.2_
* [safari-7616.1.3-branch](https://github.com/UInt2048/CyberKit/tree/safari-7616.1.3-branch): 25 February 2023 (not used in release)
    * _Diverged 18 February 2023; built in Xcode 14.2_
* [safari-7615.1.15-branch](https://github.com/UInt2048/CyberKit/tree/safari-7615.1.15-branch): 31 January 2023 - 24 February 2023 (not used in release)
    * _Diverged 11 December 2022; built in Xcode 14.2_

## Reference Implementations
* [safari-607-branch](https://github.com/UInt2048/CyberKit/tree/safari-607-branch): 19 May 2023 - 21 July 2023 (used in v0.0.8 ref607)
    * _Diverged 7 January 2019; built in Xcode 11.7_
* [safari-608-branch](https://github.com/UInt2048/CyberKit/tree/safari-608-branch): 21 July 2023 - 22 July 2023 (used in v0.0.8 ref608)
    * _Diverged 15 July 2019; built in Xcode 11.7_
* [safari-609-branch](https://github.com/UInt2048/CyberKit/tree/safari-609-branch): 22 July 2023 - 24 July 2023 (used in v0.0.8 ref609)
    * _Diverged 3 January 2020; built in Xcode 11.7_
* [safari-610-branch](https://github.com/UInt2048/CyberKit/tree/safari-610-branch): 24 July 2023 - present (not used in release)
    * _Diverged 21 August 2020; built in Xcode 11.7_

## Building from Source
If building yourself, you may wish to use the version of Xcode used at the time to build the commit you are building.

On branches diverging before 1 May 2024 (that is, before `safari-7619.1.12-branch`, see WebKit#27941), you must run `Tools/Scripts/configure-xcode-for-embedded-development` before 1st build or any time you reinstall/update Xcode or its SDKs.

Beginning 2 January 2024, you can just [ad hoc sign](https://akemi.ai/?page/how2asu) with no changes to CyberKit itself which is especially convenient if you want to build in a macOS VM on Apple Silicon [where you can't sign in to your Apple ID](https://developer.apple.com/forums/thread/707682).

You will build the "Everything up to CyberKit" target then the appropriate app.

### Development Environment Notes

* Development is performed on macOS using Xcode.
* The rename script requires `gnu-sed` and `rename`, which can be obtained using Homebrew.
* Beginning with [fa2170c](https://github.com/UInt2048/CyberKit/commit/fa2170c3604b4ccacbc4f2475f91c0638ac7a2a0) [7 April 2023], Xcode 14.3 is used.
* Before this, Xcode 14.2 was used.
