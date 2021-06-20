<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.6-informational.svg)

Good morning and welcome to _import IdeaKit_!

Shout-out to [Artjoms Vorona](https://people.accenture.com/People/user/artjoms.vorona) for his contribution to 3<sup>rd</sup> issue of the newsletter! The backlog has plenty more unassigned user stories, consider this as an invitation to join the team. All aboard!

Congratulations to all Midyear Cycle promotees, prominently to the Latvia ATC iOS developers - [Artjoms Vorona](https://people.accenture.com/People/user/artjoms.vorona), [Kristaps Knets](https://people.accenture.com/People/user/kristaps.knets), and [Armands Mikanovskis-Mikalovskis](https://people.accenture.com/People/user/armands.mikanovskis)! 👏🏼

During [WWDC21](https://developer.apple.com/wwdc21) [Apple](https://twitter.com/Apple) announced [Xcode Cloud](https://developer.apple.com/xcode-cloud), concurrency in Swift, Universal Control, tab groups in Safari, live text, mentions and tags in Notes, focus mode, and notification summary among a vast amount of other features, watch [keynote](https://www.apple.com/apple-events/event-stream/index.html) and [Platforms State of the Union](https://developer.apple.com/videos/play/wwdc2021/102) (a deeper dive into the new tools, technologies, and advances across Apple platforms) if you have missed the event.

Happy learning!

## News

### Swift 5.5

Swift 5.5 comes with a lot of changes providing major new language features that deliver power and safety to the Swift developers. [Paul Hudson](https://twitter.com/twostraws) in his [article](https://www.hackingwithswift.com/articles/233/whats-new-in-swift-5-5) offers [code samples](https://www.whatsnewinswift.com/?from=5.4&to=5.5) of all of the main changes.

### App Store Review Guideline updates

"Apps supporting account creation must also offer account deletion" and other additions to the App Store Review Guidelines you can get familiar with in [Apple's](https://twitter.com/apple) news [article](https://developer.apple.com/news/?id=dovxb62h).

## Fundamentals

### `class` and `struct`

In case I was your _TechBuddy_ (also known as a technical mentor) during your iOS internship you most likely have received feedback to use structures instead of classes for data models when decoding HTTP responses. [Pedro Rojas](https://twitter.com/pitt500) in his YouTube [video](https://www.youtube.com/watch?v=zOeC7pxOIhk) compares both of them and points out the differences.
Additionally, [Sean Allen](https://twitter.com/seanallen_dev) offers YouTube [video](https://www.youtube.com/watch?v=EhDML-fAqTM) explaining classes and YouTube [video](https://www.youtube.com/watch?v=3ox38NBBiNM) explaining structures.

### Tips to improve your Swift code

In his YouTube [video](https://www.youtube.com/watch?v=4TTSZZkdOs4), [Vincent Pradeilles](https://twitter.com/v_pradeilles) advises increasing the quality of your Swift code. It is also recommended that you refer to any Swift style guide (e.g., Airbnb Swift [style guide](https://github.com/airbnb/swift), LinkedIn Swift [style guide](https://github.com/linkedin/swift-style-guide), raywenderlich.com Swift [style guide](https://github.com/raywenderlich/swift-style-guide), or Google Swift [style guide](https://google.github.io/swift)) to have a clear, consistent, and precise codebase.

### Debugging with breakpoints

Breakpoints are locations in your source code where the Xcode debugger will pause so that you can inspect the state of your program and step through your code to pinpoint the root cause of an issue or isolate a bug. [Sean Allen](https://twitter.com/seanallen_dev) in his YouTube [video](https://www.youtube.com/watch?v=qPWfOkHcKdU) exhibits how to debug an application with the help of breakpoints.

### `UINavigationController`

Watch a YouTube [video](https://www.youtube.com/watch?v=LbAd2FIlnos) by [Sean Allen](https://twitter.com/seanallen_dev) where he explains what navigation controllers are, how do they work, and how to customize a navigation controller to match your application's look and feel.

### Higher-order functions

[Manish Jain](https://www.linkedin.com/in/manish-jain-b5911620) wrote a short [article](https://medium.com/xebia-engineering/higher-order-functions-in-swift-c2f823f970fe) educating about some of the most common higher-order functions such as `map(_:)`, `filter(_:)`, and `contains(_:)`.

## Tutorials

### Firebase Dynamic Links

[Danijela Vrzan](https://twitter.com/dvrzan) in her [tutorial](https://www.raywenderlich.com/21376846-firebase-dynamic-links-getting-started) teaches how to implement deep linking on iOS using Firebase Dynamic Links. By the end of the tutorial you will be able to create, test, handle deep links if the application is not installed, and navigate to a specific view with `SwiftUI`.

### Building your application using Xcode build configuration files

[Saleh Albuga](https://twitter.com/salehalshami) created a comprehensive [tutorial](https://www.raywenderlich.com/21441177-building-your-app-using-build-configurations-and-xcconfig) educating how to use Xcode build configuration files, manage build settings across multiple environments and targets, and access build settings from source code.
Additionally, study [article](https://nshipster.com/xcconfig) by [Matthew Thomas Thompson](https://twitter.com/mattt) where he encourages developers to extract their applications' configurations to `.xcconfig` files.

### Create a new Xcode project without storyboards

Concise YouTube [video tutorial](https://www.youtube.com/watch?v=Htn4h51BQsk) by [Sean Allen](https://twitter.com/seanallen_dev) demonstrating how to create a fresh Xcode project with programmatically initialized `UIViewController` subclasses in iOS 13.0+.

## Enhanced programming

### WWDC 2021 highlights

WWDC 2021 has concluded, [Apple](https://twitter.com/apple) has followed up with a [selection of documentation](https://developer.apple.com/documentation/New-Technologies-WWDC-2021) for new technologies, frameworks, and APIs introduced at the event.

### `DocC` documentation in Xcode

[Apple](https://twitter.com/apple) has announced the [DocC](https://developer.apple.com/documentation/docc) framework, watch the WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10166) in which software engineers [Victoria Mitchell](<!--Couldn't find Victoria Mitchell's single social media account-->) and [Ethan Kusters](https://twitter.com/ethankusters) give you an introduction to the new Swift package and framework documentation compiler available in Xcode 13.
In [Paul Hudson's](https://twitter.com/twostraws) [article](https://www.hackingwithswift.com/articles/238/how-to-document-your-project-with-docc), you can walk through the fundamentals of
generating and exporting documentation for a framework.  
Furthermore, [Apple](https://twitter.com/apple) provides an [article](https://developer.apple.com/documentation/docc/building-an-interactive-tutorial) explaining how to build an interactive tutorial for your Swift package or framework.

### Streamline your localized strings

Discover best practices for building your localization workflow, including how to write and format strings accurately, and learn how to prepare strings for localization in different languages using Xcode in [Apple's](https://twitter.com/apple) WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10221) by [Thomas Naudet](https://twitter.com/tomn94).

### Automatic Reference Counting in Swift

[Meghana Gupta](https://www.linkedin.com/in/meghana-gupta) educates developers about the basics of object lifetimes and Automatic Reference Counting (ARC) in Swift. Learn what language features make object lifetimes observable, what are the consequences of relying on observed object lifetimes, and some techniques to avoid them in [Apple's](https://twitter.com/apple) WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10216).

### Swift concurrency

#### Meet `async`/`await` in Swift

Swift beta supports asynchronous functions. Discover how to make your codebase more readable and easier to understand, learn what happens once a function suspends itself, and find out how to adapt existing completion handlers to asynchronous functions in [Apple's](https://twitter.com/apple) WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10132) by [Nate Chandler](https://twitter.com/neightchan) and [Robert Widmann](https://twitter.com/CodaFi_).

#### Protect mutable state with Swift actors

Data races occur when two separate threads concurrently access the same mutable state. In [Apple's](https://twitter.com/apple) WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10133) (to get the most out of the session, they first recommend watching [_Meet `async`/`await` in Swift_](#meet-asyncawait-in-swift)) [Dario Rexin](https://twitter.com/evonox) and [Doug Gregor](https://twitter.com/dgregor79) instruct how to synchronize access to data and prevent data races with Swift actors. Learn how actors work, how to share values between 'em, as well as how actor isolation affects protocol conformances.

#### Explore structured concurrency in Swift

Watch WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10134) (to get the most out of the session, it is recommended first watching [_Meet `async`/`await` in Swift_](#meet-asyncawait-in-swift)) by [Apple](https://twitter.com/apple) where [Kavon Farvardin](https://twitter.com/call1cc) and [Joe Groff](https://twitter.com/jckarter) take you through the different kinds of concurrent tasks developers can create in Swift, show how to create groups of tasks, and share how to cancel running tasks.

#### Swift concurrency in action

Follow along and obtain real-world experience with `async`/`await`, actors, and continuations as [Ben Cohen](https://twitter.com/AirspeedSwift) updates an existing sample application in WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10194) (it is recommended viewing [_Meet `async`/`await` in Swift_](#meet-asyncawait-in-swift) and [_Protect mutable state with Swift actors_](#protect-mutable-state-with-swift-actors) before participating in this code-along) by [Apple](https://twitter.com/apple).

#### Behind the scenes of Swift concurrency

Explore how Swift tasks differ from Grand Central Dispatch (GCD), how the cooperative threading model works, and how to ensure the best performance for your applications in [Apple's](https://twitter.com/apple) WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10254) (to get the most out of the session, they recommend first watching [_Meet `async`/`await` in Swift_](#meet-asyncawait-in-swift), [_Explore structured concurrency in Swift_](#explore-structured-concurrency-in-swift), and [_Protect mutable state with Swift actors_](#protect-mutable-state-with-swift-actors)) by [Rokhini Prabhu](https://twitter.com/rokhinip) and [Varun Gandhi](https://www.linkedin.com/in/varungandhi15).

#### Structured concurrency

[Doug Gregor](https://twitter.com/dgregor79) had joined [John Sundell](https://twitter.com/johnsundell) at [Swift by Sundell](https://twitter.com/swiftbysundell) podcast to discuss new concurrency features in great detail. Listen to their conversation about inner-workings of asynchronous functions and Swift actors in an [episode](https://podcasts.apple.com/lv/podcast/swift-by-sundell/id1267161825?i=1000525108228).

### Application capabilities

A capability grants the application access to an app service provided by Apple, such as iCloud, HealthKit, In-App Purchase, or push notifications. [Apple](https://twitter.com/apple) in an [article](https://developer.apple.com/documentation/Xcode/adding-capabilities-to-your-app) guides you through the process of adding application capabilities.

### Sign in with Apple user authentication 

Have you ever abandoned the idea of trying out a new application after realizing sign-up is mandatory? I believe it's safe to claim that the majority of users value their privacy, I've never felt comfortable in linking my account to Google or Facebook, and at the same time, I do not wish to unnecessarily expose my e-mail address. [Sign in with Apple](https://developer.apple.com/sign-in-with-apple) grants user's a choice to keep their e-mail address private. [Apple](https://twitter.com/apple) provides a [sample code](https://developer.apple.com/documentation/authenticationservices/implementing_user_authentication_with_sign_in_with_apple) on how to use the [Authentication Services](https://developer.apple.com/documentation/authenticationservices) framework to provide users an interface to set up an account and authenticates the user’s Apple ID with Sign in with Apple.

### Kotlin Multiplatform for iOS developers

Starting the 18<sup>th</sup> of February 2021 in Latvia ATC there have occurred multiple _BrownBag_ sessions lead by [Mykhailo Dontsov](https://people.accenture.com/People/user/mykhailo.dontsov) and [Aleksejs Frolovs](https://people.accenture.com/People/user/aleksejs.frolovs) on the topic of [Kotlin Multiplatform](https://kotlinlang.org/lp/mobile). Kotlin Multiplatform enables you to use a single codebase for the business logic of multiple applications. At the same time, native user interfaces can be written in a platform-specific language. [Dinorah Tovar](https://twitter.com/DDinorahtovar) in her [presentation](https://vimeo.com/showcase/7769418/video/479639284) talks about how to get started with Kotlin Multiplatform for iOS.

### Scan and verify identity documents with `Core NFC`

Using the [Core NFC](https://developer.apple.com/documentation/corenfc) framework you can detect Near Field Communication (NFC) tags and read messages that contain NFC Data Exchange Format (NDEF) data. [Maxim Tsvetkov](https://twitter.com/777maxxx777) gave a [presentation](https://vimeo.com/showcase/7769418/video/479350475) on what tools are available out-of-the-box, what data can be extracted, and how to verify document authenticity.

### Data formatters to display human-friendly content

Learn about the best practices of converting data into readable strings or Swift objects and how to avoid common mistakes using formatters in [Apple's](https://twitter.com/apple) [sample code](https://developer.apple.com/documentation/foundation/formatter/displaying_human-friendly_content) (sample code is associated with WWDC20 [session](https://developer.apple.com/videos/play/wwdc2020/10160) where [Karan Miśra](https://www.linkedin.com/in/karanmisra) walks viewers through the formatter APIs as well as how `SwiftUI` works with `.stringsdict` files.
Further, learn about modern formatter API in [_Data formatting in iOS 15_](#data-formatting-in-ios-15).

### Data formatting in iOS 15

Up until recently, to format data we were creating and configuring different formatter classes (highlighted in [_Data formatters to display human-friendly content_](#data-formatters-to-display-human-friendly-content)), which are expensive operations (e.g., [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) has an [article](https://sarunw.com/posts/how-expensive-is-dateformatter) where he provides statistics on the cost of `DateFormatter` creation and property mutation). Hopefully, that will be the thing of the past with the introduction of a new formatter API. Read [article](https://nemecek.be/blog/106/new-approach-to-formatters-in-ios-15) by [Filip Němeček](https://twitter.com/nemecek_f).

### `UISheetPresentationController`

iOS 15 adds the means to present the view controller as a sheet. In an [article](https://nemecek.be/blog/108/meet-the-new-bottom-sheet-in-ios-15), [Filip Němeček](https://twitter.com/nemecek_f) describes resizable sheet implementation and customization.
Alternatively, discover how to create layered and fine-tuned sheet experience in `UIKit` in [Apple's](https://twitter.com/apple) WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10063) by [Russell Ladd](https://www.linkedin.com/in/russellladd).

### iOS 15 `UIButton` configuration API

iOS 15 enhances how we configure `UIButton` appearance and behavior with a new API that takes many common and previously time-consuming layout and styling tasks and turns them into one-line configuration properties. [John Sundell](https://twitter.com/johnsundell) in his [article](https://wwdcbysundell.com/2021/uikits-new-button-configuration-api) has a first look at how to use the new button configuration API.
Alternatively, [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) has written an [article](https://sarunw.com/posts/new-way-to-style-uibutton-in-ios15) claiming that, with `UIButton.Configuration`, we are not obligated to subclass `UIButton` anymore.

### Core Data with `NSInMemoryStoreType`

In the [article](https://useyourloaf.com/blog/core-data-in-memory-store) by [Keith Harrison](https://twitter.com/kharrison), you can find out how to speed up your tests and `SwiftUI` previews by creating a `Core Data` stack with an in-memory store.

### Notifying users of application updates

What percentage of your userbase is on the latest version of the application you are working on? [Andy Ibanez](https://twitter.com/AndyIbanezK) claims that users may not be updating as often as you believe and shares his solution to let them know a new version is available without being invasive in an [article](https://www.andyibanez.com/posts/quick-tip-notifying-users-app-updates-for-free).

### Why should you care about manual testing?

[Tomáš Šurín](https://twitter.com/tomassurin) gives his perspective on manual testing as another tool that, when put to good use, can improve product quality significantly in his [article](https://pspdfkit.com/blog/2021/pragmatic-manual-testing).

### A first look at `AttributedString`

[John Sundell](https://twitter.com/johnsundell) has written an [article](https://wwdcbysundell.com/2021/a-first-look-at-attributed-string) comparing `NSAttributedString` and `AttributedString` implementation and new type's integration with `SwiftUI`. Spoiler, `AttributedString` has built-in Markdown (lightweight markup language for creating formatted text using a plain-text editor) support.
Additionally, take a look at the [article](https://betterprogramming.pub/ios-15-attributed-strings-in-swiftui-markdown-271204bec5c1) by [Andrew Zheng](https://www.linkedin.com/in/aheze) where he supplies multiple examples on working with `AttributedString`.

### Avoiding problematic cases when using enumerations

[John Sundell](https://twitter.com/johnsundell) wrote an [article](https://swiftbysundell.com/articles/avoiding-problematic-enum-cases-in-swift) warning about certain `enum` cases that can arguably be good to avoid.

### Modern `RxSwift` architectures

In an [article](https://academy.realm.io/posts/try-swift-nyc-2017-krunoslav-zaher-modern-rxswift-architectures), [Krunoslav Zaher](https://twitter.com/KrunoslavZaher) shares his experience solving cycling data dependencies with `RxFeedback` architecture.
Alternatively, you can watch the [presentation](https://www.youtube.com/watch?v=qZZTYIwrhsY) he gave at a conference.

## Tools

### Xcode 13

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=pq8tb86o) announced [Xcode 13 beta](https://developer.apple.com/services-account/download?path=/Developer_Tools/Xcode_13_beta/Xcode_13_beta.xip). Review several of the IDE's latest key features, source editor improvements, and performance enhancements in an [article](https://www.hackingwithswift.com/articles/236/whats-new-in-xcode-13) by [Paul Hudson](https://twitter.com/twostraws).

### Xcode Cloud

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=uno5w59d) opened a sign-up for Xcode Cloud (continuous integration and delivery beta service) that accelerates the development and delivery of applications by bringing together cloud-based tools that help developers to run automated tests in parallel, deliver applications to testers, and view and manage user feedback.

### SF Symbols 3

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=30qc8oh0) declared the availability of [SF Symbols 3](https://developer.apple.com/sf-symbols) beta.
Additionally, visit [guide](https://www.hackingwithswift.com/articles/237/complete-guide-to-sf-symbols) in which [Paul Hudson](https://twitter.com/twostraws) demonstrates techniques how to interact with SF Symbols 3 in both `UIKit` and `SwiftUI`.

### Introducing `ShazamKit`

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=s0s8up0f) announced `ShazamKit`. The framework uses a unique acoustic signature of an audio recording to find a match to the millions of songs in a vast catalog or to make any prerecorded audio recognizable by building a custom catalog using audio from video, podcasts, etc. Apple provides beta [sample code](https://developer.apple.com/documentation/shazamkit/building_a_custom_catalog_and_matching_audio) on matching the audio to a custom reference signature and associated metadata (sample code is associated with WWDC21 [session](https://developer.apple.com/videos/play/wwdc2021/10045) where [Alex Telek](https://twitter.com/alextelek) guides viewers through the process of using exact audio matching to recognize audio against a custom catalog).

### Simulating adverse networking environments with Network Link Conditioner

StackOverflow [answer](https://stackoverflow.com/questions/2593971/iphone-simulator-simulate-a-slow-connection/27363671#27363671) by [Alan Hogan](https://twitter.com/b01dface)
Additionally, [article](https://nshipster.com/network-link-conditioner) by [Matthew Thomas Thompson](https://twitter.com/mattt)

### Xcode build settings

A convenient [online reference](https://xcodebuildsettings.com) of available build settings for Xcode projects maintained by [Matthew Thomas Thompson](https://twitter.com/mattt).

## Tips

### `defer` in Swift

[Vincent Pradeilles](https://twitter.com/v_pradeilles) in his YouTube [video](https://www.youtube.com/watch?v=_VswqQqVlHo) offers an exemplary use case for `defer` keyword.

### Confusing Swift syntaxes

[Vincent Pradeilles](https://twitter.com/v_pradeilles) created a YouTube [video](https://www.youtube.com/watch?v=p3qdi6KyzDk) to underscore multiple valid but counter-intuitive Swift syntaxes that you too, most likely, have never come across before.

### Custom `UIStackView` spacing

Twitter [post](https://twitter.com/sarunw/status/1403516739615404041) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) calls to our attention that to apply custom spacing between arranged subviews there hasn't been the need to add additional  `UIStackView` as arranged subview since iOS 11 which extended `UIStackView` with `setCustomSpacing(_:after:)` instance method.
Additionally, read an [article](https://sarunw.com/posts/custom-uistackview-spacing) where he features few caveats.

### `UIKit` asynchronous image decoding

I was delighted to read a Twitter [post](https://twitter.com/marcoarment/status/1401997686102970369) by [Marco Arment](https://twitter.com/marcoarment) in which he shared with his find — native asynchronous image decoding and creation of image thumbnails.

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
