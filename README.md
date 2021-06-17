<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.6-informational.svg)

Good morning and welcome to _import IdeaKit_!

Shout-out to [Artjoms Vorona](https://people.accenture.com/People/user/artjoms.vorona) for his contribution to 3<sup>rd</sup> issue of the newsletter! The backlog has plenty more unassigned user stories, consider this as an invitation to join the team. All aboard!

Congratulations to all Midyear Cycle promotees, prominently to the Latvia ATC iOS developers - [Artjoms Vorona](https://people.accenture.com/People/user/artjoms.vorona), [Kristaps Knets](https://people.accenture.com/People/user/kristaps.knets), and [Armands Mikanovskis-Mikalovskis](https://people.accenture.com/People/user/armands.mikanovskis)! 👏🏼

During [WWDC21](https://developer.apple.com/wwdc21) [Apple](https://twitter.com/Apple) announced [Xcode Cloud](https://developer.apple.com/xcode-cloud), concurrency in Swift, Universal Control, tab groups in Safari, live text, mentions and tags in Notes, focus mode, and notification summary among a vast amount of other features, watch [keynote](https://www.apple.com/apple-events/event-stream/index.html) and [Platforms State of the Union](https://developer.apple.com/videos/play/wwdc2021/102) (a deeper dive into the new tools, technologies, and advances across Apple platforms) if you have missed the event.

## News

### App Store Review Guideline updates now available

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=dovxb62h)

## Fundamentals

### `class` and `struct`

YouTube [video](https://www.youtube.com/watch?v=zOeC7pxOIhk) by [Pedro Rojas](https://twitter.com/pitt500)

YouTube [video](https://www.youtube.com/watch?v=EhDML-fAqTM) (explaining classes) and YouTube [video](https://www.youtube.com/watch?v=3ox38NBBiNM) (explaining structs) by [Sean Allen](https://twitter.com/seanallen_dev)

### Beginner tips

YouTube [video](https://www.youtube.com/watch?v=4TTSZZkdOs4) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

### Debugging with breakpoints

YouTube [video](https://www.youtube.com/watch?v=qPWfOkHcKdU) by [Sean Allen](https://twitter.com/seanallen_dev)

### `UINavigationController`

YouTube [video](https://www.youtube.com/watch?v=LbAd2FIlnos) by [Sean Allen](https://twitter.com/seanallen_dev)

### Higher order functions

[article](https://medium.com/xebia-engineering/higher-order-functions-in-swift-c2f823f970fe) by [Manish Jain](https://www.linkedin.com/in/manish-jain-b5911620)

## Tutorials

### Firebase Dynamic Links

[Danijela Vrzan](https://twitter.com/dvrzan) in her [tutorial](https://www.raywenderlich.com/21376846-firebase-dynamic-links-getting-started) teaches how to implement deep linking on iOS using Firebase Dynamic Links. By the end of the tutorial you will be able to create, test, handle deep links if the application is not installed, and navigate to a specific view with `SwiftUI`.

### Building Your App Using Build Configurations and `.xcconfig`

[tutorial](https://www.raywenderlich.com/21441177-building-your-app-using-build-configurations-and-xcconfig) by [Saleh Albuga](https://twitter.com/salehalshami)

### Create a New Project - No Storyboard

YouTube [video tutorial](https://www.youtube.com/watch?v=Htn4h51BQsk) by [Sean Allen](https://twitter.com/seanallen_dev)

## Enhanced programming

### WWDC 2021 highlights

Apple Worldwide Developers Conference has concluded. Aftermath, [Apple](https://twitter.com/apple) provides [selection of documentation](https://developer.apple.com/documentation/New-Technologies-WWDC-2021) for new technologies, frameworks, and APIs introduced at WWDC 2021.

### `DocC` documentation in Xcode

Discover how you can use DocC to build and share documentation for Swift packages and frameworks. We'll show you how to begin generating documentation from your own code — or from third-party code you depend upon — and write and format it using Markdown. And we'll also take you through the export process, helping you generate DocC archives to share with the public.
[Apple](https://twitter.com/apple) announced [DocC](https://developer.apple.com/documentation/docc) framework, watch WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10166) by [Victoria Mitchell](<!--Couldn't find Victoria Mitchell's single social media account-->) and [Ethan Kusters](https://twitter.com/ethankusters)

[article](https://www.hackingwithswift.com/articles/238/how-to-document-your-project-with-docc) by [Paul Hudson](https://twitter.com/twostraws)

A tutorial expands your Swift framework or package’s reference documentation with interactive educational content. Create a tutorial by adding a table of contents and individual tutorial pages that walk the reader through coding exercises that teach your APIs.
[Apple](https://twitter.com/apple) [article](https://developer.apple.com/documentation/docc/building-an-interactive-tutorial)

### Streamline your localized strings

When you localize the text within your app, you can help make your app more accessible to a worldwide audience. Discover best practices for building your localization workflow, including how to write and format strings accurately, and learn how to prepare strings for localization in different languages using Xcode.
[Apple](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10221) by [Thomas Naudet](https://twitter.com/tomn94)

### Automatic Reference Counting in Swift

Learn about the basics of object lifetimes and ARC in Swift. Dive deep into what language features make object lifetimes observable, consequences of relying on observed object lifetimes and some safe techniques to fix them.
[Apple](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10216) by (she/her) [Meghana Gupta](https://www.linkedin.com/in/meghana-gupta)

### Swift concurrency

#### Meet `async`/`await` in Swift

Swift now supports asynchronous functions — a pattern commonly known as async/await. Discover how the new syntax can make your code easier to read and understand. Learn what happens when a function suspends, and find out how to adapt existing completion handlers to asynchronous functions.
[Apple](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10132) by [Nate Chandler](https://twitter.com/neightchan) and [Robert Widmann](https://twitter.com/CodaFi_)

#### Protect mutable state with Swift actors

Data races occur when two separate threads concurrently access the same mutable state. They are trivial to construct, but are notoriously hard to debug. Discover how you can stop these data races in their tracks with Swift actors, which help synchronize access to data in your code. Discover how actors work and how to share values between them. Learn about how actor isolation affects protocol conformances. And finally, meet the main actor, a new way of ensuring that your code always runs on the main thread when needed. To get the most out of this session, we recommend first watching [_Meet async/await in Swift_](#meet-asyncawait-in-swift).
[Apple](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10133) by [Dario Rexin](https://twitter.com/evonox) and [Doug Gregor](https://twitter.com/dgregor79)

#### Explore structured concurrency in Swift

When you have code that needs to run at the same time as other code, it's important to choose the right tool for the job. We'll take you through the different kinds of concurrent tasks you can create in Swift, show you how to create groups of tasks, and find out how to cancel tasks in progress. We'll also provide guidance on when you may want to use unstructured tasks. To get the most out of this session, we first recommend watching [_Meet async/await in Swift_](#meet-asyncawait-in-swift).
[Apple](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10134) by [Kavon Farvardin](https://twitter.com/call1cc) and [Joe Groff](https://twitter.com/jckarter)

#### Swift concurrency in action

Discover Swift concurrency in action: Follow along as we update an existing sample app. Get real-world experience with async/await, actors, and continuations. We'll also explore techniques for migrating existing code to Swift concurrency over time. To get the most out of this code-along, we recommend first watching [_Meet async/await in Swift_](#meet-asyncawait-in-swift) and [_Protect mutable state with Swift actors_](#protect-mutable-state-with-swift-actors).
[Apple](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10194) by [Ben Cohen](https://twitter.com/AirspeedSwift)

#### Behind the scenes of Swift concurrency

Dive into the details of Swift concurrency and discover how Swift provides greater safety from data races and thread explosion while simultaneously improving performance. We'll explore how Swift tasks differ from Grand Central Dispatch, how the new cooperative threading model works, and how to ensure the best performance for your apps. To get the most out of this session, we recommend first watching [_Meet async/await in Swift_](#meet-asyncawait-in-swift), [_Explore structured concurrency in Swift_](#explore-structured-concurrency-in-swift), and [_Protect mutable state with Swift actors_](#protect-mutable-state-with-swift-actors).
[Apple](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10254) by [Rokhini Prabhu](https://twitter.com/rokhinip) and [Varun Gandhi](https://www.linkedin.com/in/varungandhi15)

#### Structured concurrency

Doug Gregor from Apple joins John to discuss Swift 5.5’s new concurrency features in great detail. How do features like async/await and actors work under the hood, and how were those concepts adapted in order to feel right at home within Swift’s existing ecosystem? That, and much more, on this WWDC21 special episode of the show.
[Swift by Sundell](https://twitter.com/swiftbysundell) [John Sundell](https://twitter.com/johnsundell) [podcast](https://podcasts.apple.com/lv/podcast/swift-by-sundell/id1267161825?i=1000525108228) with special guest [Doug Gregor](https://twitter.com/dgregor79)

### Data formatters to display human-friendly content

Convert data into readable strings or Swift objects using formatters.
[Apple](https://twitter.com/apple) has a [sample code](https://developer.apple.com/documentation/foundation/formatter/displaying_human-friendly_content)

Save yourself time and frustration: When you display data in your app — including dates, times, measurements, names, lists, numbers, or strings — learn how to format it correctly and provide a great experience. We'll walk you through the Formatter APIs as well as how SwiftUI works with stringsdict, and show you how they can help do the heavy lifting of formatting data. Learn about best practices and how to avoid common mistakes.
[Apple](https://twitter.com/apple) WWDC20 session [video](https://developer.apple.com/videos/play/wwdc2020/10160) by [Karan Miśra](https://www.linkedin.com/in/karanmisra)

### Application capabilities

A capability grants the application access to an app service provided by Apple, such as iCloud, HealthKit, In-App Purchase, or push notifications. [Apple](https://twitter.com/apple) in an [article](https://developer.apple.com/documentation/Xcode/adding-capabilities-to-your-app) guide you through the process of adding application capabilities.

### Sign in with Apple user authentication 

Have you ever abbandoned the idea of trying out new application after realising sign-up is mandatory? I believe it's safe to claim that the majority of user's value their privacy, I've never felt comfortable in linking account to Google or Facebook and at the same time I do not wish to uneccessary expose my e-mail address. [Sign in with Apple](https://developer.apple.com/sign-in-with-apple) grants user's a choice to keep their e-mail address private. [Apple](https://twitter.com/apple) provides a [sample code](https://developer.apple.com/documentation/authenticationservices/implementing_user_authentication_with_sign_in_with_apple) on how to use [Authentication Services](https://developer.apple.com/documentation/authenticationservices) framework to provide users an interface to set up account and authenticates the user’s Apple ID with Sign in with Apple.

### Kotlin Multiplatform for iOS developers

Starting the 18<sup>th</sup> of February 2021 in Latvia ATC there have occured multiple _BrownBag_ sessions lead by [Mykhailo Dontsov](https://people.accenture.com/People/user/mykhailo.dontsov) and [Aleksejs Frolovs](https://people.accenture.com/People/user/aleksejs.frolovs) on the topic of [Kotlin Multiplatform](https://kotlinlang.org/lp/mobile). Kotlin Multiplatform enables you to use a single codebase for the business logic of multiple applications. At the same time, native user interfaces can be written in a platform-specific language. [Dinorah Tovar](https://twitter.com/DDinorahtovar) in her [presentation](https://vimeo.com/showcase/7769418/video/479639284) talks about how to get started with Kotlin Multiplatform for iOS.

### Scan and verify identity documents with `Core NFC`

Using [Core NFC](https://developer.apple.com/documentation/corenfc) framework you can detect Near Field Communication (NFC) tags and read messages that contain NFC Data Exchange Format (NDEF) data. [Maxim Tsvetkov](https://twitter.com/777maxxx777) gave a [presentation](https://vimeo.com/showcase/7769418/video/479350475) on what tool are available out-of-the-box, what data can be extracted, and how to verify document authenticity. 

### Data formatting in iOS 15

Up until recently, in order to format data we were creating and configuring different formatter classes, which are expensive operations (e.g., [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) has an [article](https://sarunw.com/posts/how-expensive-is-dateformatter) where he provides statistics on the cost of `DateFormatter` creation and property mutation). Hopefully, that will be tthe thing of the past wiith the introduuction of new formatting API. Read [article](https://nemecek.be/blog/106/new-approach-to-formatters-in-ios-15) by [Filip Němeček](https://twitter.com/nemecek_f).

### `UISheetPresentationController`

iOS 15 adds means to present view controller as a sheet. In an [article](https://nemecek.be/blog/108/meet-the-new-bottom-sheet-in-ios-15) [Filip Němeček](https://twitter.com/nemecek_f)
describes resizable sheet implementation and customization.
Alternatively, discover how to create layered and fine-tuned sheet experience in `UIKit` in [Apple's](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10063) by [Russell Ladd](https://www.linkedin.com/in/russellladd).

### Taking UIKit’s new button configuration API for a spin

With iOS 15, `UIButton` - one of the most fundamental UIKit classes, is getting a new system for configuring a button's appearance and behavior.
[John Sundell](https://twitter.com/johnsundell) has a first look [article](https://wwdcbysundell.com/2021/uikits-new-button-configuration-api) on how to use a new button configuration API.

### Core Data In Memory Store

In the [article](https://useyourloaf.com/blog/core-data-in-memory-store) by [Keith Harrison](https://twitter.com/kharrison), you can find out how to speed up your tests and `SwiftUI` previews by creating `Core Data` stack with an in-memory store.

### Swift 5.5

Swift 5.5 comes with a lot of improvements  – async/await, actors, throwing properties, and many more. [Paul Hudson](https://twitter.com/twostraws) in his [article](https://www.hackingwithswift.com/articles/233/whats-new-in-swift-5-5) walks through each of the changes with [code samples](https://www.whatsnewinswift.com/?from=5.4&to=5.5). 

### Quick Tip: Notifying Users of App Updates - For Free

[article](https://www.andyibanez.com/posts/quick-tip-notifying-users-app-updates-for-free) by [Andy Ibanez](https://twitter.com/AndyIbanezK)

### Why Should You Care about Manual Testing?

[article](https://pspdfkit.com/blog/2021/pragmatic-manual-testing) by [Tomáš Šurín](https://twitter.com/tomassurin)

### A first look at Swift’s new AttributedString

[article](https://wwdcbysundell.com/2021/a-first-look-at-attributed-string) by [John Sundell](https://twitter.com/johnsundell)

iOS 15 Brings Attributed Strings to SwiftUI [article](https://betterprogramming.pub/ios-15-attributed-strings-in-swiftui-markdown-271204bec5c1) by [Andrew Zheng](https://www.linkedin.com/in/aheze)

### Avoiding problematic cases when using Swift enums

[article](https://swiftbysundell.com/articles/avoiding-problematic-enum-cases-in-swift) by [John Sundell](https://twitter.com/johnsundell)

## Tools

### Xcode 13 is now available

Xcode 13 adds powerful new team development features, perfect for working with Xcode Cloud as well as with GitHub, Bitbucket, and GitLab collaboration features. Initiate, review, comment, and merge pull requests directly within Xcode. See your teammates’ comments right inside your code. And quickly compare any two versions of your code files.
[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=pq8tb86o)

[article](https://www.hackingwithswift.com/articles/236/whats-new-in-xcode-13) by [Paul Hudson](https://twitter.com/twostraws)

### Xcode Cloud

Xcode Cloud is a continuous integration and delivery service built into Xcode and designed expressly for Apple developers. It accelerates the development and delivery of high-quality apps by bringing together cloud-based tools that help you build apps, run automated tests in parallel, deliver apps to testers, and view and manage user feedback. Sign up for the beta today.
[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=uno5w59d)

### SF Symbols 3

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=30qc8oh0)
[SF Symbols 3](https://developer.apple.com/sf-symbols) beta now available
[guide](https://www.hackingwithswift.com/articles/237/complete-guide-to-sf-symbols) by [Paul Hudson](https://twitter.com/twostraws)

### Introducing `ShazamKit`

Enrich your app experience with audio recognition. Now you can match music to the millions of songs in Shazam's vast catalog or make any prerecorded audio recognizable by building your own custom catalog using audio from video, podcasts, and more.
[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=s0s8up0f)

**Building a Custom Catalog and Matching Audio**
[Apple](https://twitter.com/apple) provides [sample code](https://developer.apple.com/documentation/shazamkit/building_a_custom_catalog_and_matching_audio)

This sample code project is associated with WWDC21 session
**Create custom audio experiences with ShazamKit**
Bring custom audio matching to your app with ShazamKit. Discover how you can use Shazam's exact audio matching to recognize audio against any source when you use custom catalogs on device. Download our starter project and code along with the presenter as we guide you through the process of matching audio against a custom catalog. We'll also explore how easy it is to connect content across devices by building an interactive iOS app that can synchronize perfectly with video being streamed from a TV. To learn more about ShazamKit, check out "Explore ShazamKit" from WWDC21.
[Apple](https://twitter.com/apple) WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10045) by [Alex Telek](https://twitter.com/alextelek)

### Simulating adverse networking environments with Network Link Conditioner

StackOverflow [answer](https://stackoverflow.com/questions/2593971/iphone-simulator-simulate-a-slow-connection/27363671#27363671) by [Alan Hogan](https://twitter.com/b01dface)
Additionally, [article](https://nshipster.com/network-link-conditioner) by [Matthew Thomas Thompson](https://twitter.com/mattt)

## Tips

### `defer` in Swift

YouTube [video](https://www.youtube.com/watch?v=_VswqQqVlHo) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

### Custom `UIStackView` spacing

Twitter [post](https://twitter.com/sarunw/status/1403516739615404041) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)
Additionally, [article](https://sarunw.com/posts/custom-uistackview-spacing)

### Native async image decoding

Twitter [post](https://twitter.com/marcoarment/status/1401997686102970369) by [Marco Arment](https://twitter.com/marcoarment)

<br>
<p align="center">
<img width="35%" alt="Curators" src="curators.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit the <a href="https://github.com/esesmuedgars/IdeaKit/blob/issue2/README.md">previous issue</a>!
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
Subscribe to the <a href="https://blog.accenture.com/design">Riga Interactive blog</a> and follow the <a href="https://web.yammer.com/main/groups/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI1Nzg0ODAwNDYwOCJ9/all">Riga Interactive Yammer community</a> for further insightful content!
</p>
