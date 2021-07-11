<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.7-informational.svg)

**TODO:** Prefix

## News

### **TODO:** News

## Swift challenge

What Swift challenges are not? Swift challenges are not programming or mathematical problems that have universal solutions.
What Swift challenges are? Swift challenges highlight problems with purpose to grant insight into Swift syntactical sugar and uncommon, native APIs.
Each consecutive newsletter's issue will provide solution(-s) (as well as explanation(-s) and resource hyperlink(-s), where applicable) to a problem described in issue before, besides following challenge.

Let's start things slow, Swift challenge No. 1:

Even as simple problem as this has more clever solutions than the one your initial instinct suggests.

```swift
/**
For numbers in the range between 0 and 9 return spelled out number value.
Implement `spellOut` method.
 */
 
 extension Int {
     /// Spell out number in the range from 0 to 9 (e.g., calling `0.spelledOut` returns `"Zero"`).
     /// - returns: Capitalized, spelled out number value.
     var spelledOut: String {
         assert(0...9 ~= self, "Value is out-of-bounds")
         
         return spellOut()
     }
     
     private func spellOut() -> String {
         <#String#>
     }
 }
```
<!--
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
-->

## Fundamentals

### **TODO:** _Fundamentals_ article

## Tutorials

### **TODO:** Tutorial

## Enhanced programming

### **TODO:** _Enhanced programming_ article

## Tools

### **TODO:** Tool

## Tips

### **TODO:** Tip

<br>
<p align="center">
<img width="25%" alt="Curator" src="curator.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge! For additional study materials visit the <a href="https://github.com/esesmuedgars/IdeaKit/blob/issue3/README.md">previous issue</a>!
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
