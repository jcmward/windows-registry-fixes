# Windows Registry Fixes

> *For the OS we love to hate.*

## Introduction

This repository contains a collection of Windows Registry fixes aimed at improving UX and privacy.

It's no secret that Microsoft Windows' relationship with its users leaves something to be desired.
Windows 10 in particular came with a number of anti-features, especially from a privacy standpoint.
Therefore, I collected some Registry settings to (at least partially) disable the invasive spyware and advertisements.

By comparison, Windows 11 didn't seem to be as big of a downgrade for users, but there was one thing that ***really*** irked me: the new right-click context menu, which doesn't even support [keyboard mnemonics](https://en.wikipedia.org/wiki/Mnemonics_(keyboard)).
Fortunately, as with several other UI issues, there's a Registry value that can be set as a workaround.

Less fortunately, certain public institutions still require the use of non-free software, including Microsoft Windows, so switching to GNU/Linux is not yet an option for all my devices.

## Overview

- `ui-fixes.reg`: Fixes UI annoyances like the Windows 11 context menu.
- `uac-require-password.reg`: Require Administrator password for UAC elevation prompts.
- `touchpad.reg`: Modify touchpad slide/tap behaviour.
- `spyware-bloatware.reg`: Disables obnoxious spyware and bloatware like telemetry and Bing search integration.
    - **Disclaimer:** I'm not a Windows expert, and these fixes are by no means comprehensive.
      I'm sure much more could be done to protect user privacy (such as using a different OS).
- `search-highlights.reg`: Disable obnoxiously distracting "search highlights."
- `restore-wt-context-menu.reg`: Restore option to "Open in Terminal" to File Explorer context menu.
- `remove-onedrive-button.reg`: Removes OneDrive button from the File Explorer.
- `long-paths.reg`: Enables file paths longer than 260 characters.
- `lock-screen-skip.reg`: Skip empty lock screen; go directly to sign-in page.
- `lock-screen-enable.reg`: Re-enable lock screen.
- `creative-cloud.reg`: Removes Adobe Creative Cloud integration from File Explorer.
- `confirm-delete.reg`: Require user confirmation to delete files in File Explorer.

## Usage

> [!WARNING]
> 
> Editing the Windows Registry can cause system instability if done incorrectly.
> Use these files at your own risk.
> Always back up your Registry before making changes.

1.  Backup your Registry: Open `regedit`, go to `File > Export`, and save a backup.
2.  Double-click the `.reg` file(s) you want to apply.
3.  Confirm the changes when prompted.

**Note**: some Registry keys must be added by an Administrator.
