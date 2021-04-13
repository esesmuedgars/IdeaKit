<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 3 minute read

![Issue](https://img.shields.io/badge/issue-1.4-informational.svg)

Welcome back! I would like to thank you for your activity, pilot issue [of the newsletter] was a success, so let's continue by building on top of that!

There has been a pair of improvements to the newsletter. Firstly, the _[News](#news)_ section highlighting the must-know security threats and important Apple announcements.

Secondly, on 29<sup>th</sup> of March multiple people have begun their journey in Accenture Latvia ATC as mobile development interns. To support new talents _[Fundamentals](#fundamentals)_ section has been added to the newsletter. Fundamentals is a beginner-friendly section dedicated to interns, trainees, junior developers, and anyone and everyone who is looking to get familiar with the Swift programming language.

## News ![new](https://img.shields.io/badge/new-success.svg)

### XcodeSpy targets Xcode developers with EggShell backdoor ![important](https://img.shields.io/badge/important-important.svg)

A new backdoor threat has been discovered that aims to compromise developers’ macOS devices with a trojanized Xcode project along with a persistence mechanism. This malware can record victims’ microphones, cameras, keyboards as well as upload and download files. [Phil Stokes](https://twitter.com/philofishal) of Sentinel Labs provides simple method developers can use to scan their existing local Xcode repositories in the _Detection and Mitigation_ section of [report](https://labs.sentinelone.com/new-macos-malware-xcodespy-targets-xcode-developers-with-eggshell-backdoor). 
If you uncover any trace of XcodeSpy on your Accenture-owned macOS device, you should immediately call the Accenture Security Operations Center (ASOC) hotline at +1 202 728 0645.

### macOS minumum version update for Accenture workstations ![important](https://img.shields.io/badge/important-important.svg)

On 17<sup>th</sup> of May the minimum compliant version of macOS will be set to macOS Catalina 10.15.7. Afterward, if your macOS device version is below Catalina you will lose _Conditional Access_ (with it access to resources such as Microsoft Office, Microsoft Teams, etc.). Read full Accenture Mac Workstation blog [post](https://blog.accenture.com/accenturemacworkstation/2021/04/13/conditional-access-minimum-version-macos-update) by [Chad Proctor](https://people.accenture.com/People/user/r.chad.proctor).

### macOS Big Sur available for Accenture workstations

Visit Accenture Mac Workstation blog [post](https://blog.accenture.com/accenturemacworkstation/2021/04/07/macos-11-big-sur-pilot) by [Chad Proctor](https://people.accenture.com/People/user/r.chad.proctor) to check if your macOS device meets recommended requirements and upgrade today to use operating systems [latest features](https://www.apple.com/macos/big-sur/features).

### WWDC 2021

[Apple](https://twitter.com/apple) announced that an all-online [Apple Worldwide Developers Conference](https://developer.apple.com/wwdc21) will take place on 7<sup>th</sup> of June.

###  `AppTrackingTransparency` framework

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=8h0btjq7) incentivizes to prepare applications for upcoming public release. To access app-related data for tracking the user or the device all applications must use the `AppTrackingTransparency` framework to request the user's permission.

## Fundamentals ![new](https://img.shields.io/badge/new-success.svg)

### Becoming iOS developer in this day and age

[Paul Hudson](https://twitter.com/twostraws) describes the core skills you need to know to become an iOS developer as well as extension skills that are nice to have and will help you stand out. Highlights common mistakes beginners make when they are trying to learn and lists free resources that will help you learn Swift, among other things in his [article](https://www.hackingwithswift.com/articles/230/how-to-become-an-ios-developer) aimed at two groups of people: absolute beginners to Swift – folks who have never built anything for iOS before – and also so-called false beginners, who are folks who might have tried to learn Swift before but never really reached their goal of getting a full-time job.

### Protocols in Swift

Working with protocols is one of Swift’s most fundamental features. With protocols, you define a blueprint that an adopting class must conform to. This principle lets you write decoupled, modular, and extensible Swift code. [Video series](https://www.youtube.com/watch?v=80Qma2hUyUk&list=PLHWvYoDHvsOX_H712wbhzSW0xqHsFy2j9) by [Pedro Rojas](https://twitter.com/pitt500), [video](https://www.youtube.com/watch?v=QZjz2PL9IS8) by [Kyle Lee](https://twitter.com/kilo_loco), and [article](https://learnappmaking.com/protocols-swift-how-to) by [Reinder de Vries](https://twitter.com/reinder42) attempt to help you understand.

### Delegate pattern

The purpose of the delegate pattern is to allow an object to communicate with another object in a decoupled way. One of the most common example of delegate pattern is `UITableViewDataSource` with two required methods `tableView(_:numberOfRowsInSection)` and `tableView(_:cellForRowAt:)`. Visit [video](https://www.youtube.com/watch?v=UQnSdXFDAQQ) by [Alex Nagy](https://twitter.com/alex_rebeloper), [video](https://www.youtube.com/watch?v=DBWu6TnhLeY) by [Sean Allen](https://twitter.com/seanallen_dev) and [article](https://www.swiftbysundell.com/articles/delegation-in-swift) by [John Sundell](https://twitter.com/johnsundell) to learn about delegation pattern.

### Closures in Swift

Closures are self-contained blocks of functionality that can be passed around and used in your code. [Kushal Pagolu](https://hashnode.com/@kushalp) wrote an [article](https://mandovision.hashnode.dev/closures) explaining closures and their nuances.

### Generics in Swift

Generics are one of the most powerful features of Swift, and much of the Swift standard library is built with generic code. Generic code enables you to write flexible, reusable functions and types that can work with any type. You can write code that avoids duplication and expresses its intent in a clear, abstracted manner. All resources - [video series](https://www.youtube.com/watch?v=W947iXBIFu4&list=PLHWvYoDHvsOVP-9UvMBBYJCqxrJ3E8Cry) by [Pedro Rojas](https://twitter.com/pitt500), [tutorial](https://www.raywenderlich.com/3535703-swift-generics-tutorial-getting-started) written by [Mikael Konutgan](https://twitter.com/mkonutgan) and updated by [Michael Katz](https://twitter.com/TheMikeKatz), [video](https://www.youtube.com/watch?v=EUgAiOSSI3A) by [Daniel Autenrieth](https://twitter.com/brianadventcode), and [article](https://medium.com/codex/swift-generics-made-simple-13a1894a2f9d) by [Artturi Jalli](https://twitter.com/ArtturiJalli) - will help you understand generics clearer.

### Networking in Swift with `URLSession`

[article](https://learnappmaking.com/urlsession-swift-networking-how-to) by [Reinder de Vries](https://twitter.com/reinder42).

## Tutorials

### Firebase Cloud Messaging for iOS in SwiftUI

[tutorial](https://www.raywenderlich.com/20201639-firebase-cloud-messaging-for-ios-push-notifications) by [Andy Pereira](https://twitter.com/macandyp).

## Enhanced programming

### Dependency injection for property wrappers

[article](https://otbivnoe.ru/2021/03/13/Dependency-Injection-for-Property-Wrappers.html) by [Nikita Ermolenko](https://twitter.com/iOtbivnoe).

### Introducing Swift collections

Swift blog [post](https://swift.org/blog/swift-collections) by [Karoy Lorentey](https://twitter.com/lorentey).
  
### Distributing Your App for Beta Testing and Releases

[article](https://developer.apple.com/documentation/xcode/distributing_your_app_for_beta_testing_and_releases) by [Apple](https://twitter.com/apple).

### Transferring data between Bluetooth Low Energy devices

[sample code](https://developer.apple.com/documentation/corebluetooth/transferring_data_between_bluetooth_low_energy_devices) by [Apple](https://twitter.com/apple).

### Monitoring basic memory statistics

[article](https://developer.apple.com/documentation/metal/frame_capture_debugging_tools/improving_memory_and_resource_usage/monitoring_basic_memory_statistics) by [Apple](https://twitter.com/apple).

### Unsafe memory pointers in Swift

[article](https://theswiftdev.com/unsafe-memory-pointers-in-swift) by [Tibor Bödecs](https://twitter.com/tiborbodecs).

### XCFrameworks advancements

[article](https://pspdfkit.com/blog/2021/advances-in-xcframeworks) by [Rad Azzouz](https://twitter.com/radazzouz).

### Demystifying autoclosures

[article](https://medium.com/codex/swift-demystifying-autoclosures-dc106e4bc04a) by [Artturi Jalli](https://twitter.com/ArtturiJalli).

### Scene Delegate vs. App Delegate explained

[article](https://learnappmaking.com/scene-delegate-app-delegate-xcode-11-ios-13) by [Reinder de Vries](https://twitter.com/reinder42).

### Understanding and resolving `EXC_BAD_ACCESS` crash errors

[article](https://www.avanderlee.com/swift/exc-bad-access-crash) by [Antoine van der Lee](https://twitter.com/twannl).

### Manually symbolicate crash reports

[article](https://sarunw.com/posts/symbolicate-crash-reports) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw).

### Encrypt DNS In iOS 14 applications

[article](https://stavrosschizas.com/post/encrypt-dns-in-ios-14-applications) by [Stavros Schizas](https://twitter.com/StavrosSchizas).

### Unpopular `Foundation` formatter types

[article](https://www.swiftbysundell.com/articles/exploring-some-of-the-lesser-known-formatter-types) by [John Sundell](https://twitter.com/johnsundell).

### Customizing the appearance of a navigation bar

iOS 13+
[article](https://sarunw.com/posts/uinavigationbar-changes-in-ios13) and [article](https://sarunw.com/posts/uinavigationbar-changes-in-ios13-part2) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw).

### Preferred `var array: [Int] = []`

Twitter [thread](https://twitter.com/AirspeedSwift/status/1372912675785568256) by [Ben Cohen](https://twitter.com/AirspeedSwift)

### How to use the `rethrows` in Swift

[article](https://www.avanderlee.com/swift/rethrows) by [Antoine van der Lee](https://twitter.com/twannl).

### Decrease application launch time

[article](https://www.avanderlee.com/optimization/launch-time-performance-optimization) by [Antoine van der Lee](https://twitter.com/twannl).

### Flatten a nested JSON response into a single `struct` using `Codable`

[article](https://www.donnywals.com/flattening-a-nested-json-response-into-a-single-struct-with-codable) by [Donny Wals](https://twitter.com/DonnyWals).

### Codable synthesis for enums with associated values

[Dario Rexin's](https://twitter.com/evonox) [SE-0295](https://github.com/apple/swift-evolution/blob/main/proposals/0295-codable-synthesis-for-enums-with-associated-values.md) proposal to extend the support for auto-synthesis of `Encodable` and `Decodable` conformance for `class` and `struct` types to enums with associated values has been accepted.

### Xcode new file templates

[article](https://www.andyibanez.com/posts/xcode-new-file-templates) by [Andy Ibanez](https://twitter.com/AndyIbanezK).

### Limit `WKWebView` to a list of specified domains

[article](https://useyourloaf.com/blog/app-bound-domains) by [Keith Harrison](https://twitter.com/kharrison).

## Tools

### Complete SwiftUI documentation with examples

SwiftOnTap tool [documentation](https://swiftontap.com) [open-source](https://twitter.com/swiftontap).

### Convert JSON into Swift objects

[Quicktype](https://app.quicktype.io) tool and Xcode [extension](https://apps.apple.com/us/app/paste-json-as-code-quicktype/id1330801220) by [David Siegel](https://twitter.com/dvdsgl).

### Testing application's accessibility with Evinced

Evinced iOS accessibilty debugger [review](https://mobilea11y.com/blog/evinced-ios) by [Rob Whitaker](https://twitter.com/RobRWAPP).

### Inspect application's network traffic using Charles Proxy

Learn how to use Charles Proxy to inspect unencrypted and encrypted network traffic for both your own applications, as well as third-party applications in [tutorial](https://www.raywenderlich.com/1827524-charles-proxy-tutorial-for-ios) written by [Aaron Douglas](https://twitter.com/astralbodies) and updated by [Tom Elliott](https://twitter.com/temelliott).

<br>
<p align="center">
<img width="25%" alt="Curator" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/character.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit <a href="https://github.com/esesmuedgars/IdeaKit/blob/pilot/README.md">previous issue</a>!
<br>
<br>
Found a topic insightful? You can add your comments and open a discussion using the comment section below.
<br>
Help others improve their Swift knowledge by liking and sharing this post.
<br>
<br>
Reach out in case you would like to contribute or spot any errors! Feedback and suggestions are also welcome.
</p>
