# Registry Fixes

## Introduction

This repository contains a collection of Windows Registry fixes aimed at
improving UX and privacy.

It's no secret that Microsoft Windows' relationship with its users leaves
something to be desired.  Windows 10 in particular came with a number of
headaches, especially from a privacy standpoint.  Therefore, I collected some
Registry hacks to disable the spyware.

By comparison, Windows 11 didn't seem to be as big of a downgrade for users,
but there was one thing that ***really*** irked me: the broken context
(right-click) menu, which doesn't even have keyboard shortcuts.  That one is a
doozy, as it directly interferes with my productivity.  Fortunately, as with
several other UI issues, there's a Registry hack that can be used as a
workaround.

## Overview

- `ui-fixes.reg`: Fixes UI annoyances like the Windows 11 context menu.
- `spyware-bloatware.reg`: Disables Windows spyware and bloatware features like
  telemetry, Cortana, and Bing search integration.
    - **Disclaimer:** I'm not a Windows expert, and these fixes are by no means
      comprehensive.  I'm sure much more could be done to protect user privacy
      (apart from just using a different OS).
- `search-highlights.reg`: Disable obnoxiously distracting "search highlights."
- `remove-onedrive-button.reg`: Removes OneDrive button from the File Explorer.
- `long-paths.reg`: Enables file paths longer than 260 characters.
- `lock-screen.reg`: Fixes lock screen annoyances.
- `creative-cloud.reg`: Removes Adobe Creative Cloud integration from File
  Explorer.
- `confirm-delete.reg`: Requires user confirmation to delete files in File
  Explorer.

## How to Use

> [!WARNING]
> 
> Editing the Windows Registry can cause system instability if done
> incorrectly.  Use these files at your own risk.  Always back up your Registry
> before making changes.

1. Backup your Registry: Open `regedit`, go to `File > Export`, and save a
backup.
2. Double-click the `.reg` file(s) you want to apply.
3. Confirm the changes when prompted.

## Related

There are some interesting-looking tools available that can do a lot more.
Personally I just want a minimal solution without extra dependencies though.

- ["Awesome" Win11](https://github.com/awesome-windows11/windows11)
- [Windows 11 Fixer](https://github.com/99natmar99/Windows-11-Fixer)
- [CrapFixer](https://github.com/builtbybel/CrapFixer)

