# Windows Terminal Settings

Customised settings file for [Windows Terminal](https://learn.microsoft.com/en-us/windows/terminal/).

## Install

1. In Windows Terminal, go to _Settings > Open JSON file_
1. Overwrite the content of the settings file that opens with the content of [`settings.json`](settings.json) in this repository
1. Save the settings file and restart Windows Terminal

## Features

The custom settings differ from the default settings mainly in the following points:

1. Does only include the default _Windows PowerShell_ and _Command Prompt_ profiles
1. Does only include the custom [_iTerm2 Default_](https://github.com/weibeld/iTerm2-Color-Schemes/blob/master/windowsterminal/iTerm2%20Default.json) colour scheme
1. Has _Automatically copy selection to clipboard_ enabled
1. Sets the following profile defaults:
   1. _Starting directory_ is `%USERPROFILE%/Desktop`
   1. _Color scheme_ is _iTerm2 Defaults_
   1. _Font face_ is _Cascadia Mono_
   1. _Font size_ is 11
   1. _Cursor shape_ is _Filled box_
   1. _Intense text style_ is _Bold font_
   1. _Bell notification style_ is _none_

## Icons

When adding profiles to Windows Terminal, you may use the icons in `icons` as the profile icons (requires to download and store them locally).
