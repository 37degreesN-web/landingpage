# Privacy Policy — 37°N Connected Apps & Accounts

**37°N Accounts, NOD, Squad Hub & Protocol Explorer**  
**Last updated:** October 14, 2026

*Looking for Health Data by 37°N? Health Data operates strictly on your phone with no user accounts, no cloud servers, and no tracking. Read its standalone policy here: [Health Data by 37°N Privacy Policy](health-data-privacy.md).*

---

This Privacy Policy explains how 37°N ("we," "us," or "our") collects, protects, uses, and handles data when you use a 37°N account and our connected applications: **NOD (Nightly Open Data)**, **Squad Hub**, and **Protocol Explorer** (collectively, the "Services"). We treat health records and personal information with utmost care and transparency.

## 1. Shared 37°N Account (All Connected Apps)

A single 37°N account works seamlessly across our connected applications: NOD, Squad Hub, and Protocol Explorer. When you create or sign in to an account, the following policies apply:

### Sign-In & Authentication
You can sign in using your email and password or Google Sign-In, authenticated through **Google Firebase Authentication**. We never store raw passwords on our servers.

### User Profile Information
Your profile data is stored on 37°N cloud servers hosted on Google Cloud (Firestore / Cloud SQL in the United States). Your profile can include:
- **Account identifiers:** display name and registered email address.
- **Preferences:** preferred units of measurement (e.g., metric vs. imperial weight units).
- **Demographics:** age, sex at birth, racial background, and other self-reported demographic information you choose to enter.
- **Personal goals & wellness history:** user-entered health goals, medications, or health conditions that you voluntarily record to personalize your experience.

**Profile Security at Rest:** Profile data is encrypted at rest using industry-standard AES-256 encryption provided by Google Cloud and is protected by Firebase Security Rules and identity-based access controls. *Note: Profile information is not end-to-end encrypted*, as our backend cloud functions must process it to verify permissions, deliver squad rosters, and manage account services.

### Analytics: No Ads, No Selling of Data
We use **Firebase Analytics** to understand aggregated feature usage and app health. Analytics tracks events such as screens viewed, sign-in attempts, search terms queried, protocols joined, squad actions, and app opens. Analytics **never records raw health measurements**.

NOD explicitly disables the collection of the Android Advertising ID (`AD_ID`). Across all 37°N apps, **we do not show advertisements, we do not use third-party data brokers, and we never sell, rent, or trade your personal or health data to anyone**.

### Push Notifications
If you grant notification permission, we store your device push token via **Firebase Cloud Messaging** so our servers can send timely reminders, streak alerts, and squad updates. In addition, NOD schedules local reminders directly on your phone.

### Feedback and Support Correspondence
When you send feedback or support inquiries from within the apps, your message and chosen category are transmitted to 37°N servers along with your account identifier. Support correspondence is reviewed exclusively by authorized 37°N engineering and support personnel to diagnose technical issues and assist you. Support inquiries are retained for up to 12 months for quality assurance, after which they are deleted.

### Third-Party Service Processors
We rely on vetted infrastructure providers to deliver our cloud services under strict confidentiality and security terms:
- **Google Cloud & Firebase (United States):** Firebase Authentication, Cloud Firestore, Cloud Functions, Cloud SQL, Firebase Analytics, and Firebase Cloud Messaging.

---

## 2. NOD (Nightly Open Data — Sleep App) {#nod}

NOD is our personal sleep optimization and N-of-1 self-experimentation application for iOS and Android.

### Health Data Read
With your explicit operating system permission, NOD reads the following categories from **Apple Health** (iPhone) or **Health Connect** (Android):
- **Sleep telemetry:** time in bed, asleep duration, awake periods, sleep sessions, and sleep stages (light, deep, REM).
- **Heart metrics:** heart rate and resting heart rate.

**Strictly Read-Only:** NOD never writes to, modifies, or deletes records in Apple Health or Health Connect.

### Background Health Sync
With your permission, NOD performs background reads so your morning sleep scores, nightly metrics, and check-in prompts are updated as soon as you wake up.

### Encrypted Cloud Sync
Your sleep records, daily check-ins, reflection notes, and experiment data (protocol runs, nightly yes/no answers, and custom experiment templates) are **encrypted locally on your phone before they are uploaded** to cloud storage (Firestore).

### Key Management & Account Recovery
To ensure you do not permanently lose your historical sleep data if you replace, damage, or upgrade your phone, encryption keys are backed up to your account. 37°N's recovery service can unlock and restore these keys for your verified, authenticated account upon sign-in. Because keys are recoverable through your account, we do not claim that 37°N could never mathematically decrypt this data or that it is end-to-end encrypted beyond recovery; rather, your records are encrypted on-device before transmission, and keys are isolated and released exclusively to your authenticated account.

### Onboarding Answers and Sleep Goals
Your responses to initial onboarding questions and your target sleep duration are saved to your account profile to calculate your personalized 37° Sleep Score.

### Optional Degradation Studies
NOD may offer optional scientific studies (such as measuring the impact of specific late-night habits on deep sleep). Participating in or leaving a study is recorded on our servers along with the consent version for compliance auditing. Study data is used solely to evaluate habit outcomes within your encrypted experiment runs. You can withdraw consent and leave a study at any time.

