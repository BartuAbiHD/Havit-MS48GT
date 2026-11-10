# Havit MS48GT

**English** | [Türkçe](README-TR.md)

Windows cursor settings tool for the **Havit MS48GT** wireless mouse. One small `.exe`, no installation, no Python needed.

**[⬇ Download the latest version](https://github.com/BartuAbiHD/Havit-MS48GT/releases/latest)** (`Havit-MS48GT.exe`, 64-bit Windows)

## What it does

- Pointer speed (1-20) and *Enhance pointer precision* (acceleration) on/off
- Mouse wheel scroll lines and double-click time
- Swap left/right buttons
- Profiles: save your current settings under a name and load them again later
- Keeps running in the system tray when you close the window (quit from the tray menu)
- Languages: English, Türkçe, Azərbaycanca, Deutsch, Français, Español, Русский

> The MS48GT has no DPI button, side buttons, lighting or vendor software, and its battery level cannot be read, so there is nothing to configure on the mouse itself. This tool changes the **Windows** pointer settings. They apply to all mice, not only this one.

## Usage

1. Download `Havit-MS48GT.exe` from the [Releases](https://github.com/BartuAbiHD/Havit-MS48GT/releases) page.
2. Run it. Change a setting and press **Apply**. **Read** loads the current Windows values.
3. To save a set of values, type a name and press **Save current**. Pick it from the list and press **Load** to apply it again.
4. Closing the window hides the program in the system tray. Left-click the tray icon to open it, right-click for **Exit**.

Settings are stored in `%APPDATA%\havit_ms` (`profiles.json`, `settings.json`). Delete that folder to reset the program.

## Windows SmartScreen warning

The program is not code-signed, so Windows may show *"Windows protected your PC"*. Click **More info** > **Run anyway**. To check that your download is the original file, compare its SHA256 with the one in the release notes:

```powershell
Get-FileHash .\Havit-MS48GT.exe -Algorithm SHA256
```

## Requirements

- Windows 10 or 11, 64-bit
- Nothing else. Python and all libraries are inside the exe.

## Links

- Website: [lojitekno.tr](https://lojitekno.tr)
- Forum: [sosyal.lojitekno.tr](https://sosyal.lojitekno.tr)
- YouTube: [yton.tr/@lojitekno](https://yton.tr/@lojitekno)

## License

Copyright © 2026 BartuAbiHD. All rights reserved.

The program is free to use. It is provided "as is", without warranty of any kind. The source code is not published, and the program may not be modified, decompiled or redistributed without permission. Third-party components keep their own licenses, see below.

## Third-party notices

`Havit-MS48GT.exe` contains the following open-source components.

- **Dear PyGui** 2.3.1 (MIT), which includes **Dear ImGui** (MIT): https://github.com/hoffstadt/DearPyGui
- **hidapi** (Python package *hidapi* 0.15.0, used under its BSD license): https://github.com/trezor/cython-hidapi
- **Python** (PSF License): https://docs.python.org/3/license.html
- **PyInstaller** (GPL-2.0-or-later with the exception that allows distributing programs built with it under any license): https://pyinstaller.org

<details>
<summary>Dear PyGui - MIT License</summary>

```
MIT License

Copyright (c) 2026 Dear PyGui, LLC

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

</details>

<details>
<summary>hidapi - BSD License</summary>

```
Copyright (c) 2011, Gary Bishop
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

    * Redistributions of source code must retain the above copyright notice,
      this list of conditions and the following disclaimer.
    * Redistributions in binary form must reproduce the above copyright
      notice, this list of conditions and the following disclaimer in the
      documentation and/or other materials provided with the distribution.
    * Neither the name of Signal 11 Software nor the names of its
      contributors may be used to endorse or promote products derived from
      this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
POSSIBILITY OF SUCH DAMAGE.
```

</details>
