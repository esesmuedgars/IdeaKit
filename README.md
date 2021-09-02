<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.9-informational.svg)

Good morning and welcome back!

~~iPhone 13 devices have been announced~~

If you would fancy to take ownership of the newsletter reach out to [Kaspars Auzarejs-Auzers](https://people.accenture.com/People/user/k.auzarejs-auzers) I shared with him [guidelines](https://github.com/esesmuedgars/IdeaKit/blob/latest/CONTRIBUTING.md) necessary to recreate the newsletter.

for obvious reason I will not present you with a new challenge, instead think of ways how you could improve software application you’re currently working on.

Will not leave you hanging, I suggest three newsletter to subsribe to [iOS Dev Weekly](https://iosdevweekly.com) curated by [Dave Verwer](https://twitter.com/daveverwer), [Swift Weekly Brief](https://swiftweeklybrief.com) curated by [Kristaps Grinbergs](https://twitter.com/fassko), and [iOS Goodies](https://ios-goodies.com) curated by [Marius Constantinescu](https://twitter.com/marius_const). Another important thing is twitter.

If you'd like, follow me on Twitter where I don't post anything.

Happy learning!  ⚠️

## News

### Additional banking information required in App Store Connect ⚠️

[Apple](https://twitter.com/Apple) in their news [article](https://developer.apple.com/news/?id=ep8chzr8)

### Package Collections ⚠️

Swift blog [post](https://swift.org/blog/package-collections) by [Tom Doron](https://twitter.com/tomerdoron)

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

## Fundamentals

### Learning new application programming interfaces ⚠️

Listen to [Empower Apps podcast](https://www.empowerapps.show) [episode](https://share.transistor.fm/s/31b2d4ab) with guest [Stewart Lynch](https://twitter.com/StewartLynch)

### iOS interview preparation ⚠️

YouTube [video series](https://www.youtube.com/watch?v=CBcuwRV4cPU&list=PLodDrxt4jmVDtxpFBpuPGk0X7BnB8lxBD) by [Aryaman Sharda](https://twitter.com/aryamansharda)

### Observing properties in Swift ⚠️

[article](https://www.jessesquires.com/blog/2021/08/08/different-ways-to-observe-properties-in-swift) by [Jesse Squires](https://twitter.com/jesse_squires)

## Tutorials

### `SwiftGen` for iOS ⚠️

[tutorial](https://www.raywenderlich.com/23709326-swiftgen-tutorial-for-ios) by [Andy Pereira](https://twitter.com/macandyp)

###  One time passcode (OTP) user interface ⚠️

YouTube [video](https://www.youtube.com/watch?v=mHxAvSs914g) by [Kyle Lee](https://twitter.com/kilo_loco)

### The Composable Architecture (TCA) ⚠️

[tutorial](https://dev.to/atimca/the-composable-architecture-tutorial-29a9) by [Maxim Smirnov](https://twitter.com/atimca)

## Enhanced programming

### Creating and customizing views and controls ⚠️

[Apple](https://twitter.com/Apple) provides [sample code](https://developer.apple.com/documentation/uikit/mac_catalyst/uikit_catalog_creating_and_customizing_views_and_controls)

### `AnyCancellable` in `Combine` ⚠️

[article](https://www.donnywals.com/what-exactly-is-a-combine-anycancellable) by [Donny Wals](https://twitter.com/DonnyWals)

### Unit testing best practices ⚠️

[article](https://medium.com/revolut/best-practices-for-unit-testing-at-revolut-45428879ca07) by [Arsen Gasparyan](https://twitter.com/ansenro)

### `StaticString` ⚠️

[article](https://swiftrocks.com/staticstring-in-swift) by [Bruno Rocha](https://twitter.com/rockbruno_)

### `#selector` and the responder chain ⚠️

[article](https://dasdom.dev/posts/selector-and-the-responder-chain) by [Dominik Hauser](https://twitter.com/dasdom)

### Reverse engineering `UIKit` to fix our top crash ⚠️

[article](https://pspdfkit.com/blog/2021/reverse-engineering-uikit) by [Adrian Kashivskyy](https://twitter.com/akashivskyy)

## Tools

### The Importance of Restarting Your Accenture workstations running macOS ⚠️

[article](https://blog.accenture.com/accenturemacworkstation/2021/09/02/the-importance-of-restarting-your-mac) by [Brandon Peek](https://people.accenture.com/People/user/brandon.w.peek)

### Getting started with AWS Amplify ⚠️

[AWS Amplify](https://aws.amazon.com/amplify)
YouTube [video](https://www.youtube.com/watch?v=mL54fosQphI) by [Kyle Lee](https://twitter.com/kilo_loco)

### Using fastlane to automating App Store screenshots ⚠️

[article](https://lickability.com/blog/automating-app-store-screenshots-with-fastlane-and-swiftui) by (her/she) [Daisy Ramos](https://twitter.com/daisyr317)

## Tips

### Using `#function` for `String` values ⚠️

Twitter [post](https://twitter.com/nicklockwood/status/1430429295994888198) by [Nick Lockwood](https://twitter.com/nicklockwood)

### Overriding argument's default value ⚠️

YouTube [video](https://www.youtube.com/watch?v=2h8eJq_dCh4) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

### Compiler flags for Swift concurrency ⚠️

Twitter [post](https://twitter.com/olebegemann/status/1421144304127463427) by [Ole Begemann](https://twitter.com/olebegemann)

### Checking if Mobile Data is enabled  ⚠️

[article](https://nemecek.be/blog/119/how-to-check-if-mobile-data-is-enabled-for-your-app) by [Filip Němeček](https://twitter.com/nemecek_f)

### Why you shouldn't result to using conditional view modifiers ⚠️

[article](https://www.objc.io/blog/2021/08/24/conditional-view-modifiers) by [Chris Eidhof](https://twitter.com/chriseidhof)

### Spell checking in Xcode ⚠️

2-minute [article](https://sarunw.com/posts/spell-checking-in-xcode) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)

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
Subscribe to the <a href="https://blog.accenture.com/design">Baltic Interactive blog</a> and follow the <a href="https://web.yammer.com/main/groups/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI1Nzg0ODAwNDYwOCJ9/all">Riga Interactive Yammer community</a> for further insightful content!
</p>
