<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.8-informational.svg)

Introduction

## News

### New public betas are available

[Apple](https://twitter.com/Apple) has expanded its public beta program with software that was announced in early June during [WWDC21](https://developer.apple.com/wwdc21). Sign up to the [Apple Beta Software Program](https://beta.apple.com/sp/betaprogram), enroll your personal devices to access iOS 15, iPadOS 15, macOS Monterey, tvOS 15, and watchOS 8 public betas, and try out the latest features. Remember to back up all of your data before installing any beta software.

### Upcoming tax and price changes for apps and in-app purchases ⚠️

<!--
When taxes or foreign exchange rates change, we sometimes need to update prices on the App Store in certain regions and/or adjust your proceeds.
In the next few days, prices of apps and in-app purchases (excluding auto-renewable subscriptions) on the App Store will decrease in:
South Africa
United Kingdom
All territories that use the Euro currency
Prices will increase in Georgia and Tajikistan. The increases also consider the following tax changes, and Exhibit B of the Paid Applications Agreement has been updated to indicate that Apple collects and remits applicable taxes in these locations.
Georgia: New value-added tax of 18%
Tajikistan: New value-added tax of 18% that applies to developers based outside of Tajikistan
Your proceeds will be adjusted accordingly and will be calculated based on the tax-exclusive price.
In addition, your proceeds on the App Store in Italy will be increased to reflect a change to the Digital Services Tax effective rate.
Once these changes go into effect, the Pricing and Availability section of My Apps will be updated. You can change the price of your apps and in-app purchases (including auto-renewable subscriptions) at any time in App Store Connect. If you offer subscriptions, you can choose to preserve prices for existing subscribers.
-->
[article](https://developer.apple.com/news/?id=o0uodgu7) by [Apple](https://twitter.com/Apple)

### Get ready for a new Game Center authentication certificate ⚠️

<!--
Starting August 4, 2021, a new certificate for server-based Game Center verification will be available via the publicKeyUrl. The previous certificate will no longer be available after this date. As a reminder, make sure your app always retrieves and uses the current publicKeyUrl value so it automatically uses the new certificate. If your app caches the certificate or hardcodes the certificate URL, it will require an update.

Please note, this root certificate issuer has been updated from Symantec Corporation to DigiCert, Inc. Make sure to check that the new root certificate issuer is on your list of trusted CAs. You can download the trusted root CA (DigiCert trusted G4) here.
-->
[article](https://developer.apple.com/news/?id=stttq465) by [Apple](https://twitter.com/Apple)

<!--more-->

## Swift challenge

Prefix

```swift
// Swift challenge No. 1

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

Even as a simple problem as this has more clever solutions than the one your initial instinct suggests.

```swift
...
```

## Fundamentals

### Title

## Tutorials

### Title

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

## Tools

### Your AI pair programmer ⚠️

Access is limited to a small group of testers during the technical preview of GitHub Copilot. Sign up today for your chance to try it out and help us improve.
[GitHub](https://twitter.com/github) [Copilot](https://copilot.github.com) get suggestions for whole lines or entire functions right inside your editor.
Hilarious Twitter [post](https://twitter.com/krzyzanowskim/status/1410320595221463044) remark by [Marcin Krzyzanowski](https://twitter.com/krzyzanowskim)

### `DocC` archived and analyzed ⚠️

[article](http://www.alwaysrightinstitute.com/docz) by [Helge Heß](https://twitter.com/helje5)

### (?) A Deep Dive into Airbnb’s Server-Driven UI System ⚠️ (Kotlin)

[article](https://medium.com/airbnb-engineering/a-deep-dive-into-airbnbs-server-driven-ui-system-842244c5f5) by [Ryan Brooks](https://www.linkedin.com/in/rbro112)

## Tips

### How to manually add existing certificates to the Fastlane match ⚠️

[article](https://sarunw.com/posts/how-to-manually-add-existing-certificates-to-fastlane-match) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)

### File name extensions in Xcode ⚠️

Twitter [post](https://twitter.com/qdoug/status/1411948641292521478) by [Douglas Hill](https://twitter.com/qdoug)

### Make Debugger Console Output Stand Out ⚠️

[article](https://dasdom.dev/posts/changing-color-for-debugger-output) by [Dominik Hauser](https://twitter.com/dasdom)

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
