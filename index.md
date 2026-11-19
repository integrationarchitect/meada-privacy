---
title: Meada Privacy Policy
---

# Meada Privacy Policy

Effective date: 2026-11-19 · Version 1.3

Meada is an Android app that files your conversation transcripts into topic folders in **your own Google Drive**, builds a knowledge graph of them in that same Drive, and answers your questions using the AI provider **you** choose. This policy explains what data Meada touches, where it goes, and your rights. It is written to meet the EU General Data Protection Regulation (GDPR, in particular Articles 12–22), Brazil's Lei Geral de Proteção de Dados (LGPD, in particular Articles 9 and 18), and the Google API Services User Data Policy, including its Limited Use requirements.

## 1. Who is responsible

- **Publisher of the app ("we"):** Cadisa Systems, contact: support@cadisa.systems. We publish the software. **We do not operate servers that receive, store or process your content.** Meada has no developer back end, no analytics, no advertising and no crash reporting service.
- **Your Google Drive data:** you control it. Meada reads and writes it on your phone, with the access you grant, on your behalf.
- **Your AI provider** (Anthropic, OpenAI or Google Gemini — the one you configure): processes the text and audio Meada sends on your behalf under **your own account and API key**, under that provider's terms and privacy policy. In GDPR terms, the provider acts for you under your contract with it; Meada only routes your request from your phone.

Because nothing reaches us, we hold no copy of your content and cannot read, recover or hand it over.

## 2. What data Meada accesses

| Data | Where it comes from | Why |
|---|---|---|
| Files and folders inside the Google Drive folder you choose (transcripts, topic folders, `README.md` summaries, `graphify-out/graph.json`) | Your Google Drive, with the Drive permission you grant | To list topics, file new transcripts, show, move and merge files, and build the graph |
| Your Google account email address | Google Drive (`about` endpoint) | Shown on screen so you know which account is connected |
| `.md`, `.txt`, Word (`.docx`) and audio files you share with Meada or pick in the app | Other apps on your phone, at your request | To file them. Word files are converted to text on your phone; the original is kept in your Drive |
| Your AI provider API keys | You type them | To call the provider you chose |
| App settings, spending records, the queue of files waiting to be filed | Created on your phone | To run the app |
| Your Ask history: questions, answers and the sources they cited | Created on your phone when you ask | So you can read an answer again without asking (and paying) twice; delete one, or all with **Clear history** |

Meada does **not** access your contacts, location, camera, microphone, call logs or any Drive files outside the folder you chose for its normal work. Meada requests Google's `drive.file` permission: it can see only the folders and files Meada itself creates, never the rest of your Drive.

## 3. Where your data goes

- **Your Google Drive:** your transcripts, filed segments, summaries and the knowledge graph are stored there, in your account, under Google's terms. You can open, download or delete them at any time.
- **Your chosen AI provider:** the text of a transcript you file (and, for audio, the audio file) is sent over HTTPS to the provider configured for "Organize". The questions you ask, with the matching segments from your Drive, are sent to the provider configured for "Answer". The app shows which provider will receive data on the AI connections screen before you save it. Nothing is sent to any other party.
- **Nowhere else.** All network traffic is HTTPS to Google (Drive and sign-in) and to the AI provider you configured.

## 4. How data is protected on your phone

- API keys are encrypted with **AES-256-GCM** using a key that lives in the **Android Keystore** and never leaves the device's secure hardware. The plain key is never written to storage, logs or Drive.
- Android cloud backup and device-to-device transfer are **disabled** for all of Meada's local files, so keys, tokens, settings and queued transcripts are never copied into backups.
- With the optional lock enabled, Meada requires your fingerprint, face or screen lock to open, and hides its content from the recent-apps screen and screenshots.
- Meada writes no logs containing your content, keys or tokens.

## 5. Google user data: Limited Use

Meada's use and transfer of information received from Google APIs adheres to the [Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy), including the Limited Use requirements. In particular:

