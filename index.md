# Privacy Policy — Pennify

**Effective date:** May 8, 2026  
**Last updated:** June 12, 2026  
**App name:** Pennify – Expense Tracker  
**Package:** com.grizplayapp.pennify  
**Developer:** GrizPlay Apps  
**Contact:** grizplayapp@gmail.com

---

## 1. Overview

Pennify is a personal expense tracker designed with privacy as a core principle. The app is **local-only** — no account is required, no registration is needed, and your financial data never leaves your device unless **you** choose to export it. We do not operate any backend servers that receive or store your personal information.

This Privacy Policy explains what information is collected, how it is used, and your rights as a user.

---

## 2. Information We Collect

### 2.1 Information You Enter (Stored Locally on Your Device Only)

When you use Pennify, you may enter the following information:

- **Display name** – used to greet you on the home screen
- **Transactions** – amount, category, type (income or expense), date, and optional notes
- **Recurring transactions** – transactions you mark to auto-repeat each month on a chosen day
- **Budget limits** – optional per-category monthly budget amounts
- **Preferences** – currency selection (20 supported currencies), default transaction type, and app theme

This information is stored exclusively on your device using your phone's local storage (AsyncStorage, key: `@spendly/state`). It is **never transmitted to our servers, never uploaded to the cloud automatically, and never shared with any third party** by us.

You can delete all of this data at any time from **Settings → Clear all data**.

### 2.2 Backup & Export (User-Initiated Only)

Pennify offers two optional data export features, both fully under your control:

- **Export as CSV** – generates a spreadsheet of your transactions and opens your phone's native share sheet. You choose where to send it (email, files, Google Drive, etc.). Pennify does not transmit this file anywhere.
- **Backup (.pennify file)** – generates a full snapshot of your app data and opens your phone's native share sheet. You choose where to store it. Restore is also manual — you select the file from your device using the system file picker.
- **Share app (Settings)** – tapping "Share app" opens your phone's native share sheet with a pre-written text message containing a link to Pennify on the Google Play Store. **No personal or financial data is included.** This feature only shares a static promotional text you choose to forward.

None of these features transmit data to our servers. All actions happen on your device; destination is your choice.

### 2.3 Information Collected Automatically by Third-Party Advertising (Google AdMob)

Pennify displays banner advertisements served by **Google AdMob** (a service operated by Google LLC). To serve and measure ads, Google may automatically collect:

- **Advertising identifier (GAID)** – a resettable device identifier used for ad personalisation
- **IP address** – used to determine approximate geographic location
- **Device information** – device model, OS version, screen size, language
- **Ad interaction data** – whether an ad was viewed or tapped
- **App usage signals** – general signals used for ad targeting and fraud prevention

This data is collected and processed by Google, not by Pennify. We do not receive, store, or have access to this data.

---

## 3. Permissions We Request

| Permission | Why We Need It |
|---|---|
| `INTERNET` | Required to load and display Google AdMob banner ads |
| `VIBRATE` | Used for haptic feedback when you interact with the app |
| `POST_NOTIFICATIONS` | Required on Android 13+ to send you optional daily reminder notifications. **You are asked before this is enabled** — notifications are off by default and only activated if you turn them on in Settings. |

We do **not** request:
- `READ_EXTERNAL_STORAGE` or `WRITE_EXTERNAL_STORAGE` — file export/import uses Android's Storage Access Framework (SAF), which does not require these permissions
- `READ_CONTACTS`, `CAMERA`, `LOCATION`, or any other sensitive permissions
- `android:allowBackup` — Android's automatic device-backup for Pennify is **disabled** (`android:allowBackup="false"`), so your financial data is not included in Android's automatic cloud backup

---

## 4. Notifications

If you enable daily reminders in Settings, Pennify will schedule a local notification at the time you choose. These notifications:

- Are generated entirely on your device (no push notification servers are used)
- Contain only a generic reminder message ("Time to log your expenses!")
- Are never used to collect or transmit any data

You can disable notifications at any time from **Settings → Daily Reminder** or from your phone's system notification settings.

---

## 5. How We Use Information

