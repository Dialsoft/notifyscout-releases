# Notify Scout

Where did that notification come from? A Windows tool by Dialsoft LLC.

Notify Scout catches Windows notifications and pop-up windows, tells you exactly which app or program sent each one and what started it, and lets you turn them off. It also catches windows that flash by too fast to read.

## Download

**[⬇ Download Notify Scout (latest)](https://github.com/Dialsoft/notifyscout-releases/raw/main/NotifyScout.exe)**. Current version: **1.0.0** (2026-11-15)

- A single program file with nothing to install. Just double-click it.
- For Windows 10 and 11 (64-bit).
- Run it from a folder you can write to (Desktop, Downloads, or `C:\Tools`) rather than Program Files, so it can update itself.
- The first time, Windows may say "Windows protected your PC". Click **More info**, then **Run anyway**.

Notify Scout checks this page when it starts and every 6 hours, and offers new versions with an **Update now** button. Every download is verified against the SHA-256 checksum in `latest.json` before it installs.

## What's new in 1.0.0

- First release. Catches Windows notifications (the banners at the corner of the screen) and shows which app sent each one and what it said.
- Catches pop-up windows from any program, including windows that flash for a split second, with the program file, the exact command line, what started it, and how long it stayed on screen.
- Turn Off: silences a Windows notification app using Windows' own switch, or makes Notify Scout close a pop-up window the instant it appears. Turn On undoes it.
- Lists every app allowed to send Windows notifications so you can switch any of them off without waiting for it to appear.
- Details gives plain-English advice on stopping the source at the root: Task Scheduler, a service, a startup item, or a website's permission in your browser.
- Keeps watching from the icon next to the clock when you close the window, can start with Windows, and writes everything it catches to a log file.
- Run as Admin for programs Windows otherwise hides, Save Report, automatic updates, Share tab, and detailed tooltips on every control.

See [CHANGELOG.md](CHANGELOG.md) for every version.

# User guide

Notify Scout answers one question: **"What just popped up, and how do I make it stop?"**

It is a single file, `NotifyScout.exe`. There is nothing to install. Double-click it to start.

### The two things it catches

1. **Windows notifications.** These are the banners that slide in at the bottom-right corner and pile up in the Notification Center. Notify Scout tells you which app sent each one and what it said.
2. **Pop-up windows.** Anything else a program puts on your screen by itself: an ad or "reminder" from some utility, a dialog box, or a black window that flashes open and shut too fast to read. Notify Scout tells you which program file it was, the exact command that was run, and what started it.

### Catching something

1. Start Notify Scout and leave it running. Clicking the **X** only hides the window; Notify Scout keeps watching from its icon next to the clock (click the little **^** arrow if you don't see it).
2. Carry on working. When the thing appears again, click the icon to open Notify Scout.
3. Look at the top of the **Caught so far** list. The newest item is first.

| Row color | Meaning |
|---|---|
| Blue | A Windows notification arrived. |
| Orange | A pop-up style window appeared by itself. |
| White, "Program window" | An ordinary program window opened. |
| White, "(earlier)" | A notification that was already in the Notification Center when Notify Scout started. |
| Gray | A pop-up you turned off, which Notify Scout closed for you. |
| Green text | A note from Notify Scout itself. |

The **On screen** column shows how long a window stayed up. "A flash" means under a second and a half, which is typical of scheduled tasks and updaters.

### Finding out where it came from

Double-click the row (or click it and choose **Details**). You get:

- the full program file and folder
- the command line: exactly what was run. For a flashing black window this names the script.
- **Started by**: the program that launched it, and the program that launched that one
- plain-English advice on stopping it at the root: Task Scheduler, a Windows service, a startup item, or a website's permission in your browser

If the program file or command line says "not available", click **Run as Admin** on the Home tab and wait for it to happen again. Windows hides those details for programs that run as administrator.

### Turning it off

Click the row, then click **Turn Off**. You are always asked to confirm first.

- **Windows notification:** flips Windows' own on/off switch for that app, the same one found in Windows Settings > System > Notifications. The app keeps working; it just can't show banners. Windows normally obeys right away. If one more slips through, sign out and back in once.
- **Pop-up window:** Notify Scout closes that type of window from that program the instant it appears, usually before you can see it. This only works while Notify Scout is running, so turn on **Start with Windows** on the Settings tab.

**Turn On** undoes either one.

### If the notification came through a web browser

When "From" is Chrome, Edge or Firefox, a *website* was given permission to send notifications. The notification text usually names the site. Turning the browser off in Notify Scout silences every website. To stop just the one site, open the browser and go to Settings > Privacy > Site settings > Notifications, then remove or block it.

### The bottom list

**Everything that can notify you** lists every app registered with Windows to send notifications, in A-Z order, plus any pop-up programs Notify Scout has seen or blocked. You can turn any of them off here without waiting for it to send something. Rows that are off are gray.

### Settings (all take effect immediately)

| Setting | What it does |
|---|---|
| List ordinary program windows too | On: every window that opens is listed. Off: only pop-up style windows. Leave on if you are chasing a flashing window. |
| Include the program I'm using | Off (recommended): windows opened by the program you are actively working in are skipped, because you caused those yourself. |
| Beep when something is caught | Plays a sound for each notification or pop-up. |
| Keep running when I close the window | On: the X hides the window and Notify Scout keeps watching. Use **Exit** on the Home tab to close it completely. |
| Start with Windows | Starts Notify Scout quietly next to the clock each time you sign in. Needed for blocked pop-ups to stay blocked after a restart. |
| Keep a log file | Writes everything caught to a text file with the date and time, so you can look back over days. Open it with Home > Open Log File. |
| Always on top | Keeps the Notify Scout window in front. |
| Check for updates automatically | Checks for a new version at startup and every 6 hours. Nothing installs until you click Update now. |

### Good to know

- Notify Scout only reads Windows' notification history; it never changes or deletes it.
- A blocked pop-up's program is still running in the background. Details shows what starts it, so you can disable the scheduled task, service or startup item, or uninstall the product.
- If the pop-up comes from the very program you are working in, turn on **Include the program I'm using**.
- Hover over any button, list or setting for a detailed explanation.

---
© 2026 Dialsoft LLC. All rights reserved. Built with Claude by Anthropic.
