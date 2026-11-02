# SSŠVT Drive

> **Unofficial app by Filip Bukovina ([FBukovina](https://github.com/FBukovina)).**
> Not affiliated with, endorsed by or supported by SSŠVT or Fortinet. Their names
> belong to their owners and appear here only to describe what the app works with.

A small macOS app for browsing and downloading the files you can already reach
through the school's web portal at `gw.sssvt.cz`, with a Finder-like interface,
search, a download manager, and light and dark themes.

It is not a VPN client. It only uses the web portal, you sign in on the school's
own page, and it can only read: it never uploads, renames, edits or deletes
anything. You need your own valid school account.

This repository holds release files only. The source code is not published here.

## Install

You need a Mac with Apple silicon and macOS 12 or later.

1. Download the `.dmg` from the [latest release](https://github.com/FBukovina/ssvt-drive-releases/releases/latest).
2. Open it and drag **SSŠVT Drive** to Applications.
3. Open the app. It isn't notarized by Apple, so macOS will block it the first
   time. Go to **System Settings → Privacy & Security** and choose **Open Anyway**.

## Updates

The app checks for new versions shortly after launch and every 6 hours, then
shows a notice. Nothing installs until you click **Install and Restart**. Every
update is signed, and the app refuses any update whose signature doesn't match.

## Privacy

- The app never sees, stores or sends your password.
- There is no analytics, telemetry or server of its own.
- Your session stays in macOS WebKit on your Mac for up to 12 hours, so you can
  reopen the app without signing in again if the school's gateway still accepts
  it. On macOS 12 and 13 it ends when you quit. **Sign out** erases it.
- Apart from the school's portal, the app only contacts GitHub to check for
  updates. GitHub sees your IP address, as with any download.

## Good to know

- Browsing, sign-in and single-file downloads have been tested on the real
  portal. Multi-file and folder downloads have not been tested there yet.
- The school's gateway decides how long a session lasts, so you may need to sign
  in again, especially after your Mac has been asleep.
- Opening a new folder or downloading from another folder waits for running
  downloads to finish.
