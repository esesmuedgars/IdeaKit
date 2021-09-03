<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 6 minute read

![Issue](https://img.shields.io/badge/issue-1.9-informational.svg)

Good morning and welcome back!

This very minute, my cryptocurrency portfolio is profitable, so I am leaving Accenture to go on an adventure. Thank you for choosing _import IdeaKit_ as your go-to source of information on anything and everything Swift!

I will not leave you hanging, when one door closes another one opens, therefore, to replace _import IdeaKit_ I suggest subscribing to three newsletters I enjoy reading the most — [iOS Dev Weekly](https://iosdevweekly.com) curated by [Dave Verwer](https://twitter.com/daveverwer), [Swift Weekly Brief](https://swiftweeklybrief.com) curated by [Kristaps Grinbergs](https://twitter.com/fassko), and [iOS Goodies](https://ios-goodies.com) curated by [Marius Constantinescu](https://twitter.com/marius_const).

Another step you can take to excel at your professional career is to create a Twitter account and follow active members of the Swift community, you can learn a great deal. If you'd like, you can also follow [me](https://twitter.com/esesmuedgars) where I don't post anything.

If you would fancy taking ownership of the newsletter, reach out to [Kaspars Auzarejs-Auzers](https://people.accenture.com/People/user/k.auzarejs-auzers), I've shared [guidelines](https://github.com/esesmuedgars/IdeaKit/blob/latest/CONTRIBUTING.md) necessary to recreate the newsletter with him.

Happy learning, au revoir!

## News

### Additional banking information required in App Store Connect

[Apple](https://twitter.com/Apple) in their news [article](https://developer.apple.com/news/?id=ep8chzr8) alerts that to avoid a potential, future interruption of payments from them, it is mandatory to add a valid address to the existent bank account information by the 22<sup>nd</sup> of October, 2021. Action requires Account Holders, Admins, or Finance role and can be done in the Agreements, Tax, and Banking section of the App Store Connect.

### Swift Package Collections

[Tom Doron](https://twitter.com/tomerdoron) had written a Swift blog [post](https://swift.org/blog/package-collections) announcing Package Collections addition to the Swift Package Manager in Swift 5.5, aiming to improve package discovery and to help select the right tool for the job.

<!--more-->

## Swift challenge

A couple of solutions to Swift challenge No. 2:

```swift
// MARK: Solution A

func checkIfFileExists(_ fileURL: URL) -> Bool {
    guard fileURL.isFileURL else {
        return false
    }
    
    return FileManager.default.fileExists(atPath: fileURL.path)
}

// MARK: Solution B

/**
 If you are unsure if the URL exists or not before opening it, just go ahead and open it, 
 as checking first will duplicate the amount of work the file system needs to perform. 
 However, if you do not need to open the file but verify if it exists using URL's 
 `checkResourceIsReachable`instance method will work for the vast majority of URLs and
 is recommended over getting a file system path and then checking with the file manager 
 if the file exists.
 */
func checkIfFileExists(_ fileURL: URL) -> Bool {
    guard fileURL.isFileURL else {
        return false
    }
    
    do {
        return try fileURL.checkResourceIsReachable()
    } catch {
        return false
    }
}
```

For the reason mentioned above, I will not be presenting you with a new challenge, instead, I encourage you to think of the ways how you could improve the software application you’re currently working on.

## Fundamentals

### Learning new application programming interfaces

Listen to [Empower Apps podcast](https://www.empowerapps.show) [episode](https://share.transistor.fm/s/31b2d4ab) with guest [Stewart Lynch](https://twitter.com/StewartLynch) as he shares, in his empirical experience, the best approaches to learning new application programming interfaces.

### iOS interview preparation

Even if you do not intend to terminate your employment agreement you can't avoid having technical interviews as you are considered for a new assignment. I believe it is important to keep your finger on the pulse of Swift developer recruitment, to know the most common questions, and best replies, and to be prepared to tackle any coding challenge. [Aryaman Sharda](https://twitter.com/aryamansharda) offers a YouTube [video series](https://www.youtube.com/watch?v=CBcuwRV4cPU&list=PLodDrxt4jmVDtxpFBpuPGk0X7BnB8lxBD) where he goes over different assessments presented at iOS developer role interviews.

### Observing properties in Swift

There are multiple ways to observe property changes, [Jesse Squires](https://twitter.com/jesse_squires) showcases a few of those options in his [article](https://www.jessesquires.com/blog/2021/08/08/different-ways-to-observe-properties-in-swift).

## Tutorials

### `SwiftGen` for iOS

Follow a [tutorial](https://www.raywenderlich.com/23709326-swiftgen-tutorial-for-ios) by [Andy Pereira](https://twitter.com/macandyp) to learn how to make your values of type `String` type-safe using [SwiftGen](https://github.com/SwiftGen/SwiftGen) (a tool that automatically generates Swift code for project's resources).

### One-time passcode text-input user interface

In a YouTube [video](https://www.youtube.com/watch?v=mHxAvSs914g), [Kyle Lee](https://twitter.com/kilo_loco) created one-time passcode (OTP) entry text field.

### The Composable Architecture (TCA)

[Maxim Smirnov](https://twitter.com/atimca) created a [tutorial](https://dev.to/atimca/the-composable-architecture-tutorial-29a9) demonstrating the concepts of [Composable Architecture](https://www.pointfree.co/collections/composable-architecture) by building a composable, modular, and testable product.

## Enhanced programming

### Creating and customizing views and controls

[Apple](https://twitter.com/Apple) provides [sample code](https://developer.apple.com/documentation/uikit/mac_catalyst/uikit_catalog_creating_and_customizing_views_and_controls) guiding you through several types of customizations you can make in your iOS applications.

### `AnyCancellable` in `Combine`

[Donny Wals](https://twitter.com/DonnyWals) wrote an [article](https://www.donnywals.com/what-exactly-is-a-combine-anycancellable) exploring the implementation of `AnyCancellable` and explained classes' objects that we retain for our subscriptions.

### The best practices of unit testing

[Arsen Gasparyan](https://twitter.com/ansenro) shares the practices he applies when writing unit tests in an [article](https://medium.com/revolut/best-practices-for-unit-testing-at-revolut-45428879ca07). He reckons that following those practices makes writing unit tests easy and fun. 

### `StaticString`

In an [article](https://swiftrocks.com/staticstring-in-swift), [Bruno Rocha](https://twitter.com/rockbruno_) traverses into how `StaticString` is built in the compiler and expresses an opinion if you should be using it.

### `#selector` and the responder chain

[Dominik Hauser](https://twitter.com/dasdom) wrote an [article](https://dasdom.dev/posts/selector-and-the-responder-chain) reminding everyone that there is a responder chain and that we can use it to react to button events.

### Reverse engineering `UIKit` to fix our hard-to-reproduce crash

[Adrian Kashivskyy](https://twitter.com/akashivskyy) in an [article](https://pspdfkit.com/blog/2021/reverse-engineering-uikit) shared what he had to go through to track down the root cause of a hard-to-reproduce crash and how did he tackle the error.

## Tools

### The importance of restarting Accenture workstations running macOS

[Brandon Peek](https://people.accenture.com/People/user/brandon.w.peek) published a [Mac Workstation Blog](https://blog.accenture.com/accenturemacworkstation) [post](https://blog.accenture.com/accenturemacworkstation/2021/09/02/the-importance-of-restarting-your-mac) reasoning why it is crucial to regularly reboot your Accenture-owned macOS device.

### Getting started with Amazon Web Services Amplify

Recently, many talents became certified cloud professionals, to those of you I would like to say mazel tov! View a YouTube [video](https://www.youtube.com/watch?v=mL54fosQphI) by [Kyle Lee](https://twitter.com/kilo_loco) as he guides viewers through initial steps with Amazon Web Services [Amplify](https://aws.amazon.com/amplify) (a set of tools (e.g., open-source framework, admin user interface, console) and services (e.g., static web hosting) to accelerate the development of software applications on Amazon Web Services).

### Create App Store screenshots effortlessly

In her [article](https://lickability.com/blog/automating-app-store-screenshots-with-fastlane-and-swiftui), [Daisy Ramos](https://twitter.com/daisyr317) shares how to 
automate screenshot creation for the application submission to the App Store process utilizing fastlane [snapshot](https://docs.fastlane.tools/actions/snapshot) and fastlane [frameit](https://docs.fastlane.tools/actions/frameit) actions.

## Tips

### Using `#function` for `String` values

In his Twitter [post](https://twitter.com/nicklockwood/status/1430429295994888198), [Nick Lockwood](https://twitter.com/nicklockwood) suggests using `#function` when implementing static properties of type `String` to avoid copy-paste errors.

### Overriding argument's default value

Watch a YouTube [video](https://www.youtube.com/watch?v=2h8eJq_dCh4) by [Vincent Pradeilles](https://twitter.com/v_pradeilles) as he illustrates the pitfall of overriding a default value of an argument of an overridden method.

### Compiler flags for Swift concurrency

[Ole Begemann](https://twitter.com/olebegemann) created a Twitter [post](https://twitter.com/olebegemann/status/1421144304127463427) stimulating to enable compiler flags that will identify unsafe constructs in case you are writing concurrent code.

### Checking if Mobile Data is enabled

[Filip Němeček](https://twitter.com/nemecek_f) in his direct [article](https://nemecek.be/blog/119/how-to-check-if-mobile-data-is-enabled-for-your-app) shares how to indicate whether an application can access cellular data.

### Why you shouldn't result to using conditional view modifiers

[Chris Eidhof](https://twitter.com/chriseidhof) described problems that conditional view modifies in `SwiftUI`  introduce. Read his [article](https://www.objc.io/blog/2021/08/24/conditional-view-modifiers) to understand why you should steer clear of implementing them.

### Spell-checking in Xcode

[Sarun Wongpatcharapakornand](https://twitter.com/sarunw) wrote a 2-minute [article](https://sarunw.com/posts/spell-checking-in-xcode) educating how to enable and use Xcode's hidden feature - spell-checking.

<br>
<p align="center">
<img width="25%" alt="Curator Edgars Vanags" src="curator_edgars.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit the <a href="https://github.com/esesmuedgars/IdeaKit/blob/issue5/README.md">previous issue</a>!
<br>
<br>
Found a topic insightful? You can add your comments and open a discussion using the comment section below.
<br>
Help others improve their Swift knowledge by liking and sharing this post.
<br>
<br>
Reach out in case you spot any errors! Feedback is also welcome.
<br>
<br>
Subscribe to the <a href="https://blog.accenture.com/design">Baltic Interactive blog</a> and follow the <a href="https://web.yammer.com/main/groups/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI1Nzg0ODAwNDYwOCJ9/all">Riga Interactive Yammer community</a> for further insightful content!
</p>
