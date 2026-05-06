# Privacy Policy — Iron Pulse

**Effective date:** May 6, 2026
**Last updated:** May 6, 2026

This Privacy Policy describes how Iron Pulse ("we", "our", "the App") handles personal information. Iron Pulse is an iOS fitness application designed to help users plan, log, and analyze their workouts. **The App does not collect, transmit, sell, or share personal data with anyone.** All information you create stays on your device and (optionally, with your consent) in your private iCloud account.

---

## 1. Summary (TL;DR)

- **No analytics, no advertising, no tracking.** We do not run third-party SDKs.
- **No account on our servers.** We don't have servers; we don't have your data.
- **Your fitness data lives on your iPhone** and, if you enable iCloud, in your private iCloud database that only you can access.
- **HealthKit data** stays on your device. We never read or write Health data outside the workout session you started in the App.
- **In-App Purchases** are handled by Apple. We never see your payment details.

If a section below contradicts this summary, the section governs.

---

## 2. Who we are

Iron Pulse is published by:

**Iron Pulse**
Independent developer — Latvian citizen (EU), currently residing in Georgia
Contact: as28873728@gmail.com

For privacy questions, write to **as28873728@gmail.com**. We respond to verified requests within 30 days (or shorter where required by law).

---

## 3. Data we process

### 3.1 Data you create inside the App (stored on-device)

When you use Iron Pulse you generate workout records. Examples:

- **Profile**: display name, age, gender, height, weight, body fat percentage, body measurements
- **Workouts**: exercises performed, sets, reps, weight, rest time, RPE (rate of perceived exertion), workout duration, notes
- **Programs and timers**: training programs you build (Standard, Tabata, EMOM, AMRAP, Interval, Circuit, Yoga); timer presets
- **Personal records (PRs)**: max weight, max reps, time records, custom records
- **Wellness logs**: hydration glass count, sleep bedtime/wake time, body weight history, body measurements
- **Calendar**: scheduled workouts, week templates, mesocycle plans
- **Optional media**: photos / videos you attach to personal records (Plus subscription only)

This data is stored locally in Apple's SwiftData (a local SQLite-backed database) and is **never sent to Iron Pulse**.

### 3.2 Data Apple processes on our behalf

Three Apple-provided systems hold or relay your data. Apple, not Iron Pulse, is the processor:

| System | What it stores | Where |
|---|---|---|
| **iCloud (CloudKit)** — optional, only with Apple Sign-In | Encrypted copy of your workouts, programs, profile, records, media | Your private iCloud account, end-to-end encrypted; only you can read it |
| **HealthKit** — optional, only after permission | Heart rate, active calories, workout summaries you choose to write back | Apple Health database on your device, encrypted |
| **App Store / StoreKit 2** | Subscription receipts, purchase history | Apple's billing system; we receive an anonymous "subscribed / not subscribed" signal |

We have **no direct access** to your iCloud, HealthKit, or App Store records. Apple's privacy policy (https://www.apple.com/legal/privacy/) governs that data.

### 3.3 Data we do NOT collect

We **do not** process any of the following:

