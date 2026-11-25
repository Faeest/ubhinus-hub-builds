# UBHINUS Hub — builds

Android app for UBHINUS students: your class schedule, deadlines and QR attendance in one place.

**This repository contains only release builds. The source is kept private.**

## Download

Get the latest build here:

**https://github.com/Faeest/ubhinus-hub-builds/releases/latest/download/UBHINUS-Hub.apk**

That link always points at the newest version, so it is safe to share.

## Install

1. Open the link above on your phone and download the file.
2. Tap **Download complete** → **Install**. If Android warns about installing from an
   unknown source, allow it for your browser or file manager (this build is not on
   Play yet, so that prompt is expected).
3. Sign in with your campus account.

## Requirements

| | |
|---|---|
| Android | 11 (API 30) or newer |
| Network | only needed to sync; the app reads from its own copy otherwise |
| Storage | about 60 MB installed |

## What it does

- **Beranda** — the class you have now or next, anything due today, anything late.
- **Matkul** — your Moodle courses and their assignments.
- **Jadwal** — weekly timetable and exam schedule, with per-day view.
- **Absensi** — scan the lecturer's QR code to submit attendance.
- **Profil** — account, student card, theme, diagnostics.

Your campus password is encrypted on the device with a key held in the Android
Keystore. Nothing is sent to any server other than the campus systems themselves.

## Notes

- **Google Play is not used yet.** Installing means uninstalling any older build first,
  which deletes its saved data (accounts, cached schedule, attendance history). That is
  a one-time cost of moving to this version.
- Reminders need the notification permission, and exact timing needs the exact-alarm
  permission. Without them the app still works; reminders may arrive a few minutes late.
- Attendance submission is deliberately hard to do by accident: a scanned code can only
  be submitted once, and the app warns you before retrying anything that timed out.

## Privacy

No analytics, no ads, no third-party SDKs, no crash upload. The app talks only to
`ebelajar.stiki.ac.id` (course data), `zuko.stiki.ac.id` (schedule and attendance) and
nothing else.
