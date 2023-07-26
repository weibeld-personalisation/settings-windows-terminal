# Windows Terminal Settings

Custom settings file for [Windows Terminal](https://learn.microsoft.com/en-us/windows/terminal/).

## Import

1. Press _Ctrl-Shift-,_ to open the Windows Terminal settings file
   - Alternatively go to _Settings > Open JSON file_
1. Make a copy of the non-built-in profile objects in `profiles.list` in the settings file
   - The non-built-in profiles include all profiles except _Command Prompt_ and _Windows PowerShell_
1. Paste the content of [`settings.json`](settings.json) into the settings file
1. Add the copied profile objects from above to `profiles.list` in the settings file
1. Save the file and restart Windows Terminal

## Export

1. Press _Ctrl-Shift-,_ to open the Windows Terminal settings file
   - Alternatively go to _Settings > Open JSON file_
1. Copy the settings file content into [`settings.json`](settings.json)
1. In `profiles.list` of the copied settings, remove all but the built-in profiles
   - The built-in profiles include _Command Prompt_ and _Windows PowerShell_
1. Set `defaultProfile` to `{0caa0dad-35be-5f56-a8ff-afceeeaa6101}` (_Command Prompt_)

## Notes

### Characteristics

The main customisations in these settings are as follows:

1. Only includes the _Windows PowerShell_ and _Command Prompt_ profiles (other default profiles are removed)
1. Adds the [_iTerm2 Default_](https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/windowsterminal/iTerm2%20Default.json) colour scheme
1. Enables _Automatically copy selection to clipboard_
1. Sets the following profile defaults (i.e. settings that will be applied to all profiles):
   1. Starting directory: `%USERPROFILE%/Desktop`
   1. Color scheme: _iTerm2 Default_
   1. Font face: _Cascadia Mono_
   1. Font size: _11_
   1. Cursor shape: _Filled box_
   1. Intense text style: _Bold font_
   1. Bell notification style: _none_

### Icons

The [`icons`](icons) directory contains images that can be used as icons for new profiles.

Windows Terminal also includes some built-in icons that can be accessed through the following application content URIs from within Windows Terminal:

| Icon           | URI                                                                  |
|:---------------|:---------------------------------------------------------------------|
| Tux            | `ms-appx:///ProfileIcons/{9acb9455-ca41-5af7-950f-6bca1bc9722f}.png` |
| PowerShell     | `ms-appx:///ProfileIcons/{61c54bbd-c2c6-5271-96e7-009a87ff44bf}.png` |
| Command Prompt | `ms-appx:///ProfileIcons/{0caa0dad-35be-5f56-a8ff-afceeeaa6101}.png` |
