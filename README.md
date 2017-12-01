# vscode-discord

> Display your current project on vscode in discord with Rich Presence

![Badge](https://img.shields.io/github/license/maxerbox/vscode-discord.svg)
![Badge](https://img.shields.io/david/maxerbox/vscode-discord.svg)

![Example](https://i.imgur.com/pLLPexT.png)

## Features

* Show up an icon for the current language in the rich embed

* Disable/enable for each workspace

* Strings entirely modifiable

* Removed registery writing

## Install

* Install the extension. The extension needs Discord to be launched.

* Facultative: Add Visual Studio Code as "Game" on Discord. **If you don't add it, it will still display "Playing Visual Studio Code" when you close it**.

## Changing the default icons

To change the default language icons, see [#12](https://github.com/maxerbox/vscode-discord/issues/12)

## Extension Settings

This extension contributes the following settings:

* `discord.enable`: enable/disable this extension
* `discord.showDebug`: Show the debugging icon in the rich presence when debugging
* `discord.debugIconText`: The small image debug text when debugging
* `discord.showElapsedTime`: Show/hide the time that has elapsed since you started editing a certain file
* `discord.clientID`: the client ID used by discord-rpc
* `discord.state`: The dicord rich presence state. Default to `Working on {projectName}`. `{projectName}`:workspace name
* `discord.details`: The discord rpc details. Default to `Editing {filename}`. {filename}: filename, {language} : language id.
* `discord.vscodeIconText`: The small icon hint (smallImageText). Default to Visual Studio Code
* `discord.languageIconText`: The hint for the language icon (largeImageText). Default to `{language}` {language} : language id
* `discord.idle`: The default text when there is no editor opened. Default to `idle`
* `discord.iconMap`: The iconMap for the filename extensions
* `discord.interval`: The interval time to update the informations in ms. Default to 3000ms

## Frequently asked Questions

#### Can I get banned?
Well, [someone already asked for it](https://github.com/maxerbox/vscode-discord/issues/3). I emailed the Discord Team, and that's totally fine, unless you disrespect their Terms and Conditions.

#### It's not showing on Discord?
Check out if Visual Studio Code is added as game on your Discord client.

## License

The source code is licensed under the [ISC](LICENSE) License.

The icons are licensed under the [Creative Commons - ShareAlike (CC BY-SA)](https://creativecommons.org/licenses/by-sa/4.0/) license.

## Release Notes

### 0.0.1

Initial release of `vscode-discord`

### 0.0.2

Rewritten Discord Register

### 0.0.3

* Removed Discord Registers for OSs other than Windows.
* Added python support
* Added a VSCode disposable client, to let the Rich Presence reset when the process quit.

### 1.0.0

* First realease

* Removed Registry

* Added a new option: show debug

### 1.0.1

* Better Icon Mapping

* Patched time issue

* Made elapsed time toggel-able through `discord.showElapsedTime` setting

---
