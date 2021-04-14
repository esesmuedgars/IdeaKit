<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 9 minute read

![Issue](https://img.shields.io/badge/issue-1.4-informational.svg)

Welcome back! I would like to thank you for your activity, pilot issue [of the newsletter] was a success, so let's continue by building on top of that!

There has been a pair of improvements to the newsletter. Firstly, the _[News](#news-)_ section highlighting the must-know security threats and important announcements.

Secondly, on the 29<sup>th</sup> of March, multiple people have begun their journey in Accenture Latvia ATC as mobile development interns. To support new talents _[Fundamentals](#fundamentals-)_ section has been added to the newsletter. _[Fundamentals](#fundamentals-)_ is a beginner-friendly section dedicated to interns, trainees, junior developers, and anyone and everyone who is looking to get familiar with the Swift programming language.

## News ![new](https://img.shields.io/badge/new-success.svg)

### XcodeSpy targets Xcode developers with EggShell backdoor ![important](https://img.shields.io/badge/important-important.svg)

A new backdoor threat has been discovered that aims to compromise developers’ macOS devices with a trojanized Xcode project along with a persistence mechanism. This malware can record victims’ microphones, cameras, keyboards as well as upload and download files. [Phil Stokes](https://twitter.com/philofishal) of Sentinel Labs provides simple method developers can use to scan their existing local Xcode repositories in the _Detection and Mitigation_ section of the [report](https://labs.sentinelone.com/new-macos-malware-xcodespy-targets-xcode-developers-with-eggshell-backdoor). 
If you uncover any trace of XcodeSpy on your Accenture-owned macOS device, you should immediately call the Accenture Security Operations Center (ASOC) hotline at +1 202 728 0645.

### macOS minumum version update for Accenture workstations ![important](https://img.shields.io/badge/important-important.svg)

On the 17<sup>th</sup> of May, the minimum compliant version of macOS will be set to macOS Catalina 10.15.7. Afterward, if your macOS device version is below Catalina you will lose _Conditional Access_ (with it access to resources such as Microsoft Office, Microsoft Teams, etc.). Read the full Accenture Mac Workstation blog [post](https://blog.accenture.com/accenturemacworkstation/2021/04/13/conditional-access-minimum-version-macos-update) by [Chad Proctor](https://people.accenture.com/People/user/r.chad.proctor).

### WWDC 2021

[Apple](https://twitter.com/apple) announced that an all-online [Apple Worldwide Developers Conference](https://developer.apple.com/wwdc21) will take place on the 7<sup>th</sup> of June.

###  `AppTrackingTransparency` framework

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=8h0btjq7) incentivizes to prepare applications for upcoming public release. To access app-related data for tracking the user or the device all applications must use the `AppTrackingTransparency` framework to request the user's permission.

## Fundamentals ![new](https://img.shields.io/badge/new-success.svg)

### Becoming an iOS developer in this day and age

[Paul Hudson](https://twitter.com/twostraws) describes the core skills you need to know to become an iOS developer as well as extension skills that are nice to have and will help you stand out. Highlights common mistakes beginners make when they are trying to learn and lists free resources that will help you learn Swift, among other things in his [article](https://www.hackingwithswift.com/articles/230/how-to-become-an-ios-developer) aimed at two groups of people: absolute beginners to Swift – folks who have never built anything for iOS before – and also so-called false beginners, who are folks who might have tried to learn Swift before but never really reached their goal of getting a full-time job.

### Protocols in Swift

Working with protocols is one of Swift’s most fundamental features. With protocols, you define a blueprint that an adopting class must conform to. This principle lets you write decoupled, modular, and extensible Swift code. [Video series](https://www.youtube.com/watch?v=80Qma2hUyUk&list=PLHWvYoDHvsOX_H712wbhzSW0xqHsFy2j9) by [Pedro Rojas](https://twitter.com/pitt500), [video](https://www.youtube.com/watch?v=QZjz2PL9IS8) by [Kyle Lee](https://twitter.com/kilo_loco), and [article](https://learnappmaking.com/protocols-swift-how-to) by [Reinder de Vries](https://twitter.com/reinder42) attempt to help you understand.

### Delegate pattern

The purpose of the delegate pattern is to allow an object to communicate with another object in a decoupled way. One of the most common example of delegation pattern is `UITableViewDataSource` with two required methods `tableView(_:numberOfRowsInSection)` and `tableView(_:cellForRowAt:)`. Visit [video](https://www.youtube.com/watch?v=UQnSdXFDAQQ) by [Alex Nagy](https://twitter.com/alex_rebeloper), [video](https://www.youtube.com/watch?v=DBWu6TnhLeY) by [Sean Allen](https://twitter.com/seanallen_dev), and [article](https://www.swiftbysundell.com/articles/delegation-in-swift) by [John Sundell](https://twitter.com/johnsundell) to learn about delegation pattern.

### Closures in Swift

Closures are self-contained blocks of functionality that can be passed around and used in your code. [Kushal Pagolu](https://hashnode.com/@kushalp) wrote an [article](https://mandovision.hashnode.dev/closures) explaining closures and their nuances.

### Generics in Swift

Generics are one of the most powerful features of Swift, and much of the Swift standard library is built with generic code. Generic code enables you to write flexible, reusable functions and types that can work with any type. You can write code that avoids duplication and expresses its intent in a clear, abstracted manner. All resources - [video series](https://www.youtube.com/watch?v=W947iXBIFu4&list=PLHWvYoDHvsOVP-9UvMBBYJCqxrJ3E8Cry) by [Pedro Rojas](https://twitter.com/pitt500), a [tutorial](https://www.raywenderlich.com/3535703-swift-generics-tutorial-getting-started) written by [Mikael Konutgan](https://twitter.com/mkonutgan) and updated by [Michael Katz](https://twitter.com/TheMikeKatz), [video](https://www.youtube.com/watch?v=EUgAiOSSI3A) by [Daniel Autenrieth](https://twitter.com/brianadventcode), and [article](https://medium.com/codex/swift-generics-made-simple-13a1894a2f9d) by [Artturi Jalli](https://twitter.com/ArtturiJalli) - will help you understand generics clearer.

### Networking in Swift with `URLSession`

I could name only a handful of iOS applications that support offline mode, most of which are by Apple. Nowadays most applications require a network connection to provide access to some, or all, of the features. We could depend on network data-transfer libraries (e.g., [Alamofire](https://github.com/Alamofire/Alamofire)) to execute HTTP requests or we could use a first-party `URLSession` class. [Reinder de Vries](https://twitter.com/reinder42) wrote an [article](https://learnappmaking.com/urlsession-swift-networking-how-to) on how to use the latter one.

## Tutorials

### Firebase Cloud Messaging for iOS in SwiftUI

Push notifications enable developers to inform users when new data becomes available for application. Follow the [tutorial](https://www.raywenderlich.com/20201639-firebase-cloud-messaging-for-ios-push-notifications) written by [Andy Pereira](https://twitter.com/macandyp) to learn how to use Firebase Cloud Messaging, formerly known as Google Cloud Messaging, to send and receive remote push notifications in the SwiftUI iOS application.

### Inspect application's network traffic using Charles Proxy

Learn how to use Charles Proxy to inspect unencrypted and encrypted network traffic for both your applications, as well as third-party applications in a [tutorial](https://www.raywenderlich.com/1827524-charles-proxy-tutorial-for-ios) written by [Aaron Douglas](https://twitter.com/astralbodies) and updated by [Tom Elliott](https://twitter.com/temelliott).

## Enhanced programming

### Dependency injection for property wrappers

[Nikita Ermolenko](https://twitter.com/iOtbivnoe) in his [article](https://otbivnoe.ru/2021/03/13/Dependency-Injection-for-Property-Wrappers.html) describes his counterintuitive solution to property wrapper dependency injection.

### Introducing Swift Collections

[Karoy Lorentey](https://twitter.com/lorentey) announced `Collections`, a new open-source package focused on extending the set of available Swift Standard Library data structures, in his Swift blog [post](https://swift.org/blog/swift-collections). Currently, available data structures are `Deque`, `OrderedSet`, and `OrderedDictionary`.
  
### Distributing your app for beta testing and releases

[Apple](https://twitter.com/apple) has an [article](https://developer.apple.com/documentation/xcode/distributing_your_app_for_beta_testing_and_releases) guiding you through the application's distribution process.

### Transferring data between Bluetooth Low Energy devices

[Apple](https://twitter.com/apple) provides a [sample code](https://developer.apple.com/documentation/corebluetooth/transferring_data_between_bluetooth_low_energy_devices) showing how to create a Bluetooth LE central and peripheral device, and how to transfer data between two iOS devices.

### Unsafe memory pointers in Swift

On rare occasions, when interacting with low-level or legacy APIs, developers are required to use manual memory management. [Tibor Bödecs](https://twitter.com/tiborbodecs) wrote an [article](https://theswiftdev.com/unsafe-memory-pointers-in-swift) about how to use raw pointer references, interact with unsafe pointers, and manually manage memory addresses in Swift.

### Advancements in XCFramework

The XCFramework format allows developers to conveniently distribute binary libraries for multiple platforms and architectures in a single bundle. [Rad Azzouz](https://twitter.com/radazzouz) in his [article](https://pspdfkit.com/blog/2021/advances-in-xcframeworks) goes over the recent advances in the XCFramework format in Xcode 12.

### Demystifying `@autoclosure`

[Artturi Jalli](https://twitter.com/ArtturiJalli) wrote an [article](https://medium.com/codex/swift-demystifying-autoclosures-dc106e4bc04a) explaining what is `@autoclosure`, describes its benefits, and how to use it in Swift.

### `AppDelegate` vs. `SceneDelegate` 

If you’ve developed an application before iOS 13, you probably are familiar with `AppDelegate`. In iOS 13, Apple has moved some of the `AppDelegate` responsibilities to the `SceneDelegate`. [Reinder de Vries](https://twitter.com/reinder42) wrote an [article](https://learnappmaking.com/scene-delegate-app-delegate-xcode-11-ios-13) where he outlines the different roles of both and how they interact to launch an application.

### Understanding and resolving `EXC_BAD_ACCESS` crash errors

`EXC_BAD_ACCESS` is a common crash we run into. [Antoine van der Lee](https://twitter.com/twannl) in his [article](https://www.avanderlee.com/swift/exc-bad-access-crash) not only translates the error but also proposes actions to help track down and solve the root cause of the issue.

### Manually symbolicate crash reports

[Sarun Wongpatcharapakornand](https://twitter.com/sarunw) wrote an [article](https://sarunw.com/posts/symbolicate-crash-reports) where he reports on how to acquire Xcode Debugging Symbol file (dSYM) and manually symbolicate crash reports.

### Encrypt DNS In iOS 14 applications

In iOS 14, Apple introduced support for passing the DNS queries over HTTPS (DoH) or TLS (DoT). Learn how to increase your application user's privacy by encrypting DNS queries in an [article](https://stavrosschizas.com/post/encrypt-dns-in-ios-14-applications) by [Stavros Schizas](https://twitter.com/StavrosSchizas).

### Unpopular `Foundation` formatter types

`DateFormatter` is arguably the most popular formatter type, [John Sundell](https://twitter.com/johnsundell) brings to our attention lesser-known, built-in formatter types such as `PersonNameComponentsFormatter`, `CNPostalAddressFormatter`, `RelativeDateTimeFormatter`, and `ListFormatter` in the following [article](https://www.swiftbysundell.com/articles/exploring-some-of-the-lesser-known-formatter-types).

### Customizing the appearance of a navigation bar

Apple changed the navigation bar appearance in iOS 13. [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) illustrates the differences and demonstrates how to customize `UINavigationBar` appearance using appearance proxy in his [article](https://sarunw.com/posts/uinavigationbar-changes-in-ios13). Additionally, a separate [article](https://sarunw.com/posts/uinavigationbar-changes-in-ios13-part2) has been dedicated to the navigation bar with `UISearchBar` and `UISearchController`.

### `var array: [Int] = []` is the only correct syntax

[Ben Cohen](https://twitter.com/AirspeedSwift) in his Twitter [thread](https://twitter.com/AirspeedSwift/status/1372912675785568256) arguments why you should prefer `var array: [Int] = []` to any other initialization syntax.

### How to use the `rethrows` in Swift

[Antoine van der Lee](https://twitter.com/twannl) wrote an [article](https://www.avanderlee.com/swift/rethrows) explaining `rethrows` keyword and walks us through a real-case example.

### Decrease application launch time

Improve the launch performance of your application by decreasing launch time. Follow optimization tips [Antoine van der Lee](https://twitter.com/twannl) gives in his [article](https://www.avanderlee.com/optimization/launch-time-performance-optimization).

### Flatten a nested JSON response into a single `struct` using `Codable`

When JSON you receive is nested several levels deep and you do not require nested objects as separate data structures, you can use nested containers instead. Learn how to decode nested JSON data into a single data structure using `Codable` in an [article](https://www.donnywals.com/flattening-a-nested-json-response-into-a-single-struct-with-codable) by [Donny Wals](https://twitter.com/DonnyWals).

### Codable synthesis for enums with associated values

[Dario Rexin's](https://twitter.com/evonox) [SE-0295](https://github.com/apple/swift-evolution/blob/main/proposals/0295-codable-synthesis-for-enums-with-associated-values.md) proposal to extend the support for auto-synthesis of `Encodable` and `Decodable` conformance for `class` and `struct` types to enums with associated values has been accepted.

### Xcode new file templates

Learn how to create your own Xcode template for common files in an [article](https://www.andyibanez.com/posts/xcode-new-file-templates) by [Andy Ibanez](https://twitter.com/AndyIbanezK).

### Limit `WKWebView` to a list of specified domains

Many applications use `WKWebView` as a convenient way to display websites without requiring users to leave the app. App-Bound Domains is opt-in `WKWebView` technology that improves in-app browsing by offering greater privacy to users limiting the domains on which an app can utilize APIs to track users. [Keith Harrison](https://twitter.com/kharrison) uses App-Bound Domains to limit navigable domains described in his [article](https://useyourloaf.com/blog/app-bound-domains).

## Tools

### macOS Big Sur available for Accenture workstations

Visit the Accenture Mac Workstation blog [post](https://blog.accenture.com/accenturemacworkstation/2021/04/07/macos-11-big-sur-pilot) by [Chad Proctor](https://people.accenture.com/People/user/r.chad.proctor) to check if your macOS device meets recommended requirements and upgrade today to use the operating system's [latest features](https://www.apple.com/macos/big-sur/features).

### Complete SwiftUI documentation with examples

Apple's documentation is often criticized, SwiftUI developer community has created [SwiftOnTap](https://swiftontap.com) [open-source](https://twitter.com/swiftontap) SwiftUI documentation with examples.

### Convert JSON into Swift objects

[Quicktype](https://app.quicktype.io) web tool and Xcode [extension](https://apps.apple.com/us/app/paste-json-as-code-quicktype/id1330801220) by [David Siegel](https://twitter.com/dvdsgl) save developer's time by eliminating the need to type out data structures of data transfer objects.

### Testing application's accessibility with Evinced

There aren't any shortcuts to testing the application's accessibility, manual tests will always be the most valuable form of accessibility testing possible. But with some carefully designed automated checks, you can detect common accessibility issues quicker and earlier. [Rob Whitaker](https://twitter.com/RobRWAPP)
[reviewed](https://mobilea11y.com/blog/evinced-ios) Evinced - digital accessibility platform.

<br>
<p align="center">
<img width="25%" alt="Curator" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/character.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit the <a href="https://github.com/esesmuedgars/IdeaKit/blob/pilot/README.md">previous issue</a>!
<br>
<br>
Found a topic insightful? You can add your comments and open a discussion using the comment section below.
<br>
Help others improve their Swift knowledge by liking and sharing this post.
<br>
<br>
Reach out in case you would like to contribute or spot any errors! Feedback and suggestions are also welcome.
</p>
