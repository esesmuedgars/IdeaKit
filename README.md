<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

![Issue](https://img.shields.io/badge/issue-1.0-informational.svg)

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

## Tools

### Homebrew 3.0.0

Homebrew 3.0.0 is now available with an official Apple Silicon support and a new bottle format in formulae. Read through a [list of changes](https://brew.sh/2021/02/05/homebrew-3.0.0) by [Mike McQuaid](https://twitter.com/MikeMcQuaid).

### Testing push notifications on the iOS simulator

When developing iOS applications push notifications are common functionality. Previously, to test out push notifications we depended on physical devices,  Xcode 11.4 Beta introduced a new way to simulate push notification on iOS simulator by adding `simctl` command. Read [article](https://sarunw.com/posts/testing-remote-push-notification-in-ios-simulator) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) and [article](https://www.avanderlee.com/workflow/testing-push-notifications-ios-simulator) by [Antoine van der Lee](https://twitter.com/twannl).

### Getting to know the simulator better

[Andy Ibanez](https://twitter.com/AndyIbanezK) wrote an [article](https://www.andyibanez.com/posts/getting-to-know-the-simulator-better) about multiple simulator features provided by Xcode and the `xcrun simctl` tool.

### Swift WebSockets

When it comes to WebSocket protocol, there are two main libraries - [Starscream](https://github.com/daltoniam/Starscream) and [URLSession](https://developer.apple.com/documentation/foundation/urlsession). [Matheus Cardoso](https://twitter.com/cardosodev) wrote an [article](https://dev.to/cardoso/swift-websockets-starscream-or-urlsession-in-2021-fck) comparing both of them.

<br>
<p align="center">
<img width="25%" alt="Curator" src="https://github.com/esesmuedgars/IdeaKit/blob/1.0/character.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
<br>
<br>
Reach out if you would like to contribute.
</p>
