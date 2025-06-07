# Registry Fixes

## Introduction

This repository contains a collection of Windows registry fixes aimed at
improving UX and privacy.

It's no secret that Microsoft Windows' relationship with its users leaves
something to be desired.  Windows 10 in particular came with a number of
headaches, especially from a privacy standpoint.  Naturally, I collected some
registry hacks to disable the spyware.  By comparison, Windows 11 didn't feel
like as much of a step down for users, but there was one thing that
***really*** irked me when I first used it: the broken context (right-click)
menu.  That one is a doozy, and directly interferes with my productivity.
Fortunately, as with many other issues, there's a registry hack that can be
used as a workaround.

## Overview

- `ui-fixes.reg`: Fixes UI annoyances like the Windows 11 context menu.
- `spyware-bloatware.reg`: Disables Windows spyware and bloatware features like
  Cortana and telemetry.
    - **Disclaimer:** I'm not an expert, and I'm sure much more could be done
      to protect user privacy (apart from using a different OS).
- `long-paths.reg`: Enables support for long file paths.
- `lock-screen.reg`: Customizes lock screen behavior and fixes related issues.
- `creative_cloud.reg`: Removes Adobe Creative Cloud integration from File
  Explorer.

## How to Use

1. Backup your registry: Open `regedit`, go to `File > Export`, and save a
backup.
2. Double-click the `.reg` file(s) you want to apply.
3. Confirm the changes when prompted.

> [!WARNING]
> 
> Editing the Windows Registry can cause system instability if done
> incorrectly.  Use these files at your own risk.  Always back up your registry
> before making changes.

## Related

There are some interesting-looking tools available that can do a lot more.
Personally I just want a minimal solution though.

- ["Awesome" Win11](https://github.com/awesome-windows11/windows11)
- [Windows 11 Fixer](https://github.com/99natmar99/Windows-11-Fixer)
- [CrapFixer](https://github.com/builtbybel/CrapFixer)