| Data | Purpose |
|---|---|
| Your name | Personalise the greeting on the home screen |
| Transactions & categories | Display your dashboard, reports, charts, and streak |
| Recurring transaction settings | Auto-create scheduled transactions on the correct day each month |
| Budget limits | Show progress bars and budget status alerts in the app |
| Currency & theme preference | Apply your chosen settings across the app |
| Notification preference | Schedule or cancel your local daily reminder |
| AdMob ad data (Google) | Serve relevant ads, measure performance, prevent fraud |

We do **not** use your financial data for analytics, advertising, profiling, or any purpose other than displaying it back to you inside the app.

---

## 6. Data Storage and Security

- All your personal and financial data is stored locally on your device using React Native AsyncStorage.
- The storage key is `@spendly/state` — you can inspect or clear it at any time from your phone's app settings.
- We do not have access to your device storage and cannot read, modify, or delete your data remotely.
- Android's automatic device-backup feature is explicitly disabled for Pennify (`android:allowBackup="false"`), meaning your financial data is **not** backed up to Google's servers through Android Backup Service.
- If you uninstall Pennify, all locally stored data is permanently deleted by your operating system.
- No passwords or payment credentials are ever collected or stored.

---

## 7. Third-Party Services

Pennify integrates with the following third-party service:

### Google AdMob
- **Provider:** Google LLC, 1600 Amphitheatre Parkway, Mountain View, CA 94043, USA
- **Purpose:** Display banner advertisements within the app
- **Data collected:** As described in Section 2.3
- **Privacy policy:** [https://policies.google.com/privacy](https://policies.google.com/privacy)
- **Opt-out:** You can opt out of personalised advertising at any time in your phone's settings:
  - **Android:** Settings → Google → Ads → Delete advertising ID

We have configured AdMob with `requestNonPersonalizedAdsOnly` as the default request option, meaning the app requests non-personalised ads by default to minimise data collection.

We do **not** use Firebase Analytics, Crashlytics, or any other analytics or crash-reporting service.

---

## 8. Data Sharing

We do **not** sell, trade, rent, or share your personal information with any third party, except as described in Section 7 (Google AdMob, which operates independently under its own privacy policy).

We do not share data with:
- Data brokers
- Analytics providers (no Firebase Analytics, no Mixpanel, no Segment, no Amplitude)
- Social networks
- Government agencies (unless required by law)

---

## 9. Children's Privacy

Pennify is not directed at children under the age of 13 (or under 16 in the European Economic Area). We do not knowingly collect personal information from children. If you believe a child has provided personal information through the app, please contact us at grizplayapp@gmail.com and we will take appropriate steps.

---

## 10. Your Rights

Depending on your jurisdiction, you may have the following rights regarding your data:

- **Access** – you can view all your data directly inside the app at any time
- **Correction** – you can edit any transaction or setting from within the app
- **Deletion** – you can delete all data from **Settings → Clear all data**, or by uninstalling the app
- **Portability** – use **Settings → Export as CSV** or **Settings → Backup data** to export a copy of your data in a standard format
- **Opt-out of ads personalisation** – see Section 7 above

Since we do not collect or store your data on our servers, there is nothing for us to retrieve, correct, or delete on your behalf beyond what you can already do inside the app.

### GDPR (European Users)
The only data processor involved is Google (AdMob). Our legal basis for processing under GDPR is **legitimate interest** (serving ads to fund a free app). You may withdraw consent to personalised ads at any time via your device settings.

### CCPA (California Users)
We do not sell personal information. The AdMob integration may constitute a "share" of data under CCPA. You may opt out of personalised ads as described in Section 7.

---

## 11. Data Retention

- **Your app data (transactions, settings):** Retained on your device until you clear it or uninstall the app. We have no copy.
- **Exported files (CSV / .pennify backup):** Stored wherever you chose to save them. Pennify has no record of these files after export.
- **AdMob data:** Retained and managed by Google under their own data retention policies.

---

## 12. Changes to This Policy

We may update this Privacy Policy from time to time. When we do, we will update the **"Last updated"** date at the top of this page. We encourage you to review this policy periodically. Continued use of Pennify after a change constitutes acceptance of the updated policy.

---

## 13. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy, please contact us:

**Email:** grizplayapp@gmail.com  
**Developer:** GrizPlay Apps  
**App:** Pennify – Expense Tracker (`com.grizplayapp.pennify`)

---

*This privacy policy was written for the Pennify Android application published on the Google Play Store by GrizPlay Apps.*
