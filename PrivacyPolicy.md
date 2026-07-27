# Privacy Policy

_Last updated: July 2026_

Miimo is built around a simple promise: what you capture stays on your device. This policy explains what that means in practice — including the few things that don't stay, so the promise means something.

## The short version

- Your recordings, transcripts, notes, summaries, and assistant conversations are stored **only on this device**. We never receive them.
- We **never sell** your data, run no advertising, and link no third-party tracking SDKs.
- Using Miimo requires a **Miimo account** (Sign in with Apple). That account holds your identity and subscription state — never your content. See below.
- We count **how often the app is opened and where you are in the subscription funnel**, tied to that account. That is the whole of our analytics.
- The one thing you can choose to send us is a **feedback message**, and only when you tap Send.

## What stays on your device

Everything you create in Miimo — audio takes, live transcripts, translations, notes, summaries, tasks, schedules, saved browser data, and assistant history — is written to local storage on your iPad, iPhone, or Mac. We operate no servers that receive your content, because there are none. Nothing in the sections below changes this: the account we do keep has no field that could hold a recording, a note, or a message you asked the assistant.

## Your Miimo account

Miimo requires an account, created with **Sign in with Apple**. We store, against that account:

- The account identifier Apple issues for you, plus the name and email address Sign in with Apple provides. If you choose Apple's **Hide My Email**, we only ever see the relay address.
- Your **subscription state** — plan, trial or paid, renewal or cancellation status, and the price of the plan — so entitlement follows your account.
- **Device and build facts**: device model, OS version, and the Miimo version and build number, refreshed when the app syncs. These tell us which builds are live and let us reproduce reported bugs. No advertising identifier is read; Miimo does not use one.
- Your **storefront region**, derived from your device locale.
- **Usage counters**: the calendar date on which you last opened Miimo (one row per day, not per launch), and one-time subscription milestones — when the paywall was first seen and how many times, when a trial started, when a purchase or restore happened, when a trial converted, and when a subscription was cancelled.

That last group is analytics, plainly: it is how we know how many people use Miimo and how many subscribe. It records **no in-app behaviour beyond those counters** — not which features you use, not what you record, not where you browse, not what you ask the assistant.

Your account is stored using Google Firebase (Authentication and Firestore), acting as our processor. We use no analytics SDK, and Firebase Analytics is deliberately not linked into the app.

## Network access

Miimo captures, transcribes, and plays back without a network connection. A few features reach the network, most of them only at your request:

- **Your account.** Signing in, and the account fields described above, sync when the app launches or returns to the foreground.
- **Speech recognition.** Transcription runs on your device. On iOS 26 and macOS 26 Miimo uses Apple's on-device speech model. If that model can't be used — an older system, or a language whose offline dictation files aren't installed on your device — Miimo falls back to Apple's system speech recognizer, and in that case Apple may process that audio on its servers under Apple's privacy policy. That audio never reaches us, and Miimo still writes the transcript only to your device.
- **Downloadable open models.** When you choose to download a local model (Llama, Qwen, Phi, Whisper, and similar), Miimo fetches it from Hugging Face. Only the model files are transferred — none of your content is sent.
- **Built-in browser.** Pages you open in Miimo's browser make ordinary web requests, exactly as any browser would.
- **On-device translation.** Apple's Translation framework may download language packs from Apple; your text is translated on device.

## Subscriptions

Miimo Pro is sold as an auto-renewable subscription through the App Store. Purchases, renewals, and billing are handled entirely by Apple. Miimo never sees or stores your payment details, Apple Account, or billing address. Your entitlement is verified on device using Apple's StoreKit; the resulting state — which plan, trial or paid, active or cancelled — is what we record on your account, as described above.

## Feedback you send

If you use **Settings → Send feedback**, the message you write is sent to us. This is the only place in Miimo where something you typed leaves your device, and it only happens when you tap Send.

What we receive is the message itself, plus the email address on your Miimo account, your app version, and your device model and OS version — shown to you on the compose screen before you send. Nothing you have captured is attached: no recordings, transcripts, notes, summaries, or assistant history, ever. We keep the message so we can act on it and reply, and we use it for nothing else.

## Data you export

Backups and exports you create stay under your control — they are written to the location you choose (Files, iCloud Drive, or wherever you save them). Sharing an export is your decision; once shared, it leaves Miimo's on-device protection.

## Deleting your account

**Settings → Account → Delete Account** permanently deletes your account record and its usage counters. Because your content was never uploaded, there is nothing else of yours to erase — your recordings, transcripts, and notes simply stay on your device, and you can delete them by deleting the app.

Two things survive deletion, and we would rather say so than surprise you: a feedback message you sent stays in our support queue so an open report remains actionable, and deleting your account does not cancel your subscription — cancel that in the App Store, under Settings → your name → Subscriptions.

## Children

Miimo is not directed at children and does not knowingly collect information from anyone, of any age, beyond what is described here.

## Changes

If this policy changes, the updated version ships inside the app and the date above is revised.

## Contact

Questions about privacy, or a request to see or delete what we hold? Reach us at **privacy@miimo.app**.
