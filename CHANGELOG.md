# Notify Scout release notes

## 1.0.0 (2026-11-15)
- First release. Catches Windows notifications (the banners at the corner of the screen) and shows which app sent each one and what it said.
- Catches pop-up windows from any program, including windows that flash for a split second, with the program file, the exact command line, what started it, and how long it stayed on screen.
- Turn Off: silences a Windows notification app using Windows' own switch, or makes Notify Scout close a pop-up window the instant it appears. Turn On undoes it.
- Lists every app allowed to send Windows notifications so you can switch any of them off without waiting for it to appear.
- Details gives plain-English advice on stopping the source at the root: Task Scheduler, a service, a startup item, or a website's permission in your browser.
- Keeps watching from the icon next to the clock when you close the window, can start with Windows, and writes everything it catches to a log file.
- Run as Admin for programs Windows otherwise hides, Save Report, automatic updates, Share tab, and detailed tooltips on every control.
