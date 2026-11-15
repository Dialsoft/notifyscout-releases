# Notify Scout release notes

## 1.3.0 (2026-11-15)
- Simpler and safer out of the box: Notify Scout now watches website notifications in Chrome, Edge and Brave only. App notifications and pop-up windows from programs are off until you turn them on.
- New Settings page: click the Settings tab for a full page of options, each with a plain-English description. Every change still takes effect immediately.
- The everyday Home tab has just four buttons: Website Cleanup, Close Browsers, Pause and Exit. Nothing on it can stop a program from working.
- Expert tools (Turn Off for any source, End Program, Run as Admin, the full lists and more) are hidden until you tick "Show expert tools" on the Settings page.
- If you used an earlier version: app notifications and pop-up windows are now off by default. Tick them on the Settings page to get them back. Pop-ups you already blocked stay blocked.

## 1.2.0 (2026-11-15)
- New Website Cleanup (Home tab, the Simple View page, and the tray icon's menu): lists every website allowed to send you notifications in Chrome, Edge and Brave, across all browser profiles, without waiting for one to pop up.
- Junk detection: Notify Scout checks each website's name and marks the suspicious ones (random-letter names, cheap throw-away endings such as .xyz or .top, bait words such as push, alert or prize, or notifications that used fake-virus wording). Suspicious websites are ticked for you; one click blocks them all.
- The banner turns orange when suspicious websites are allowed to notify you, and Notify Scout tells you when a new website is given permission while it is running.
- New Close Browsers button (also in the tray icon's menu): the escape hatch for a fake virus warning that has taken over the whole screen.
- Suspicious websites are shown in red in the lists, with the reasons spelled out in Details.

## 1.1.0 (2026-11-15)
- New Simple View (now the default): one big page showing the last thing that popped up, who sent it and what it said, with one button to stop it. Earlier and Later buttons walk through everything caught. Click Simple View on the Home tab to switch to the full lists and back.
- New "Want it stopped?" prompt: the moment a notification or pop-up is caught, a small window appears at the top-right corner with Stop these and Leave it alone buttons. It goes away by itself after 30 seconds and can be switched off on the Settings tab.
- Website notifications: when a notification comes through Chrome, Edge or Brave, Notify Scout now names the website that sent it (for example finance.yahoo.com) and can block just that one website, without silencing the whole browser.
- Websites already blocked in the browser are listed with the other sources and can be turned back on.

## 1.0.0 (2026-11-15)
- First release. Catches Windows notifications (the banners at the corner of the screen) and shows which app sent each one and what it said.
- Catches pop-up windows from any program, including windows that flash for a split second, with the program file, the exact command line, what started it, and how long it stayed on screen.
- Turn Off: silences a Windows notification app using Windows' own switch, or makes Notify Scout close a pop-up window the instant it appears. Turn On undoes it.
- Lists every app allowed to send Windows notifications so you can switch any of them off without waiting for it to appear.
- Details gives plain-English advice on stopping the source at the root: Task Scheduler, a service, a startup item, or a website's permission in your browser.
- Keeps watching from the icon next to the clock when you close the window, can start with Windows, and writes everything it catches to a log file.
- Run as Admin for programs Windows otherwise hides, Save Report, automatic updates, Share tab, and detailed tooltips on every control.
