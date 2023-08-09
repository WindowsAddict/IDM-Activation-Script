# IDM Activation Script

An open source tool to activate and reset trial of [Internet Download Manager](https://www.internetdownloadmanager.com/)

## Features

-   IDM activation with registry key lock method
-   Activation persists even after installing IDM updates
-   IDM trial reset
-   Fully open source
-   Based on transparent batch script

## IAS Latest Release

Last Release - v0.8 (10-Aug-2023)\
[GitHub](https://github.com/WindowsAddict/IDM-Activation-Script)

## Download / How to use it?

-   First fresh install [Internet Download Manager](https://www.internetdownloadmanager.com/). Make sure previous cracks/patches are removed/uninstalled if there are any.
-   After that follow below steps to activate it.

### Method 1 - PowerShell

(Recommended)

-   On Windows 8.1/10/11, right-click on the windows start menu and select PowerShell or Terminal (Not CMD).
-   Copy-paste the below code and press enter\
    `irm https://massgrave.dev/ias | iex`
-   You will see the activation options, and follow onscreen instructions.
-   That's all.

### Method 2 - Traditional

-   Download the file from [here](https://github.com/WindowsAddict/IDM-Activation-Script/archive/refs/heads/main.zip)
-   Right click on the downloaded zip file and extract
-   In the extracted folder, run the file named `IAS.cmd`
-   You will see the activation options, and follow onscreen instructions.
-   That's all.

## Info

#### Activation

-   This script applies registry lock method to activate Internet download manager (IDM).
-   This method requires Internet at the time of activation.
-   IDM updates can be installed directly without having to activate again.
-   After the activation, if in some case, the IDM starts to show activation nag screen, then just run the activation option again.

#### Reset IDM Activation / Trial

-   Internet download manager provides 30 days trial period, you can use this script to reset this Activation / Trial period whenever you want.
-   This option also can be used to restore status if in case the IDM reports fake serial key and other similar errors.

#### OS requirement

-   Project is supported for Windows 7/8/8.1/10/11 and their Server equivalent.
-   Powershell method to run IAS is supported on Windows 8 and higher.

#### Advanced Info

-   To add a custom name in IDM license info, edit the line number 21 in the script file.
-   For activation in unattended mode, run the script with `/act` parameter.
-   For reset in unattended mode, run the script with `/res` parameter.
-   To enable silent mode with above two methods, run the script with `/s` parameter.

## How does it work?

-   IDM stores the data related to trial and activation in across various registry keys. Some of these keys are locked to protect them from tampering and data is stored in a pattern to track the fake serial issue and the remaining trial days. To activate it, script here simply generate those registry keys by triggering a few downloads in IDM and identifies those registry keys and locks them so IDM can't edit and view. That way IDM can not show the warning that it's activated with a fake serial key.

## Troubleshoot

-   Browser Integration Fix: [Chrome](https://www.internetdownloadmanager.com/register/new_faq/bi9.html) [FireFox](https://www.internetdownloadmanager.com/register/new_faq/bi4.html)
-   Reach out to us on [Discord](https://discord.gg/gjJEfq7ux8) (signup not required) with an error screenshot.

[![](https://lookimg.com/images/2023/03/21/QTvjcD.png)](https://discord.gg/gjJEfq7ux8)

## Changelog

v0.8

-   Move the project to [Github](https://github.com/WindowsAddict/IDM-Activation-Script) and [massgrave.dev](https://massgrave.dev/idm-activation-script.html)
-   Minor bug fixes
-   Add an info to inform users that empty registry keys are being deleted when script deletes a lot of them

## Screenshots

![](https://github.com/massgravel/mas-docs/blob/main/IAS.png?raw=true)

![](https://github.com/massgravel/mas-docs/blob/main/IAS_Activation.png?raw=true)

## Credits

|                                             |                                                                                                                                                                                                                                        |
|---------------------|---------------------------------------------------|
| Dukun Cabul                                 | Original researcher of this IDM trial reset and activation logic, made an Autoit tool for these methods, [IDM-AIO_2020_Final](https://nsaneforums.com/topic/371047-discussion-internet-download-manager-fixes/page/8/#comment-1632062) |
| AveYo aka BAU                               | [reg_own lean and mean snippet](https://pastebin.com/XTPt0JSC)                                                                                                                                                                         |
| [abbodi1406](https://github.com/abbodi1406) | Help in coding                                                                                                                                                                                                                         |
| WindowsAddict                               | IAS Author                                                                                                                                                                                                                             |

And thanks to the IAS users for their interest, feedback, and assistance.

------------------------------------------------------------------------

Made with Love ❤️
