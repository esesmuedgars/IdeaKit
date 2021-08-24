<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.8-informational.svg)

Hey, hey!

Apple has yet to set a date to parade iPhone 13, but September is the traditional launch month.
The 14<sup>th</sup> of September. ⚠️

Happy learning! ⚠️

## News

### New public betas are available

[Apple](https://twitter.com/Apple) has expanded its public beta program with software that was announced in early June during [WWDC21](https://developer.apple.com/wwdc21). Sign up to the [Apple Beta Software Program](https://beta.apple.com/sp/betaprogram), enroll your personal devices to access iOS 15, iPadOS 15, macOS Monterey, tvOS 15, and watchOS 8 public betas, and try out the latest features. Remember to back up all of your data before installing any beta software.

### Tax and price changes for applications and in-app purchases

[Apple](https://twitter.com/Apple) in their news [article](https://developer.apple.com/news/?id=o0uodgu7) notify of decreased App Store prices of applications and in-app purchases (excluding auto-renewable subscriptions) in all territories that use the Euro currency, United Kingdom, and South Africa, however increased prices in Georgia and Tajikistan.

### Retrieve and use current Game Center authentication certificate

[Apple](https://twitter.com/Apple) in their news [article](https://developer.apple.com/news/?id=stttq465) informs that a new certificate for server-based Game Center verification is available via the `publicKeyUrl` property of `fetchItems(forIdentityVerificationSignature:)` or `generateIdentityVerificationSignature` and cautions that previous certificate is no longer available.
Please note, this root certificate issuer has been updated from Symantec Corporation to DigiCert, Inc. Validate that the new root certificate issuer is on your list of trusted certificate authorities.
Download the trusted root [certificate authority](https://knowledge.digicert.com/content/dam/digicertknowledgebase/attachments/code-signing/roots/digicert-trusted-root-g4.cer).

<!--more-->

## Swift challenge

Swift challenge No. 1:

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

Swift challenge No. 2:

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
If you are unsure if URL exists or not before opening it, just go ahead and open it as checking first will dublicate the amount of work the file system needs to perform.
However, if you do not need to open the file but verfity if it exists using URL's check resource is reachable will work for vast majority of URLs and is recommended over getting a file system path and then checking with the file manager if the file exists.

```swift
func checkIfFileExists(_ fileURL: URL) -> Bool {
    <#Bool#>
}
```
-->

## Fundamentals

### Pragmatic guide to unit testing

Unit testing facilitates changes and simplifies integration. In addition to giving confidence when refactoring code by confirming module works after introduced changes, executing tests before every commit saves you from accidentally committing a version that doesn’t compile. [Marina Gornostaeva](https://twitter.com/hybridcattt) in her [article](https://hybridcattt.com/blog/start-testing-pragmatic-guide) covers how to configure project for testing, differentiate between different kinds of tests, and approach seemingly untestable code.

### Copy-on-assignment and copy-on-write semantics

It is crucial to understand memory management to avoid performance issues and crashes. Read an [article](https://aymanmoo.medium.com/copy-on-assignment-vs-copy-on-write-in-swift-c3016b343d06) where [Ayman Fayez](https://www.linkedin.com/in/ayman-fayez-7ab174156) illustrates the difference between copy-on-assignment and copy-on-write semantics.

### Implementing feature flags in iOS

Feature toggles are used to enable or disable features during runtime and allow features to be tested even before they are completed and ready for release. [Aryaman Sharda](https://twitter.com/aryamansharda) wrote an [article](https://digitalbunker.dev/2021/07/23/implementing-feature-flagging-in-ios) explaining the benefits of feature flags as well as exhibiting how to implement them.

## Tutorials

### Apple iOS Developer course ⚠️

[Apple](https://twitter.com/Apple) offers [tutorials](https://developer.apple.com/tutorials/app-dev-training/?utm_source=swiftlee&utm_medium=swiftlee_weekly&utm_campaign=issue_71) on both `SwiftUI` and `UIKit`

### Resolver for iOS Dependency Injection ⚠️

[tutorial](https://www.raywenderlich.com/22203552-resolver-for-ios-dependency-injection-getting-started) by (she/her) [Mina Ashna](https://twitter.com/minaashna)

### SceneKit 3D Programming for iOS ⚠️

[tutorial](https://www.raywenderlich.com/23483920-scenekit-3d-programming-for-ios-getting-started) by [Keegan Rush](https://twitter.com/rushkeegan)

## Enhanced programming

### Grouping Tests into Substeps with Activities ⚠️

[Apple](https://twitter.com/Apple) provides an [article](https://developer.apple.com/documentation/xctest/activities_and_attachments/grouping_tests_into_substeps_with_activities)

### Authenticating Users with a Cryptographic Token ⚠️

[Apple](https://twitter.com/Apple) provides an [article](https://developer.apple.com/documentation/cryptotokenkit/authenticating_users_with_a_cryptographic_token)

### Building a Safari App Extension ⚠️

[Apple](https://twitter.com/Apple) provides an [article](https://developer.apple.com/documentation/safariservices/safari_app_extensions/building_a_safari_app_extension)

### Placeholder view in `SwiftUI` ⚠️

Previously used, since then archived, Facebook's [Shimmer](https://github.com/facebookarchive/Shimmer) library
[article](https://sarunw.com/posts/make-placeholder-view-in-swiftui-with-redacted) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)

### Why we got rid of most dependencies ⚠️

[article](https://chris.eidhof.nl/post/fewer-dependencies) by [Chris Eidhof](https://twitter.com/chriseidhof)

### Starter Workflows with Xcode Cloud ⚠️

[article](https://www.alexanderlogan.co.uk/wwdc21/004-xcode-cloud) by [Alex Logan](https://twitter.com/swiftyalex)

### Preparing for Growth: Architecting Giant Apps for Scalability and Build Speed ⚠️

watch [presentation](https://www.youtube.com/watch?v=sZuI6z8qSmc) by [Bruno Rocha](https://twitter.com/rockbruno_)

### AppKit ⚠️

[article](https://kean.blog/post/appkit-is-done) about building [Pulse](https://kean.blog/pulse) (free, [open-source](https://github.com/kean/Pulse), powerful logging system for Apple Platforms) by [Alex Grebenyuk](https://twitter.com/a_grebenyuk)

### Lessons from indie application developer with over 50 million downloads ⚠️

listen to [podcast](https://subclub.co/episode/david-smith-widgetsmith-lessons-from-50-million-downloads) where [David Smith](https://twitter.com/_davidsmith)

### Using Swift in React Native application ⚠️

[article](https://dev.to/akinncar/how-to-use-swift-in-your-react-native-app-46mj) by [Akinn Rosa](https://twitter.com/akinncar)

### Defining dynamic colors in Swift ⚠️

[article](https://www.swiftbysundell.com/articles/defining-dynamic-colors-in-swift) by [John Sundell](https://twitter.com/johnsundell)

### Serialization for Backward Compatibility in Swift ⚠️

[article](https://medium.com/@lightricks-tech-blog/backwards-compatibility-in-swift-990d3ca05624) by [Dekel Avrahami](https://www.linkedin.com/in/dekel-avrahami-b999a1146)

### How to use throwing properties to catch failures in Swift ⚠️

[article](https://www.avanderlee.com/swift/throwing-properties) by [Antoine van der Lee](https://twitter.com/twannl)
Alternatively, [article](https://sarunw.com/posts/different-ways-to-catch-throwing-errors-in-swift) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)

### Setting default values for `UserDefaults` ⚠️

[article](https://sarunw.com/posts/setting-default-value-for-nsuserdefaults) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)

### Dependency Injection in Swift using latest Swift features ⚠️

[article](https://www.avanderlee.com/swift/dependency-injection) by [Antoine van der Lee](https://twitter.com/twannl)

### Benchmarking Swift Code Properly with Attabench ⚠️

[article](https://swiftrocks.com/benchmarking-swift-code-properly-with-attabench) by [Bruno Rocha](https://twitter.com/rockbruno_)

### Backporting new features with `@_alwaysEmitIntoClient` ⚠️

[article](https://www.fivestars.blog/articles/alwaysEmitIntoClient) by [Federico Zanetello](https://twitter.com/zntfdr)

## Tools

### AI powered code assistant

[GitHub Copilot](https://copilot.github.com) is available as a Visual Studio Code extension. It uses the provided context to synthesizessuggestions for whole lines or entire functions to match. During the technical preview of GitHub Copilot, access is limited to a small group of testers. Join the [waitlist](https://github.com/features/copilot/signup) if you would like to receive a chance to try it out.
Additionaly, have a laught at a hilarious remark [Marcin Krzyzanowski](https://twitter.com/krzyzanowskim) made in his Twitter [post](https://twitter.com/krzyzanowskim/status/1410320595221463044) .

### `DocC` archived and analyzed

[Helge Heß](https://twitter.com/helje5) wrote an [article](http://www.alwaysrightinstitute.com/docz) about his investigation of `DocC` produced documentation archive. He found that `DocC` archive doesn't only contain a version of the documentation suitable for the Xcode Documentation Viewer but also generated documentation as a raw, parseable data, in a hierarchy of JSON files and images.

### Swift Package Index

Selecting the proper dependencies is about more than just finding code that does what you need. Are the libraries you are choosing well maintained? How long have they been in development? Are they well tested? Picking high-quality packages is challenging, and the [Swift Package Index](https://swiftpackageindex.com) (a search engine for packages that support the Swift Package Manager) helps you make better decisions about your dependencies.

## Tips

### Manually adding existing certificates to the fastlane match

Fastlane match stores certificates, private keys, and provisioning profiles in a separate git repository, Google Cloud, or Amazon S3 to sync them across your development team. Sharing a single code signing identity simplifies code signing setup and prevents code signing issues. [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) in his [article](https://sarunw.com/posts/how-to-manually-add-existing-certificates-to-fastlane-match) takes us through how to import an existing certificate into the match repository.

### File extensions in Xcode

[Douglas Hill](https://twitter.com/qdoug) in his Twitter [post](https://twitter.com/qdoug/status/1411948641292521478) demonstrates that in Xcode 13 developers can hide inferable file extensions.

### Making debugger console output stand out

[Dominik Hauser](https://twitter.com/dasdom) in his [article](https://dasdom.dev/posts/changing-color-for-debugger-output) demonstrates how to make debugger console output easier to find by customizing its color.

### Avoiding retain cycles in `Combine`

[Eneko Alonso](https://twitter.com/eneko) in his Twitter [post](https://twitter.com/eneko/status/1416143468070465537) shares an example of the retain cycle remedy while working with `Combine` or any other escaping closure.

### When should you use a throwing initializer

When constructing an object using a failable initializer, the result is an optional that either contains the object (when the initialization succeeded) or contains `nil` (when the initialization failed). [Vincent Pradeilles](https://twitter.com/v_pradeilles) in his YouTube [video](https://www.youtube.com/watch?v=bWWj8zgd--c) briefs that throwing initializer can be used to convey failure information.

### Assert xib files exist

In case a project you are working on relies a lot on xib files, [Vincent Pradeilles](https://twitter.com/v_pradeilles) in his YouTube [video](https://www.youtube.com/watch?v=qowbAhsDuO0) encourages you to implement tests that validate xib file for specified class is in the bundle.

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
