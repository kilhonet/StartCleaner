# StartCleaner

**A free Windows startup manager that shows the programs, scheduled tasks and services that launch at boot in one place, and tidies them up safely by turning them off instead of deleting them.**

English · [한국어](README.ko.md) · [简体中文](README.zh-CN.md) · [日本語](README.ja.md) · [Español](README.es.md) · [Português (Brasil)](README.pt-BR.md) · [Français](README.fr.md)

> This document is a translation. If anything differs, the [Korean version](README.ko.md) is authoritative.

![Platform](https://img.shields.io/badge/platform-Windows%2010%20%2F%2011%20(64--bit)-0078D4)
![License](https://img.shields.io/badge/license-Freeware-brightgreen)
[![Download](https://img.shields.io/badge/download-kilho.net-orange)](https://down.kilho.net/startcleaner?lang=en)

![StartCleaner window](images/startcleaner-en.webp)

## Overview

Every time you turn on your PC, messengers, update helpers and all kinds of services start along with it. Each one is small, but together they slow down startup and take up memory.

StartCleaner gathers everything that starts automatically from four places — **Startup** folders, the **Registry**, scheduled **Task**s and **Service**s — and shows it in a single list. Select an item you don't need and click **Disable**, and it won't start from the next boot on. Nothing is deleted, only turned off, so a single click on **Enable** brings it back exactly as it was.

Windows components that the system really needs are hidden from the list in advance, so there's little chance of turning off something you shouldn't.

## Features

- **One list for everything** — See autorun items scattered across startup folders, the registry, Task Scheduler and services in one place.
- **Turn off instead of delete** — Switch items off with **Disable** and bring them back any time with **Enable**.
- **Windows essentials hidden** — Windows components that must not be turned off don't appear in the list. When you're online, it fetches the latest list of items to hide.
- **Easy-to-recognize names** — Shows each program's product name and icon instead of a file name.
- **Delete for good** — Leftover entries from programs you no longer use can be turned off and then removed from the list entirely.
- **Look it up** — Double-click an item you don't recognize to look it up on the web.
- **Save the list** — Save every current autorun item to a text file.
- **Dark mode** — Colors follow the Windows app mode (light · dark).
- **9 languages** — Korean · English · Japanese · Chinese · Russian · Italian · French · Spanish · Arabic.

## Download / Installation

| Type | Link |
|---|---|
| Installer | [Download](https://down.kilho.net/startcleaner?lang=en) |
| Portable (ZIP) | [Download](https://down.kilho.net/startcleaner?lang=en&nosetup) |

The installer launches StartCleaner as soon as setup finishes. For the portable version, unzip it and run `StartCleaner.exe`. Both versions have the same features.

Changing autorun items requires administrator rights, so Windows shows an administrator permission prompt when you run it. Click **Yes**.

## Usage

### Getting started

1. Run StartCleaner and click **Yes** in the administrator permission prompt.
2. Items that start at boot appear in the list with their **Program** name and **Source**.
3. Click the item you want to turn off once, then click **Disable** at the bottom.
4. The row turns gray and the button changes to **Enable**. From the next time Windows starts, that item won't run.
5. To turn it back on, click the same row and click **Enable**.

Items you turn off don't disappear from the list right away; they stay in place, grayed out, so you can undo what you just did immediately.

### Screen layout

| Element | What it does |
|---|---|
| **Home** | The screen with the autorun list |
| KILHO.net logo | Opens the StartCleaner product page |
| **Program** column | The program's icon and name (its product name, when it has one) |
| **Source** column | Where the item is registered — an icon and a name |
| Gray row | An item that is currently disabled |
| **All Programs** | When checked, shows everything, including items you've turned off |
| **Disable** / **Enable** | Turns the selected item off or on. Grayed out until you select an item |
| Right-click menu | **Delete** (disabled items only) · **Save List** |

**Source** — where each item starts from

| Source | Meaning |
|---|---|
| **Startup** | Shortcuts and programs in the Start menu's "Startup" folder (all users · current user) |
| **Registry** | Items a program registered to "run at sign-in" when it was installed |
| **Task** | Tasks registered in Task Scheduler that run at set times (update checks and the like) |
| **Service** | Background services that start automatically when Windows starts |

### When you want to…

**See what starts along with your PC**
Just run StartCleaner. Autorun items scattered across four places are gathered into one list, and the **Source** column tells you where each one is registered. If you've just installed a program, press **F5** to reload the list.

**Stop a messenger or update helper from starting every time you sign in**
Click that program in the list and click **Disable**. The program isn't removed and still works as usual; it just no longer starts on its own when Windows starts. Run it yourself whenever you need it. **Startup** and **Registry** items also show as "Disabled" in the **Startup apps** tab of Task Manager.

**Turn a disabled item back on**
Check **All Programs** and items you turned off earlier appear as gray rows. Click the row and click **Enable**, and it runs again from the next boot.

**Turn off update tasks that run in the background**
Rows whose **Source** is **Task** are tasks registered in Task Scheduler. Many browser and program update checks live here. Select the task you want to stop and click **Disable**; it won't run even when its scheduled time comes.

**Keep an unneeded service from starting at boot**
Clicking **Disable** on a **Service** row keeps that service from starting when Windows starts — and other programs can't start it either. Clicking **Enable** sets it to start automatically with Windows. It's best to check which program a service belongs to before turning it off — look up any service you don't recognize first, as described below.

**Find out what an item is**
Double-click the row, and your browser opens with information about that item. Use it to check what a program does before turning it off.

**Leftover autorun entries from a program you've uninstalled**
If a program is gone but its name is still in the list, first switch the row to **Disable**, then right-click → **Delete**. Click **Yes** in the confirmation, and the item is removed from the list completely. Deleted items can't be restored, so only delete what you're sure you don't need. The **Delete** menu doesn't appear for items that are still enabled — turning an item off first and using your PC for a few days before deleting it is the safe way.

**Remove a service completely**
Only services switched to **Disable** can be deleted. A running service is stopped before it's deleted. Afterward, a notice says "A service that was running is fully removed after a restart" — restart your PC once and it's gone for good.

**Gray services in All Programs**
**All Programs** also shows, as gray rows, services that are set to start only when needed. Clicking **Enable** on one of these makes it start automatically every time Windows starts, so leave them alone unless you turned them off yourself.

**Keep a record of the current state before cleaning up**
Right-click the list → **Save List** and choose where to save. Every autorun item — including the Windows essentials hidden from the list — is saved to a text file. Use it to compare before and after, or to compare against another PC.

**Why Windows essentials aren't in the list**
Services and tasks that Windows needs to work — audio, networking, security and so on — are hidden from the list from the start. Turning them off could stop Windows from working properly, so StartCleaner doesn't let you touch them at all. They stay hidden even when **All Programs** is checked.

**Browse the list with the keyboard**
Use **↑** · **↓** to move between rows; the list scrolls along so the selected row always stays in view. **F5** reloads the list.

**Names cut off because they're too long**
Drag the window's edge to make it wider, and the **Program** column widens with it. You can also drag the border between column headers to set the column width yourself.

**Running it again while it's already running**
Only one StartCleaner runs at a time. Running it again while the window is open doesn't start a new copy; the window that's already open comes to the front (and is restored if it was minimized).

## Configuration

There's nothing to set. StartCleaner follows these on its own:

| Item | Follows |
|---|---|
| Language | The Windows region setting (English if the language isn't supported) |
| Colors | The Windows app mode (light · dark) — changes are picked up right away, even while StartCleaner is open |

## Requirements

- Windows 10 · Windows 11 (64-bit)
- Administrator rights — needed to change autorun items. A permission prompt appears when you run it.
- No other components to install.
- The internet connection is used only for new-version notices and for fetching the list of Windows essentials to hide. Without a connection, it works as usual with its built-in list.

## Updates

StartCleaner does **not** update itself. At startup it checks for a new version and shows a notice; clicking **[Yes]** opens the download page and closes the program. New versions are released manually after internal testing and announced on the [StartCleaner page](https://kilho.net/startcleaner). See the [update policy notice](https://en.kilho.net/archives/notice/2940).

## License

StartCleaner is **freeware**. Use it for free without restriction anywhere — at work, at home, in government offices or at school — and redistribute it freely.

## Links

- Website: <https://kilho.net/startcleaner>
- Forum: <https://kilho.top/forum/qna>
- X (Twitter): <https://www.twitter.com/kilhonet>

© KILHO.NET
