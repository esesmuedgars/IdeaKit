<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read ⚠️

![Issue](https://img.shields.io/badge/issue-1.7-informational.svg)

Welcome back!

The summer vacation period is here, therefore, these issues of the newsletter might also seem slightly lighter than anticipated. I encourage you too to take a well-deserved break, disconnect, clear your mental cache. To be the best you need some rest, take care of yourself!

Happy learning!

## News

### Tax category setting now available in App Store Connect

[Apple](https://twitter.com/Apple) in their news [article](https://developer.apple.com/news/?id=2bbbudbw) announced App Store Connect feature to assign tax categories to your application and in-app purchases. Categories are based on your application's content (e.g., videos, books, or news publications) and determine which tax regulations apply in each territory, allowing Apple to administer tax for you at specific rates.

<!--more-->

## Swift challenge

What Swift challenges are not? Swift challenges are not programming or mathematical problems that have universal solutions.
What Swift challenges are? Swift challenges highlight problems with purpose to grant insight into Swift syntactical sugar and uncommon native APIs.
Each consecutive newsletter's issue will provide solution(-s) (as well as explanation(-s) and resource hyperlink(-s), where applicable) to a problem described in an issue before, besides following challenge.

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

### 5 tips to help you become a well-rounded developer

[Donny Wals](https://twitter.com/DonnyWals) shares his opinion on how to grow as a developer in an [article](https://www.donnywals.com/five-tips-to-help-you-become-a-well-rounded-developer). No surprise, soft skills matter, a lot.

### `lazy` in Swift

A lazy stored property is a property whose initial value isn’t calculated until the first time it’s called. Both [Sean Allen](https://twitter.com/seanallen_dev) in his YouTube [video](https://www.youtube.com/watch?v=xKoua1Mi6qE) and [Vincent Pradeilles](https://twitter.com/v_pradeilles) in his YouTube [video](https://www.youtube.com/watch?v=JLg8C8IYICo) convey practical examples of lazy stored property applications.

### MVVM (Model-View-ViewModel) architectural design pattern

MVVM offers multiple advantages over MVC (Model-View-Controller) such as reusability of views, reduced complexity, improved readability, increased expressiveness, and introduced testability. Learn about MVVM components and their employment in  `SwiftUI` in YouTube [video](https://www.youtube.com/watch?v=FwGMU_Grnf8) by [Sean Allen](https://twitter.com/seanallen_dev). Alternatively, follow [tutorial](https://www.raywenderlich.com/6733535-ios-mvvm-tutorial-refactoring-from-mvc), written by [Chuck Krutsinger](https://twitter.com/CountermindLLC), and refactor MVC to MVVM architectural design pattern. Additionally, [John Codeos](https://twitter.com/johncodeos) wrote an [article](https://johncodeos.com/how-to-implement-mvvm-pattern-with-swift-in-ios) describing building an application with MVVM architectural design pattern in mind.

### Linting versus formatting

[Jason Zurita](https://twitter.com/jasonalexzurita) wrote an [article](https://jasonzurita.com/linting-and-formatting-swift-part-1) making distinction between linting and formatting.

### What is a run loop?

[Valerie Don](https://twitter.com/valeriedon) answers "What is a run loop?" interview question in her YouTube [video](https://www.youtube.com/watch?v=jk5UFJWc-2w).

## Tutorials

### Drag and drop in `SwiftUI`

Learn how to use the implicit collection drag and drop API in `SwiftUI` by building an application in a [tutorial](https://www.raywenderlich.com/21679742-drag-and-drop-tutorial-for-swiftui) by [Warren Burton](https://twitter.com/troutdev).

### Load images asynchronously in `SwiftUI` using `AsyncImage`

[Simon Ng](https://twitter.com/simonng) created a [tutorial](https://www.appcoda.com/asyncimage) educating on how to work with `AsyncImage` view to load and display an image from the specified URL.

### A beginner's guide to thread-safe concurrency

Purpose of actors in Swift is to solve data-races and memory issues, learn how to start working with actors in [tutorial](https://theswiftdev.com/swift-actors-tutorial-a-beginners-guide-to-thread-safe-concurrency) by [Tibor Bödecs](https://twitter.com/tiborbodecs). Additionally, read an [article](https://www.avanderlee.com/swift/actors) by [Antoine van der Lee](https://twitter.com/twannl).

## Enhanced programming

### Handling bidirectional stream of data copying with App Proxy Provider

[Apple](https://twitter.com/Apple) provides an [article](https://developer.apple.com/documentation/networkextension/app_proxy_provider/handling_flow_copying) on using proxy-provider classes to exchange data streams and explaining how to read from the remote connection and write to the local bidirectional stream of data and vice versa.

### Setting up Core Data stack

Assimilate how to set up the classes (collectively referred to as the Core Data stack) that manage and persist your application's objects in [Apple's](https://twitter.com/Apple) [article](https://developer.apple.com/documentation/coredata/setting_up_a_core_data_stack).

### Customizing password AutoFill rules

[Apple](https://twitter.com/Apple) supplies an [article](https://developer.apple.com/documentation/security/password_autofill/customizing_password_autofill_rules)
enlightening how to add individual restrictions to your application's strong password rules using a combination of specification keywords.

### Improve discoverability using static member lookup in generic contexts

[SE-0299](https://github.com/apple/swift-evolution/blob/main/proposals/0299-extend-generic-static-member-lookup.md) proposal by [Pavel Yaskevich](https://www.linkedin.com/in/pavel-yaskevich-5b02a318/), [Sam Lazarus](https://twitter.com/slazaruseth), and [Matt Ricketson](https://twitter.com/ricketson_) has been implemented in Swift 5.5 and aims to relax restrictions on accessing static members on protocols to afford the same call-site legibility to generic APIs. Read an [article](https://www.avanderlee.com/swift/static-member-lookup-generic-contexts) by [Antoine van der Lee](https://twitter.com/twannl) where he offers practical example of the new feature.

### iOS 15 `SFSafariViewController` improvements

[Filip Němeček](https://twitter.com/nemecek_f) wrote an [article](https://nemecek.be/blog/110/sfsafariviewcontroller-improvements-in-ios-15) with reference to `SFSafariViewController` recently added options to run a custom extension on the web page content as well as preload content.

### Making a Swift Package Collection

[Alejandro Martinez](https://twitter.com/alexito4) in his [article](https://alejandromp.com/blog/use-spm-collections-to-have-easy-access-to-your-favourite-packages) displays how you can describe a curated list of packages and associated metadata which makes it easier to discover an existing package for a particular use case.

### Table and collection view cell reloading improvements in iOS 15

In an [article](https://swiftsenpai.com/development/cells-reload-improvements-ios-15) [Lee Kah Seng](https://twitter.com/Lee_Kah_Seng) walks readers through iOS 15 diffable data source improvement that permits to reload value type items in addition to of reloading reference type items.

### Elevate the structure of your Xcode projects

[Tomas Reimers](https://twitter.com/tomasreimers) wrote an [article](https://screenplay.dev/blog/post/Xr88fIeCmhQN3iTkZt4v) where he dives into the details of what Xcode projects are, how do they work, and how you can better structure your projects for your iOS applications.

### Adopting `SwiftUI`

There has been an ongoing debate among the developer community about adopting `SwiftUI` since Apple introduced this framework back in 2019. [Olivier Rigault](https://www.linkedin.com/in/origault) in his [article](https://dev.to/newday-technology/adopting-swiftui-32go) shares the journey that he and his team embraced and challenged that they have faced by adopting `SwiftUI` in their iOS development process early.

### An introduction to synchronizing access with Swift’s actors

[Donny Wals](https://twitter.com/DonnyWals) wrote an [article](https://www.donnywals.com/an-introduction-to-synchronizing-access-with-swifts-actors) to illustrate how an object that isolates access to it's mutable state to empower developer to avoid runtime crashes by solving data races.

### Using Xcode behaviors to speed up workflow

Default behaviors help you already by showing, for example, the debug navigator when pausing on a breakpoint, in an [article](https://www.avanderlee.com/xcode/xcode-behaviours-optimized) by [Antoine van der Lee](https://twitter.com/twannl) learn how to customize Xcode's response to certain events with bahaviors to reduce the amount of required, mundane navigation in Xcode.

### Make blazing fast lists and collection views

View [Apple's](https://twitter.com/Apple) WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10252) where [Aditya Krishnadevan](https://twitter.com/caughtinflux) and [Patrick Metcalfe](https://twitter.com/PDucks32) teach how to use diffable data source and cell registration APIs, refreshes viewers' undesrtanding of a lifecycle of a cell, and show how to improve overall scrolling experience with optimized image loading and automatic cell prefetching.

### Xcode 13 Vim support

I've always had minimalistic approach to my work environment, no additional monitors, external keyboard, or mouse. I use multiple virtual desktops, MacBook's integrated keyboard and trackpad, for me it simply works. Has the time come to remove the trackpad from the equation? Watch [video](https://nsscreencast.com/episodes/491-xcode-13-vim) where [Ben Scheirman](https://twitter.com/subdigital) instructs how to enable Vim key bindings and gives a quick tour of how to navigate using them.

### Using test repetitions in Xcode 13 to resolve flaky tests

[Antoine van der Lee](https://twitter.com/twannl) wrote an [article](https://www.avanderlee.com/debugging/flaky-tests-test-repetitions) to help you identify flaky tests and their possible causes, as well as proposes solutions to avoid introducing flaky tests in the first place. 

### iOS simple search algorithm

[Geoff Hackworth](https://twitter.com/geoffhackworth) shared an search algorithm, that he applied in several iOS applications, that is superior than a trivial substring match but not as complex as Xcode’s matching of method names in an [article](https://hacknicity.medium.com/a-simple-smart-search-algorithm-for-ios-in-swift-65f71b2f221a).

### Faster application launch times in iOS 15

[Noah Martin](https://twitter.com/sond813) carried out colossal investigation in iOS 15 dynamic link editor (dyld) improvement to use chained fixups format and reported his uncoverings in an [article](https://medium.com/geekculture/how-ios-15-makes-your-app-launch-faster-51cf0aa6c520).

### How to share an iOS distribution certificate

[Sarun Wongpatcharapakornand](https://twitter.com/sarunw) created a [guide](https://sarunw.com/posts/how-to-share-ios-distribution-certificate) navigating reader through the process of creating, exporting and importing of distribution certificate.

### Detecting memory leaks via tests

[António Lima](https://twitter.com/aclima93) wrote an [article](https://aclima93.com/swift/2021/06/24/01.html) defining a memory leak and automating leak detection with test cases. In his supplementary [article](https://aclima93.com/swift/2021/07/23/01.html) he pursues automation of asserts for lingering references and the ability to use non-reference types such as structures and enumerations in tests.

## Tools

### Prioritize work with Quality of Service classes

Mobile applications are competing to use finite resources — CPU (central processing unit), memory, network interfaces, etc. In order for application to remain responsive and efficient it is crucial to prioritize tasks. [Apple](https://twitter.com/Apple) provides [documentation](https://developer.apple.com/library/archive/documentation/Performance/Conceptual/EnergyGuide-iOS/PrioritizeWorkWithQoS.html) on a QoS (Quality of Service) classes and describes their [classes'] intended type of work.

### Analyze network traffic with new instrument

[Charles Proxy](https://www.charlesproxy.com) has been a pivotal tool to inspect unencrypted and encrypted network traffic, it has various other features, but those are rarily required in a day-to-day development (if, however, you are looking for more advanced debugging [Emad Ghorbaninia](https://twitter.com/emadgnia) wrote a [tutorial](https://www.raywenderlich.com/22070831-advanced-charles-proxy-tutorial-for-ios) teaching how to configure Charles Proxy, manipulate requests and responses, automate using Rewrite and Repeat features, use breakpoints, filtering requests). Instruments 13 introduces HTTP traffic instrument, contained in the Network template, focusing on auditing the traffic coming from your application through the Apple Networking stack. Read an [article](https://michaelabadi.com/articles/analyse-http-instruments) by [Michael Abadi Santoso](https://twitter.com/michaelabadiii).

### 7 well-known iOS applications that collectively could save 500MB of user's storage

[Noah Martin](https://twitter.com/sond813) shared his findings in an [article](https://medium.com/swlh/how-7-ios-apps-could-save-you-500mb-of-storage-a828782c973e) about common mistakes that are increasing application installation sizes discovered using [Emerge](https://www.emergetools.com) — binary size profiling tool.

## Tips

### `CoreLocationUI` framework

[Filip Němeček](https://twitter.com/nemecek_f) wrote a short [article](https://nemecek.be/blog/109/core-location-ui-new-way-to-get-one-time-location) reviewing a `CLLocationButton` that provides an easy, low-friction way to grant your application location access only when needed.

### Refactoring completion closures to asynchronous methods

Learn how to refactor legacy completion closure implementations to use iOS 15 `async`/`await` API in a YouTube [video](https://www.youtube.com/watch?v=9CI8O7iufDI) by [Vincent Pradeilles](https://twitter.com/v_pradeilles).

### Column breakpoints

Xcode 13 aims to make debugging more productive and introduces column breakpoints which work like a more granular version of line breakpoints. [Keith Harrison](https://twitter.com/kharrison) illustrates how to use them in his 2 minute [article](https://useyourloaf.com/blog/xcode-column-breakpoints).

### Specific class protocol

[Sarun Wongpatcharapakornand](https://twitter.com/sarunw) created a Twitter [post](https://twitter.com/sarunw/status/1409270071176880131) demonstrating that in Swift 5 developer can declare protocol for a specific class. Additionally, read his in-depth [article](https://sarunw.com/posts/how-to-declare-swift-protocol-for-specific-class) about the topic.

### Keep the structture's default memberwise initializer

[Leonardo Maia Pugliese](https://twitter.com/Leo_Pugliese) in his [article](https://holyswift.app/a-trick-to-keep-the-structs-default-memberwise-initializer-in-swift) shared his know-how on how to add custom initializer to the structure without overwriting the default initializer.

### Measuring scrolling performance with UI test

In Twitter [post](https://twitter.com/mecid/status/1408071686587490304) [Majid Jabrayilov](https://twitter.com/mecid) brings out that you can write a UI test that measures scrolling performance in your application that fails if performance is not satisfactory.

### Why `#if DEBUG` conditional should be avoided in libraries

[Arek Holko](https://twitter.com/arekholko) had written an [article](https://holko.pl/2018/09/24/compilation-directives-in-libraries) about an issue he had to solve when application running in Debug configuration unknowingly called library with Release configuration and proposes a substitute implementation when writing libraries.

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
