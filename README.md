# Windows Terminal Settings

Custom settings file for [Windows Terminal](https://learn.microsoft.com/en-us/windows/terminal/).

## Import

1. Go to _Settings > Open JSON file_ in Windows Terminal
1. Paste the entire content of [`settings.json`](settings.json) into the local `settings.json` file
1. Save the file and restart Windows Terminal

## Features

The main differences to the default settings are as follows:

1. Does only include the _Windows PowerShell_ and _Command Prompt_ profiles (other default profiles are removed)
1. Adds the [_iTerm2 Default_](https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/windowsterminal/iTerm2%20Default.json) colour scheme
1. Has _Automatically copy selection to clipboard_ enabled
1. Sets the following profile defaults (i.e. settings that will be applied to all profiles):
   1. Starting directory: `%USERPROFILE%/Desktop`
   1. Color scheme: _iTerm2 Default_
   1. Font face: _Cascadia Mono_
   1. Font size: _11_
   1. Cursor shape: _Filled box_
   1. Intense text style: _Bold font_
   1. Bell notification style: _none_

## Icons

The [`icons`](icons) directory contains image files that may be used as icons for new profiles.

Windows Terminal also includes some built-in icons that can be accessed through the following application content URIs from within the Windows Terminal settings:

| Icon           | URI                                                                  |
|:---------------|:---------------------------------------------------------------------|
| Tux            | `ms-appx:///ProfileIcons/{9acb9455-ca41-5af7-950f-6bca1bc9722f}.png` |
| PowerShell     | `ms-appx:///ProfileIcons/{61c54bbd-c2c6-5271-96e7-009a87ff44bf}.png` |
| Command Prompt | `ms-appx:///ProfileIcons/{0caa0dad-35be-5f56-a8ff-afceeeaa6101}.png` |
