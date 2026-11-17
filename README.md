# All Blue Protocol — Android starter project

A native Android Studio project for an offline-first personal activity tracker.

## Included in this starter
- Local sign-up and sign-in (username + password hash stored on device)
- One-time character choice and automatically assigned symbol avatar
- Character selection list including Luffy, Zoro, Sanji, Shanks, Garp, Eustass Kid, Ace, Law, Sabo, Mihawk, Jinbe, Nami, Robin, Usopp, Chopper, Franky, Brook, Yamato, Hancock, Koby, Smoker, Marco, Katakuri, Killer and Beckman
- Local task creation, completion and deletion
- Android notification receiver and exact-alarm scheduling foundation
- JSON export and restore through Android document picker
- Dark interface

## Important scope notes
This is a starter source project, not a compiled or tested APK. It requires Android Studio and an Android SDK to build. Review and test it before personal use.

The sign-up is **local-only**: it does not create an internet account, provide multi-device sync, or offer password recovery. Do not reuse an important password. The password hash is stored locally; this starter should be upgraded to Android Keystore-backed secure storage before production.

The character avatars are assigned emoji/symbol badges, not AI-generated character portraits. A truly generative AI avatar feature needs an AI model/service or bundled model assets. It cannot be honestly described as AI-generated in this offline starter. Use licensed/original art assets if adding portraits; this project does not include official One Piece artwork.

Notifications require notification permission. Android exact alarm access and battery settings may affect delivery. Tasks can be created with an optional one-time daily-clock reminder (24-hour time). The alarm is scheduled for the next occurrence of that time. Reminders are not yet automatically reconstructed after reboot in this starter.

Habit tracking, detailed activity timelines, charts, recurring tasks, and reminder editing are not fully implemented yet. The UI labels these as future upgrades rather than pretending they are complete.

## Build
1. Install Android Studio on a computer.
2. Open this project folder.
3. Allow Gradle sync and install the requested Android SDK.
4. Run on an Android device/emulator.
5. Use Build > Build Bundle(s) / APK(s) > Build APK(s).

## Backup
Profile and task data are stored locally in app preferences. Use Profile & backup > Export backup regularly. Restoring replaces the stored JSON data.
