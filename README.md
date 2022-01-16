# Windows10Debloater

[![made-with-powershell](https://img.shields.io/badge/PowerShell-1f425f?logo=Powershell)](https://microsoft.com/PowerShell)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

Script/Utility/Application to debloat Windows 10, to remove Windows pre-installed unnecessary applications, stop some telemetry functions, stop Cortana from being used as your Search Index, disable unnecessary scheduled tasks, and more...

Be sure to look at the Contributors' GitHubs to see if they have GitHub sponsorships as well since they have contributed to this open-source project. (https://github.com/BOB450/Windows10Debloater/graphs/contributors)

## Disclaimer

**WARNING:** I do **NOT** take responsibility for what may happen to your system! Run scripts at your own risk!
Also, other variants of this repo are not technically "new" versions of this, but they are different in their own respective ways. There are some sites saying that other projects are "new" versions of this, but that is inaccurate. 

## How To Run the Windows10Debloater.ps1 and the Windows10DebloaterGUI.ps1 files

There are different methods of running the PowerShell script. The methods are as follows:

### First Method

1) Download the .zip file on the main page of the GitHub and extract the .zip file to your desired location
2) Once extracted, open [PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/overview?view=powershell-5.1) (or [PowerShell ISE](https://docs.microsoft.com/en-us/powershell/scripting/windows-powershell/ise/introducing-the-windows-powershell-ise?view=powershell-7)) as an Administrator
3) Enable PowerShell execution
<code>Set-ExecutionPolicy Unrestricted -Force</code>
4) On the prompt, change to the directory where you extracted the files:
  e.g. - `cd c:\temp`
5) Next, to run either script, enter in the following:
  e.g. - `.\Windows10DebloaterGUI.ps1`

### Second Method

1) Download the .zip file on the main page of the GitHub and extract the .zip file to your desired location
2) Right-click the PowerShell file that you'd like to run and click on "Run With PowerShell"
3) This will allow the script to run without having to do the above steps but Powershell will ask if you're sure you want to run this script.

Remember this script **NEEDS** to be run as admin in order to function properly.

## Sysprep, Interactive, and GUI Application

There are now 3 versions of **Windows10Debloater** - There is an interactive version, a GUI app version, and a pure silent version.



- **`Windows10Debloater.ps1`** -> This interactive version is what it implies - a Windows10Debloater script with interactive prompts. This one should not be used for deployments that require a silent script with optional parameters. This script gives you choices with prompts as it runs so that you can make the choices of what the script does.

- **`Windows10DebloaterGUI.ps1`** -> There is now a GUI Application named Windows10DebloaterGUI.ps1 with buttons to perform all of the functions that the scripts do. This is better for the average user who does not want to work with code, or if you'd prefer to just see an application screen. 

## These registry keys are

EclipseManager,
ActiproSoftwareLLC,
Microsoft.PPIProjection,
Microsoft.XboxGameCallableUI

You can choose to either 'Debloat' or 'Revert'. Depending on your choice, either one will run specific code to either debloat your Windows 10 machine.

## The Debloat switch choice runs the following functions

Debloat,
Remove-Keys,
Protect-Privacy,
Stop-EdgePDF (If chosen)

## The Revert switch choice runs the following functions

Revert-Changes,
Enable-EdgePDF

The Revert option reinstalls the bloatware and changes your registry keys back to default. 

## The scheduled tasks that are disabled are

XblGameSaveTaskLogon,
XblGameSaveTask,
Consolidator,
UsbCeip,
DmClient

These scheduled tasks that are disabled have absolutely no impact on the function of the OS.

## Bloatware that is removed

[3DBuilder](https://www.microsoft.com/en-us/p/3d-builder/9wzdncrfj3t6),
[ActiproSoftware](https://www.microsoft.com/en-us/p/actipro-universal-windows-controls/9wzdncrdlvzp),
[Alarms](https://www.microsoft.com/en-us/p/windows-alarms-clock/9wzdncrfj3pr?activetab=pivot:overviewtab),
[Appconnector](https://www.microsoft.com/en-us/p/connector/9wzdncrdjmlj?activetab=pivot:overviewtab),
[Asphalt8](https://www.microsoft.com/en-us/p/asphalt-8-racing-game-drive-drift-at-real-speed/9wzdncrfj26j?activetab=pivot:overviewtab),
[Autodesk SketchBook](https://www.microsoft.com/en-us/p/autodesk-sketchbook/9nblggh4vzw5),
[MSN Money](https://www.microsoft.com/en-us/p/msn-money/9wzdncrfhv4v?activetab=pivot:overviewtab),
[Food And Drink](https://www.microsoft.com/en-us/p/food-and-drink/9nblggh0jhqg),
[Health And Fitness](https://www.microsoft.com/en-us/p/health-fitness-free/9wzdncrcwcdp),
[Microsoft News](https://www.microsoft.com/en-us/p/microsoft-news/9wzdncrfhvfw#activetab=pivot:overviewtab),
[MSN Sports](https://www.microsoft.com/en-us/p/msn-sports/9wzdncrfhvh4?activetab=pivot:overviewtab),
[MSN Travel](https://www.microsoft.com/en-us/p/msn-travel/9wzdncrfj3ft?activetab=pivot:overviewtab),
[MSN Weather](https://www.microsoft.com/en-us/p/msn-weather/9wzdncrfj3q2?activetab=pivot:overviewtab),
BioEnrollment,
[Windows Camera](https://www.microsoft.com/en-us/p/windows-camera/9wzdncrfjbbg#activetab=pivot:overviewtab),
CandyCrush,
CandyCrushSoda,
Caesars Slots Free Casino,
ContactSupport,
CyberLink MediaSuite Essentials,
DrawboardPDF,
Duolingo,
EclipseManager,
Facebook,
FarmVille 2 Country Escape,
Flipboard,
Fresh Paint,
Get started,
iHeartRadio,
King apps,
Maps,
March of Empires,
Messaging,
Microsoft Office Hub,
Microsoft Solitaire Collection,
Microsoft Sticky Notes,
Minecraft,
Netflix,
Network Speed Test,
NYT Crossword,
Office Sway,
OneNote,
OneConnect,
Pandora,
People,
Phone,
Phototastic Collage,
PicsArt-PhotoStudio,
PowerBI,
Royal Revolt 2,
Shazam,
Skype for Desktop,
SoundRecorder,
TuneInRadio,
Twitter,
Windows communications apps,
Windows Feedback,
Windows Feedback Hub,
Windows Reading List,
Zune Music,
Zune Video.

## Allowlist and Blocklist
There may be some confusion, but when using the Allowlist/Blocklist, the checkmark means it is on the blocklist, and that it will be removed.

## Credits

Thank you to [a60wattfish](https://github.com/a60wattfish), [abulgatz](abulgatz), [xsisbest](https://github.com/xsisbest), [Damian](https://github.com/Damian), [Vikingat-RAGE](https://github.com/Vikingat-RAGE), Reddit user [/u/GavinEke](https://github.com/GavinEke), and all of the contributors (https://github.com/Sycnex/Windows10Debloater/graphs/contributors) for the suggestions, code, changes, and fixes that you have all graciously worked hard on and shared! You all have done a fantastic job!
