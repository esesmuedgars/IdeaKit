<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 8 minute read

![Issue](https://img.shields.io/badge/issue-1.8-informational.svg)

Hey, hey!

Apple has yet to set the date to parade iPhone 13, but according to rumors, new devices will be announced on Tuesday, the 14<sup>th</sup> of September.

Happy learning!

## News

### New public betas are available

[Apple](https://twitter.com/Apple) has expanded its public beta program with software that was announced in early June during [WWDC21](https://developer.apple.com/wwdc21). Sign up to the [Apple Beta Software Program](https://beta.apple.com/sp/betaprogram), enroll your personal devices to access iOS 15, iPadOS 15, macOS Monterey, tvOS 15, and watchOS 8 public betas, and try out the latest features. Remember to back up all of your data before installing any beta software.

### Tax and price changes for applications and in-app purchases

[Apple](https://twitter.com/Apple) in their news [article](https://developer.apple.com/news/?id=o0uodgu7) notifies of decreased App Store prices of applications and in-app purchases (excluding auto-renewable subscriptions) in all territories that use the Euro currency, United Kingdom, and South Africa, however, increased prices in Georgia and Tajikistan.

### Retrieve and use current Game Center authentication certificate

[Apple](https://twitter.com/Apple) in their news [article](https://developer.apple.com/news/?id=stttq465) informs that a new certificate for server-based Game Center verification is available via the `publicKeyUrl` property of `fetchItems(forIdentityVerificationSignature:)` or `generateIdentityVerificationSignature` and cautions that the previous certificate is no longer available.
Please note, this root certificate issuer has been updated from Symantec Corporation to DigiCert, Inc. Validate that the new root certificate issuer is on your list of trusted certificate authorities.
Download the trusted root [certificate authority](https://knowledge.digicert.com/content/dam/digicertknowledgebase/attachments/code-signing/roots/digicert-trusted-root-g4.cer).

<!--more-->

## Swift challenge

Few possible solutions to Swift challenge No. 1:

```swift
// MARK: Solution A

private func spellOut() -> String {
    switch self {
    case 0: return "Zero"
    case 1: return "One"
    case 2: return "Two"
    case 3: return "Three"
    case 4: return "Four"
    case 5: return "Five"
    case 6: return "Six"
    case 7: return "Seven"
    case 8: return "Eight"
    case 9: return "Nine"
    default: return String()
    }
}

// MARK: Solution B

private func spellOut() -> String {
    let spelledOutNumbers = ["Zero",
                             "One",
                             "Two",
                             "Three",
                             "Four",
                             "Five",
                             "Six",
                             "Seven",
                             "Eight",
                             "Nine"]

    return spelledOutNumbers[self]
}

// MARK: Solution C

private func spellOut() -> String {
    let numberFormatter = NumberFormatter()
    numberFormatter.numberStyle = .spellOut

    guard let number = numberFormatter.string(from: NSNumber(value: self)) else {
        return String()
    }

    return number.capitalized
}

// MARK: Solution D

private func spellOut() -> String {
    let number = NumberFormatter.localizedString(from: NSNumber(value: self), number: .spellOut)

    return number.capitalized
}
```

Followed by Swift challenge No. 2:

```swift
/**
Survey if the file at path exists or not.
Implement `checkIfFileExists(_:)` method.
 */

func checkIfFileExists(_ fileURL: URL) -> Bool {
    <#Bool#>
}
```

<!--
If you are unsure if the URL exists or not before opening it, just go ahead and open it as checking first will duplicate the amount of work the file system needs to perform.
However, if you do not need to open the file but verify if it exists using URL's check resource is reachable will work for the vast majority of URLs and is recommended over getting a file system path and then checking with the file manager if the file exists.

```swift
func checkIfFileExists(_ fileURL: URL) -> Bool {
    <#Bool#>
}
```
-->

## Fundamentals

### A pragmatic guide to unit testing

Unit testing facilitates changes and simplifies integration. In addition to giving confidence when refactoring code by confirming module works after introduced changes, executing tests before every commit saves you from accidentally committing a version that doesn’t compile. [Marina Gornostaeva](https://twitter.com/hybridcattt) in her [article](https://hybridcattt.com/blog/start-testing-pragmatic-guide) covers how to configure the project for testing, differentiate between different kinds of tests, and approach seemingly untestable code.

### Copy-on-assignment and copy-on-write semantics

It is crucial to understand memory management to avoid performance issues and crashes. Read an [article](https://aymanmoo.medium.com/copy-on-assignment-vs-copy-on-write-in-swift-c3016b343d06) where [Ayman Fayez](https://www.linkedin.com/in/ayman-fayez-7ab174156) illustrates the difference between copy-on-assignment and copy-on-write semantics.

### Implementing feature flags in iOS

Feature toggles are used to enable or disable features during runtime and allow features to be tested even before they are completed and ready for release. [Aryaman Sharda](https://twitter.com/aryamansharda) wrote an [article](https://digitalbunker.dev/2021/07/23/implementing-feature-flagging-in-ios) explaining the benefits of feature flags as well as exhibiting how to implement them.

### Error handling in Swift

[Sarun Wongpatcharapakornand](https://twitter.com/sarunw) covers the majority of scenarios you could encounter while catching errors in an [article](https://sarunw.com/posts/different-ways-to-catch-throwing-errors-in-swift).

## Tutorials

### Apple iOS developer tutorials

[Apple](https://twitter.com/Apple) offers [tutorials](https://developer.apple.com/tutorials/app-dev-training) to learn the basics of Xcode, `SwiftUI`, and `UIKit` to create iOS applications.

### Dependency injection in iOS

[Mina Ashna](https://twitter.com/minaashna) created a [tutorial](https://www.raywenderlich.com/22203552-resolver-for-ios-dependency-injection-getting-started) educating how to use the [Resolver](https://github.com/hmlongco/Resolver) framework to implement dependency injection in SwiftUI iOS applications to achieve readable and maintainable codebases. She also goes over related topics such as imitating dependencies for unit testing and dependency inversion principle.

### 3D programming for iOS using `SceneKit`

Visit a [tutorial](https://www.raywenderlich.com/23483920-scenekit-3d-programming-for-ios-getting-started) by [Keegan Rush](https://twitter.com/rushkeegan) if you would like to learn the fundamentals of 3D programming, lightings influence on scenes, and how to modify the user's perspective with cameras and constraints using the [SceneKit](https://developer.apple.com/documentation/scenekit) framework.

## Enhanced programming

### Grouping tests into substeps with activities

[Apple](https://twitter.com/Apple) provides an [article](https://developer.apple.com/documentation/xctest/activities_and_attachments/grouping_tests_into_substeps_with_activities) describing how to create named activities within lengthy test methods, such as UI tests or integration tests, to simplify test reports.

### Authenticating users with a cryptographic token

[Apple](https://twitter.com/Apple) has an [article](https://developer.apple.com/documentation/cryptotokenkit/authenticating_users_with_a_cryptographic_token) demonstrating how to grant access to the keychain by creating a smart card macOS application extension.

### Building a Safari application extension

An [article](https://developer.apple.com/documentation/safariservices/safari_app_extensions/building_a_safari_app_extension) by [Apple](https://twitter.com/Apple) dictates the steps to build Safari Extension delivered as a part of a macOS application. When a user runs an application for the first time, its extension immediately becomes available in Safari.

### Placeholder view in `SwiftUI`

Previously, you might have resolved to depend on Facebook's [Shimmer](https://github.com/facebookarchive/Shimmer) library for an unobtrusive loading indicator functionality. [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) wrote an [article](https://sarunw.com/posts/make-placeholder-view-in-swiftui-with-redacted) sharing that `SwiftUI` views have a simple API to redact content in a way to be used as a placeholder before the actual content is loaded.

### Why did we got rid of most dependencies?

[Chris Eidhof](https://twitter.com/chriseidhof) in his [article](https://chris.eidhof.nl/post/fewer-dependencies) shared his team's reasons for fewer dependencies in their website written in Swift.

### Starter workflows with Xcode Cloud

[Alex Logan](https://twitter.com/swiftyalex) wrote an [article](https://www.alexanderlogan.co.uk/wwdc21/004-xcode-cloud) escorting readers through a process of creating a workflow to distribute his application's beta version using Testflight on successful test completion with [Xcode Cloud](https://developer.apple.com/documentation/Xcode/Xcode-Cloud).

### Architecting applications for scalability and build speed

Watch a [presentation](https://www.youtube.com/watch?v=sZuI6z8qSmc) by [Bruno Rocha](https://twitter.com/rockbruno_) where he delivers a speech about developing a scalable application that has hundreds of features while preserving a good degree of flexibility and swift build times.

### `AppKit` framework is done

[Alex Grebenyuk](https://twitter.com/a_grebenyuk) crafted an [article](https://kean.blog/post/appkit-is-done) about building a [Pulse](https://kean.blog/pulse) (powerful, [open-source](https://github.com/kean/Pulse) logging system for Apple platforms) application for macOS entirely in `SwiftUI`. Alex highlights some of the features and their implementations, in addition to supplying some valuable tips for working with `SwiftUI`.

### Lessons from indie application developer with over 50 million downloads

Listen to the [Sub Club Podcast](https://subclub.co) [episode](https://subclub.co/episode/david-smith-widgetsmith-lessons-from-50-million-downloads) with [David Smith](https://twitter.com/_davidsmith) as he discusses his journey and what he has learned from his multiple successful and, eight times more, unsuccessful applications.

### Using Swift in React Native application

[Akinn Rosa](https://twitter.com/akinncar) wrote an [article](https://dev.to/akinncar/how-to-use-swift-in-your-react-native-app-46mj) reporting how to create a bridge between Swift and Objective-C code and then exposing native Objective-C methods to React Native with yet another bridge (between Objective-C and JavaScript).

### Defining dynamic colors in Swift

Learn how to programmatically create colors that adapt to the environment using either `SwiftUI` or `UIKit` in an [article](https://www.swiftbysundell.com/articles/defining-dynamic-colors-in-swift) by [John Sundell](https://twitter.com/johnsundell).

### Serialization for backward compatibility

[Dekel Avrahami](https://www.linkedin.com/in/dekel-avrahami-b999a1146) shares with his team's gained experience from building [Facetune Video by Lightricks](https://apps.apple.com/us/app/facetune-video-by-lightricks/id1505478179) application and discoveries they made about serialization with backward compatibility in mind in an [article](https://medium.com/@lightricks-tech-blog/backwards-compatibility-in-swift-990d3ca05624).

### Using throwing properties to catch errors

In an [article](https://www.avanderlee.com/swift/throwing-properties), [Antoine van der Lee](https://twitter.com/twannl) guides readers through newly added improvement to Swift 5.5 — throwing properties.

### Setting default values for `UserDefaults`

[Sarun Wongpatcharapakornand](https://twitter.com/sarunw) wrote an [article](https://sarunw.com/posts/setting-default-value-for-nsuserdefaults) bringing to our attention that it isn't necessary to equate value to `nil` to determine if you must set initial value, instead use the `UserDefaults` instance method to add default values of the specified dictionary to the registration domain.

### Dependency injection using the latest Swift features

Dependency injection is a software design pattern that is a commonly used technique that enhances code reusability and  simplifies testing by allowing to substitute data. Read an [article](https://www.avanderlee.com/swift/dependency-injection) by [Antoine van der Lee](https://twitter.com/twannl) where he proposes an alternative strategy for establishing dependency injection into a codebase.

### Backporting new features with `@_alwaysEmitIntoClient`

[Federico Zanetello](https://twitter.com/zntfdr) in his [article](https://www.fivestars.blog/articles/alwaysEmitIntoClient) educates how binary frameworks can make additive changes to their APIs while remaining binary-compatible with earlier versions of operating systems using `@_alwaysEmitIntoClient`.

## Tools

### AI-powered code assistant

[GitHub Copilot](https://copilot.github.com) is available as a Visual Studio Code extension. It uses the provided context to synthesizes suggestions for whole lines or entire functions to match. During the technical preview of GitHub Copilot, access is limited to a small group of testers. Join the [waitlist](https://github.com/features/copilot/signup) if you would like to receive a chance to try it out.
Additionally, a hilarious remark [Marcin Krzyzanowski](https://twitter.com/krzyzanowskim) made in his Twitter [post](https://twitter.com/krzyzanowskim/status/1410320595221463044) made me laugh, check it out!

### `DocC` archived and analyzed

[Helge Heß](https://twitter.com/helje5) wrote an [article](http://www.alwaysrightinstitute.com/docz) about his investigation of `DocC` produced documentation archive. He found that the `DocC` archive doesn't only contain a version of the documentation suitable for the Xcode Documentation Viewer but also generated documentation as raw, parseable data, in a hierarchy of JSON files and images.

### Swift Package Index

Selecting the proper dependencies is about more than just finding code that does what you need. Are the libraries you are choosing well maintained? How long have they been in development? Are they well tested? Picking high-quality packages is challenging, and the [Swift Package Index](https://swiftpackageindex.com) (a search engine for packages that support the Swift Package Manager) helps you make better decisions about your dependencies.

### Benchmarking Swift code with Attabench framework and GUI macOS application

If you too have been benchmarking the speed of code by adding multiple timestamps using `Date` object and calculating the time difference, [Bruno Rocha](https://twitter.com/rockbruno_) in his [article](https://swiftrocks.com/benchmarking-swift-code-properly-with-attabench) suggests using the [Attabench](https://github.com/attaswift/Attabench) framework that is accompanied by a GUI macOS application for microbenchmarking. The tool compiles your application in the release configuration and repeatedly performs the same operation on random data of various sizes, while continuously charting the results which makes it ideal for seeing your algorithm's performance at a glance.

## Tips

### Manually adding existing certificates to the fastlane match

Fastlane match stores certificates, private keys, and provisioning profiles in a separate git repository, Google Cloud, or Amazon S3 to sync them across your development team. Sharing a single code signing identity simplifies code signing setup and prevents code signing issues. [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) in his [article](https://sarunw.com/posts/how-to-manually-add-existing-certificates-to-fastlane-match) takes us through how to import an existing certificate into the match repository.

### File extensions in Xcode

[Douglas Hill](https://twitter.com/qdoug) in his Twitter [post](https://twitter.com/qdoug/status/1411948641292521478) demonstrates that in Xcode 13 developers can hide inferable file extensions.

### Making debugger console output stand out

[Dominik Hauser](https://twitter.com/dasdom) in his [article](https://dasdom.dev/posts/changing-color-for-debugger-output) demonstrates how to make debugger console output easier to find by customizing its color.

### Avoiding retain cycles in `Combine`

[Eneko Alonso](https://twitter.com/eneko) in his Twitter [post](https://twitter.com/eneko/status/1416143468070465537) shares an example of the retain cycle remedy while working with `Combine` or any other escaping closure.

### When should you use a throwing initializer?

When constructing an object using a failable initializer, the result is an optional that either contains the object (when the initialization succeeded) or contains `nil` (when the initialization failed). [Vincent Pradeilles](https://twitter.com/v_pradeilles) in his YouTube [video](https://www.youtube.com/watch?v=bWWj8zgd--c) briefs that throwing initializer can be used to convey failure information.

### Assert xib files exist

In case a project you are working on relies a lot on xib files, [Vincent Pradeilles](https://twitter.com/v_pradeilles) in his YouTube [video](https://www.youtube.com/watch?v=qowbAhsDuO0) encourages you to implement tests that validate xib file for the specified class is in the bundle.

<br>
<p align="center">
<img width="35%" alt="Curators" src="curators.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit the <a href="https://github.com/esesmuedgars/IdeaKit/blob/issue4/README.md">previous issue</a>!
<br>
<br>
Found a topic insightful? You can add your comments and open a discussion using the comment section below.
<br>
Help others improve their Swift knowledge by liking and sharing this post.
<br>
<br>
Reach out in case you would like to contribute or spot any errors! Feedback and suggestions are also welcome.
<br>
<br>
Subscribe to the <a href="https://blog.accenture.com/design">Baltic Interactive blog</a> and follow the <a href="https://web.yammer.com/main/groups/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI1Nzg0ODAwNDYwOCJ9/all">Riga Interactive Yammer community</a> for further insightful content!
</p>
