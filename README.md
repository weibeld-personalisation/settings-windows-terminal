# Windows Terminal Settings

Customised settings file for [Windows Terminal](https://learn.microsoft.com/en-us/windows/terminal/).

## Install

1. Go to _Settings > Open JSON file_ in Windows Terminal
1. Overwrite the entire content of the settings JSON file that opens with the content of [`settings.json`](settings.json)
1. Save the settings file and restart Windows Terminal

## Features

The custom settings differ from the default settings as follows:

1. Does only include the _Windows PowerShell_ and _Command Prompt_ profiles (other default profiles are removed)
1. Adds the [_iTerm2 Default_](https://github.com/weibeld/iTerm2-Color-Schemes/blob/master/windowsterminal/iTerm2%20Default.json) colour scheme
1. Has _Automatically copy selection to clipboard_ enabled
1. Sets the following profile defaults (i.e. settings that will be applied to all profiles):
   1. _Starting directory_ is `%USERPROFILE%/Desktop`
   1. _Color scheme_ is _iTerm2 Defaults_
   1. _Font face_ is _Cascadia Mono_
   1. _Font size_ is 11
   1. _Cursor shape_ is _Filled box_
   1. _Intense text style_ is _Bold font_
   1. _Bell notification style_ is _none_

## Icons

The [`icons`](icons) directory contains image files that may be used as icons for new profiles.

Windows Terminal also includes some built-in icons that can be accessed through the following application content URIs from within the Windows Terminal settings:

| Icon           | URI                                                                  |
|:---------------|:---------------------------------------------------------------------|
| Linux penguin  | `ms-appx:///ProfileIcons/{9acb9455-ca41-5af7-950f-6bca1bc9722f}.png` |
| PowerShell     | `ms-appx:///ProfileIcons/{61c54bbd-c2c6-5271-96e7-009a87ff44bf}.png` |
| Command Prompt | `ms-appx:///ProfileIcons/{0caa0dad-35be-5f56-a8ff-afceeeaa6101}.png` |
