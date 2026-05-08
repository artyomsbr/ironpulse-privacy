# Privacy Policy

**Strenos** · Last updated: May 8, 2026

This Privacy Policy explains how Strenos ("the app", "we", "us") handles information you provide while using the Strenos iOS application. Strenos is a workout tracker for strength training, conditioning, and recovery analytics.

> **Summary in plain English.** Strenos runs no servers. Your workout data, photos, videos, and personal records are stored privately in *your own iCloud account* (Apple's CloudKit private database) and on your device. We do not collect, sell, or share your data with anyone. There are no advertising SDKs, no analytics SDKs, and no third-party tracking.

---

## 1. Who is responsible for your data

The app developer is the data controller. For privacy questions, account deletion requests, or to exercise your rights under GDPR, CCPA, or other applicable law, contact:

- Email: [strenos.support@gmail.com](mailto:strenos.support@gmail.com)

## 2. Information we collect

The categories below correspond 1:1 to our App Store privacy labels. All data stays in your iCloud and on your device unless explicitly noted.

### 2.1 Health & Fitness data

If you grant permission, Strenos reads from and writes to Apple Health (HealthKit):

- **Heart rate** — read during and after workouts to display real-time and average HR.
- **Active energy (calories)** — read to display calories burned per workout.
- **Workouts** — written when you complete a session, so the workout appears in Apple Health and contributes to your Activity rings.

You control HealthKit access at any time in *iOS Settings → Privacy & Security → Health → Strenos*. Health data never leaves Apple Health and your iCloud. Apple does not share your HealthKit data with us as a developer.

### 2.2 User-generated content

Information you create inside the app:

- Workout logs (exercises, sets, reps, weights, RPE, notes)
- Custom training programs
- Personal records (PRs) and record types
- Calendar entries and week templates
- Body weight, sleep, hydration logs
- Photos and videos you attach to personal records

This content is stored in **your private CloudKit database**, accessible only to you with your Apple ID. We have no ability to access it.

### 2.3 Account identifier (Sign in with Apple)

If you choose to sign in, Apple provides a stable per-app identifier so the app can keep your data linked to *your* profile across devices. We never receive your real name, email, or phone number unless you explicitly share them with Apple.

Sign in with Apple is optional. Strenos works fully offline on a single device without an account.

### 2.4 External heart-rate sensors (Bluetooth)

If you pair a Bluetooth heart-rate monitor (e.g., Polar, Wahoo), readings flow directly from the sensor to your device through Apple's CoreBluetooth framework. Strenos displays the live values during your workout. We do not store or transmit raw sensor data outside of your device and iCloud.

### 2.5 Subscription and purchase information

All purchases (Strenos Plus subscriptions and the Lifetime option) are processed by Apple via StoreKit 2. We never see your payment method, card number, or Apple ID balance. Apple sends us only an anonymous transaction signature that proves the purchase is valid; this signature is verified cryptographically (JWS) and never stored on a remote server.

## 3. Information we do NOT collect

- No real name, email, or phone number (unless you email us directly)
- No location, GPS, or geolocation data
- No browsing history, search history, or cookies
- No contacts, calendar (system), or photo library content beyond items you explicitly attach to a record
- No advertising identifiers (IDFA), no third-party analytics
- No biometric data outside HealthKit
- No usage tracking that leaves the device

## 4. How we use your data

The sole purpose of every category we collect is **App Functionality**:

| Data | Purpose |
|---|---|
| Health (HR, calories) | Show metrics during/after workouts; compute readiness score and recovery insights locally |
| Fitness (workouts) | Sync sessions to Apple Health; build progress charts |
| User content (logs, programs, PRs) | Power the workout tracker, programs, calendar, and analytics |
| Photos/videos | Allow you to attach visual proof to personal records |
| Apple Sign In ID | Identify your private CloudKit data across your devices |

We do **not** use your data for: advertising, marketing, analytics, profiling, personalization across users, training third-party AI models, or any commercial purpose beyond running the app on your devices.

## 5. Where your data lives

- **On your device**: workouts and programs are stored locally using Apple's SwiftData framework.
- **In your iCloud**: the same data is mirrored to your Apple-managed private CloudKit database, encrypted by Apple in transit and at rest. Only you can access it.
- **In Apple Health**: workouts and metrics live in HealthKit, controlled entirely by you via iOS Settings.

Strenos has no backend servers, no databases under our control, and no remote logging service.

## 6. Data sharing

We do not sell or share your data with third parties. The only entity that processes your data on our behalf is **Apple Inc.**, in the role of an infrastructure provider:

- **Apple iCloud / CloudKit** — storage of your private data, in your account.
- **Apple HealthKit** — system framework for reading/writing health data on your device.
- **Apple StoreKit** — processing of in-app purchases and subscriptions.
- **Apple Sign In** — optional authentication.
- **Apple Push Notification service (APNs)** — delivery of local workout reminders if you enable them.

Apple's use of this data is governed by Apple's own privacy policy: [apple.com/legal/privacy](https://www.apple.com/legal/privacy/).

## 7. International data transfers

Your data is stored in the iCloud region Apple assigns to your Apple ID. Apple maintains data centers across the EU, US, and other jurisdictions. We do not transfer your data ourselves; all transfers are governed by Apple's standard contractual mechanisms.

## 8. Data retention

Your data persists as long as you keep the app installed and your iCloud account active. You can delete all of it at any time:

1. Inside the app: **Settings → Delete Account**. This wipes your local profile and removes your data from your private CloudKit database.
2. To remove HealthKit data written by Strenos: *Apple Health app → Sources → Strenos → Delete All Data*.

Once deleted, the action is permanent. We retain no copies because we hold no copies to begin with.

## 9. Your rights (GDPR, CCPA, and similar)

Because all your personal data lives under your control in iCloud and HealthKit, the following rights are exercised directly through Apple's system tools:

- **Right to access** — export workout data via Strenos's built-in JSON backup (Settings → Backup), or use Apple's standard data-export tools at [privacy.apple.com](https://privacy.apple.com).
- **Right to erasure** — Settings → Delete Account inside the app.
- **Right to restrict processing** — revoke HealthKit permission, sign out of Apple Sign In, or uninstall the app.
- **Right to portability** — Strenos's JSON backup contains your full dataset.
- **Right to object** — not applicable; we do not process your data for marketing, profiling, or analytics.

For any privacy-related request that cannot be handled through the app or iOS, email [strenos.support@gmail.com](mailto:strenos.support@gmail.com). We respond within 30 days.

## 10. Children's privacy

Strenos is rated 4+ on the App Store but is designed for adult athletes. We do not knowingly collect personal information from children under 13 (or under 16 in the EU). If you believe a minor has used Strenos, contact us and we will assist with deletion.

## 11. Security

Because all your data is stored in your iCloud and on your device, security is anchored to Apple's infrastructure: end-to-end encryption for HealthKit, encryption at rest and in transit for CloudKit private databases, and Secure Enclave protection for purchase signatures (StoreKit 2 JWS). The app does not handle or transmit unencrypted data over the network.

## 12. Subscriptions and the free trial

Strenos offers an optional **10-day free trial of Plus features** on first launch. The trial is implemented locally in the app (no card required, no automatic charge afterward) and ends silently when the period expires.

If you choose to subscribe to **Strenos Plus** or buy **Plus Lifetime**, the transaction is processed by Apple StoreKit. Auto-renewable subscriptions renew automatically until you cancel them through Apple's subscription management UI (Settings → Manage Subscription inside the app, or *iOS Settings → [Apple ID] → Subscriptions*). Apple's standard [EULA](https://www.apple.com/legal/internet-services/itunes/dev/stdeula/) applies to all purchases.

## 13. Changes to this policy

If this policy changes materially, we will update the "Last updated" date at the top and, where required, notify you within the app. Continued use of Strenos after a change means you accept the revised terms.

## 14. Contact

For privacy questions, account-deletion requests, or to exercise any of your rights:

- Email: [strenos.support@gmail.com](mailto:strenos.support@gmail.com)
- Support page: [artyomsbr.github.io/strenos-privacy/support/](https://artyomsbr.github.io/strenos-privacy/support/)

We typically respond within 24–48 hours.

---

[Support](https://artyomsbr.github.io/strenos-privacy/support/) · Strenos © 2026
