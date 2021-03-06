# WindowsToolkit

## THIS REPO WILL BE UPDATED ONCE WINDOWS 11 COMES OUT WITH THE USE OF WINGET

A collection of **Windows 10 apps and scripts** to optimize user and poweruser experience.

To make it in this list, apps must meet two or more of the following criteria:
* *Free to use* / *open source*
* *Theme Support* / *Fluent design*
* *Plugin Support*
* *Available in [Chocolatey Repository](https://community.chocolatey.org/packages)* / [Microsoft Store](https://www.microsoft.com/en-us/store/apps/windows)
* *Mobile version*

This list tries to give at least one alternative to every top pick for each app section, I tried to avoid apps that have been reported to contain spyware or adware in their bundle and apps that, in my opinion, are not worth mentioning.

## Table of contents

* [WindowsToolkit](#windowstoolkit)
  * [Why was this repository made?](#why-was-this-repository-made)
  * [Chocolatey Installation](#chocolatey-installation)
* [Applications](#applications)
  * [Browsers](#browsers)
  * [Email Clients](#email-clients)
  * [To do lists](#to-do-lists)
  * [Text Editors](#text-editors)
  * [Code Editors](#code-editors)
  * [Terminals](#terminals)
  * [FTP Clients](#ftp-clients)
  * [Torrent Clients](#torrent-clients)
  * [Media Players](#media-players)
  * [Photo Viewers](#photo-viewers)
  * [PDF Readers](#pdf-readers)
  * [Instant Messengers](#instant-messengers)
  * [Password Managers](#password-managers)
  * [Game Launchers](#game-launchers)
  * [Finder Utilities](#finder-utilities)
  * [Audio Utilities](#audio-utilities)
  * [Windows Utilities](#windows-utilities)
  * [Discord](#discord)
  * [Aesthetics](#aesthetics)
  * [Others](#others)

## Why was this repository made?

I believe that Windows is still far behind in terms of application installation, making use of a packet manager like Chocolatey can help you keep track of what's installed and of updates.

I also think that many applications are simply unknown to many people, therefore I want to give light to some of them. If, like me, you're using Windows, Android and iOS on a daily basis you will be able to find some nice Mobile apps.

I take no responsibility for misuse or problems encountered in these applications, I am simply listing them and all credits go to their respective authors.

If you want to provide feedback please do so using GitHub Issues.

## Chocolatey Installation

While Microsoft Store is pre-installed in Windows 10, [Chocolatey](https://chocolatey.org/install) is not, so here is how to install it.

> The information below is taken from the official Chocolatey site, link above.
> Keep in mind **most** Chocolatey packages are not official, but user-made, so sometimes they may take longer to update or be fixed.

**Requirements:**
* Windows 7+ / Windows Server 2003+
* PowerShell v3+
* .NET Framework 4.5+

**Installation:**
1. Press **Windows+R** to open the *Run* box.
2. Type `cmd` into the box and then press **Ctrl+Shift+Enter** to run the command as an administrator.
3. Run `Get-ExecutionPolicy`. If it returns `Restricted`, then run `Set-ExecutionPolicy AllSigned` ***OR*** `Set-ExecutionPolicy Bypass -Scope Process`.
4. Run the code below:

       Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

5. Wait a few seconds for the command to complete.
6. If you don't see any errors, you are ready to use Chocolatey! Type `choco` or `choco -?` now, or see [Getting Started](https://docs.chocolatey.org/en-us/getting-started) for usage instructions.

Now that the Chocolatey installation is done, let's get started!

# Applications

If you haven't done so already, make sure you install Chocolatey first following [Chocolatey Installation](#chocolatey-installation), if you have then you can move forward.

**Notes**:
* In the **Free** table column, if you see a `²` it means the application is also open source.
* I recommend using **Revo Uninstaller** to uninstall programs, instead of the default Windows method, this is because Revo also cleans any leftover files and registry entries, it won't break Chocolatey.
* If you're unsure whether to download the **Microsoft Store** version or the **Chocolatey** package of an app then my recommendation is using the Microsoft Store version first, if you have problems with it, then switch to the Chocolatey package.
* If you see that there is a **portable version** of the application, I would recommend giving it a try before installing.

## Browsers

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Google Chrome](https://www.google.com/chrome/) | :heavy_check_mark: | :heavy_check_mark: [Browse](https://chrome.google.com/webstore/category/themes) | :heavy_check_mark: [Browse](https://chrome.google.com/webstore/category/extensions) | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/GoogleChrome) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.android.chrome&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/google-chrome/id535886823) | Most used browser due to its simplicity and tools |
[Microsoft Edge](https://www.microsoft.com/en-us/edge) | :heavy_check_mark: | :heavy_check_mark: [Browse](https://microsoftedge.microsoft.com/addons/microsoft-edge-themes) | :heavy_check_mark: [Browse](https://microsoftedge.microsoft.com/addons/Microsoft-Edge-Extensions-Home) | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/microsoft-edge) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.microsoft.emmx&hl=en&gl=US), [iOS](https://apps.apple.com/app/id1288723196) | New Chromium-based build actually makes sense |
[Mozilla Firefox](https://www.mozilla.org/en-US/firefox/new/) | :heavy_check_mark:² | :heavy_check_mark: [Browse](https://addons.mozilla.org/en-US/firefox/themes/) | :heavy_check_mark: [Browse](https://addons.mozilla.org/en-US/firefox/extensions/) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/Firefox) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=org.mozilla.firefox&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/firefox-private-safe-browser/id989804926) | Great alternative to Chromium-based browsers |
[Vivaldi](https://vivaldi.com/) | :heavy_check_mark: | :heavy_check_mark: In app | :heavy_check_mark: [Browse](https://chrome.google.com/webstore/category/extensions) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/Vivaldi/3.7.2218.49) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.vivaldi.browser&hl=en&gl=US) | Feature-child of Chrome and Opera, but on steroids |

## Email Clients

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Mail and Calendar](https://www.microsoft.com/store/productId/9WZDNCRFHVQM) | :heavy_check_mark: | :heavy_check_mark: Fluent | :x: | :heavy_check_mark: [MS Store](https://www.microsoft.com/store/productId/9WZDNCRFHVQM) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.microsoft.office.outlook&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/microsoft-outlook/id951937596) | Plain and simple, the mobile version is basically Outlook for Mobile |
[MailSpring](https://getmailspring.com/) | :heavy_check_mark:² | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/mailspring) | :x: | Hidden gem among the email clients |
[Mozilla ThunderBird](https://www.thunderbird.net/en-US/) | :heavy_check_mark:² | :heavy_check_mark: [Browse](https://addons.thunderbird.net/en-US/thunderbird/static-themes/) | :heavy_check_mark: [Browse](https://addons.thunderbird.net/en-US/thunderbird/extensions/) | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/thunderbird) | :x: | Great community, has amazing import and export features |

## To do lists

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Microsoft To Do](https://to-do.microsoft.com/tasks/) | :heavy_check_mark: | :heavy_check_mark: Fluent | :x: | :heavy_check_mark: [MS Store](https://www.microsoft.com/store/productId/9NBLGGH5R558) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.microsoft.todos&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/microsoft-to-do/id1212616790) | This used to be called Wunderlist, Microsoft rebranded it and added more features, it's amazing |
[Trello](https://trello.com/home) | :heavy_check_mark:² | :heavy_check_mark: In app | :x: | :heavy_check_mark: [MS Store](https://www.microsoft.com/store/productId/9NBLGGH4XXVW) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.trello&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/trello-organize-anything/id461504587)  | Hidden gem among the email clients |

## Text Editors

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Notepad++](https://notepad-plus-plus.org/downloads/) | :heavy_check_mark:² | :heavy_check_mark: In app | :heavy_check_mark: [Browse](https://github.com/notepad-plus-plus/nppPluginList/blob/master/doc/plugin_list_x64.md) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/notepadplusplus), [MS Store (Unofficial)](https://www.microsoft.com/store/productId/9PHSCTZMKC27) | :x: | Community favorite for a long time |
[Notepads App](https://www.notepadsapp.com/) | :heavy_check_mark:² | :heavy_check_mark: Fluent | :x: |:heavy_check_mark: [MS Store](https://www.microsoft.com/store/productId/9NHL4NSC67WM) | :x: | Great looking new alternative for daily use |

## Code Editors

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Atom](https://atom.io/) | :heavy_check_mark:² | :heavy_check_mark: [Browse](https://atom.io/themes) | :heavy_check_mark: [Browse](https://atom.io/packages) | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/Atom/1.55.0) | :x: | If you're looking for something very minimalistic, this is for you |
[Sublime Text 3](https://www.sublimetext.com/) | :yellow_circle: Freemium | :heavy_check_mark: [Browse](https://packagecontrol.io/) | :heavy_check_mark: [Browse](https://packagecontrol.io/) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/SublimeText3) | :x: | Great and fast code editor, written in Python |
[Visual Studio Code](https://code.visualstudio.com/) | :heavy_check_mark:² | :heavy_check_mark: [Browse](https://vscodethemes.com/) | :heavy_check_mark: [Browse](https://marketplace.visualstudio.com/VSCode) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/vscode) | :x: | The most used code editor with A LOT of plugins |

## Terminals

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Fluent Terminal](https://github.com/felixse/FluentTerminal) | :heavy_check_mark:² | :heavy_check_mark: Fluent, In app | :x: | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/fluent-terminal), [MS Store](https://www.microsoft.com/store/productId/9P2KRLMFXF9T) | :x: | A brand new and very customizable terminal |
[Windows Terminal](https://github.com/microsoft/terminal) | :heavy_check_mark:² | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/microsoft-windows-terminal/1.6.10571.0), [MS Store](https://www.microsoft.com/store/productId/9N0DX20HK701) | :x: | Microsoft's own open source Terminal, very intuitive and sleek |

## FTP Clients

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[CarotDAV](http://rei.to/carotdav_en.html) | :heavy_check_mark: | :yellow_circle: Background image | :x: | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/carotdav) | :x: | Very minimalistic interface and includes WebDAV Local Server |
[FFFTP](https://github.com/ffftp/ffftp) | :heavy_check_mark:² | :x: | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/ffftp) | :x: | Many features packed in a small and open source package |
[WinSCP](https://winscp.net/eng/index.php) | :heavy_check_mark: | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/winscp), [MS Store (Paid)](https://www.microsoft.com/store/productId/9P0PQ8B65N8X) | :x: | The most popular out of the three, this is a no-brainer |

## Torrent Clients

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Deluge](https://deluge-torrent.org/) | :heavy_check_mark: | :heavy_check_mark: In app | :heavy_check_mark: [Browse](https://dev.deluge-torrent.org/wiki/Plugins) | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/deluge) | :x: | Very fast bittorrent client made in Python |
[qBitTorrent](https://github.com/ffftp/ffftp) | :heavy_check_mark:² | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/qbittorrent) | :x: | Very popular open source bittorrent client |

## Media Players

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[mpv](https://mpv.io/) | :heavy_check_mark:² | :x: | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/mpv) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=is.xyz.mpv) | Small and clean open source media player |
[PotPlayer](https://potplayer.daum.net/) | :heavy_check_mark: | :heavy_check_mark: [Browse](https://daumpotplayer.com/category/skins/) | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/potplayer) | :x: | Good looking media player, plays most types of files |
[VLC](https://www.videolan.org/vlc/) | :heavy_check_mark:² | :heavy_check_mark: [Browse](https://www.videolan.org/vlc/skins.html) | :heavy_check_mark: [Browse](https://addons.videolan.org/browse/cat/323/ord/latest/) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/vlc), [MS Store (Different)](https://www.microsoft.com/store/productId/9NBLGGH4VVNH) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=org.videolan.vlc&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/vlc-for-mobile/id650377962) | The most feature-rich player available |

## Photo Viewers

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[IrfanView](https://www.irfanview.com/) | :heavy_check_mark: | :heavy_check_mark: [Browse](https://www.irfanview.com/skins.htm) | :heavy_check_mark: [Browse](https://www.irfanview.com/plugins.htm) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/IrfanView), [MS Store](https://www.microsoft.com/store/productId/9PJZ3BTL5PV6) | :x: | An all-round complete viewer, great community |
[Microsoft Photos](https://www.microsoft.com/store/productId/9WZDNCRFJBH4) | :heavy_check_mark: | :heavy_check_mark: Fluent | :x: |:heavy_check_mark: [MS Store](https://www.microsoft.com/store/productId/9WZDNCRFJBH4) | :x: | The default photo viewer in Windows 10, it's getting better, but it's very basic |
[XnViewMP](https://www.xnview.com/en/xnviewmp/) | :heavy_check_mark: | :heavy_check_mark: In app | :heavy_check_mark: In app | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/XnViewMP) | :x: | A very nice photo viewer in a small package |

## PDF Readers

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Adobe Acrobat Reader](https://get.adobe.com/reader/) | :heavy_check_mark: | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/adobereader) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.adobe.reader&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/adobe-acrobat-reader-pdf-maker/id469337564) | The most popular PDF reader ever, free version is useful for signing |
[Xodo](https://www.xodo.com/) | :heavy_check_mark: | :heavy_check_mark: In app | :x: |:heavy_check_mark: [MS Store](https://www.microsoft.com/store/productId/9WZDNCRDJXP4) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.xodo.pdf.reader&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/pdf-reader-annotator-by-xodo/id805075929)  | The most feature packed free PDF viewer, able to edit, export and import pages |
[Okular](https://okular.kde.org/) | :heavy_check_mark:² | :x: | :x: | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/okular) | :x: | Very simple interface, but A TON of features, plus it's open source |

## Instant Messengers

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Signal](https://signal.org/en/) | :heavy_check_mark:² | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/signal) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=org.thoughtcrime.securesms&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/signal-private-messenger/id874139669) | The newest, open source instant messaging app |
[Telegram](https://telegram.org/) | :heavy_check_mark:² | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/telegram), [MS Store](https://www.microsoft.com/store/productId/9NZTWSQNTD0S) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=org.telegram.messenger&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/telegram-messenger/id686449807)  | The most feature rich messaging app, including bots, channels and more |
[WhatsApp](https://www.whatsapp.com/) | :heavy_check_mark: | :heavy_check_mark: In app | :x: | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/WhatsApp), [MS Store](https://www.microsoft.com/store/productId/9NKSQGP7F2NH) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.whatsapp&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/whatsapp-messenger/id310633997) | Old and popular, but has the least features out of the three |

## Password Managers

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[Bitwarden](https://bitwarden.com/) | :heavy_check_mark:² | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/bitwarden), [MS Store](https://www.microsoft.com/store/productId/9PJSDV0VPK04) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.x8bit.bitwarden&hl=en&utm_source=downloadatoz.com), [iOS](https://apps.apple.com/us/app/bitwarden-password-manager/id1137397744) | Integrates everywhere wonderfully, if you want to use it I recommend installing the browser extension as well |
[KeePass](https://keepass.info/) | :heavy_check_mark:² | :x: | :heavy_check_mark: [Browse](https://keepass.info/plugins.html) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/keepass) | :heavy_check_mark: [Android](https://keepass.info/download.html), [iOS](https://keepass.info/download.html)  | Simple password manager with plugin support |

## Game Launchers

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[GOG Galaxy](https://www.gog.com/galaxy) | :heavy_check_mark: | :x: | :heavy_check_mark: In app|:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/goggalaxy) | :x: | A great way to group all your games from different launchers, growing rapidly |
[Playnite](https://github.com/microsoft/terminal) | :heavy_check_mark:² | :heavy_check_mark: [Browse](https://playnite.link/forum/forum-8.html) | :heavy_check_mark: [Browse](https://playnite.link/forum/forum-6.html) |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/playnite) | :x: | Amazing, customizable open source game launcher |
[Steam](https://store.steampowered.com/) | :heavy_check_mark: | :heavy_check_mark: In app | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/steam-client) | :heavy_check_mark: [Android](https://play.google.com/store/apps/details?id=com.valvesoftware.android.steam.community&hl=en&gl=US), [iOS](https://apps.apple.com/us/app/steam-mobile/id495369748) | The biggest videogame marketplace and launcher available |

## Finder Utilities

Application | Free | Themes | Plugins | Packages | Mobile | Notes |
----------- | ---- | ------ | ------- | -------- | ------ | ----- |
[7-Zip](https://www.7-zip.org/) | :heavy_check_mark:² | :x: | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/7zip/19.0), [MS Store (Unofficial)](https://www.microsoft.com/store/productId/9MZ81RMK8JFD)  | :x: | The best archive manager, period. |
[File Converter](https://file-converter.org/?from=readme.md) | :heavy_check_mark:² | :x: | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/file-converter) | :x: | Very cool finder extension to quickly convert photos, audio, videos and documents. |
[Files](https://files-community.github.io/) | :heavy_check_mark:² | :heavy_check_mark: Fluent design | :x: |:heavy_check_mark: [Choco](https://community.chocolatey.org/packages/files), [MS Store](https://www.microsoft.com/store/productId/9NGHP3DX8HDX) | :x: | Very cool and modern file explorer alternative. |
[QTTabBar](http://qttabbar.wikidot.com/) | :heavy_check_mark: | :x: | :heavy_check_mark: In app | :heavy_check_mark: [Choco](https://community.chocolatey.org/packages/QTTabBar) | :x: | File Explorer extension which lets you have tabs and a few other functionalities. |

## Audio Utilities

- VB-AudioCable
- VoiceMeeter
- Audacity
- fre:ac
- Mp3Tag

## Windows Utilities

- Revo Uninstaller
- Everything
- PowerToys
- EarTrumpet
- ShareX
- Snip & Sketch

## Discord

- Discord
- PreMid

## Aesthetics

- ModernFlyouts
- Rainmeter
- Wallpaper Engine

## Others

- SoundPad
- Touch Portal
- Spotify
- Local
- JetBrains Toolbox
- AnyDesk
- Simplenote