- Google Drive data is used **only** to provide the features you see in the app (filing, topics, merging, the knowledge graph and answers to your questions).
- It is transferred only to the AI provider **you** configure, only to perform the action you started, and to no one else.
- It is **never** used for advertising, never sold, and never used to build user profiles.
- It is **never** used to develop, improve or train generalized AI or machine-learning models by us. We have no access to it.
- No human at the publisher reads your Drive data. We have no means to.

Your AI provider's own handling of API requests is governed by its API terms (for example, whether API inputs are retained for a limited time for abuse monitoring). Review your provider's API data policy; Meada sends data only under your account with that provider.

## 6. Legal bases (GDPR Art. 6, LGPD Art. 7)

- **Performing the service you asked for** (GDPR Art. 6(1)(b); LGPD Art. 7, V): reading and writing your Drive folder, sending your content to the AI provider you chose, and keeping app settings on your phone.
- **Your consent** (GDPR Art. 6(1)(a); LGPD Art. 7, I): the Google permission you grant on the consent screen and the AI connection you configure. You can withdraw consent at any time (section 8); withdrawal does not affect processing already done.

Meada does not use your data for any other purpose, does not make automated decisions with legal or similarly significant effects about you, and does not profile you (GDPR Art. 22).

## 7. Retention and deletion

- **On your phone:** data is kept until you delete it. Settings → **Disconnect & delete local data** revokes Meada's Google access and deletes everything Meada keeps on the phone (API keys and their Keystore key, settings, spend records, the Ask history, the queue and cached files). Uninstalling the app or clearing its storage in Android settings has the same local effect.
- **In your Google Drive:** your files stay there until **you** delete them; Meada never deletes them on disconnect. Delete the Meada folder in Google Drive to remove them. Undo and merge actions move files to Drive's trash, which Google empties after 30 days or when you empty it.
- **Google access:** revoke it in the app (above) or at any time at [myaccount.google.com/permissions](https://myaccount.google.com/permissions).
- **At your AI provider:** retention of API inputs is set by your provider; see its API data policy and your account settings there.
- **With us:** nothing to retain, because we receive nothing.

## 8. Your rights

Under the GDPR (Arts. 15–22) and the LGPD (Art. 18) you have the right to confirmation and access, rectification, erasure, restriction, objection, portability, information about sharing, and to withdraw consent. Because your content lives in your Drive and on your phone, you exercise most of these rights directly:

| Right | How |
|---|---|
| Access / confirmation | Open your Meada folder in Google Drive; everything Meada stores is there as readable files |
| Rectification | Edit or move any file in Drive or in the app |
| Erasure | Delete files or the folder in Drive; use **Disconnect & delete local data** for the phone |
| Portability | All data is in open formats: Markdown with YAML front matter, and `graph.json` (NetworkX node-link JSON, Graphify-compatible); download it from Drive |
| Information about sharing | Section 3: only your AI provider, only for the action you start |
| Withdraw consent / object | Disconnect in the app, revoke access at Google, or remove the AI connection |
| Restriction | Turn off auto-file, README summaries, AI concept extraction or graph auto-update in Settings |

For anything else, contact support@cadisa.systems. We will answer within one month (GDPR) or 15 days (LGPD, Art. 19). You may also complain to your data protection authority, for example your EU supervisory authority or Brazil's ANPD.

## 9. International transfers

Your AI provider and Google may process data outside your country (for example in the United States). These transfers happen under your agreements with those providers and their safeguards (such as Standard Contractual Clauses). Meada itself transfers nothing to us.

## 10. Children

Meada is not directed at children under 16 and should not be used by them.

## 11. Changes

We will update this policy when Meada's data handling changes, with a new effective date and version, and show it in the app. If a future version adds a managed service that relays your content, it will be stateless (processing in memory only, no logging or storage of content) and this policy will be updated before it is offered.

## 12. Contact

Cadisa Systems · support@cadisa.systems · For LGPD: data protection officer (encarregado): leonardo.fernandes@cadisa.systems.
