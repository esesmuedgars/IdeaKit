<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.7-informational.svg)

**TODO:** Prefix

## News

### Tax Category Setting Now Available in App Store Connect

<!--
The App Store makes it easy for you to manage transactions in 175 territories, and Apple administers tax on behalf of developers in 64 of those territories. Now App Store Connect provides the ability to assign tax categories to your apps and in-app purchases. These categories are based on your app's content (for example, videos, books, or news publications) and determine which tax regulations apply in each territory, allowing Apple to administer tax for you at specific rates.

To assign categories, visit the Pricing and Availability section for your app in App Store Connect. If a category applies to your app, select it at the app level to apply it to the app and its associated in-app purchases. You can also manage each in-app purchase individually. Your selections will be applied to future transactions and you can view the new Transaction Tax report the first full month after you configure your settings. If you choose not to make any changes, your apps and in-app purchases will be assigned the App Store software category at the same tax rate used today. Adjust these settings at any time as the characterization of your apps or in-app purchases evolve or as tax legislation changes.
-->
[article](https://developer.apple.com/news/?id=2bbbudbw)

<!--more-->

## Swift challenge

What Swift challenges are not? Swift challenges are not programming or mathematical problems that have universal solutions.
What Swift challenges are? Swift challenges highlight problems with purpose to grant insight into Swift syntactical sugar and uncommon native APIs.
Each consecutive newsletter's issue will provide solution(-s) (as well as explanation(-s) and resource hyperlink(-s), where applicable) to a problem described in issue before, besides following challenge.

Let's start things slow, Swift challenge No. 1:

Even as simple problem as this has more clever solutions than the one your initial instinct suggests.

```swift
/**
For numbers in the range between 0 and 9 return spelled out number value.
Implement `spellOut` method.
 */

extension Int {
    /// Spell out number in the range from 0 to 9 (e.g., calling `0.spelledOut` returns `"Zero"`).
    /// - returns: Capitalized, spelled out number value.
    var spelledOut: String {
        assert(0...9 ~= self, "Value is out-of-bounds")
         
        return spellOut()
    }
     
    private func spellOut() -> String {
        <#String#>
    }
}
```

<!--
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
-->

## Fundamentals

### Five tips to help you become a well-rounded developer

[article](https://www.donnywals.com/five-tips-to-help-you-become-a-well-rounded-developer) by [Donny Wals](https://twitter.com/DonnyWals)

### `lazy` in Swift

YouTube [video](https://www.youtube.com/watch?v=xKoua1Mi6qE) by [Sean Allen](https://twitter.com/seanallen_dev) and YouTube [video](https://www.youtube.com/watch?v=JLg8C8IYICo) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

### MVVM (Model-View-ViewModel) architectural design pattern

YouTube [video](https://www.youtube.com/watch?v=FwGMU_Grnf8) by [Sean Allen](https://twitter.com/seanallen_dev). Additionally, [tutorial] on how to refactor MVC (Model-View-Controller) to MVVM  by [Chuck Krutsinger](https://twitter.com/CountermindLLC). Plus, an [article](https://johncodeos.com/how-to-implement-mvvm-pattern-with-swift-in-ios) by [John Codeos](https://twitter.com/johncodeos).

### Linting vs formatting

[article](https://jasonzurita.com/linting-and-formatting-swift-part-1) by [Jason Zurita](https://twitter.com/jasonalexzurita)

### What is a runloop?

YouTube [video](https://www.youtube.com/watch?v=jk5UFJWc-2w) by [Valerie Don](https://twitter.com/valeriedon)

## Tutorials

### Drag and Drop Tutorial for `SwiftUI`

[tutorial](https://www.raywenderlich.com/21679742-drag-and-drop-tutorial-for-swiftui) by [Warren Burton](https://twitter.com/troutdev)

### Using AsyncImage in `SwiftUI` for Loading Images Asynchronously

[article](https://www.appcoda.com/asyncimage) by [Simon Ng](https://twitter.com/simonng)

### Swift actors tutorial - a beginner's guide to thread safe concurrency

[article](https://theswiftdev.com/swift-actors-tutorial-a-beginners-guide-to-thread-safe-concurrency) by [Tibor Bödecs](https://twitter.com/tiborbodecs)

## Enhanced programming

### App Proxy Provider: Handling Flow Copying

[Apple](https://twitter.com/Apple) provides [article](https://developer.apple.com/documentation/networkextension/app_proxy_provider/handling_flow_copying)

### Setting Up a Core Data Stack

[Apple](https://twitter.com/Apple) provides [article](https://developer.apple.com/documentation/coredata/setting_up_a_core_data_stack)

### Customizing Password AutoFill Rules

[Apple](https://twitter.com/Apple) provides [article](https://developer.apple.com/documentation/security/password_autofill/customizing_password_autofill_rules)

### Improve discoverability using Static Member Lookup in Generic Contexts

[article](https://www.avanderlee.com/swift/static-member-lookup-generic-contexts) by [Antoine van der Lee](https://twitter.com/twannl)

### iOS 15 `SFSafariViewController` improvements

[article](https://nemecek.be/blog/110/sfsafariviewcontroller-improvements-in-ios-15) by [Filip Němeček](https://twitter.com/nemecek_f)

### Swift concurency

Swift Programming language book updated concurency [topic](https://docs.swift.org/swift-book/LanguageGuide/Concurrency.html)

### Make a Swift Package Collection with your favorites

[article](https://alejandromp.com/blog/use-spm-collections-to-have-easy-access-to-your-favourite-packages) by [Alejandro Martinez](https://twitter.com/alexito4)

### Table and Collection View Cells Reload Improvements in iOS 15

[article](https://swiftsenpai.com/development/cells-reload-improvements-ios-15) by [Lee Kah Seng](https://twitter.com/Lee_Kah_Seng)

### How to better structure your Xcode projects

[article](https://screenplay.dev/blog/post/Xr88fIeCmhQN3iTkZt4v) by [Tomas Reimers](https://twitter.com/tomasreimers)

### Adopting `SwiftUI`

[article](https://dev.to/newday-technology/adopting-swiftui-32go) by [Olivier Rigault](https://www.linkedin.com/in/origault)

### An introduction to synchronizing access with Swift’s Actors

[article](https://www.donnywals.com/an-introduction-to-synchronizing-access-with-swifts-actors) by [Donny Wals](https://twitter.com/DonnyWals)

### Speeding up with Xcode Behaviors

[article](https://www.avanderlee.com/xcode/xcode-behaviours-optimized) by [Antoine van der Lee](https://twitter.com/twannl)

### Make blazing fast lists and collection views

<!--
Build consistently smooth scrolling list and collection views: Explore the lifecycle of a cell and learn how to apply that knowledge to eliminate rough scrolling and missed frames. We'll also show you how to improve your overall scrolling experience and avoid costly hitches, with optimized image loading and automatic cell prefetching. To get the most out of this video, we recommend a basic familiarity with diffable data sources and compositional layout.
-->
[Apple's](https://twitter.com/Apple) WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10252) by [Aditya Krishnadevan](https://twitter.com/caughtinflux) and [Patrick Metcalfe](https://twitter.com/PDucks32).

### Xcode 13 Vim Mode

I like developing lightly, just mac, no external keyboard, additonal monitors, or mouse. Using multiple virtual desktops and it works for me. Maybe it is time to forget touchbar as well? [video](https://nsscreencast.com/episodes/491-xcode-13-vim) by [Ben Scheirman](https://twitter.com/subdigital)

### Flaky tests resolving using Test Repetitions in Xcode

[article](https://www.avanderlee.com/debugging/flaky-tests-test-repetitions) by [Antoine van der Lee](https://twitter.com/twannl)

### A Simple, Smart Search Algorithm for iOS in Swift

[article](https://hacknicity.medium.com/a-simple-smart-search-algorithm-for-ios-in-swift-65f71b2f221a) by [Geoff Hackworth](https://twitter.com/geoffhackworth)

### How iOS 15 makes your app launch faster

[article](https://medium.com/geekculture/how-ios-15-makes-your-app-launch-faster-51cf0aa6c520) by [Noah Martin](https://twitter.com/sond813)

### How to share an iOS distribution certificate

[article](https://sarunw.com/posts/how-to-share-ios-distribution-certificate) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)

### Detecting memory leaks via tests

[article](https://aclima93.com/swift/2021/06/24/01.html) and [article](https://aclima93.com/swift/2021/07/23/01.html) by [António Lima](https://twitter.com/aclima93)

## Tools

### Prioritize Work with Quality of Service Classes

[Apple](https://twitter.com/Apple) provides [documentation](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/EnergyGuide-iOS/PrioritizeWorkWithQoS.html)

### Analyze HTTP Traffic with new HTTP Instrument

[article](https://michaelabadi.com/articles/analyse-http-instruments) by [Michael Abadi Santoso](https://twitter.com/michaelabadiii)

### How 7 iOS Apps Could Save You 500MB of Storage

[Emerge](https://www.emergetools.com)
[article](https://medium.com/swlh/how-7-ios-apps-could-save-you-500mb-of-storage-a828782c973e) by [Noah Martin](https://twitter.com/sond813)

## Tips

### Core Location UI: New way to get one-time location

[article](https://nemecek.be/blog/109/core-location-ui-new-way-to-get-one-time-location) by [Filip Němeček](https://twitter.com/nemecek_f)

### How do you go from completionHandler to async / await?

YouTube [video](https://www.youtube.com/watch?v=9CI8O7iufDI) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

### Xcode Column Breakpoints

[article](https://useyourloaf.com/blog/xcode-column-breakpoints) by [Keith Harrison](https://twitter.com/kharrison)

### Declare Swift protocol for a specific class

Twitter [post](https://twitter.com/sarunw/status/1409270071176880131) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw). Additionally, an [article](https://sarunw.com/posts/how-to-declare-swift-protocol-for-specific-class)

### A trick to keep the Struct's Default Memberwise initializer in Swift

[article](https://holyswift.app/a-trick-to-keep-the-structs-default-memberwise-initializer-in-swift) by [Leonardo Maia Pugliese](https://twitter.com/Leo_Pugliese)

### Measuring scrolling performance with UI Tests

Twitter [post](https://twitter.com/mecid/status/1408071686587490304) by [Majid Jabrayilov](https://twitter.com/mecid)

### Why #if DEBUG Conditional Should Be Avoided in Library Code

[article](https://holko.pl/2018/09/24/compilation-directives-in-libraries) by [Arek Holko](https://twitter.com/arekholko)

<br>
<p align="center">
<img width="25%" alt="Curator" src="curator.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit the <a href="https://github.com/esesmuedgars/IdeaKit/blob/issue3/README.md">previous issue</a>!
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
