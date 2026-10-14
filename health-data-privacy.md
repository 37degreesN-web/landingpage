# Privacy Policy — Health Data by 37°N

**Health Data by 37°N**  
**Last updated:** October 14, 2026

*This privacy policy applies specifically to **Health Data by 37°N**, our on-device health record explorer for iPhone and Android. For Protocols from 37°N, see the [Protocols Privacy Policy](privacy-policy.md).*

---

This Privacy Policy explains how **Health Data by 37°N** ("the app," "we," or "our") accesses and handles data on your device. We believe your personal health records belong exclusively to you. Health Data is built from the ground up as a private, on-device utility.

## 1. What the App Does

Health Data by 37°N is a free mobile application for iPhone and Android. It reads health records stored locally in Apple Health (on iPhone) or Health Connect (on Android), lets you view which apps and devices supplied those records, inspect timestamps and counts, and optionally export loaded records as a comma-separated values (CSV) file.

## 2. Read-Only Access & Health Categories

Health Data is strictly **read-only**. It never writes, modifies, or deletes health records in Apple Health or Health Connect.

The app requests access only to the categories you explicitly choose to authorize. These categories may include:

- **Activity:** steps, workouts, active energy, distance.
- **Body measurements:** height, weight, body fat percentage, body mass index.
- **Cycle tracking & reproductive health:** menstruation, ovulation test results, cervical mucus quality, sexual activity, and intermenstrual bleeding. We explicitly identify these reproductive-health categories because of their sensitive nature.
- **Nutrition & hydration:** dietary intake, water consumption.
- **Sleep:** sleep stages, duration, and bedtimes.
- **Vitals:** heart rate, resting heart rate, heart rate variability (HRV), blood pressure, respiratory rate, and blood oxygen saturation.

You may revoke or modify permissions for any of these data types at any time in your phone's system settings (Apple Health on iPhone or Health Connect on Android).

## 3. Nothing Collected: No Accounts, No Trackers, No Servers

We do not collect your data. Specifically:

- **No accounts:** There is no sign-in, account creation, or email requirement. The app opens directly to the explorer.
- **No analytics or tracking:** There are no third-party tracking SDKs, data brokers, telemetry tools, or advertising networks embedded in the app.
- **No company servers:** 37°N operates no servers or cloud databases for the Health Data app. 37°N never receives, accesses, or processes your health records.
- **No internet permission on Android:** The Android release build does not include the internet permission (`android.permission.INTERNET`), ensuring the app cannot transmit health records over the network.

## 4. Records Stay on Your Phone

Health records read from Apple Health or Health Connect are held in transient device memory while the app is open. The app does not save raw health records or measurement values to persistent local disk storage.

To provide monitoring and history features, the app stores only minimal operational metadata locally on your phone:

- **Local check history (journal):** A rolling log of up to 2,000 read events over the preceding 7 days. Entries record only the check timestamp, the source app name, device name, and record count. The journal holds **no measurement values and no notes**.
- **Record index:** A bounded local index of record IDs (cryptographic fingerprints) used solely to recognise new records across read cycles.
- **Local preferences:** Simple settings such as pinned metrics, whether background monitoring is enabled, and whether permissions were granted.

All local journal files and settings are stored in application-private storage and are explicitly **excluded from operating system backups** (such as iCloud Backup or Android backup). You can permanently clear the local check history and discovery index at any time inside the app by navigating to **Local journal → Clear local journal**, or remove all stored data by deleting the app from your device.

## 5. Background Monitoring

Background monitoring is entirely **optional and disabled by default**. If you choose to enable it, the app periodically checks for newly arrived records in the background:

- On Android, the app requests periodic checks approximately every 15 minutes via system job scheduling.
- On iPhone, the app relies on Apple Health's native background update mechanisms.

All check results and logs remain strictly on your phone. You can disable background monitoring at any time within the app's settings.

## 6. CSV Export Under Your Control

The app exports records only when you explicitly tap **Export records**. The app generates a CSV file of the loaded snapshot on your device and opens your operating system's standard file picker. You choose where to send or save the file — such as the local Files app, an email, or another application. Once saved or shared, you and your selected destination control that file. On iPhone, any temporary export cache file is removed as soon as the file picker completes.

## 7. Feedback and Support Correspondence

Health Data includes an optional feedback and support option:

- Tapping feedback launches your phone's default email client, addressing an email to **pranam@37degreesn.com** with only the message text you wrote. No data is transmitted automatically by the app.
- Generating a diagnostic support report is entirely optional. If created, you can review its text yourself and manually choose whether to copy and include it in your email. It never includes raw health measurement values.

**Support email retention and deletion:** If you contact us by email, we use your message and email address solely to troubleshoot reported issues and assist you. We do not use support correspondence for marketing or share it with third parties. Support emails are retained only for as long as necessary to address your inquiry (up to a maximum of 12 months for record-keeping), after which they are deleted. You may request immediate deletion of your support correspondence at any time by sending an email to pranam@37degreesn.com with the subject line "Support Data Deletion."

## 8. Prohibition of Secondary Uses

In accordance with Apple HealthKit guidelines and Google Health Connect policies:

- We do not sell, rent, or monetize health data.
- We do not use health data for advertising, marketing, or interest-based profiling.
- We do not share health data with data brokers or third parties.
- We do not use health data to train artificial intelligence (AI) or machine learning (ML) models.
- Health records accessed by the app are not stored in iCloud or any cloud repository operated by 37°N.

## 9. Not a Medical Device or Medical Advice

Health Data by 37°N is an informational and diagnostic utility designed to help you inspect and export records from your device's health repositories. It is **not a medical device**, does not provide medical diagnosis, treatment, or clinical advice, and should never be used as a substitute for professional healthcare guidance.

## 10. Children's Privacy

Health Data by 37°N is not directed to children under 16 years of age, and we do not knowingly collect personal information from children.

## 11. Earlier Test Versions

Early pre-release test builds of the app (prior to version 0.13.0) included an experimental Google sign-in mechanism that saved account identity tokens locally in device secure storage. Current versions of Health Data automatically and permanently delete any legacy account session data upon launch or update without reading, using, or transmitting it.

## 12. Changes to This Policy

We may update this Privacy Policy from time to time. If revisions are made, we will update the "Last updated" date at the top of this page. Because the app does not collect user contact information, we encourage users to review this page periodically.

## 13. Contact Us

If you have any questions or requests regarding this Privacy Policy or Health Data by 37°N, please contact:

**Pranam Lipinski**  
37°N Labs  
Email: [pranam@37degreesn.com](mailto:pranam@37degreesn.com)  
General privacy inquiries: [privacy@37degreesn.com](mailto:privacy@37degreesn.com)
