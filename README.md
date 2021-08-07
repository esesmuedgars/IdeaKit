<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.8-informational.svg)

Introduction

## News

### New public betas are available

[Apple](https://twitter.com/Apple) has expanded its public beta program with software that was announced in early June during [WWDC21](https://developer.apple.com/wwdc21). Sign up to the [Apple Beta Software Program](https://beta.apple.com/sp/betaprogram), enroll your personal devices to access iOS 15, iPadOS 15, macOS Monterey, tvOS 15, and watchOS 8 public betas, and try out the latest features. Remember to back up all of your data before installing any beta software.

<!--more-->

## Swift challenge

Prefix

```swift
// Swift challenge No. 1

// MARK: Solution A

private func spellOut() -> String {
    switch self {
    case 0: return "Zero"
    case 1: return "One"
    case 2: return "Two"
    case 3: return "Three"
    case 4: return "Four"
    case 5: return "Five"
    case 6: return "Six"
    case 7: return "Seven"
    case 8: return "Eight"
    case 9: return "Nine"
    default: return String()
    }
}

// MARK: Solution B

private func spellOut() -> String {
    let spelledOutNumbers = ["Zero",
                             "One",
                             "Two",
                             "Three",
                             "Four",
                             "Five",
                             "Six",
                             "Seven",
                             "Eight",
                             "Nine"]

    return spelledOutNumbers[self]
}

// MARK: Solution C

private func spellOut() -> String {
    let numberFormatter = NumberFormatter()
    numberFormatter.numberStyle = .spellOut

    guard let number = numberFormatter.string(from: NSNumber(value: self)) else {
        return String()
    }

    return number.capitalized
}

// MARK: Solution D

private func spellOut() -> String {
    let number = NumberFormatter.localizedString(from: NSNumber(value: self), number: .spellOut)

    return number.capitalized
}
```

Swift challenge No. 2:

Even as a simple problem as this has more clever solutions than the one your initial instinct suggests.

```swift
...
```

## Fundamentals

### Title

## Tutorials

### Title

## Enhanced programming

### Placeholder view in `SwiftUI`

Previously used, since then archived, Facebook's [Shimmer](https://github.com/facebookarchive/Shimmer) library
[article](https://sarunw.com/posts/make-placeholder-view-in-swiftui-with-redacted) by [Sarun Wongpatcharapakornand](https://twitter.com/sarunw)

## Tools

### Title

## Tips

### Title

<br>
<p align="center">
<img width="35%" alt="Curators" src="curators.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit the <a href="https://github.com/esesmuedgars/IdeaKit/blob/issue4/README.md">previous issue</a>!
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
Subscribe to the <a href="https://blog.accenture.com/design">Baltic Interactive blog</a> and follow the <a href="https://web.yammer.com/main/groups/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI1Nzg0ODAwNDYwOCJ9/all">Riga Interactive Yammer community</a> for further insightful content!
</p>
