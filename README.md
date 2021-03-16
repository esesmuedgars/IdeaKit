<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

![Issue](https://img.shields.io/badge/issue-pilot-informational.svg)

Extra! Extra! Read all about it!
<br>
Under the _Interactive_ umbrella, in the _Mobile_ division, we have multiple teams delivering various software applications. In my opinion, recent activity indicates that we're shifting towards a developer community mindset. There has been less of an "I'm a developer, it's not my job to do anything besides programming" mentality. [Artjoms Vorona](https://my.accenture.lv/users/artjoms_vorona) created several My Accenture posts about Apple developer topics, there are regular _Brown Bags_ where [Kristaps Knets](https://my.accenture.lv/users/kristaps_knets) introduced Unity, [Mykhailo Dontsov](https://my.accenture.lv/users/mykhailo_dontsov) introduced Kotlin Multiplatform. There are _Demo Days_ where [Arkadzi Daniyelian](https://my.accenture.lv/users/arkadzi_daniyelian), [Pavels Vetlugins](https://my.accenture.lv/users/pavels_vetlugins) and [Deniss Lapins](https://my.accenture.lv/users/deniss_lapins) had a chance to brag about [Channel 4](https://apps.apple.com/gb/app/all-4-watch-live-on-demand/id432494037). 

There is a lot of information available - release notes, newsletters, blog posts, articles, tutorials, presentations, podcasts, etc., but how to navigate such a vast amount of information? I'm excited to announce the first issue of _import IdeaKit - Swift Monthly Newsletter_ a list of hand-picked items about Swift that I commit to bundle and deliver at your digital doorstep every month.

**NB!** This is a pilot issue and you directly impact the newsletter's future outcome. Timeline, concept, and title are subject to change.

## Table of Contents

- [Tutorials](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#tutorials)
  * [Swift Accelerate and vImage frameworks](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#swift-accelerate-and-vimage-frameworks)
  * [Re-creating Apple Photos layout and animations with compositional layout](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#re-creating-apple-photos-layout-and-animations-with-compositional-layout)
  * [How to scan images and perform text recognition in SwiftUI using VisionKit](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#how-to-scan-images-and-perform-text-recognition-in-swiftui-using-visionkit)
- [Enhanced programming]()
  * [Writing high-performance Swift code](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#writing-high-performance-swift-code)
  * [Swift and Xcode tips](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#swift-and-xcode-tips)
  * [Lifecycle bahaviors](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#lifecycle-bahaviors)
  * [GraphQL in Swift](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#graphql-in-swift)
  * [Returning an Opaque Type](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#graphql-in-swift)
  * [How Uber deals with large iOS application size](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#how-uber-deals-with-large-ios-application-size)
  * [Developing Xcode extensions](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#how-uber-deals-with-large-ios-application-size)
  * [Dependency inversion as a driver to scale mobile development](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#dependency-inversion-as-a-driver-to-scale-mobile-development)
  * [Distributing closed-source frameworks with Swift Package Manager](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#distributing-closed-source-frameworks-with-swift-package-manager)
  * [Using `async`/`await` in SwiftUI](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#distributing-closed-source-frameworks-with-swift-package-manager)
  * [`[weak self]` is not always the solution](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#weak-self-is-not-always-the-solution)
  * [How to use `@autoclosure` in Swift to improve performance](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#weak-self-is-not-always-the-solution)
- [Tools](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#tools)
  * [Homebrew 3.0.0](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#homebrew-300)
  * [Testing push notifications on the iOS simulator](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#testing-push-notifications-on-the-ios-simulator)
  * [Getting to know the simulator better](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#getting-to-know-the-simulator-better)
  * [Swift WebSockets](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#swift-websockets)
  * [Localizing strings in a project](https://github.com/esesmuedgars/IdeaKit/blob/1.0/README.md#localizing-strings-in-a-project)

## Tutorials

### Swift Accelerate and vImage frameworks

[Accelerate](https://developer.apple.com/documentation/accelerate) framework provides Apple developers with a high-performance, energy-efficient computation library for large-scale mathematical or image-based calculations. It uses the vector-processing capabilities on CPUs to perform calculations quickly while maintaining efficient energy usage. Learn how to process images using Accelerate and vImage in a SwiftUI application in [tutorial](https://www.raywenderlich.com/19456196-swift-accelerate-and-vimage-getting-started) by [Bill Morefield](https://twitter.com/bmorefield).

### Re-creating Apple Photos layout and animations with compositional layout

During WWDC 2019, Apple introduced declarative `UICollectionViewCompositionalLayout` API intending to simplify the development process of complex layouts in our applications. Learn how to re-creating Apple Photos application layout and animations in [tutorial](https://nemecek.be/blog/86/re-creating-apple-photos-layout-animations-with-compositional-layout) by [Filip Němeček](https://github.com/nemecek-filip).

### How to scan images and perform text recognition in SwiftUI using VisionKit

Previously, we had to use [Tesseract OCR](https://github.com/gali8/Tesseract-OCR-iOS) library in order to implement optical character recognition in our applications. [Gabriel Theodoropoulos](https://twitter.com/gabtheodor) uses Apple's [Vision](https://developer.apple.com/documentation/vision) and [VisionKit](https://developer.apple.com/documentation/visionkit) frameworks in his detailed [tutorial](https://www.appcoda.com/swiftui-text-recognition) to build a text recognition application.

## Enhanced programming

### Writing high-performance Swift code

What makes a good user experience? I believe it's safe to say speed is one of the determining factors. We devote a noticeable portion of effort refactoring and optimizing our codebases, but did you know Swift documents have a comprehensive [list of tips](https://github.com/apple/swift/blob/main/docs/OptimizationTips.rst) on writing high-performant Swift code?

### Swift and Xcode tips

Adding `-com.apple.CoreData.ConcurrencyDebug 1` launch argument helps you to ensure you’re not violating Core Data’s threading rules. `defaults write http://com.apple.dt.Xcode IDEAdditionalCounterpartSuffixes -array-add "ViewModel" "View" "Screen"` makes Xcode's Assistant Editor aware for your view models, views, etc. And many more great Swift and Xcode tips have been shared by developer community on [Paul Hudson's](https://twitter.com/twostraws) Twitter [thread](https://twitter.com/twostraws/status/1364538061837791232).

### Lifecycle bahaviors

View controller propagates its lifecycle methods to child view controllers, core rule [Bryan Irace](https://twitter.com/irace) used to write an [article](https://irace.me/lifecycle-behaviors) about reusable view controller’s lifecycle behaviors.

### GraphQL in Swift

We build applications of all shapes and sizes, but a common element is that they communicate with servers. Today, a handful of applications operate without some sort of internet connectivity. During rainy days, developers end up reusing web APIs which leads to oversaturated responses, not only does this impact performance, it could potentially be a security threat. In his [article](https://swiftwithmajid.com/2021/02/24/graphql-in-swift/) [Majid Jabrayilov](https://twitter.com/mecid) walks us through the benefits and practice of GraphQL.
 
### Returning an Opaque Type

With the release of SwiftUI, Apple’s declarative UI framework, one feature that stood out when looking at the sample code was the `some` keyword. This keyword enables functions, subscripts, and computed properties to declare opaque return types. Read an [article](https://learnappmaking.com/some-swift-opaque-types-how-to) where [Reinder de Vries](https://twitter.com/reinder42) explains how to get rid of unpleasant compile-time error "Protocol '...' can only be used as a generic constraint because it has Self or associated type requirements".

### How Uber deals with large iOS application size

As an application's codebase grows, so does its size. Engineers at Uber dove beyond high-level language features and calling conventions and improved Swift binary size via like time optimization. Read an [article](https://eng.uber.com/how-uber-deals-with-large-ios-app-size) where [Milind Chabbi](https://twitter.com/ChabbiMilind), [Jin Lin](https://www.linkedin.com/in/jinlin) and [Raj Barik](https://github.com/rajbarik) describe how they reduced application sizes using advanced compiler technologies.

### Developing Xcode extensions

[Artem Novichkov](https://twitter.com/iosartem) wrote an [article](https://blog.artemnovichkov.com/developing-xcode-extensions-tips-and-tricks) about Xcode extension he created that lets you create minimalistic code snippet images from selection with the help of [Ray.so](https://ray.so) tool.

### Dependency inversion as a driver to scale mobile development

Often functionality is shared across applications be it data persistence, authorization, or billing. But how are these dependencies managed in your codebase? Are they loosely coupled where dependency details are encapsulated within and dependency interfaces are used for cross-dependency communication? In his [article](https://developers.soundcloud.com/blog/dependency-inversion-as-a-driver-to-scale-mobile-development) [Firat Karatas](https://twitter.com/firatov) provides Swift examples as well as describes how to apply dependency inversion principle to frameworks.

### Distributing closed-source frameworks with Swift Package Manager

[Daniel Saidi](https://twitter.com/danielsaidi) wrote an [article](https://danielsaidi.com/blog/2021/02/15/distributing-closed-source-frameworks-with-spm) explaining how to set up a project, distribute library, and tackle problems along the way.

### Using `async`/`await` in SwiftUI

[SE-0296](https://github.com/apple/swift-evolution/blob/main/proposals/0296-async-await.md) proposal has been implemented and will be released as a part of the future version of Swift. [Peter Friese](https://twitter.com/peterfriese) in his an [article](https://peterfriese.dev/async-await-in-swiftui) describes how to install the compiler toolchain, activate this new feature, and rewrite a callback-based code using `async`/`await`.

### `[weak self]` is not always the solution

Everyone is afraid of retain cycles when working with closures, but do all closures must have `[weak self]`? Read an [article](https://iosmith.com/weak-self-not-always-the-solution) by [Zsolt Kovács](https://www.linkedin.com/in/zs-kovacs) where he offers an alternative to `[weak self]`.

### How to use `@autoclosure` in Swift to improve performance

An `@autoclosure` can be a great solution to prevent unnecessary work if code isn’t used. [Antoine van der Lee](https://twitter.com/twannl) wrote an [article](https://www.avanderlee.com/swift/autoclosure) on how you can optimize your code using `@autoclosure`.

## Tools

### Homebrew 3.0.0

Homebrew 3.0.0 is now available with an official Apple Silicon support and a new bottle format in formulae. Read through a [list of changes](https://brew.sh/2021/02/05/homebrew-3.0.0) by [Mike McQuaid](https://twitter.com/MikeMcQuaid).

### Testing push notifications on the iOS simulator

When developing iOS applications push notifications are common functionality. Previously, to test out push notifications we depended on physical devices,  Xcode 11.4 Beta introduced a new way to simulate push notifications on iOS simulator by adding `simctl` command. Read [article](https://sarunw.com/posts/testing-remote-push-notification-in-ios-simulator) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) and [article](https://www.avanderlee.com/workflow/testing-push-notifications-ios-simulator) by [Antoine van der Lee](https://twitter.com/twannl).

### Getting to know the simulator better

[Andy Ibanez](https://twitter.com/AndyIbanezK) wrote an [article](https://www.andyibanez.com/posts/getting-to-know-the-simulator-better) about multiple simulator features provided by Xcode and the `xcrun simctl` tool.

### Swift WebSockets

When it comes to WebSocket protocol, there are two main libraries - [Starscream](https://github.com/daltoniam/Starscream) and [URLSession](https://developer.apple.com/documentation/foundation/urlsession). [Matheus Cardoso](https://twitter.com/cardosodev) wrote an [article](https://dev.to/cardoso/swift-websockets-starscream-or-urlsession-in-2021-fck) comparing both of them.

### Localizing strings in a project

[Guillermo Culkin](https://twitter.com/gmoraleda_) wrote an [article](http://moraleda.info/2021/02/19/localization) about centralizing your localization strigs and generating a namespace data class for in-application usage as a part of a build process.

<br>
<p align="center">
<img width="25%" alt="Curator" src="https://github.com/esesmuedgars/IdeaKit/blob/1.0/character.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge!
<br>
<br>
Found a topic insightful? You can add your comments and open a discussion using the conversation sidebar.
<br>
Help others by moving up items with the highest ROI!
<br>
<br>
Reach out in case you spot any inconsistencies or errors! Feedback and suggestions are also welcome.
</p>
