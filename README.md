<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.6-informational.svg)

Good morning and welcome to _import IdeaKit_!

Shout-out to [Artjoms Vorona](https://people.accenture.com/People/user/artjoms.vorona) for his contribution to 3<sup>rd</sup> issue of the newsletter! The backlog has plenty more unassigned user stories, consider this as an invitation to join the team.

Congratulations to all Midyear Cycle promotees, prominently to the Latvia ATC iOS developers - [Artjoms Vorona](https://people.accenture.com/People/user/artjoms.vorona), [Kristaps Knets](https://people.accenture.com/People/user/kristaps.knets), and [Armands Mikanovskis-Mikalovskis](https://people.accenture.com/People/user/armands.mikanovskis)! 👏🏼

During [WWDC21](https://developer.apple.com/wwdc21) [Apple](https://twitter.com/Apple) announced [Xcode Cloud](https://developer.apple.com/xcode-cloud), concurrency in Swift, Universal Control, tab groups in Safari, live text, mentions and tags in Notes, focus mode, and notification summary among a vast amount of other features, watch [keynote](https://www.apple.com/apple-events/event-stream/index.html) if you have missed the event.

## News

## Fundamentals

### Beginner tips

YouTube [video](https://www.youtube.com/watch?v=4TTSZZkdOs4) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

## Tutorials

### Firebase Dynamic Links

[Danijela Vrzan](https://twitter.com/dvrzan) in her [tutorial](https://www.raywenderlich.com/21376846-firebase-dynamic-links-getting-started) teaches how to implement deep linking on iOS using Firebase Dynamic Links. By the end of the tutorial you will be able to create, test, handle deep links if the application is not installed, and navigate to a specific view with `SwiftUI`.

## Enhanced programming

### `DocC` documentation in Xcode

Discover how you can use DocC to build and share documentation for Swift packages and frameworks. We'll show you how to begin generating documentation from your own code — or from third-party code you depend upon — and write and format it using Markdown. And we'll also take you through the export process, helping you generate DocC archives to share with the public.
[Apple](https://twitter.com/apple) announced [DocC](https://developer.apple.com/documentation/docc) framework, watch WWDC21 session [video](https://developer.apple.com/videos/play/wwdc2021/10166) by [Victoria Mitchell](<!--Couldn't find Victoria Mitchell's any social media account-->) and [Ethan Kusters](https://twitter.com/ethankusters)

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

### Kotlin Multiplatform for iOS developers

Vimeo [video](https://vimeo.com/showcase/7769418/video/479639284) by (she/her) [Dinorah Tovar](https://twitter.com/DDinorahtovar)

### Scan and verify identity documents with `Core NFC`

[Core NFC](https://developer.apple.com/documentation/corenfc) framework
Vimeo [video](https://vimeo.com/showcase/7769418/video/479350475) by [Maxim Tsvetkov](https://twitter.com/777maxxx777)

### Data formatters to display human-friendly content

Convert data into readable strings or Swift objects using formatters.
[Apple](https://twitter.com/apple) has a [sample code](https://developer.apple.com/documentation/foundation/formatter/displaying_human-friendly_content)

Save yourself time and frustration: When you display data in your app — including dates, times, measurements, names, lists, numbers, or strings — learn how to format it correctly and provide a great experience. We'll walk you through the Formatter APIs as well as how SwiftUI works with stringsdict, and show you how they can help do the heavy lifting of formatting data. Learn about best practices and how to avoid common mistakes.
[Apple](https://twitter.com/apple) WWDC20 session [video](https://developer.apple.com/videos/play/wwdc2020/10160) by [Karan Miśra](https://www.linkedin.com/in/karanmisra)

## Tools

### Simulating adverse networking environments with Network Link Conditioner

StackOverflow [answer](https://stackoverflow.com/questions/2593971/iphone-simulator-simulate-a-slow-connection/27363671#27363671) by [Alan Hogan](https://twitter.com/b01dface)
Additionally, [article](https://nshipster.com/network-link-conditioner) by [Matthew Thomas Thompson](https://twitter.com/mattt)

### SF Symbols 3

[SF Symbols 3](https://developer.apple.com/sf-symbols) beta
[guide](https://www.hackingwithswift.com/articles/237/complete-guide-to-sf-symbols) by [Paul Hudson](https://twitter.com/twostraws)

## Tips

### `defer` in Swift

YouTube [video](https://www.youtube.com/watch?v=_VswqQqVlHo) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

### Custom `UIStackView` spacing

Twitter [post](https://twitter.com/sarunw/status/1403516739615404041) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)
Additionally, [article](https://sarunw.com/posts/custom-uistackview-spacing)

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
