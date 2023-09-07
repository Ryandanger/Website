---
title: Announcing Files v3
description: A design refresh, faster startup performance, support for previewing Office documents, & and speed graph for file operations.
thumbnail: /blog-resources/v3/HeroImage.jpg
date: 7/20/2023
author: files-community
---

It's hard to believe that it's two years since the launch of v2. Our mission with Files is to build the best file manager for Windows, and we're proud to be building it out in the open so everyone can participate. The feedback users submit helps shape the features we work on, & the bug reports on GitHub help to make Files more reliable. We're keenly aware that we wouldn't have gotten to this point without the support of our dedicated users and the open source community. Thanking everyone who helps with Files would take up this whole blog, so we hope it's okay to have a simple thank you.

We're pumped to announce the next major milestone for Files, starting today, v3 is now available. If you already have Files, there will be a notification on the toolbar to install the update. Otherwise, you can download Files for free from our [download page](/download/). You can also purchase Files on the [Microsoft Store](ms-windows-store://pdp/?ProductId=9nghp3dx8hdx&cid=FilesWebsite) to help support the project.

**TL;DR:** Files v3 includes a refreshed design, faster startup performance, support for previewing Offices documents, a speed graph for file operations, and more. Continue reading to learn more about these changes.

## What's new in v3

### Push Git commits to remote repositories

To further improve our integration with Git, we're excited to be adding support for pushing commits to remote repos. The Status Bar will display you how many local and remote commits you have, and you can click on it to access the sync, pull, and push options. We hope this feature makes it easier for you to collaborate with other developers and keep your code up to date.

<figure>
    <img src="/blog-resources/files2-5-20/GitPush.png" alt="Push commits to remote repos." />
</figure>

### Improvements to the startup experience

Startup performance is one of our highest priorities and something we're working on improving. We'd like the progress to be faster but unfortunately there are some limitations in the WinAppSdk framework. We hope these limitations will be resolved in future versions of WinAppSdk, but in the meantime, we've been working on a lot of smaller optimizations that we hope will add up over time. We're also adding a splash screen when the app is opened to indicate that the app is loading.  

<figure>
    <img src="/blog-resources/files2-5-20/SplashScreen.png" alt="Splash screen." />
</figure>

### Redesigned layout icons

We redesigned the icons in the layout flyout to be more consistent with the design language in Files. Additionally, the icon on the toolbar now changes to match the selected layout.

<figure>
    <img src="/blog-resources/files2-5-20/ToolbarIcon.png" alt="Toolbar icon." />
</figure>

### Edit tags and open Properties from the Details Pane

- Added support for editing file tags from the Details Pane
- Added a button to open the Properties window from the Details Pane
- Updated font styles to better utilize the space

<figure>
    <img src="/blog-resources/files2-5-20/EditTags.png" alt="Details Pane." />
</figure>

### Added support for ownCloud

Files will now detect and display ownCloud in the sidebar when the ownCloud client is installed.

### Change the behavior of actions using modifier keys

Holding down modifier keys when pressing on certain toolbar buttons will now change to behavior. For example, holding down `shift` while pressing the `delete` button on the toolbar will permanently delete the selected items.

### Added a path column when viewing search results in the Details layout

We added a path column to the Details layout when viewing the results of a search. This feature also enables you to also sort and group the search results by path.

### Added "Size on disk" property to the Properties window

We added a "Size on disk" property when viewing the properties of cloud folders.

### Added support for opening all tagged items from the Tags widget

We added a button to the Tags widget for opening all the items with that tag.

## Changes and Improvements

### Status Bar design

We added lines to divide the different sections in the Status Bar.

### Readme files are no longer automatically selected

Opening a folder with a `readme.md` file will no longer select the readme file.

### Improved quality of the icons in the pinned favorites section

We made several enhancements to improve the quality of icons in the pinned favorites section.

### Updated the Tag icon used throughout the app

The tag icon in the sidebar, right click context menu, and Tags widget was updated to have better contrast.

### Updated the Toolbar icons

We updated a number of toolbars icons, we also updated the icons for the cloud status, and Git status columns in the Details layout.

### Updated the DataGrid in the Details layout

We redesigned the DataGrid headers in the Details layout to better match the design language in Windows 11.

### Increased the maximum volume label length to 128 characters for UDF images

Based on user feedback, we increased the maximum volume label length to 128 characters for UDF images.


### Conclusion

As always, we appreciate your feedback and suggestions on how we improve Files. You can reach us through our GitHub issues page: https://github.com/files-community/Files/issues.

Thank you for using Files! 😊

---

Download Files from our [download page](/download/).



- Added round corners on the file area
- Redesigned the left hand sidebar
- Added support for renaming network drives
- Updated tag icon on the settings page
- Updated icons in the Tag column in the Details layout
- Added "open all" when right clicking a tag in the sidebar
- Added support for elevated file operations
- Added a Command Palette
- Updated the design of the home page headers
- Increased the default width of the Git status column
- Auto refresh after adding items if no directory watcher is available
- Show BitLocker options in main menu for drives
- Purge logfiles to only keep the last 100 lines
- Display error message when transferring files that are too large for FAT32
- Added support for opening shortcut files as another user
- Removed margin when using the Compact Spacing option
- Scroll to the selected file when using "Open file location"
- Updated the design of the Tags section in the Details Pane
- Restored the status icon for the ongoing tasks button
- Disabled keyboard shortcuts when renaming items
- Display keyboard shortcuts in the right click menu
- Automatically update items when the date changes
- Lazy load Git properties for better performance
- Load network icon in the sidebar instead of using a folder icon
- Added an option to keep Files running in the background when closing the window. This option is still in development, but we're including it in this build to gather feedback.
- Redesigned the app icon
- Removed the chevron from the last item in the path bar
- Theme names are now localized
- Replaced the "What's new" flyout with a popup
- Updated WinAppSdk to 1.4
- Added support for previewing Office files
- Added support for additional archive formats
- Display custom icon when Files is the registered handler for archives