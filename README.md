<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

![Issue](https://img.shields.io/badge/issue-1.0-informational.svg)

> Extra! Extra! Read all about it!
Under the Interactive umbrella, in Mobile we have a lot of different teams delivering various software applications. Recent activity indicates that we're shifting towards a more of a start-up mindset. From my observations there has been far less - I'm a developer, it's not my job to do anything besides programming - mentalitty. Individuals are creating my accenture posts, brown bags are held where knowledge is shared and Arkadi brags about C4. Like a set of companies within a bigger company. 
This is a pilot and viewing statistics will be used to determine the fate of the newsletter. It would be beneficial for me to dedicate all this time for.a single person to visit a pair of topics. As long as everyone reads a topic, I'd say we're good.

## Tutorials

### Swift Accelerate and vImage frameworks

[Accelerate](https://developer.apple.com/documentation/accelerate) framework provides Apple developers with a high-performance, energy-efficient computation library for large-scale mathematical or image-based calculations. It uses the vector-processing capabilities on CPUs to perform calculations quickly while maintaining efficient energy usage. Learn how to process images using Accelerate and vImage in a SwiftUI application in [tutorial](https://www.raywenderlich.com/19456196-swift-accelerate-and-vimage-getting-started) by [Bill Morefield](https://twitter.com/bmorefield).

### Re-creating Apple Photos layout and animations with compositional layout

During WWDC 2019, Apple introduced declarative `UICollectionViewCompositionalLayout` API with the goal to simplify the development process of complex layouts in our applications. Learn how to re-creating Apple Photos application layout and animations in [tutorial](https://nemecek.be/blog/86/re-creating-apple-photos-layout-animations-with-compositional-layout) by [Filip Němeček](https://github.com/nemecek-filip).

## Enhanced programming

### Writing high-performance Swift code

What makes a good user experience? I believe it's safe to say speed is one of the determining factors. We devote a noticeable portion of effort refactoring and optimizing our codebases, but did you know Swift documents have a comprehensive [list of tips](https://github.com/apple/swift/blob/main/docs/OptimizationTips.rst) on writing high-performant Swift code?

### Swift and Xcode tips

Adding `-com.apple.CoreData.ConcurrencyDebug 1` launch argument helps you to ensure you’re not violating Core Data’s threading rules. `defaults write http://com.apple.dt.Xcode IDEAdditionalCounterpartSuffixes -array-add "ViewModel" "View" "Screen"` makes Xcode's Assistant Editor aware for your view models, views, etc. And many more great Swift and Xcode tips have been shared by developer community on [Paul Hudson's](https://twitter.com/twostraws) Twitter [thread](https://twitter.com/twostraws/status/1364538061837791232).

### Lifecycle bahaviors

View controller propagates it's lifecycle methods to child view controllers, core rule [Bryan Irace](https://twitter.com/irace) used to write an [article](https://irace.me/lifecycle-behaviors) about reusable view controller’s lifecycle behaviors.

### GraphQL in Swift

We build applications of all shapes and sizes, but a common element is that they communicate with servers. Today, a handful of applications operate without some sort of internet connectivity. During rainy days, developers end up reusing web APIs which leads to oversaturated responses, not only does this impact 
performance, it could potentially be a security threat. In his [article](https://swiftwithmajid.com/2021/02/24/graphql-in-swift/) [Majid Jabrayilov](https://twitter.com/mecid) walks us through benefits and practice of GraphQL.
 
### Returning an Opaque Type

With the release of SwiftUI, Apple’s declarative UI framework, one feature that stood out when looking at the sample code was the `some` keyword. This keyword enables functions, subscripts, and computed properties to declare opaque return types. Read an [article](https://learnappmaking.com/some-swift-opaque-types-how-to) where [Reinder de Vries](https://twitter.com/reinder42) explains how to get rid of unpleasant compile-time error "Protocol '...' can only be used as a generic constraint because it has Self or associated type requirements".

### How Uber deals with large iOS application size

As application's codebase grows, so does it's size. Engineers at Uber dove beyond high-level language features and calling conventions and improved Swift binary size via like time optimization. Read an [article](https://eng.uber.com/how-uber-deals-with-large-ios-app-size) where [Milind Chabbi](https://twitter.com/ChabbiMilind), [Jin Lin](https://www.linkedin.com/in/jinlin) and [Raj Barik](https://github.com/rajbarik) describe how they reduced application sizes using advanced compiler technologies.

### Developing Xcode extensions

[Artem Novichkov](https://twitter.com/iosartem) wrote an [article](https://blog.artemnovichkov.com/developing-xcode-extensions-tips-and-tricks) about Xcode extension he created that let's you to create minimalistic code snippet images from selection with the help of [Ray.so](https://ray.so) tool.

### Dependency inversion as a driver to scale mobile development

Often functionality is shared accross applications be it data persistance, authorization or billing. But how are these dependencies managed in your codebase? Are they loosely coupled where dependency details are encapsulated within and dependency interfaces are used for cross-dependency communication? In his [article](https://developers.soundcloud.com/blog/dependency-inversion-as-a-driver-to-scale-mobile-development) [Firat Karatas](https://twitter.com/firatov) provides Swift examples as well as describes how to apply dependency inversion principle to frameworks.

### Distributing closed-source frameworks with Swift Package Manager

[Daniel Saidi](https://twitter.com/danielsaidi) wrote an [article](https://danielsaidi.com/blog/2021/02/15/distributing-closed-source-frameworks-with-spm) explaining how to set up project, distribute library and tackle problems along the way.

## Tools

### Homebrew 3.0.0

Homebrew 3.0.0 is now available with an official Apple Silicon support and a new bottle format in formulae. Read through a [list of changes](https://brew.sh/2021/02/05/homebrew-3.0.0) by [Mike McQuaid](https://twitter.com/MikeMcQuaid).

### Testing push notifications on the iOS simulator

When developing iOS applications push notifications are common functionality. Previously, to test out push notifications we depended on physical devices,  Xcode 11.4 Beta introduced a new way to simulate push notification on iOS simulator by adding `simctl` command. Read [article](https://sarunw.com/posts/testing-remote-push-notification-in-ios-simulator) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) and [article](https://www.avanderlee.com/workflow/testing-push-notifications-ios-simulator) by [Antoine van der Lee](https://twitter.com/twannl).

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
Thank you for taking the time to expand your knowledge.
<br>
<br>
Found a topic insightful? You can add your comments and open a discussion using conversation sidebar.
<br>
Help others by moving up items with highest ROI.
<br>
<br>
Reach out in case you spot any inconsistencies, errors or would like to make suggestions.
</p>
___


- [ ] How to Scan Images and Perform Text Recognition in SwiftUI Using VisionKit [tutorial](https://www.appcoda.com/swiftui-text-recognition) by [Gabriel Theodoropoulos](https://twitter.com/gabtheodor);
- [ ] DispatchGroup in Swift [article](https://dev.to/fmo91/dispatchgroup-in-swift-gg7) by [Fernando Martín Ortiz](https://twitter.com/fmo_91);
- [ ] Code Generating Swift Mocks with Sourcery [article](https://www.vadimbulavin.com/mocking-in-swift-using-sourcery) by [Vadim Bulavin](https://twitter.com/V8tr);
- [ ] Tuist Template: What is it and how to create them [article](https://sarunw.com/posts/tuist-template) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw);
- [ ] `[weak self]` is not always the solution [article](https://iosmith.com/weak-self-not-always-the-solution) by [Zsolt Kovács](https://www.linkedin.com/in/zs-kovacs);
- [ ] How to use `@autoclosure` in Swift to improve performance [article](https://www.avanderlee.com/swift/autoclosure) by [Antoine van der Lee](https://twitter.com/twannl).
