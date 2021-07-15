# Contributing guidelines

## Permissions

[Līva Pilvere](https://people.accenture.com/People/user/liva.pilvere)

## Tools

Newsletter featured images have been created using [Ray.so](https://ray.so) tool.

<a href="https://blog.accenture.com/design">Baltic Interactive blog's</a> media library has images uploaded up until _import IdeaKit Issue 36_, but to recrerate images used

<p align="center">
<img alt="Featured image example" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/contributing_featured_image.svg"  width="50%" />
</p>

### Configuring image through JavaSript

- Set default values using controls:
    - Colors: `Sunset` (`C`);
    - Background: `Enabled` (`B`);
    - Dark mode: `Disabled` (`D`);
    - Padding: `64` (`P`);
    - Language: `Swift` (`L`).
- Open Chrome DevTools in Console panel ( in Google Chrome `⌘` + `⌥` + `J`). Alternatively, you can right-click and element and select Inspect option;
- Update text colors to match Xcode's default light theme:
```javascript
document.getElementsByClassName("vue-codemirror code-editor")[0].style.cssText = `
--syntax-comment: #5D6C79;
--syntax-keyword: #9B2393;
--syntax-definition: rgba(0, 0, 0, 0.85);
`;
```
- Update text font to match Xcode's default light theme:
```javascript
document.querySelectorAll('.cm-keyword')[0].style.fontWeight = "Bolder";
```
- Update background gradient colors to match Swift programming language identity:
```javascript
document.getElementsByClassName('frame frame')[0].style.background = "linear-gradient(rgb(241, 178, 87), rgb(236, 73, 55))";
```
- Save as PNG (`⌘` + `S`).

### Manually configuring image

- Set default values using controls:
    - Colors: `Sunset` (`C`);
    - Background: `Enabled` (`B`);
    - Dark mode: `Disabled` (`D`);
    - Padding: `64` (`P`);
    - Language: `Swift` (`L`).
- Open Chrome DevTools in Elements panel ( in Google Chrome `⌘` + `⌥` + `C`);
- Update text colors to match Xcode's default light theme:
    - Locate and select child of `<div class="app-frame">...</div>`:
```html
<div class="vue-codemirror code-editor">...</div>
```
Replace element's `style` properties from:
```html
--syntax-text: #737568;
--syntax-background: rgba 0,0,100,0.75;
--syntax-string: #8C703C;
--syntax-comment: #7A7055;
--syntax-variable: #807410;
--syntax-variable-2: #717365;
--syntax-variable-3: #8C6A29;
--syntax-number: #856F00;
--syntax-atom: #856F00;
--syntax-keyword: #A1642C;
--syntax-property: #AD5A78;
--syntax-definition: #807410;
--syntax-meta: #6B625B;
--syntax-operator: #A1642C;
--syntax-attribute: #807410;
--syntax-tag: #A1642C;
```
to:
```html
--syntax-comment: #5D6C79;
--syntax-keyword: #9B2393;
--syntax-definition: rgba(0, 0, 0, 0.85);
```
- Update text font to match Xcode's default light theme:
    - Locate and select `<span class="cm-keyword">...</span>`;
    - Add `font-weight: bolder;` to `cm-keyword` CSS class properties
- Update background gradient colors to match Swift programming language identity:
    - Locate and select child of `<div class="content">...</div>`:
```html
<div id="frame" class="frame frame">...</div>
```
Replace element's `background` property from:
```html
background: linear-gradient(140deg, rgb(255, 207, 115), rgb(255, 122, 47));
```
to:
```html
background: linear-gradient(rgb(241, 178, 87), rgb(236, 73, 55));
```
- Save as PNG (`⌘` + `S`).

Footer characters created using [Open Peeps](https://www.openpeeps.com) by [Pablo Stanley](https://twitter.com/pablostanley).

## Resources

### Swift Newsletters

- AppCoda Weekly [newsletter](http://digest.appcoda.com);
- Awesome iOS [newsletter](https://ios.libhunt.com);
- Donny Wals Weekly [newsletter](https://www.donnywals.com/newsletter);
- iOS Dev Weekly [newsletter](https://iosdevweekly.com);
- iOS Goodies [newsletter](https://ios-goodies.com);
- Ray Wenderlich [newsletter](https://www.raywenderlich.com/newsletter);
- Sarunw's Blog [newsletter](https://sarunw.com);
- Swift Weekly [newsletter](https://swiftweekly.com);
- Swift Weekly Brief [newsletter](https://swiftweeklybrief.com);
- SwiftLee Weekly [newsletter](https://www.avanderlee.com);
- This Week in Swift [newsletter](https://swiftnews.curated.co).

### Swift Podcasts

- Apple Events (video) [podcast](https://podcasts.apple.com/podcast/apple-events-video/id275834665);
- Fireside Swift [podcast](https://podcasts.apple.com/podcast/fireside-swift/id1269435221);
- Inside iOS Dev [podcast](https://podcasts.apple.com/podcast/inside-ios-dev/id1231805301);
- iOS Dev Break [podcast](https://podcasts.apple.com/podcast/ios-dev-break/id1157188242);
- iOS Dev Discussions [podcast](https://podcasts.apple.com/podcast/ios-dev-discussions-sean-allen/id1426167395);
- iOS Lead Essentials [podcast](https://podcasts.apple.com/podcast/ios-lead-essentials-podcast-essentialdeveloper-com/id1477494716);
- More Than Just Code [podcast](https://podcasts.apple.com/podcast/more-than-just-code-podcast-ios-swift-development-news/id906987516);
- Release Notes [podcast](https://podcasts.apple.com/podcast/release-notes/id650358643);
- Stacktrace [podcast](https://podcasts.apple.com/podcast/stacktrace/id1359435443);
- Swift by Sundell [podcast](https://podcasts.apple.com/podcast/swift-by-sundell/id1267161825);
- Swift over Coffee [podcast](https://podcasts.apple.com/podcast/swift-over-coffee/id1435076502);
- Swift Unwrapped [podcast](https://podcasts.apple.com/podcast/swift-unwrapped/id1209817203);
- Swiftly Speaking [podcast](https://podcasts.apple.com/podcast/swiftly-speaking/id1505697997);
- The iDeveloper [podcast](https://podcasts.apple.com/podcast/the-ideveloper-podcast/id400664935);
- The iPhreaks Show [podcast](https://podcasts.apple.com/podcast/the-iphreaks-show/id634022060);
- Under the Radar [podcast](https://podcasts.apple.com/podcast/under-the-radar/id1055685246);
- Waiting for Review [podcast](https://podcasts.apple.com/podcast/waiting-for-review/id1199635981).
