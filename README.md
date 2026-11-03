# Mary's Angel Birthing Home — Android app

The patient and staff app for **Mary's Angel Birthing Home**, a birthing clinic in
Ibalong Village, Taysan, Legazpi City. Mothers book prenatal and postpartum visits,
keep their records and lab results in one place, and pay their bills online.
Clinic staff run the day's appointments, consultations, deliveries, and
vaccinations from the same app.

This repository only hosts the Android download. The source code is private.

## Download

**[⬇ Download the latest APK](https://github.com/itsruwins/mabh-mobile-releases/releases/latest/download/mabh-mobile.apk)** · Android · ~129 MB

Every version is listed under [Releases](https://github.com/itsruwins/mabh-mobile-releases/releases).

### Installing

1. Open the download link on your Android phone.
2. When the download finishes, tap the file to open it.
3. Android will ask to **allow installs from this source** (usually your browser).
   Allow it, then tap **Install**.
4. You may see a Play Protect warning, because the app isn't from the Play Store.
   Tap **More details → Install anyway**.

There is no iOS version available to download.

### Before you try it

- **The first load can take up to a minute.** The server sleeps when nobody is
  using it, and the app shows "Waking the server…" while it starts up.
- **Signing up needs a Philippine mobile number (+63).** The app sends a 6-digit
  code by SMS to confirm it.
- **This app is connected to the clinic's real appointment system.** If you are
  only trying the app out, please don't book an appointment.
- **Online payments are in test mode**, so no real money is charged.

## Features

### For patients

- **Book** prenatal care, immunizations for mothers and babies, pregnancy tests,
  post-partum checkups, family planning counseling, newborn screening, or a
  general consultation, then pick an open time slot.
- **Schedule:** see upcoming visits, confirm them, ask to move them, or cancel.
- **Pay online** through PayMongo with GCash, Maya, and other methods (test mode).
- **Ask:** a clinic assistant powered by Google Gemini, in English or Tagalog.
  If a message mentions a danger sign such as bleeding, the reply puts a
  **Call the clinic** button first. Suggested questions still get answers when
  the server can't be reached.
- **Documents:** photograph lab results or ultrasound reports. AI reads the
  values, and a midwife reviews each document before it is added to the record.
- **Records:** care plan, consultation history, prescriptions, transactions,
  and notifications.
- **Security:** fingerprint sign-in, an app lock, and a privacy screen that hides
  the app's contents in the app switcher.

### For clinic staff

Staff accounts are created by the clinic.

- Today's appointments, approve or decline requests, and record vital signs
- Patient search, pregnancy tracking, and high-risk screening
- Consultations, deliveries, referral transfers, and vaccination records
- Review of documents uploaded by patients

## Built with

| | |
|---|---|
| App | React Native, Expo (SDK 58), Expo Router, NativeWind, Zustand |
| API | Expo Router API routes running on Node.js, hosted on Render |
| Data | Supabase (PostgreSQL and Storage), Better Auth |
| Services | Google Gemini, PayMongo, httpSMS, Brevo |
| Builds | EAS Build |

## Version history

| Version | Date | Notes |
|---|---|---|
| [v1.0.0](https://github.com/itsruwins/mabh-mobile-releases/releases/tag/v1.0.0) | Oct 31, 2026 | First public Android build |
