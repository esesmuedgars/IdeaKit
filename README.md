<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.9-informational.svg)

Good morning and welcome back!

iPhone 13 devices have been announced ⚠️

Happy learning!

## News

### Title

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

Next up, Swift challenge No. 3:

```swift
...
```

<!--
```swift
...
```
-->

## Fundamentals

### Learning new application programming interfaces ⚠️

Listen to [Empower Apps podcast](https://www.empowerapps.show) [episode](https://share.transistor.fm/s/31b2d4ab) with guest [Stewart Lynch](https://twitter.com/StewartLynch)

## Tutorials

### Title

## Enhanced programming

### Creating and customizing views and controls ⚠️

[Apple](https://twitter.com/Apple) provides [sample code](https://developer.apple.com/documentation/uikit/mac_catalyst/uikit_catalog_creating_and_customizing_views_and_controls)

### `AnyCancellable` in `Combine` ⚠️

[article](https://www.donnywals.com/what-exactly-is-a-combine-anycancellable) by [Donny Wals](https://twitter.com/DonnyWals)

## Tools

### Title

## Tips

### Using `#function` for `String` values ⚠️

Twitter [post](https://twitter.com/nicklockwood/status/1430429295994888198) by [Nick Lockwood](https://twitter.com/nicklockwood)

### Overriding argument's default value ⚠️

YouTube [video](https://www.youtube.com/watch?v=2h8eJq_dCh4) by [Vincent Pradeilles](https://twitter.com/v_pradeilles)

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
Reach out in case you would like to contribute or spot any errors! Feedback and suggestions are also welcome.
<br>
<br>
Subscribe to the <a href="https://blog.accenture.com/design">Baltic Interactive blog</a> and follow the <a href="https://web.yammer.com/main/groups/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI1Nzg0ODAwNDYwOCJ9/all">Riga Interactive Yammer community</a> for further insightful content!
</p>
