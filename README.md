<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 11 minute read

![Issue](https://img.shields.io/badge/issue-1.5-informational.svg)

Greetings!

Another issue of the newsletter brings us another improvement. To spotlight helpful Twitter posts and minute articles with great bits of advice the _[Tips](#tips-)_ section has been added to the newsletter.

As we are a single step away from summer and nature is flourishing, developers also use energy from the sun to fuel their creativity and increase their output, ahead of you is an extensive list of great sources of information.

Happy learning!

## News

### Swift 5.4

[Ted Kremenek](https://twitter.com/tkremenek) in his Swift blog [post](https://swift.org/blog/swift-5-4-released) announced the official release of Swift 5.4, alternatively get familiar with new Swift language features by reviewing [code examples](https://www.whatsnewinswift.com/?from=5.3&to=5.4) created by [Paul Hudson](https://twitter.com/twostraws), and main changes to Swift Package Manager are described by [Federico Zanetello](https://twitter.com/zntfdr) in his [article](https://www.fivestars.blog/articles/spm-5-4).

### Updates to age rating settings in App Store Connect

An age rating is a required application information property used by the parental controls on the App Store. [Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=fwpxy9kw) describe changes to App Store Connect age rating settings.

### App Store submission update

[Apple](https://twitter.com/apple) in their news [article](https://developer.apple.com/news/?id=ib31uj1j) broadcasted that all iOS, iPadOS, and watchOS applications submitted to the App Store must be built with Xcode 12 starting the 26<sup>th</sup> of April.

### WWDC 2021

[Apple Worldwide Developers Conference](https://developer.apple.com/wwdc21) is just around the corner, an all-online event will be taking place on Monday, the 7th of June.

## Fundamentals

### Swift keywords

[Jordan Morgan](https://twitter.com/jordanmorgan10) has an [article](https://www.swiftjectivec.com/swift-keywords-v-3-0-1) explaining every single reserved keyword in Swift with added minimalistic code snippets to illustrate their use.

### `if case let` statements in Swift

When working with enumerations occasionally you may come across enumeration cases with arguments. Using a switch statement enables you to match enumeration values and optionally extract the associated values as constants or variables. Supposing your main point of interest is a single enumeration case, as opposed to using default case to cover all remaining cases that aren’t addressed explicitly, use `if case let` statement instead. [Zoë Smith](https://twitter.com/zoejessica) wrote an [article](https://fuckingifcaseletsyntax.com) explaining how to write those statements.

### Difference between a singleton and a shared instance

A common anti-pattern in Swift is to define an instance of an object that you can access in your application globally. [Donny Wals](https://twitter.com/DonnyWals) draws the line between singleton and a shared instance in his [article](https://www.donnywals.com/whats-the-difference-between-a-singleton-and-a-shared-instance-in-swift).

### Error handling in Swift

Some operations aren’t guaranteed to always complete execution or produce a useful output and when an operation fails, it’s often useful to understand what caused the failure, so that you can respond to and recover from error conditions accordingly. Visit the [article](https://www.avanderlee.com/swift/try-catch-throw-error-handling) by [Antoine van der Lee](https://twitter.com/twannl), [article](https://www.hackingwithswift.com/example-code/language/how-to-use-try-catch-in-swift-to-handle-exceptions) by [Paul Hudson](https://twitter.com/twostraws), and [video](https://www.youtube.com/watch?v=Lrc-MX8WgNc) by [Sean Allen](https://twitter.com/seanallen_dev) to learn about emitting and handling errors.

### Auto Layout in Swift

Auto Layout constraints empower us to create views that dynamically adjust to different size classes and positions. The constraints will make sure that views dynamically respond to both internal and external changes. In his [video](https://www.youtube.com/watch?v=emojd8GFB0o), [Chris Ching](https://twitter.com/codewithchris) teaches how to size and position user interface elements by setting constraints in an Interface Builder, [Antoine van der Lee](https://twitter.com/twannl) has an [article](https://www.avanderlee.com/swift/auto-layout-programmatically) that will help you create constraints programmatically, and [Paul Hudson](https://twitter.com/twostraws) had created a [cheat sheet](https://www.hackingwithswift.com/articles/140/the-auto-layout-cheat-sheet) addressing common Auto Layout requirements.

## Tutorials

### iOS unit and UI testing

There is nothing worse than to find out some functionality of the application you're building doesn't work when it previously did. When scaling and optimizing our applications we often revisit previous implementations in our codebases. It is crucial to be confident that no defects have been introduced when releasing new features. The purpose of well-written tests is to reassure. In a [tutorial](https://www.raywenderlich.com/21020457-ios-unit-testing-and-ui-testing-tutorial) written by [Audrey Tam](https://twitter.com/mataharimau) and updated by [David Piper](https://twitter.com/HeyDaveTheDev) you can learn how to write test cases, imitate services, and gather test coverage.

### Geofencing with `UNLocationNotificationTrigger`

In [tutorial](https://www.raywenderlich.com/20690666-location-notifications-with-unlocationnotificationtrigger) by [Graham Connolly](https://www.linkedin.com/in/graham-connolly-37756a53) learn how to use  `UNLocationNotificationTrigger` to schedule a local notification to be delivered when a device enters or leaves a specific geographic region.

### Monitoring for iOS with `MetricKit`

In iOS 13 Apple introduced [MetricKit](https://developer.apple.com/documentation/metrickit) to help you receive on-device application diagnostics as well as power and performance metrics captured by the system. [Adam Rush](https://twitter.com/adam9rush) has created a [tutorial](https://www.raywenderlich.com/20952676-monitoring-for-ios-with-metrickit-getting-started), where you'll explore framework APIs by simulating receiving diagnostics in Xcode.

### `UIView` animations

[Midhet Sulemani](https://twitter.com/itsnotmidget) in her [tutorial](https://dev.to/midhetfatema94/uiview-animations-in-swift-5cnj) tutors about animatable properties of `UIView` class.

## Enhanced programming

### Logging into the application with Face ID or Touch ID

[Apple](https://twitter.com/apple) provide a [sample code](https://developer.apple.com/documentation/localauthentication/logging_a_user_into_your_app_with_face_id_or_touch_id) showing how you can supplement your authentication scheme with biometric authentication, making it easy for users to access sensitive parts of your application.

### Improving application's performance

[Apple](https://twitter.com/apple) describe the continuous improvement cycle and share a list of resources to model, measure, and boost the performance of your application in the following [article](https://developer.apple.com/documentation/metrickit/improving_your_app_s_performance).

### Pushing background updates

[Apple](https://twitter.com/apple) has an [article](https://developer.apple.com/documentation/usernotifications/setting_up_a_remote_notification_server/pushing_background_updates_to_your_app) detailing how to deliver background notifications to wake your application without displaying an alert, playing a sound, or badging your application's icon and updating it in the background.

### Customizing the appearance of iOS application's notification alerts

[Apple](https://twitter.com/apple) has an [article](https://developer.apple.com/documentation/usernotificationsui/customizing_the_appearance_of_notifications) guiding you through the process of customizing the appearance of your iOS application’s notification alerts with a notification content application extension.

### Extending capabilities of an iOS simulator

[Ahmed Sulaiman](https://twitter.com/ahmed_sulajman) had written an [article](https://medium.com/flawless-app-stories/simulator-on-steroids-c12774ca6b) exploring various hidden features of an iOS simulator.

### Unit test best practices

When was the last time you've refactored and optimized your unit tests and not just added a new case? [Antoine van der Lee](https://twitter.com/twannl) in his [article](https://www.avanderlee.com/swift/unit-tests-best-practices) shares his rules for writing clean unit tests.

### Caching in Swift

Caching data to avoid unnecessary work repetition will positively impact the application's performance. No matter how optimized your approach to loading data is, not having to load data at all will always be faster — and caching can be a great way to achieve that. Learn how to cache data in an [article](https://swiftbysundell.com/articles/caching-in-swift) by [John Sundell](https://twitter.com/johnsundell).

### Every SwiftUI public protocol explained

[Federico Zanetello](https://twitter.com/zntfdr) wrote an [article](https://www.fivestars.blog/articles/swiftui-protocols) where he looks at all of the exposed protocols in SwiftUI.

### Implementing `AppTrackingTransparency` framework

With the public releases of iOS 14.5, iPadOS 14.5, and tvOS 14.5, to access app-related data for tracking the user or the device all applications must use the `AppTrackingTransparency` framework to request the user's permission. [Lee Kah Seng](https://twitter.com/Lee_Kah_Seng) wrote an [article](https://swiftsenpai.com/development/get-ready-apptrackingtransparency) clarifying Identifier for Advertisers (IDFA) and how to request user's permission to gather data for tracking.
Additionally, review the [article](https://appfigures.com/resources/guides/att-prompt-copywriting) by [Ariel Michaeli](https://twitter.com/arielmichaeli) in which he evaluates some of the pre-prompt examples and lays out some rules to follow when creating one for yourself.

### Coordinator structural design pattern

Read an [article](https://holyswift.app/coordinators-and-tab-bars-a-love-story) by [Leonardo Maia Pugliese](https://twitter.com/Leo_Pugliese) on how he solves a problem navigating from one tab navigation stack's topmost view controller to another tab navigation stack's topmost view controller implementing coordinator structural design pattern.

### `print` in-depth

How many days you can last without calling the `print` function? Learn how to customize and redirect the output of print statements in an [article](https://www.andyibanez.com/posts/swift-print-in-depth) by [Andy Ibanez](https://twitter.com/AndyIbanezK).

### `OSLog` and unified logging as recommended by Apple

Migrate from print statements to `OSLog` class, introduced in iOS 14, in combination with [Console](https://support.apple.com/guide/console/welcome/mac) application to debug issues more efficiently. [Antoine van der Lee](https://twitter.com/twannl) had written an [article](https://www.avanderlee.com/debugging/oslog-unified-logging) illustrating how to make that replacement.

### Hacking native ARM64 binaries to run on the iOS simulator

[Bogo Giertler](https://twitter.com/giertler) in his [article](https://bogo.wtf/arm64-to-sim.html) reports his findings on ARM64 architecture static library transmogrification.

### Debugging Core Data

[Keith Harrison](https://twitter.com/kharrison) wrote an [article](https://useyourloaf.com/blog/debugging-core-data) highlighting valuable launch arguments and environment variables you can add to your Xcode scheme to catch and debug Core Data issues.

### The `NSDateInterval` object

[Andy Ibanez](https://twitter.com/AndyIbanezK) wrote an [article](https://www.andyibanez.com/posts/the-nsdateinterval-object) educating on how to use  `NSDateInterval` to calculate the time interval between two dates or to check if a given date is within a certain time frame.

### Hash functions in Swift

Cryptography gained wider acknowledgment with the increasing popularity of cryptocurrencies. Hashing is a basic concept of cryptography used to equate. The technique allows you to immediately know if both comparables are different without exposing any details. In iOS 13, Apple released [CryptoKit](https://developer.apple.com/documentation/cryptokit) whereas previously you might have used [CryptoSwift](https://cryptoswift.io) developed by [Marcin Krzyżanowski](https://twitter.com/krzyzanowskim). [Leonardo Maia Pugliese](https://twitter.com/Leo_Pugliese) wrote an [article](https://holyswift.app/hash-function-in-swift) explaining what are hash values and how to create them using `CryptoKit`.

### Automated deployment with fastlane on iOS

Development effort is better spent elsewhere than manually generating and distributing application builds. Learn how to automate application deployment using [fastlane](https://fastlane.tools) in an [article](https://www.rubicon-world.com/blog/2019/05/automated-deployment-with-fastlane-on-ios) by [Sabahudin Kodro](https://twitter.com/cuperdino).

### Swift actors

[John McCall's](https://twitter.com/pathofshrines), [Doug Gregor's](https://twitter.com/dgregor79), [Konrad Malawski's](https://twitter.com/ktosopl), and [Chris Lattner's](https://twitter.com/clattner_llvm) proposal [SE-0306](https://github.com/apple/swift-evolution/blob/main/proposals/0306-actors.md) has been implemented and will be released as a part of the future version of Swift. An actor is a reference type that protects access to its mutable state and is introduced with the keyword `actor`. Each actor protects its data through actor isolation, ensuring that only a single thread will access that data at a given time, even when many clients are concurrently making requests. [Marin Todorov](https://twitter.com/icanzilb) wrote an [article](https://trycombine.com/posts/swift-actors) exploring Swift actors and supplies a practical example.
Additionally, a separate [article](https://trycombine.com/posts/swift-actors-combine) has been dedicated to Swift actors and the [Combine](https://developer.apple.com/documentation/combine) framework.

### Setting up iOS environments

We can't afford to develop and test our applications in the same environment that our users use, which can escalate quickly and put users in harm's way. We require multiple environments for our development. [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) wrote an [article](https://sarunw.com/posts/how-to-set-up-ios-environments) demonstrating how to set up multiple environments.

### Create a dynamic form in UIKit

Learn how to use `UICollectionViewCompositionalLayout` and `UICollectionViewDiffableDataSource` classes to build a scalable dynamic form in UIKit with self-sizing collection view cells in a [video](https://www.youtube.com/watch?v=4YIckjckiWI) by [Tunde Adegoroye](https://twitter.com/tundsdev) 

### Allowing parallel iOS UI test runs in CI

If your CI machine allows multiple jobs to run in parallel you most likely have encountered a problem that you cannot run multiple iOS UI tests in the same simulator at the same time. [Igor Kulman](https://twitter.com/igorkulman) in his [article](https://blog.kulman.sk/parallel-ui-test-runs) describes how to solve it by creating a new iOS simulator instance for every job.

### Testing in-app purchases locally in iOS simulator

During the development of [Tripzy](https://apps.apple.com/th/app/tripzy/id1564625604) [Michael Abadi](https://twitter.com/michaelabadiii) discovered that you do not need a device with an internal tester account and you can test in-app purchases using a simulator. Read about his findings in the [article](https://levelup.gitconnected.com/testing-in-app-purchases-locally-in-simulator-7cdfd5031462).

### UIKit automatic keyboard avoidance

Every iOS developer, at least once in their career, had to adjust the layout of the interface to accommodate for surfacing keyboard frame. In iOS 14, Apple added automatic keyboard avoidance as the default behavior in SwiftUI. [Lee Kah Seng](https://twitter.com/Lee_Kah_Seng) wrote an [article](https://swiftsenpai.com/development/uikit-keyboard-avoidance) sharing implementation to enable automatic keyboard avoidance in UIKit.

## Tools

### Accenture workstations running macOS Big Sur VPN connectivity issues

After the recent security updates for macOS Big Sur 11.3 and 11.3.1, you may be experiencing issues with connecting to VPN on the Accenture workstation. The [article](https://in.accenture.com/mycomputer/mac-workstation-vpn-configuration) describes a workaround that leverages an older method of connecting to VPN via the Safari web browser. 
If you are in a Client Delivery Location, contact your local support channels for any questions or issues. 

### Xcode 12.5 iOS simulator HTTPS traffic recording issues using Charles Proxy

If you're like me and were unable to use Charles Proxy SSL proxying from the Xcode 12.5 iOS simulator, [Simon Støvring](https://twitter.com/simonbs) in his Twitter [thread](https://twitter.com/simonbs/status/1382578719412338691) highlights that “Install Charles Root Certificate in iOS Simulators” doesn't work with Xcode 12.5. You work around that by manually exporting the certificate, dragging it into the simulator, and trusting it.

### Integrating the Firebase App Distribution iOS SDK

Google I/O 2021 had a [codelab](https://firebase.google.com/codelabs/appdistribution-ios#0) and a [workshop](https://events.google.com/io/session/78925eb3-8781-4475-af7d-431b180b9b33) hosted by [Ibrahim Ulukaya](https://twitter.com/iulukaya) that help you integrate the Firebase App Distribution iOS SDK to distribute new releases and trigger new build in-app alerts.

### A complete guide for Apple's devices' screen sizes

[Screen Sizes](https://www.screensizes.app) application developed by [Trevor Kay](https://twitter.com/trevormkay) and [Christopher Muller](https://twitter.com/CHRISmullerWEB) is a great reference source for all Apple's devices' screen sizes.

## Tips ![new](https://img.shields.io/badge/new-success.svg)

### Multi-cursor editing in Xcode

[Sarun Wongpatcharapakornand](https://twitter.com/sarunw) has an [article](https://sarunw.com/posts/multi-cursor-editing-in-xcode) illustrating how to enable multi-cursor editing and provides a couple of usage examples.

### Output object's contents using its mirror to the stream using `dump` function

All of us have used the `print` function in debugging, [Vincent Pradeilles](https://twitter.com/v_pradeilles) created a [video](https://www.youtube.com/watch?v=fyjdnqLvJcc) to point out that there exists a powerful alternative - `dump` function.

### Detecting a retain cycle in a view controller

Apple offers sophisticated tools, such as Instruments (using Allocations and Leaks profiling templates) and Memory Graph Debugger, for debugging memory leaks, however empirically for many cases adding a print statement to the deinitializer of a view controller is sufficient to detect a retain cycle. Referring to [Cédric Luthi's](https://twitter.com/0xced) Twitter [post](https://twitter.com/0xced/status/900692839557992449) [Sarun Wongpatcharapakornand](https://twitter.com/sarunw) wrote an [article](https://sarunw.com/posts/easy-way-to-detect-retain-cycle-in-view-controller) encouraging to use of a Symbolic Breakpoint to play a sound when a view controller is deinitialized to help detect retain cycles.

### Documentation deep linking into source code

[Jordan Morgan](https://twitter.com/JordanMorgan10) in his Twitter [post](https://twitter.com/JordanMorgan10/status/1384865768039399430) shows how to deep-link from a markdown file to the source code.

### Recording videos using an iOS simulator and saving them as animated GIF images

[Simon Ng](https://twitter.com/simonng) wrote an [article](https://www.appcoda.com/xcode-simulator-animated-gif) explaining how to record videos and save them as animated GIF images using Xcode 12.5 iOS simulator's capabilities.

### The LLDB Debugger `v` command preference over `po` command

[Dave Lee](https://twitter.com/kastiglione) in his Twitter [post](https://twitter.com/kastiglione/status/1392565131826003971) added to [Krzysztof Zabłocki's](https://twitter.com/merowing_) Twitter [post](https://twitter.com/merowing_/status/1392389928844156928) promoting the use of LLDB Debugger `v` command which is faster because it doesn’t compile and execute any code.
Additionally, [Michael Dube](https://twitter.com/dubemike) had written an [article](https://medium.com/@dubemike/level-up-your-debugging-skills-with-lldbs-v-p-and-po-commands-fec76c1ffee) describing LLDB Debugger's three basic commands - `po`, `p`, and `v`.

<br>
<p align="center">
<img width="25%" alt="Curator" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/character.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit the <a href="https://github.com/esesmuedgars/IdeaKit/blob/issue1/README.md">previous issue</a>!
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