### Squads in NOD
Social accountability and peer sharing within NOD are powered by our Squads framework and are governed by the Squad Hub section below.

---

## 3. Squad Hub (and Squads inside NOD) {#squad-hub}

Squad Hub powers peer accountability, shared streaks, and protocol compliance across our ecosystem.

### Squad Membership Data
Squad names, membership rosters, invite links, roles (Captain or Member), and streak milestones are stored on 37°N servers. To safeguard personal privacy, **members can choose a pseudonym** instead of displaying their real name or email to squad peers.

### Shared Health & Sleep Summaries
When you join a squad and explicitly agree to share progress, your daily sleep scores, recovery vitals, and check-ins are **encrypted separately for each member of that squad**. Only active members of your squad hold the keys to decrypt and view your shared summaries. Sharing begins only after you join and agree; leaving a squad immediately revokes future data sharing.

**Key Recovery Caveat:** As with individual records, squad encryption keys can be recovered through verified account authentication; we do not claim that the server is incapable of decryption.

### What Other Squad Members See
Members of a squad you join can see:
- Your display name or chosen pseudonym, avatar/profile image (if uploaded), role (Captain or Member), and active consistency streak.
- Your recent activity status (e.g., "Active 10m ago") and daily check-in completion status (morning, afternoon, or evening check-in completed).
- Shared sleep and recovery metrics (when shared): 37° Sleep Score, total sleep time, sleep efficiency, quality and alertness ratings, bedtime and wake-up times, sleep stage breakdown (deep, REM, light), and morning reflection notes.
- Social reactions and nudges: fist-bumps, kudos, and Captain boosts.

---

## 4. Protocol Explorer {#protocol-explorer}

Protocol Explorer enables users to discover, search, and evaluate evidence-based health and wellness protocols.

### What is Stored
Protocol Explorer requires a 37°N sign-in. When you search for or view protocols, search keywords, filters, viewed protocols, and bookmarked protocols are sent to 37°N servers to deliver search results and improve protocol rankings, and may appear in aggregated analytics.

**Zero Health Repository Access:** Protocol Explorer does **not** request, access, or read any records from Apple Health or Health Connect.

### Protocol Sharing
Sharing a protocol uses your phone's native operating system share sheet. You choose the destination application or recipient; 37°N does not monitor or control where links are shared.

---

## 5. Deleting Your Account and Data {#account-deletion}

You have the absolute right to delete your 37°N account and all associated records at any time. When an account deletion is executed, we permanently delete:
- Your authentication credentials and registered email.
- Your user profile, demographics, and health preferences.
- All squad memberships, roles, invite records, and shared status.
- All encrypted sleep records, check-ins, vitals history, and key backups stored on our cloud servers.
- All device push notification tokens.

**How to Request Deletion:** You can initiate permanent account and data deletion at any time through our public web deletion portal at [delete-account.html](delete-account.html) or by emailing [privacy@37degreesn.com](mailto:privacy@37degreesn.com?subject=Account%20and%20Data%20Deletion%20Request) with the subject line "Account and Data Deletion Request."

**Timeframe:** All account deletion requests are completed within **30 calendar days**. Once deleted, your account and historical records cannot be restored.

---

## 6. Your Rights and Choices

Depending on your jurisdiction (including under the EU/UK GDPR, California Consumer Privacy Act CCPA/CPRA, and Washington My Health My Data Act), you have the right to:
- **Access & Export:** Request a copy of your account information and export your data in a portable format.
- **Correction:** Update or correct inaccurate profile details directly in your account settings.
- **Deletion:** Permanently delete your account and all stored cloud data.
- **Revoke Permissions:** Revoke Apple Health or Health Connect permissions at any time via your device's system settings. Revoking access stops all subsequent reads.
- **Withdraw Consent:** Leave any squad or optional degradation study at any time.

To exercise any of these privacy rights, contact us at [privacy@37degreesn.com](mailto:privacy@37degreesn.com).

---

## 7. Not Medical Advice or a Medical Device

None of our applications (NOD, Squad Hub, Protocol Explorer, or Health Data) are medical devices, and 37°N does not provide clinical diagnosis, medical treatment, or healthcare services. Content, sleep scores, and protocols are provided solely for personal informational and self-tracking purposes. Always consult a qualified physician or healthcare provider before altering your sleep habits, medication, supplement, or exercise routine.

---

## 8. Children's Privacy

The Services are not directed to children under 16 years of age, and we do not knowingly collect personal information from children. If you believe that a child has provided us with personal information, please contact us immediately so we can delete it.

---

## 9. Changes to This Privacy Policy

We may update this Privacy Policy periodically to reflect app updates or regulatory changes. If we make material modifications, we will notify you through the app or by email before they take effect. The "Last updated" date at the top of this page indicates the effective date of the latest revision.

---

## 10. Contact Us

If you have any questions, requests, or privacy inquiries regarding your 37°N account or our applications, please contact:

**Pranam Lipinski**  
37°N Labs  
Email: [privacy@37degreesn.com](mailto:privacy@37degreesn.com)  
Support: [support@37degreesn.com](mailto:support@37degreesn.com)
