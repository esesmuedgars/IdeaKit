<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

![Issue](https://img.shields.io/badge/issue-1.0-informational.svg)

## Tutorials

[Accelerate](https://developer.apple.com/documentation/accelerate) framework provides Apple developers with a high-performance, energy-efficient computation library for large-scale mathematical or image-based calculations. It uses the vector-processing capabilities on CPUs to perform calculations quickly while maintaining efficient energy usage. Learn how to process images using Accelerate and vImage in a SwiftUI application in [tutorial](https://www.raywenderlich.com/19456196-swift-accelerate-and-vimage-getting-started) by [Bill Morefield](https://twitter.com/bmorefield).

During WWDC 2019, Apple introduced declarative `UICollectionViewCompositionalLayout` API with the goal to simplify the development process of complex layouts in our applications. Learn how to re-creating Apple Photos application layout and animations in [tutorial](https://nemecek.be/blog/86/re-creating-apple-photos-layout-animations-with-compositional-layout) by [Filip Němeček](https://github.com/nemecek-filip).

## Enhanced programming

What makes a good user experience? I believe it's safe to say speed is one of the determining factors. We devote a noticeable portion of effort refactoring and optimizing our codebases, but did you know Swift documents have a comprehensive [list of tips](https://github.com/apple/swift/blob/main/docs/OptimizationTips.rst#enabling-optimizations) on writing high-performant Swift code?

Adding `-com.apple.CoreData.ConcurrencyDebug 1` launch argument helps you to ensure you’re not violating Core Data’s threading rules. `defaults write http://com.apple.dt.Xcode IDEAdditionalCounterpartSuffixes -array-add "ViewModel" "View" "Screen"` makes Xcode's Assistant Editor aware for your view models, views, etc. And many more great Swift and Xcode tips have been shared by developer community on [Paul Hudson's](https://twitter.com/twostraws) Twitter [thread](https://twitter.com/twostraws/status/1364538061837791232).

## Tools

Homebrew 3.0.0 is now available with an official Apple Silicon support and a new bottle format in formulae. Read through a [list of changes](https://brew.sh/2021/02/05/homebrew-3.0.0) by [Mike McQuaid](https://twitter.com/MikeMcQuaid).

When developing iOS applications remote push notifications are common functionality. Previously, to test out remote push notifications we depended on physical devices,  Xcode 11.4 Beta introduced a new way to simulate remote push notification on iOS simulator by adding `simctl` command. Read [article](https://sarunw.com/posts/testing-remote-push-notification-in-ios-simulator) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) and [article](https://www.avanderlee.com/workflow/testing-push-notifications-ios-simulator) by [Antoine van der Lee](https://twitter.com/twannl).

[Andy Ibanez](https://twitter.com/AndyIbanezK) wrote an [article](https://www.andyibanez.com/posts/getting-to-know-the-simulator-better) about multiple simulator features provided by Xcode and the `xcrun simctl` tool.