- Email addresses, phone numbers, or postal addresses
- IP addresses or device fingerprints
- Crash reports identifying you (Apple's optional analytics may include them; see below)
- Advertising identifiers (IDFA / IDFV)
- Browsing behavior, app usage timestamps, session length, screens viewed
- Microphone, camera, contacts, calendar events, photos (we only request video write access for record clips, never read)
- Location data
- Any information derived from third-party SDKs — **we don't use any**

The App's `PrivacyInfo.xcprivacy` Privacy Manifest declares the same — we declare zero `NSPrivacyCollectedDataTypes` to Apple.

---

## 4. Apple Sign-In

If you choose to sign in with Apple ("Apple Sign-In"), the App receives a stable opaque identifier from Apple. This identifier:

- Is unique per app + Apple ID, but is **not** an email or name
- Is stored locally on your device
- Is used **only** to associate your local data with your iCloud database so the same data appears on your other devices

We do not transmit this identifier to any server we control. If you provide an email at sign-in, Apple may forward a private-relay email to us; we do not currently use it.

To revoke: Settings → Apple ID → Password & Security → Sign in with Apple → Iron Pulse → Stop Using.

---

## 5. HealthKit

Iron Pulse integrates with Apple HealthKit when you grant permission. We use HealthKit for:

- **Reading**: heart rate and active calories during a workout you started in the App, so we can show real-time stats
- **Writing**: workout records (start/end, calories, heart rate samples) so they appear in Apple Health and contribute to your Activity rings

HealthKit data **never** leaves your device through Iron Pulse. We do not back up, transmit, sell, or share HealthKit information. Apple's HealthKit framework is end-to-end encrypted and inaccessible to us outside of an active in-app workout session.

You can revoke HealthKit access any time: Settings → Privacy & Security → Health → Iron Pulse.

---

## 6. iCloud sync (CloudKit)

When you sign in with Apple, Iron Pulse uses **CloudKit** to mirror your data across your own Apple devices. Specifically:

- Container: `iCloud.com.ironpulse.IronPulse.data`
- Database type: **Private** (only you can read/write — we cannot)
- Encryption: end-to-end encrypted by Apple

We do not run any custom backend; the only "server" is Apple's CloudKit. If you sign out of iCloud, the data remains in your iCloud account and on the local device until you delete it.

---

## 7. In-App Purchases

Iron Pulse offers an optional subscription, **Iron Pulse Plus**, plus a one-time Lifetime purchase. All payments are handled exclusively by Apple via StoreKit 2. We **never** see:

- Your card number
- Your billing address
- Your Apple ID password or any credential

We receive only:
- An anonymous boolean from Apple indicating whether you currently have an active subscription / lifetime entitlement
- Apple's standard product identifiers (e.g. `com.ironpulse.IronPulse.plus.monthly`)

Refunds, cancellations, and family-sharing are managed entirely through your Apple ID. See https://support.apple.com/HT202039.

---

## 8. Optional widgets and extensions

Iron Pulse includes a Home Screen widget bundle, an Apple Watch app, and a Lock Screen Live Activity. These extensions:

- Read **only** the data already stored in your local SwiftData store and a private App Group container
- Do **not** transmit anything outside your device
- Are governed by the same data-handling rules as the main App

---

## 9. Children

Iron Pulse is not directed at users under 13. We do not knowingly process data from anyone under 13. If you believe a minor has used the App, contact as28873728@gmail.com and we will help you erase any local data on the affected device.

---

## 10. Your rights

Because we store no personal data on our servers, the right to access, rectify, delete, port, or restrict processing is exercised on your device:

| Right | How to exercise |
|---|---|
| **Access** | Open the App; all your data is visible in Settings → Profile, Progress, Calendar, etc. |
| **Rectification** | Edit any record directly in the App |
| **Erasure ("right to be forgotten")** | Settings → Удалить все данные ("Delete all data"). Permanently removes every workout, record, profile, and media file from this device, and from your iCloud private database when re-synced |
| **Portability** | Settings → Backup → Export. Produces a JSON file with all your data |
| **Restriction / Objection** | Disable HealthKit, iCloud, and Bluetooth in Settings → Privacy at any time |
| **Withdraw consent** | Apple Sign-In: revoke via iOS Settings → Apple ID → Iron Pulse → Stop Using |

**EU / UK users (GDPR)**: legal basis for processing on-device data is your consent (Art. 6(1)(a)) and legitimate interest in delivering the requested fitness service (Art. 6(1)(f)). No data is transferred outside your device by us.

**California residents (CCPA / CPRA)**: we do not sell or share personal information for cross-context behavioral advertising. Submit verified requests to as28873728@gmail.com. We will respond within 45 days.

**Brazil (LGPD), Quebec (Law 25), other regional laws**: equivalent rights apply; same contact email.

---

## 11. Data retention

- **On-device**: until you delete the App, delete the data through Settings, or factory-reset the device.
- **iCloud**: until you sign out and delete the iCloud container, or use Apple's "Manage Storage" to remove Iron Pulse data.
- **App Store receipts**: governed by Apple's retention policy.

We have **no separate retention timer** because we do not hold the data.

---

## 12. Security

Iron Pulse uses Apple's standard on-device encryption:

- SwiftData store is encrypted at rest when the device passcode is set
- HealthKit data is encrypted by Apple
- iCloud private database uses end-to-end encryption
- StoreKit 2 transactions are signed and verified
- No HTTP traffic is initiated by the App; the only network calls Apple may make on our behalf are App Store metadata, CloudKit sync, and Apple's analytics (if you opted in)

If you discover a vulnerability, please email **as28873728@gmail.com**. We follow coordinated disclosure.

---

## 13. Third-party services we **do not** use

To be explicit — Iron Pulse contains no integrations with:

- Google Analytics, Firebase, Crashlytics, Sentry, Bugsnag, AppCenter
- Facebook SDK, Meta Pixel, AppsFlyer, Adjust, Branch
- Mixpanel, Amplitude, Heap, Segment
- AdMob, Unity Ads, ironSource, AppLovin
- OneSignal, Pushwoosh, or any third-party push provider
- TikTok, Twitter, or social-media SDKs

The App's binary contains no third-party SDKs at all. The only "external" frameworks are Apple's first-party APIs (HealthKit, CloudKit, StoreKit, WidgetKit, ActivityKit, Bluetooth, etc.).

---

## 14. Changes to this policy

If we change how we handle your data, we will:

1. Update the "Last updated" date at the top
2. Display a notice inside the App on next launch
3. For material changes (new data type, new third-party recipient), require your renewed consent before the change takes effect

Older versions of this policy are available on request.

---

## 15. Apple's privacy policy

Because Apple processes your iCloud, HealthKit, and App Store interactions, their privacy policy also applies:
**https://www.apple.com/legal/privacy/**

---

## 16. Contact

| Topic | Address |
|---|---|
| Privacy questions, GDPR / CCPA requests | as28873728@gmail.com |
| Security disclosure | as28873728@gmail.com |
| Support | as28873728@gmail.com |

We aim to respond within **30 days**.

---

*Iron Pulse — built by athletes, for athletes. We respect the same privacy on your data that we want for ours.*
