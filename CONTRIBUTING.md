# Contributing guidelines

## Distribution

### Permissions

`Contributor` role is enough to create and publish posts, but at least `Editor` role is required to add images to the media library and add featured image to the blog post.
Request access from [Līva Pilvere](https://people.accenture.com/People/user/liva.pilvere).

### Structure

In _Baltic Interactive_ [blog](https://blog.accenture.com/design)  `<!--more-->` seperator is inserted before _Body_ of the newsletter, which results in title, introduction and _News_ section to be displayed in the blog's list of posts and "Continue reading" is inserted afterward, as well as this information is included in blog's subscriber e-mail notifications.

```bash
.
├── Title (w/ featured image)
│   ├── Introduction
│   └── News
├── Body
│   ├── Swift challenge
│   ├── Fundamentals
│   ├── Tutorials
│   ├── Enhanced programming
│   ├── Tools
│   └── Tips
└── Footer
    └── Footnote
```

### Syntax conversion

There is open proposal [#10](https://github.com/esesmuedgars/IdeaKit/issues/10) to automate Markdown to WordPress syntax conversion, but at the moment it is done manually:

- Open `README.md` in Xcode;
- Open Find and Replace in the document (`⌘` + `⌥` + `F`);
- Keep default case-insensitive contains search condition;
- Click the Insert Pattern button (+) to include line breaks, web addresses or special characters in search term;
- Replace all `<#Line Break 1#>## <#Any Characters#><#Line Break 2#>` matches with `<#Line Break 1#><h3><#Any Characters#></h3><#Line Break 2#>` to convert syntax of titles:

<p align="center">
<img alt="Find and Replace titles" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/find_and_replace_titles.png" />
</p>

- Replace all `<#Line Break 1#>### <#Any Characters#><#Line Break 2#>` matches with `<#Line Break 1#><h4><#Any Characters#></h4><#Line Break 2#>` to convert syntax of subtitles:

<p align="center">
<img alt="Find and Replace subtitles" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/find_and_replace_subtitles.png" />
</p>

- Replace all `[<#Any Characters#>](<#Web Address#>)` matches with `<a href="<#Web Address#>"><#Any Characters#></a>` to convert syntax of hyperlinks:

<p align="center">
<img alt="Find and Replace hyperlinks" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/find_and_replace_hyperlinks.png" />
</p>

- Replace all `` `<#Any Characters#>` `` matches with `<code><#Any Characters#></code>` to convert syntax of code:

<p align="center">
<img alt="Find and Replace code" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/find_and_replace_code.png" />
</p>

- Update footnote's image (if applicable) and hyperlink to the previous issue.

### Tags

Static list of tags are used (`Apple, IdeaKit, import IdeaKit, iOS, iPadOS, macOS, newsletter, swift, Swift Monthly Newsletter, tvOS, Xcode` append `Swift challenges` tag to the comma seperated list if issue contains a challenge) which could be improved by adding only relevant tags (e.g., use `tvOS` only if the issue has an article about the topic).

### Categories

Use _Swift_ subcategory of _Mobile_ category.

### Swift challenges

[_import IdeaKit_ issue 4](https://github.com/esesmuedgars/IdeaKit/tree/issue4) introduced Swift challenges. From that point onward each consecutive newsletter's issue is providing a solution (as well as explanation and resource hyperlink, where applicable) to a problem described in an issue before, besides the following challenge.
Due to some problems having multiple valid solutions it can greatly extend the newsletter, plus, if the reader did not read the previous issue he is robbed of a challenge by instantly presented solution. To avoid that spoiler warning image is added and linked with solution image:

<p align="center">
<img alt="Swift challenge solution spoiler warning" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/Swift_challenge_solution_spoiler_warning.png" width="60%" />
</p>

- Upload a solution image to the [media library](https://blog.accenture.com/design/wp-admin/upload.php);
- Add caption to the image; ⚠️
- Select uploaded image and save to clipboard (`⌘` + `C`) it's Copy Link (Pro tip: Copy Link is generated from the original image name, I would recommend using random filenames instead of easily recognisable pattern to eliminate cheating option);
- Click the Add Media button while editing post to insert an image;
- Select spoiler warning image;
- Click the Insert into post button (which will insert selected image(-s) in cursors current location);
- Downscale image to appropriate size;
- Link spoiler warning image with solution image:
    - In visual editor, <#String#>; ⚠️
    - In textual editor, <#String#>. ⚠️

### Announcements

Specify your own subject and edit permalink. My approach has been to shorten both of them (e.g., replace `Baltic Interactive: import IdeaKit – Swift Monthly Newsletter Issue 5` with `Baltic Interactive: import IdeaKit Issue 5` and edit `<#Generated URL Path#>/import-ideakit-swift-monthly-newsletter-issue-5/` to `<#Generated URL Path#>/import-ideakit-5/`).

Once a new newsletter's issue has been published, all subscribers of the blog will receive automatic e-mail announcements. However, to attract additional traffic manual announcements are required. Following is the list of channels that have been used for communication as well as message examples:

- _Riga Interactive_ Yammer [community](https://web.yammer.com/main/groups/eyJfdHlwZSI6Ikdyb3VwIiwiaWQiOiI1Nzg0ODAwNDYwOCJ9/all):

<p align="center">
<img alt="Yammer new issue announcement examples" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/Yammer_announcements.png" width="50%" />
</p>

- _Baltic Interactive_ (General) [channel](https://teams.microsoft.com/l/channel/19%3a44cee4a866b443dcad8be62b72443948%40thread.skype/General?groupId=4fc3b8f5-e079-4567-980c-3c159d453ed0&tenantId=e0793d39-0939-496d-b129-198edd916feb):

<p align="center">
<img alt="Microsoft Teams new issue announcement examples" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/Teams_announcements.png" width="60%" />
</p>

- _Interactive All Hands_ meeting updates:

<p align="center">
<img alt="Interactive All Hands meeting update examples" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/All_Hands_updates.png" width="70%" />
</p>

## Versioning

_Baltic Interactive_ [blog's](https://blog.accenture.com/design) newsletter's issue number is incremented by one with each consecutive release.
_GitHub_ [repository](https://github.com/esesmuedgars/IdeaKit) newsletter's issues are versioned. [Shields.io](https://shields.io) displays each issue's version number.
Branches use version numbers, however, once published, tags are using issue numbers (e.g., branch `1.5` becomes tag `issue2`, branch `1.6` becomes tag `issue3`, etc.)

```swift
X.Y

/**
 X (major version) - Year number of the newsletter (begins with 1 and never resets);
 Y (minor version) - Month number of the issue (possible values are 1 - 12, when minor version resets major version is incremented by one).
 */
```
<!--
In case of the newsletter's complete revamp, an additional version could be introduced:

X.Y.Z

X (major version) - (begins with 1, resets when newsletter's general curator is replaced or redesign takes place, etc.);
Y (minor version) - Year number of the newsletter at current state (begins with 1, when minor version resets major version is incremented by one);
Z (issue version) - Month number of the issue (possible values are 1 - 12, when issue version resets minor version is incremented by one).
-->

##### Example:

It is October's issue of the first year of the newsletter. As it is the first year - the major version is `1`, October is 10<sup>th</sup> month of the year, therefore, the minor version is `10`. That would make the newsletter's version `1.10`.

## Tools

### Language

[Grammarly](https://app.grammarly.com) (requires a free account) is used to eliminate spelling, grammar, and punctuation errors. Metrics such as clarity, engagement, delivery, and overall score weren't taken into account, but typical end values have been `very clear`, `very engaging`, `just right`, and `above 85` respectively.

[Grammarly](https://app.grammarly.com), in combination with [Thesaurus.com](https://www.thesaurus.com) and [Google’s](https://www.google.com) English dictionary results, also was applied when searching for synonyms.

Estimated reading time is auto-generated for _Baltic Interactive_ [blog's](https://blog.accenture.com/design) posts, for _GitHub_ issues [Read-o-Meter](https://niram.org/read) by [Tharique Azeez](https://twitter.com/ThariqueAzeez) and [Grammarly](https://app.grammarly.com) were referenced.

### Featured image

Newsletter's featured images have been created using [Ray.so](https://ray.so) tool.

_Baltic Interactive_ [blog's](https://blog.accenture.com/design) [media library](https://blog.accenture.com/design/wp-admin/upload.php) has featured images uploaded up to and including 36<sup>th</sup> issue, below are step-by-step guides to recreate the image:

<p align="center">
<img alt="Featured image example" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/contributing_featured_image.svg"  width="60%" />
</p>

#### Configuring image with JavaScript

- Set default values using controls:
    - Colors: `Sunset` (`C`);
    - Background: `Enabled` (`B`);
    - Dark mode: `Disabled` (`D`);
    - Padding: `64` (`P`);
    - Language: `Swift` (`L`).
- Open Chrome DevTools in Console panel (in Google Chrome `⌘` + `⌥` + `J`). Alternatively, you can right-click and element and select Inspect option;
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

#### Manually configuring image

- Set default values using controls:
    - Colors: `Sunset` (`C`);
    - Background: `Enabled` (`B`);
    - Dark mode: `Disabled` (`D`);
    - Padding: `64` (`P`);
    - Language: `Swift` (`L`).
- Open Chrome DevTools in Elements panel (in Google Chrome `⌘` + `⌥` + `C`);
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

### Footnote

Footer characters have been created using [Open Peeps](https://www.openpeeps.com) by [Pablo Stanley](https://twitter.com/pablostanley). The library is free for commercial and personal use and can be customized with [Figma](https://www.figma.com) (requires a free account).

## Resources

### Swift newsletters

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
<br>

- Subscribe to the newsletters (since it is for work related activities I've used Accenture e-mail);
- Whitelist newsletter e-mails — while setting-up you will have to release and allow each sender (through [Bulk Email Digest](bulk.email.digest@accenture.com)) as they [authors] are sending their initial e-mails;
- Optionally, create contact for each newsletter (makes it a little more convenient to create rule and contact images help differentiate newsletters at a glance):

<p align="center">
<img alt="Microsoft Outlook: Newsletter contacts" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/whitelisted_newsletter_contacts.png" />
</p>

- Create "Swift Newsletters" folder and add it to favorites;
- Create a rule to move e-mails from whitelisted newsletters to dedicated folder:

<p align="center">
<img alt="Microsoft Outlook: Move to folder rule" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/move_to_folder_rule.png" />
</p>

All newsletters' issues are stored in seperate folder and doesn't cluster inbox.

<p align="center">
<img alt="Microsoft Outlook: Newsletters" src="https://github.com/esesmuedgars/IdeaKit/blob/assets/CONTRIBUTING/newsletters.png" />
</p>

### Swift podcasts

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

### Other useful resources

- Apple Developer [News and Updates](https://developer.apple.com/news);
- Swift Official [blog](https://swift.org/blog);
- The Daily iOS Twitter [account](https://twitter.com/TheDailyiOS);
- Code Completion Twitter [account](https://twitter.com/CodeCompletion);
- [Vincent Pradeilles's](https://twitter.com/v_pradeilles) YouTube [channel](https://www.youtube.com/c/VincentPradeilles);
- [Codewars](https://www.codewars.com) platform.
