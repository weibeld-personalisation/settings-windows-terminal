# Windows Terminal Settings

Custom settings file for [Windows Terminal](https://learn.microsoft.com/en-us/windows/terminal/).

## Usage

### Edit

For editing the settings, it's best to directly edit the [`settings.json`](settings.json) file.

> All the supported properties are described in the [Windows Terminal documentation](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/startup).

Before importing, validate the JSON with the [JSON Validator](https://jsonlint.com/).

### Import

To import [`settings.json`](settings.json) into Windows Terminal, proceed as follows:

1. Press _Ctrl-Shift-Comma_ to open the Windows Terminal settings file
   - Alternatively go to _Settings > Open JSON file_
1. Copy the content of [`settings.json`](settings.json) into the settings file and save
   - Before copying, make sure that no needed profiles will be overwritten in `profiles.list`
1. Restart Windows Terminal to make sure all settings get applied

### Export

If you made changes to the Windows Terminal settings through the UI, you can export the current settings file into this respository as follows:

1. Press _Ctrl-Shift-Comma_ to open the Windows Terminal settings file
   - Alternatively go to _Settings > Open JSON file_
1. Paste the settings file content into [`settings.json`](settings.json)

## Features

The custom settings differ as follows from the default settings:

1. Defines custom [keyboard shortcuts](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/actions)
1. Adds the [_iTerm2 Default_](https://github.com/mbadolato/iTerm2-Color-Schemes/blob/master/windowsterminal/iTerm2%20Default.json) colour scheme
1. Enables automatic copy of selection to clipboard ([`copyOnSelect`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/interaction#automatically-copy-selection-to-clipboard))
1. Disables automatic creation of profiles ([`disabledProfileSources`](https://learn.microsoft.com/en-us/windows/terminal/dynamic-profiles#prevent-a-profile-from-being-generated))
1. Enables launch in maximised mode ([`launchMode`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/startup#launch-mode))
1. Disables large paste warnings ([`largePasteWarning`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/interaction#warn-when-the-text-to-paste-is-very-large))
1. Hides the title bar ([`showTabsInTitlebar`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/appearance#hide-the-title-bar))
1. Disables the tab switcher UI ([`tabSwitcherMode`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/interaction#tab-switcher-interface-style))
1. Disables animations when creating and closing panes ([`disableAnimations`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/appearance#disable-pane-animations))
1. Customise the word delimiters to more closely resemble iTerm2 ([`wordDelimiters`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/interaction#word-delimiters))
1. Adds a _WSL Ubuntu_ and _WSL Debian_ profile for the corresponding WSL Linux distributions
1. Sets the following [profile defaults](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/profile-general):
   1. Set colour scheme to _iTerm2 Default_ ([`colorScheme`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/profile-appearance#color-scheme))
   1. Set font to _Cascadia Mono, 11pt_ ([`font`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/profile-appearance#font))
   1. Set cursor shape `filledBox` ([`cursorShape`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/profile-appearance#cursor-shape))
   1. Set intense text style to `bold` ([`intenseTextStyle`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/profile-appearance#intense-text-formatting))
   1. Disable bell notifications ([`bellStyle`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/profile-advanced#bell-notification-style))
   1. Set starting directory to `%USERPROFILE%/Desktop` ([`startingDirectory`](https://learn.microsoft.com/en-us/windows/terminal/customize-settings/profile-general#starting-directory))

### Icons

The [`icons`](icons) directory contains images that can be used as icons for new profiles.

Windows Terminal also includes some built-in icons that can be accessed through the following application content URIs from within Windows Terminal:

| Icon           | URI                                                                  |
|:---------------|:---------------------------------------------------------------------|
| Tux            | `ms-appx:///ProfileIcons/{9acb9455-ca41-5af7-950f-6bca1bc9722f}.png` |
| PowerShell     | `ms-appx:///ProfileIcons/{61c54bbd-c2c6-5271-96e7-009a87ff44bf}.png` |
| Command Prompt | `ms-appx:///ProfileIcons/{0caa0dad-35be-5f56-a8ff-afceeeaa6101}.png` |
