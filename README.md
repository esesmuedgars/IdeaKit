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
-->

## Fundamentals

### Unit testing: the pragmatic guide on where to start ⚠️

[article](https://hybridcattt.com/blog/start-testing-pragmatic-guide) by (she/her) [Marina Gornostaeva](https://twitter.com/hybridcattt)

### Copy-On-Assignment vs. Copy-On-Write in Swift ⚠️

[article](https://aymanmoo.medium.com/copy-on-assignment-vs-copy-on-write-in-swift-c3016b343d06) by [Ayman Fayez](https://www.linkedin.com/in/ayman-fayez-7ab174156)

### Implementing Feature Flagging in iOS ⚠️

[article](https://digitalbunker.dev/2021/07/23/implementing-feature-flagging-in-ios) by [Aryaman Sharda](https://twitter.com/aryamansharda)

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

### Your AI pair programmer ⚠️

Access is limited to a small group of testers during the technical preview of GitHub Copilot. Sign up today for your chance to try it out and help us improve.
[GitHub](https://twitter.com/github) [Copilot](https://copilot.github.com) get suggestions for whole lines or entire functions right inside your editor.
Hilarious Twitter [post](https://twitter.com/krzyzanowskim/status/1410320595221463044) remark by [Marcin Krzyzanowski](https://twitter.com/krzyzanowskim)

### `DocC` archived and analyzed ⚠️

[article](http://www.alwaysrightinstitute.com/docz) by [Helge Heß](https://twitter.com/helje5)

### Swift Package Index ⚠️

Swift Package Collections
[Swift Package Index](https://swiftpackageindex.com)

## Tips

### How to manually add existing certificates to the Fastlane match ⚠️

[article](https://sarunw.com/posts/how-to-manually-add-existing-certificates-to-fastlane-match) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)

### File name extensions in Xcode ⚠️

Twitter [post](https://twitter.com/qdoug/status/1411948641292521478) by [Douglas Hill](https://twitter.com/qdoug)

### Make Debugger Console Output Stand Out ⚠️

[article](https://dasdom.dev/posts/changing-color-for-debugger-output) by [Dominik Hauser](https://twitter.com/dasdom)

### Avoid index math in Collections ⚠️

Twitter [post](https://twitter.com/olebegemann/status/1415351550847950848) by [Ole Begemann](https://twitter.com/olebegemann)

### Retain-cycles in Combine ⚠️

Twitter [post](https://twitter.com/eneko/status/1416143468070465537) by [Eneko Alonso](https://twitter.com/eneko)

### When should you use a Failable Initializer? ⚠️

YouTube [video](https://www.youtube.com/watch?v=bWWj8zgd--c) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

### Assert XIB file exists ⚠️

YouTube [video](https://www.youtube.com/watch?v=qowbAhsDuO0) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

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
