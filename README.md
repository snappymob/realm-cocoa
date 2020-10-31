**This is a custom fork of Realm by [Snappymob](https://www.snappymob.com) that fixes release build issues when including Realm as a dependency via Swift Package Manager (SPM). This fork based on `realm-cocoa v10.1.1` and `realm-core v10.0.0`.**

**You can use it by including `git@github.com:snappymob/realm-cocoa.git` as the package repository with the specific revision `e16b9ab26bad6e3c2d1f5eb8840a052dce3a37f3`. This package also has a dependency on a patched `realm-core` version: [https://github.com/snappymob/realm-core](https://github.com/snappymob/realm-core).**

**This fork may be useful if you are building for iOS in release mode or archiving and are getting build errors related to:**

`aligned deallocation function of type 'void (void *, std::align_val_t) noexcept' is only available on iOS 11 or newer`

---

![Realm](https://github.com/realm/realm-cocoa/raw/master/logo.png)

Realm is a mobile database that runs directly inside phones, tablets or wearables.
This repository holds the source code for the iOS, macOS, tvOS & watchOS versions of Realm Swift & Realm Objective-C.

## Features

* **Mobile-first:** Realm is the first database built from the ground up to run directly inside phones, tablets and wearables.
* **Simple:** Data is directly [exposed as objects](https://realm.io/docs/objc/latest/#models) and [queryable by code](https://realm.io/docs/objc/latest/#queries), removing the need for ORM's riddled with performance & maintenance issues. Most of our users pick it up intuitively, getting simple apps up & running in minutes.
* **Modern:** Realm supports relationships, generics, vectorization and Swift.
* **Fast:** Realm is faster than even raw SQLite on common operations, while maintaining an extremely rich feature set.

## Getting Started

Please see the detailed instructions in our docs to add [Realm Objective-C](https://realm.io/docs/objc/latest/#installation) _or_ [Realm Swift](https://realm.io/docs/swift/latest/#installation) to your Xcode project.

## Documentation

### Realm Objective-C

The documentation can be found at [realm.io/docs/objc/latest](https://realm.io/docs/objc/latest).  
The API reference is located at [realm.io/docs/objc/latest/api/](https://realm.io/docs/objc/latest/api/).

### Realm Swift

The documentation can be found at [realm.io/docs/swift/latest](https://realm.io/docs/swift/latest).  
The API reference is located at [realm.io/docs/swift/latest/api/](https://realm.io/docs/swift/latest/api/).

## Getting Help

- **Need help with your code?**: Look for previous questions with the[`realm` tag](https://stackoverflow.com/questions/tagged/realm?sort=newest) on Stack Overflow or [ask a new question](https://stackoverflow.com/questions/ask?tags=realm). For general discussion that might be considered too broad for Stack Overflow, use the [Community Forum](https://developer.mongodb.com/community/forums/tags/c/realm/9/realm-sdk).
- **Have a bug to report?** [Open a GitHub issue](https://github.com/realm/realm-cocoa/issues/new). If possible, include the version of Realm, a full log, the Realm file, and a project that shows the issue.
- **Have a feature request?** [Open a GitHub issue](https://github.com/realm/realm-cocoa/issues/new). Tell us what the feature should do and why you want the feature.

## Building Realm

In case you don't want to use the precompiled version, you can build Realm yourself from source.

Prerequisites:

* Building Realm requires Xcode 11.x or newer.
* If cloning from git, submodules are required: `git submodule update --init --recursive`.
* Building Realm documentation requires [jazzy](https://github.com/realm/jazzy)

Once you have all the necessary prerequisites, building Realm.framework just takes a single command: `sh build.sh build`. You'll need an internet connection the first time you build Realm to download the core binary.

Run `sh build.sh help` to see all the actions you can perform (build ios/osx, generate docs, test, etc.).

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for more details!

This project adheres to the [Contributor Covenant Code of Conduct](https://realm.io/conduct).
By participating, you are expected to uphold this code. Please report
unacceptable behavior to [info@realm.io](mailto:info@realm.io).

## License

Realm Objective-C & Realm Swift are published under the Apache 2.0 license.  
Realm Core is also published under the Apache 2.0 license and is available
[here](https://github.com/realm/realm-core).

**This product is not being made available to any person located in Cuba, Iran,
North Korea, Sudan, Syria or the Crimea region, or to any other person that is
not eligible to receive the product under U.S. law.**

## Feedback

**_If you use Realm and are happy with it, all we ask is that you please consider sending out a tweet mentioning [@realm](https://twitter.com/realm) to share your thoughts!_**

**_And if you don't like it, please let us know what you would like improved, so we can fix it!_**

![analytics](https://ga-beacon.appspot.com/UA-50247013-2/realm-cocoa/README?pixel)
