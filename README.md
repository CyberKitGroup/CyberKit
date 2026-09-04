# CyberKit

CyberKit is a backport of WebKit to older iOS.

This browser's first release in April 2023 was contemporaneous to Google's [Blink browser prototype](https://9to5google.com/2023/03/03/first-look-google-chrome-blink-engine-iphone-ios/). Although 9to5Google was able to run their browser in the iOS Simulator, upstream WebKit has allowed internal builds on the simulator have existed [since 2009](https://github.com/WebKit/WebKit/commit/8db218434d82310a70e950d3d8e843239603cd9a), and public support for builds on the simulator has existed [since 2014](https://github.com/WebKit/WebKit/commit/a51f89b11e3114cee49938fa15fdce22ecf43a8f). This project extended this work by being the first open source public project to provide an alternative browser engine for iOS on real hardware, successfully providing more usability under some conditions than the available stock iOS browsers, and provided a [technical overview](https://www.reddit.com/r/jailbreak/comments/1gdro8i/discussion_cyberkit_explained_a_technical_overview/) in 2024 to encourage more developers to work on developing browsers for iOS.

## Recent External Developments

Following in the footsteps of the 2012 tweak [Nitrous](https://www.iclarified.com/23608/nitrous-tweak-brings-the-nitro-javascript-engine-to-third-party-iphone-apps), the tweak [Polyfills](https://poomsmart.github.io/repo/depictions/polyfills.html) improves the functionality of stock WebKit by adding polyfills for newer JavaScript features. Due to political pressure in the EU, Apple released [BrowserEngineKit](https://developer.apple.com/documentation/browserenginekit) in the 2024 updates iOS 17.4 and iPadOS 18.0. This has assisted Minh Ton's 2026 release of [Reynard Browser](https://github.com/minh-ton/reynard-browser) based on Mozilla's Gecko.

In 2026, the project author of [WebKitPlayground](https://github.com/Lessica/WebKitPlayground) appears to have also experimented with WebKit reference implementations on iOS 16 to attempt systemwide replacement of WebKit on rootless versions.

Even if it has been out of necessity due to the lack of jailbreak releases for current iOS versions, CyberKit has helped pioneer the future of web browsers on iOS, and the release of other, less experimental, browsers has itself been a success of the project's goals — to demonstrate to the jailbreaking community it was possible and to document what it did along the way in hopes that others might follow in doing so. Thank you for your support of the project.

> ⚠️ **Note:** CyberKit development is on hiatus and more is still planned for the project.
>
> This is not an official deprecation notice, as per issue [#52](https://github.com/CyberKitGroup/CyberKit/issues/52).

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

You may find https://en.wikipedia.org/w/index.php?title=Safari_version_history&oldid=1186257925 beneficial to view correspondence between Safari version and iOS version.

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

On branches diverging before 1 May 2024 (before `safari-7619.1.12-branch`, see WebKit#27941), you must run `Tools/Scripts/configure-xcode-for-embedded-development` before 1st build or any time you reinstall/update Xcode or its SDKs. If you need the xpc.h header, you can get it from https://github.com/theos/templates/tree/f0fb942c4bb90ef331126e2b38257974b18bc895/ios/xpc_service/headers.

Even now, it still may be useful to replace or supplement Xcode's SDK with one with private headers from https://github.com/theos/sdks. Officially, support for building on the public SDK was introduced in late 2014:

* JavaScript and bmalloc first built on the public SDK on 13 August 2014 (see [8af367f](https://github.com/WebKit/WebKit/commit/8af367f75c293a992e8fe1f0cadb469f5dd5db68#diff-bddc5f89deea040f3ce0332f74fa684296ce2d959ca459a541677e0699081aa9)).
* WebCore first built on the public SDK on 17 September 2014 (see [226279b](https://github.com/WebKit/WebKit/commit/226279b118c82d9a6e389fa004f00c0c6a1e4fa4#diff-c38736d473f4d11bace7995198de5ceb035d65489d9a747abdb1587143927152)).

If a branch needs a newer configure script, you can grab one like this from the ref607 branch: `OUT_FILE=~/Desktop/conf; git show 62f80e2:Tools/Scripts/configure-xcode-for-ios-development > $OUT_FILE; chmod 755 $OUT_FILE; $OUT_FILE`

On branches diverging before 18 February 2016 (before `safari-602.1.32-branch`, see [bbc738d](https://github.com/WebKit/WebKit/commit/bbc738dcb37964a7811bbc57977797e564fb86a8)), you must build LLVM. You can do so as documented in [1f5b857](https://github.com/WebKit/WebKit/commit/1f5b8575a5439c4db6a4ac348a10bade4125ba0a):

If there are already precompiled binaries:
1. Obtain the precompiled binaries: `git checkout 1f5b857 WebKitLibraries/LLVMIncludesIOS9.tar.bz2 WebKitLibraries/LLVMLibrariesIOS9.tar.bz2`
2. Run the command `perl Tools/Scripts/copy-webkitlibraries-to-product-directory --llvm --sdk=iphoneos --use-llvm-includes=WebKitLibraries/LLVMIncludesIOS9.tar.bz2 --use-llvm-libraries=WebKitLibraries/LLVMLibrariesIOS9.tar.bz2 WebKitBuild/Debug-iphoneos`

If you wish to create precompiled binaries:
1. Attain the LLVM source code for an appropriately old release. For instance, from https://releases.llvm.org/download.html#3.6.2, choose http://llvm.org/releases/3.6.2/llvm-3.6.2.src.tar.xz.
    * You can confirm if the version you selected will work if adding the precompiled OS X headers to `HEADER_SEARCH_PATHS` in `LLVMForJSC.xcconfig` allows you to build the target `llvmForJSC`. Note this will not link on iOS, due to architecture issues.
2. If your CyberKit git repo is at `~/Documents/git/CyberKit`, expand this archive to `~/Documents/git/CyberKit/llvm`.
3. If your branch diverged before 8 October 2015, run `git checkout 1f5b857 Tools/Scripts/copy-webkitlibraries-to-product-directory`.
4. Theoretically, you can run the command `perl Tools/Scripts/copy-webkitlibraries-to-product-directory --llvm --sdk=iphoneos WebKitBuild/Debug-iphoneos`. This step may require changes.

You may be able to [ad hoc sign](https://akemi.ai/?page/how2asu) in some commits beginning 2 January 2024 without changes to CyberKit itself. Support for this is limited, but it may be the only method on some Apple Silicon VMs, as explained below.

You will build the "Everything up to CyberKit" target then the appropriate app.

## Development Environment Notes

Development is performed on macOS using Xcode. However, owing to the number of Xcode versions required, you may need to virtualize or emulate other macOS versions.

Xcode versions are chosen based on the date of commits and the iOS versions supported. The minimum deployment targets can be viewed at https://developer.apple.com/support/xcode/#minimum-requirements. Note that Xcode below 10 did not have a minimum deployment target, so running Xcode 9.4.1 on macOS Mojave should be the earliest Xcode you need to use for any branch.

If you need to emulate an Intel version of macOS on Apple Silicon, you can use UTM:
1. Obtain the requisite macOS install files via https://github.com/corpnewt/gibMacOS. If you don't get a full installer, you can use BaseSystem.dmg or RestoreImage.dmg instead.
2. Obtain the UTM configuration file from https://github.com/adespoton/utmconfigs.
3. Import the macOS install file you obtained in the UTM configuration and install macOS.

For later versions, you can dualboot or use the built-in virtualization framework. Note that Apple Silicon VMs require both the host and guest to be on, and have been created on, [macOS 15 or later](https://developer.apple.com/documentation/virtualization/using-icloud-with-macos-virtual-machines), in order to sign in to your Apple ID in Xcode due to entitlement issues.

If you are running under Intel, I previously had success with virtualizing older macOS versions with https://github.com/myspaghetti/macos-virtualbox but it is no longer maintained. You might consider dualbooting for performance reasons, or check out other methods like https://github.com/kholia/OSX-KVM.
