<img width="100%" alt="import IdeaKit - Swift Monthly Newsletter" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/title.svg" />

###### 0 minute read

![Issue](https://img.shields.io/badge/issue-1.9-informational.svg)

Hey, hey!

Prefix

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

### Title

## Tutorials

### Title

## Enhanced programming

### Title

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
