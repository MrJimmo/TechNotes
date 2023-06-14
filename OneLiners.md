These are various oneliners, hotkeys, tweaks, etc. that have been useful over the years.  Some no longer work on recent versions of Windows or indicated app.

**Calculator**:  Ctrl+U Turns on unit conversion (Pre-Win10 calc), Ctrl+E turns on date conversion. See View menu for Mortgage worksheet.

**CMD**: At a cmd prompt:   `set /a 0x123ABC`  ...converts hex values to decimal (1194684)

**CMD**: `PROMPT=[ $P$+ ]$_[$T]$G`  ...creates 2 line cmd prompt; Line one is [ _current path_ ], second line is [HH:MM:SS.MS]>

**CMD**: Color  [background][foreground],  color /? for possible colors.  Color 0C == Red Text on Black background

**CMD**: `echo "This is a test" | clip`,  clipboard now contains "This is a test".   `clip < ContentsOfThisFileWillBeAddedToClipboard.txt`

**CMD**: `doskey /history` ...list history of commands to console. (_F7 to show History in text dialog_)

**Excel**:  Control+Shift+Enter to input array formula.

**Explorer**:  Shift-Right click a file and there will be a new “Copy as Path” option on the context menu.

**Explorer**: Alt+D, ‘c’,’m’,’d’,[enter], starts a cmd prompt for the path currently browsing. “Powershell” to start PS in that dir.

**IE**: Start IE with extensions turned off: `iexplore.exe -extoff`  Helps when tracking down ActiveX failures.

**IE**: Start IE with extensions turned off and in Private:   `iexplore.exe -extoff -private`  (historically) forces youtube to send HTML5 video instead of flash.

**IE**: Increase number of rows in IE about:tabs  `[HKEY_CURRENT_USER\Software\Microsoft\Internet Explorer\TabbedBrowsing\NewTabPage]  "NumRows"=dword:00000006`

**Misc**: Extracting files from msi:   `msiexec /a foo.msi /qb TARGETDIR=C:\MyTargetDir`

**Misc**: To enter extend chars:  [Alt]+nnn, where nnn is any number.  Example: [Alt]+253 == ²

**Office**: `Shift+Alt+Up/Down arrow` moves selected line(s) up or down (or single line where cursor is).

**Office**: `Control+Alt+V` brings up Paste Special.  Allows pasting unformatted text.

**Office**: `Control+Shift+L` starts bullet point list

**Office**:  `Ctl+SPACE`, removes formatting from selected text

**Office**: `Control+Select-Text` to create non-contiguous text selection, allowing for selective formatting like highlighting

**Office**:  `Shift+F10` == Right-Click

**Surface**: Hit Down Volume + Windows button to take screenshot.

**Surface**:  Enabling flash for a specific domain not on the Allowed list: `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Internet Explorer, "DebugDomain "="domain.com"` (domain means no "www.")

**Taskbar**:  `Shift+Ctrl+Right-Click` taskbar Windows button to get oldstyle system menu.

**WER**: Most recent Windows Error Report:  `wevtutil qe "Application" /c:1 /rd:true /f:text /q:"*[System[EventID=1001]]"`

**Windows**: Lock your workstation from the cmd prompt: `rundll32.exe user32.dll,LockWorkStation`  (`Window+L`  also locks)

**Windows**: Secpol.msc -> Local Policies -> Security Options -> User Account Control: Switch to the secure desktop when prompting for elevation -> Disable.  No more dramatic switch when elevating.

**Windows**: `Windows+R, shell:::{ED7BA470-8E54-465E-825C-99712043E01C}` ...brings up list of control panel tasks and other settings. Naively referred to as “God Mode”

**Windows**: Find Locked File: Resmon.exe -> "CPU" Tab -> Select all images -> Enter search criteria in Associated Handles section.

**Windows**:  Resmon.exe -> "CPU" Tab -> Right-click hung process -> "Analyze Wait Chain"

**WinDbg**: `Alt+Delete` to break in (useful when Control-C not working and/or on a laptop with no Pause/Break key)

**Windows**: `Alt+PrntScr` == Capture active Window, `Ctrl+PrntScr` == Capture entire desktop (even across multiple monitors). `Shift+Windows+S` in Windows 10

**Windows**: `Control+C` while viewing most Message Boxes (like erros), will copy information as ASCII to the clipboard for eash paste into emails/documents.

**Windows**: `Ctrl+Alt+End` when TS’d into a machine will bring up Ctrl+Alt+Del screen.

**Windows**: `SystemPropertiesComputerName.exe` to change comp name and domain.

**Windows**: `SystemPropertiesRemote.exe` to change remote settings

**Windows**: If you accidently start clic-dragging something, keep your mouse button down and hit ESC to cancel

**Windows**: `Windows Key + X` to bring up menu of some advanced option.  `Windows Key + X`, `A` will quickly launch CMD (if set as default) as Admin (shows prompt).

**Windows**: If copy/paste stops working between local and remote desktop, try killing and starting a new `rdpclip.ex`e on the remote (maybe local)

**Windows**: Open folder of Modern apps on Win8 an above:   `%windir%\explorer.exe shell:::{4234d49b-0245-4df3-b780-3893943456e1`

**Windows**: Windows Tab, create new desktops, `Control+Windows LEFT/RIGHT` to switch.

**Windows**: `Windows+Shift+S`  Frosts entire desktop, crosshair for mouse, click-drag to capture part.  Paste into documents, emails, etc.

**Windows**: `Alt+Tab`, Window in focus, `Alt+Space`, `M`, hit an `Arrow Key` once, can now move window with moues.  Helps when windows get positioned out of mouse reach.
  
