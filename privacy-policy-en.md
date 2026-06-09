# Privacy Policy — Sleeply

**Last updated:** May 14, 2026
**Effective date:** May 14, 2026

This Privacy Policy explains how Sleeply ("we", "us", "our") handles your information when you use the Sleeply mobile application (the "App") on iOS.

**TL;DR:** Sleeply stores all your data on your device. We do not run any backend servers, we do not have analytics, we do not track you, and we cannot see your data. Audio recorded for snore detection never leaves your iPhone.

---

## 1. Data we collect

### 1.1 Sleep sessions and preferences
When you complete a sleep session, the App records:
- Session start and end times
- Selected audio program / custom mode
- Detected snore events (timestamp, duration, intensity score)
- Phase events (timer-based heuristic when Apple Watch is unavailable)
- Your in-app preferences (chosen program, alarm settings, sleep timer, anti-snore settings)

This data is stored locally on your device using Apple's SwiftData framework. **It is never transmitted to us or to any third party.**

### 1.2 Microphone audio (snore detection)
The App listens through your device's microphone during active sleep sessions to detect snoring. Audio is processed entirely on-device by Apple's `SoundAnalysis` framework. **Audio is never recorded to disk, transmitted, or stored.** Only the classification result (timestamps and confidence scores of detected snores) is saved locally.

### 1.3 Apple Health data (optional)
If you connect Apple Health, the App reads the following types **with your explicit permission**:
- Heart rate
- Heart rate variability (HRV / SDNN)
- Sleep analysis (stages)
- Respiratory rate
- Oxygen saturation (SpO₂)

The App may also write completed sleep sessions to Apple Health as `sleepAnalysis` samples so you can see them alongside other sources in the Health app. You can revoke either or both permissions at any time in iOS Settings → Privacy & Security → Health.

All Apple Health data remains on your device and under your control. We never read or copy Health data outside of generating insights locally.

### 1.4 On-device AI processing
When available (iOS 26+ with Apple Intelligence), aggregated statistics (averages, trends, no raw events) are passed to Apple's on-device language model to generate natural-language insights. **Apple's on-device model runs locally on your iPhone; data does not leave the device.**

### 1.5 Subscription purchases
Subscription transactions are handled entirely by Apple via StoreKit. We receive confirmation that a transaction occurred but we do not handle, store, or process your payment details. Apple's privacy policy applies to those transactions.

### 1.6 Notifications
Local notifications (Smart Alarm, bedtime reminders) are scheduled and delivered by your device. We do not use push notifications and we do not maintain a notification service.

---

## 2. Data we do **not** collect

- We do not maintain user accounts. You do not sign up, sign in, or provide an email.
- We do not collect device identifiers, advertising IDs, or behavioural data.
- We do not use analytics SDKs (no Firebase, Mixpanel, Amplitude, etc.).
- We do not use third-party tracking, advertising, or attribution SDKs.
- We do not collect crash reports beyond Apple's optional aggregated diagnostics (controlled in iOS Settings → Privacy & Security → Analytics & Improvements).

---

## 3. How your data is used

All data described in Section 1 is used exclusively to:
- Provide the App's features (audio playback, snore detection, sleep tracking, insights, alarms)
- Compute statistics shown to you in the Insights tab
- Generate AI-coach recommendations on-device

Your data is **not** used for advertising, profiling, sale, or sharing with third parties.

---

## 4. Data retention and deletion

Your data lives on your device until you choose to delete it. To remove all data:
- Delete the App from your iPhone (this removes the local SwiftData store)
- Optionally, revoke Apple Health write permission and delete sessions written by Sleeply from the Apple Health app

If you want to remove a specific session, you can do so from the Insights tab (long-press to delete in future versions).

---

## 5. Children's privacy

Sleeply is not directed to children under 13. If you are under 13, please do not use the App.

---

## 6. Medical disclaimer

Sleeply is a **wellness app, not a medical device**. It does not diagnose, treat, cure, or prevent any disease. Binaural-beat and anti-snore intervention research is preliminary and individual responses vary. If you experience persistent sleep disturbance, loud snoring with pauses in breathing, or any concerning health symptoms, consult a qualified healthcare professional.

---

## 7. International users

The App processes all data on your device. We do not transfer data internationally because we do not collect it on any server. If you are an EU/EEA resident, your data does not leave your device and therefore is not subject to international transfer mechanisms.

---

## 8. Your rights

Because we do not collect or store your data on any server, there is nothing for us to disclose, modify, or delete on your behalf. You have full control of your data via your device:

- **Access:** All your data is visible in the App itself
- **Deletion:** Delete the App to remove all local data
- **Portability:** Sessions can be written to Apple Health (you control this in Settings)
- **Withdraw consent:** Revoke Microphone, Notification, and Health permissions at any time in iOS Settings

---

## 9. Changes to this policy

We may update this Privacy Policy. When we do, we will update the "Last updated" date at the top. Material changes will be communicated through the App.

---

## 10. Contact

Questions about this Privacy Policy can be sent to:

📧 **zzcredi@gmail.com**
