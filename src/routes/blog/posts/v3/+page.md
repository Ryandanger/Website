---
title: Announcing Files v3
description: A design refresh, faster startup performance, support for previewing Office documents, & and speed graph for file operations.
thumbnail: /blog-resources/v3/Hero.jpg
date: 7/20/2023
author: files-community
---

It's hard to believe that it's two years since the launch of v2. Our mission with Files is to build the best file manager for Windows, and we're proud to be building it out in the open so everyone can participate. User feedback helps shape the features we work on, & the bug reports on GitHub help to make Files more reliable. We're keenly aware that we wouldn't have gotten to this point without the support of our dedicated users and the open source community, and we want to extend a thank you to everyone who's been involved with the project until this point.

Starting today, v3 is now available to download. If you already have Files, there will be a notification on the toolbar to install the update. Otherwise, you can download Files for free from our [download page](/download/). You can also purchase Files on the [Microsoft Store](ms-windows-store://pdp/?ProductId=9nghp3dx8hdx&cid=FilesWebsite) to help support the project.

**TL;DR:** Files v3 includes a refreshed design, faster startup performance, a command palette, support for previewing Offices documents, a speed graph for file operations, and more. Continue reading to learn more about these changes.

## What's new in v3

### Design updates

When we set out to update the design, we wanted to ensure users would feel at home with the app they love. We were careful not to move the options and commands users are familiar with, whilst modernizing and refreshing core parts of the UI.

- With v3 being one of the larger releases to date, we decided it was a good time to refresh the logo. After exploring a number of ideas and color combinations, we asked the community to help choose a color. It's probably no surprise, but the community overwhelmingly opted in favor of the familiar yellow color. We also updated the icons for the developer and preview versions of Files (purple & blue) to make it easier to identify the different variants of the app. 

<figure>
    <img src="/blog-resources/v3/NewIcon.jpg" alt="Updated Files Icon for all branches" />
</figure>

- We redesigned the sidebar from the ground up, removing the icons from headers and the indentations from child items. We also added icons to highlight pinned folders.
- We rounded the corners on the file area and adjusted the background opacity to provide more distinction between the sidebar.

<figure>
    <img src="/blog-resources/v3/Sidebar.jpg" alt="Redesigned sidebar" />
</figure>

### Keep Files in the background

Improving startup performance is one of our top priorities we'll continue to work on this in future updates. There are a number of reasons why progress has been slow, but in order to provide a quicker solution, we added an option to keep Files in the background when closing the last window. This option is enabled by default, but can be turned on/off from the advanced settings page.

### Added a Command Palette

With hundreds of available features, it can be hard for to keep track of all the features and keyboard shortcuts. To help with this, we're excited to introduce a Command Palette where you search for and trigger commands. To access the command palette, you can use the `ctrl` + `shift` + `p` keyboard shortcut, or alternatively you can enter `>` into the address bar and start searching for a command. 

### Rich previews for your Office documents

In addition to support for previewing Office documents, we added support for previewing file formats with a registered shell preview handler.

<figure>
    <img src="/blog-resources/v3/OfficePreview.jpg" alt="Updated preview pane" />
</figure>

### Improved experience for file operations

You can now track the progress and speed of file operations in the Status Center with the new graph feature.

<figure>
    <img src="/blog-resources/v3/StatusCenter.jpg" alt="Updated status center with the speed graph" />
</figure>

## Changes and Improvements

### Added support for renaming network drives

Added support for renaming network drives from the properties window.

### Theme names are now localized in the settings dialog

The theme names in the settings dialog are now translated to make it more accessible in different localizations.

### Keyboard shortcuts are now displayed in the right click menu

Keyboard shortcuts are now displayed next to the context menu items to help increase their discoverability.

### Added support for opening shortcut files as another user

Added support for opening shortcuts to exe files as another user.

### Added support for additional archive formats

Added support for browsing and extracting items from additional archive formats.

### Added support for elevated file operations

File operations requiring admin access will now prompt to elevate the process.

### Auto refresh folder when changes are made

Folders in special locations that don't have a directory watcher will now refresh when changes are made.

### Display error message when transferring files that are too large for FAT32

An error message is now displayed when files cannot be transferred to drives formatted as FAT32, previously these file operations would fail without providing an explanation..


### Conclusion

As always, we appreciate your feedback and suggestions on how we improve Files. You can reach us through our GitHub issues page: https://github.com/files-community/Files/issues.

Thank you for using Files! 😊

---

Download Files from our [download page](/download/).



- Show BitLocker options in main menu for drives
- Removed margin when using the Compact Spacing option
- Scroll to the selected file when using "Open file location"
- Updated the design of the Tags section in the Details Pane
- Restored the status icon for the ongoing tasks button
- Disabled keyboard shortcuts when renaming items
- Automatically update items when the date changes
- Lazy load Git properties for better performance
- Load network icon in the sidebar instead of using a folder icon
- Replaced the "What's new" flyout with a popup
- Display custom icon when Files is the registered handler for archives