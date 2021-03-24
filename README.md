# Trojanized Xcode project targeting Apple developers discovered

###### 2 minute read

A new backdoor threat has been discovered that aims to compromise Apple developers’ macOS devices with a trojanized Xcode project along with a persistence mechanism. This malware can record victims’ microphone, camera, keyboard as well as upload and download files.

The new malicious Xcode project was discovered by Sentinel Labs. The researchers have named the threat XcodeSpy which is a custom variant of the EggShell backdoor.

The trojanized code hides as a malicious replica of a legitimate open-source Xcode project and works by exploiting the Run Script feature in the Xcode IDE. Sentinel Labs explains:

> We recently became aware of a trojanized Xcode project in the wild targeting iOS developers thanks to a tip from an anonymous researcher. The malicious project is a doctored version of a legitimate, open-source project available on GitHub. The project offers iOS developers several advanced features for animating the iOS Tab Bar based on user interaction.

> The XcodeSpy version, however, has been subtly changed to execute an obfuscated Run Script when the developer’s build target is launched. The script contacts the attackers’ C2 and drops a custom variant of the EggShell backdoor on the development machine. The malware installs a user LaunchAgent for persistence and is able to record information from the victim’s microphone, camera, and keyboard.

The researchers at Sentinel Labs have found two variants of the payload and so far have seen a single case of the threat found within a U.S. organization. Analyzed sample used a copy of the [TabBarInteraction](https://github.com/potato04/TabBarInteraction) project. They believe the malware campaign may have run from July to October 2020 and say the extent of the spread is unknown for now but other XcodeSpy projects may exist.

> We have thus far been unable to discover other samples of trojanized Xcode projects and cannot gauge the extent of this activity. However, the timeline from known samples and other indicators mentioned below suggest that other XcodeSpy projects may exist. By sharing details of this campaign, we hope to raise awareness of this attack vector and highlight the fact that developers are high-value targets for attackers.

Consequently, all Apple developers are cautioned to check for the presence of malicious Run Scripts whenever adopting third-party Xcode projects. Sentinel Labs provide simple method developers can use to scan their existing local Xcode repositories in the [Detection and Mitigation](https://labs.sentinelone.com/new-macos-malware-xcodespy-targets-xcode-developers-with-eggshell-backdoor/#DTM) section. If you uncover any trace of XcodeSpy on your Accenture owned macOS device, you should immediately call the Accenture Security Operations Center (ASOC) hotline at [+1 202 728 0645](tel://+12027280645).

Check out the full technical details of XcodeSpy in the [full report](https://labs.sentinelone.com/new-macos-malware-xcodespy-targets-xcode-developers-with-eggshell-backdoor).

<br>
<p align="center">
<img width="25%" alt="Curator" src="https://github.com/esesmuedgars/IdeaKit/blob/pilot/character.svg" />
<!--Character credit goes to [Pablo Stanley](https://twitter.com/pablostanley) with his [Open Peeps](https://www.openpeeps.com) hand-drawn illustration library.-->
</p>
<p align="center">
Thank you for taking the time to expand your knowledge!
<br>
<br>
Found a topic insightful? You can add your comments and open a discussion using the comment section below.
</p>
