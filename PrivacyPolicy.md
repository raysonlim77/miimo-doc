# Privacy Policy

_Last updated: August 2026_

Miimo is built around a simple promise: what you capture stays on your device. This policy explains what that means in practice — including the few things that don't stay, so the promise means something.

## The short version

- Your recordings, transcripts, notes, summaries, tasks, browser data, and assistant conversations are stored **only on this device**. We never receive them.
- Miimo's AI runs **on your device**, on Apple Intelligence. **Nothing you capture or type is sent to any third-party AI service** — Miimo has no such integration.
- We **never sell** your data, run no advertising, and link no third-party tracking SDKs.
- Using Miimo requires a **Miimo account** (Sign in with Apple). That account holds your identity and subscription state — never your content.
- We count **how often the app is opened and where you are in the subscription funnel**, tied to that account. That is the whole of our analytics.
- The one thing you can choose to send us is a **feedback message**, and only when you tap Send.
- A few features reach the internet at your request — the built-in browser, and the assistant when you ask it to search the web or read a link. Those requests go to those sites, not to us, and the assistant's web access is **off until you turn it on**.
- Before any of this happens, Miimo shows you a **data-sharing screen inside the app** — what leaves, who receives it, and a switch for the optional part — and asks you to agree. It's re-readable anytime at Settings → Privacy & data.

## Artificial intelligence: on your device, and nowhere else

Everything Miimo describes as AI — live transcription and its polish, summaries, chapters, action items, translation, flashcards, quizzes, and the assistant that answers you — runs **on this device**, on Apple's on-device Foundation Models (Apple Intelligence). This is not a fallback or a preference: Miimo requires Apple Intelligence and will not run without it, which is why the app blocks itself with an explanation on a device where it isn't available.

Stated plainly, because it is the question people ask:

- **Miimo does not send your data to any third-party AI service.** Not OpenAI, not Google Gemini, not Anthropic, not Microsoft, not any other model provider or AI API. There is no such integration in the app, no API key in the binary, and no server of ours in between.
- **Your recordings, transcripts, notes, and assistant messages are never used to train any model** — ours, Apple's, or anyone else's. They are never sold, shared, or sent to an advertiser or a data broker.
- **The model never leaves your device, and neither does what you give it.** Prompts, attached images and documents, and the answers produced from them are created and kept locally.

Two AI-adjacent downloads do use the network, and neither carries your content: Apple Intelligence and Apple's speech and translation models are fetched from Apple as model files, and if you choose to download an open model (Llama, Qwen, Phi, or a Whisper model) it comes from Hugging Face. In both cases only model weights travel, in one direction, and they then run offline.

The one place the assistant *can* reach a third party is when you ask it to search the web or read a link — described under "When Miimo uses the network" below, off by default, and never carrying your recordings or notes.

## Your permission, asked in the app

Before you sign in and before you record anything, Miimo shows a data-sharing screen that lists every way data leaves this device, names each recipient, and marks which are optional. You agree to it to continue.

The assistant's web access is presented there as a switch that starts **off**, and asking the assistant to search the web while it's off prompts you again at that moment rather than sending anything. You can review the whole disclosure, and turn web access on or off, at any time under **Settings → Privacy & data**. Turning it off applies to your very next message.

## What stays on your device

Everything you create in Miimo — audio takes, live transcripts, translations, notes, handwriting, slide and screen captures, summaries, tasks, schedules, study material, browser history and bookmarks, and assistant history — is written to local storage on your iPad, iPhone, or Mac. We operate no servers that receive your content, because there are none. There is no cloud sync and no cloud backup: your library lives in one place, and deleting the app deletes it.

Nothing in the sections below changes this. The account we do keep has no field that could hold a recording, a note, or a message you asked the assistant.

## Your Miimo account

Miimo requires an account, created with **Sign in with Apple**. There is no way to skip it. We store, against that account:

- The account identifier Apple issues for you, plus the name and email address Sign in with Apple provides. If you choose Apple's **Hide My Email**, we only ever see the relay address.
- Your **subscription state** — plan, product, trial or paid, auto-renew, purchase, renewal and cancellation dates, the price of the plan and its currency, and Apple's transaction identifiers — so entitlement follows your account and so we can tell real purchases from test ones.
- **Device and build facts**: platform, device model, OS version, the Miimo version and build number, and your device's language and region setting, refreshed when the app syncs. These tell us which builds are live and let us reproduce reported bugs. No advertising identifier is read; Miimo does not use one.
- Your **storefront region**, derived from that locale.
- **Usage counters**: when you signed up, the calendar date on which you last opened Miimo (one row per UTC day, not per launch), how many distinct days you've opened it, and one-time subscription milestones — when the paywall was first seen and how many times, when a trial started, when a purchase or restore happened, when a trial converted, and when a subscription was cancelled.

That last group is analytics, plainly: it is how we know how many people use Miimo and how many subscribe. It records **no in-app behaviour beyond those counters** — not which features you use, not what you record, not where you browse, not what you ask the assistant.

Your account is stored using Google Firebase (Authentication and Firestore), acting as our processor. We use no analytics SDK, and Firebase Analytics is deliberately not linked into the app.

## Every third party involved, and what binds them

This is the complete list. There are no others, and no AI service appears on it.

- **Apple** — receives your Sign in with Apple identity, handles App Store purchases and subscriptions, receives speech audio only where your language has no on-device dictation files installed, and serves model and language-pack downloads. Governed by Apple's Privacy Policy (apple.com/legal/privacy), which affords protections equal to or greater than those described here.
- **Google Firebase** (Authentication and Firestore) — receives your account record only: identity, subscription state, device and build facts, and the usage counters listed above. No content, ever. Firebase acts strictly as our data processor under the Google Cloud Data Processing Addendum: it may process this data only on our instructions, is bound to confidentiality and security obligations, and does not use it for its own purposes.
- **DuckDuckGo** — receives only the search words you asked the assistant to look up, and only while you have web access turned on. Governed by DuckDuckGo's Privacy Policy (duckduckgo.com/privacy); the endpoint Miimo uses sets no tracking cookies and needs no account or API key.
- **Sites you open** — in the built-in browser, or a link you hand the assistant. They receive an ordinary web request, exactly as they would from Safari, and each site's own privacy policy governs it. Miimo blocks well-known ad and tracker domains by default.
- **Hugging Face** — receives nothing about you. A model file is downloaded; nothing is uploaded, and no account or identifier is sent.

We share your data with no one else: no advertisers, no data brokers, no analytics vendors, and no AI or machine-learning provider.

## When Miimo uses the network

Miimo captures, transcribes, translates, and plays back without a network connection. These are the only things that reach out, and most of them only when you ask:

- **Your account.** Signing in, and the account fields described above, sync when the app launches or returns to the foreground.
- **Speech recognition.** Transcription runs on your device. On iOS 26 and macOS 26 Miimo uses Apple's on-device speech model, downloading the language's model files from Apple the first time you use it. If that model can't be used — an older system, or a language whose offline files aren't available on your device — Miimo falls back to Apple's system speech recognizer, and in that case Apple may process that audio on its servers under Apple's privacy policy. That audio never reaches us, and Miimo still writes the transcript only to your device.
- **The assistant's web access.** This is **off unless you turn it on**, on the first-run data-sharing screen or under Settings → Privacy & data. With it on: if you ask the assistant to search the web, your search words are sent to **DuckDuckGo**; if you give it a link to read, Miimo fetches that page from **the site that hosts it**. Both happen only in response to a message you send, and both send only the query or the link — never your recordings, notes, or the rest of the conversation. The answer is then written on your device by an on-device model. Nothing about these requests reaches us, and no AI service is involved on the far end — DuckDuckGo is a search engine, and the page is fetched as a browser would fetch it.
- **The built-in browser.** Pages you open make ordinary web requests, exactly as any browser would. Miimo blocks well-known ad and tracker domains by default, which you can turn off globally or for a single site.
- **Downloadable open models.** When you choose to download a local model — Llama, Qwen, Phi, or a Whisper model for the stop-time re-check — Miimo fetches it from Hugging Face. Only the model files are transferred; none of your content is sent, and once downloaded they run entirely offline.
- **On-device translation.** Apple's Translation framework may download language packs from Apple; your text is translated on your device.
- **Purchases.** Handled by Apple's App Store. See below.

## The built-in browser

The browser is part of the app, so its data follows the same rule as everything else: **history, bookmarks, downloads, per-site settings, and saved logins are stored on your device only** and are never sent to us.

Saved logins are kept in the system **Keychain**, marked so they stay on this device and never sync, and revealing or autofilling one asks for Face ID, Touch ID, or your device passcode. They are deliberately left out of Miimo backups, so a backup file never carries your passwords.

Miimo's browser is a real browser: sites you visit see you as any browser's visitor, and their own privacy policies govern what they do. If you join a video call in it, the camera and microphone are used by that site for that call, and Miimo neither records nor keeps that stream unless you start a recording yourself.

## Your device's own features

Some things leave Miimo's storage but not your device:

- **Spotlight.** Session titles and a short snippet — the summary headline, or the opening line of the transcript or notes — are added to your device's Spotlight index so you can find a capture from the Home Screen or Finder. It's local to your device, and removing a session removes it from the index.
- **Widgets and Live Activities.** The current recording's state is written to a shared container so the widget and Lock Screen activity can show it.
- **Reminders.** Event reminders are local notifications scheduled by your device. Nothing is sent anywhere.
- **System audio and screen capture.** On a Mac, Miimo can record the system's audio and take screenshots of a display you choose, so a call or a deck can be captured. On iPad it can hear a call playing in its own browser. All of it is written to your library on the device.

## Subscriptions

Miimo Pro is sold as an auto-renewable subscription through the App Store. Purchases, renewals, and billing are handled entirely by Apple. Miimo never sees or stores your payment details, Apple Account, or billing address. Your entitlement is verified on device using Apple's StoreKit; the resulting state — which plan, trial or paid, active or cancelled — is what we record on your account, as described above.

## Feedback you send

If you use **Settings → Send feedback**, the message you write is sent to us. This is the only place in Miimo where something you typed leaves your device for us, and it only happens when you tap Send.

What we receive is the message itself and the category you picked, plus the name and email address on your Miimo account, your app version and build, your device model, OS version and region, and whether you were subscribed at the time — the account, app, and device lines are shown to you on the compose screen before you send. Nothing you have captured is attached: no recordings, transcripts, notes, summaries, or assistant history, ever. We keep the message so we can act on it and reply, and we use it for nothing else.

## Backups and exports

Backups and exports you create stay under your control — they are written to the location you choose (Files, iCloud Drive, or wherever you save them), never to us. A backup contains your library: sessions with their audio and attachments, notes, tasks, events, browser data, and assistant history. It excludes your saved passwords and downloaded model weights. Sharing an export is your decision; once shared, it leaves Miimo's on-device protection.

## Deleting your account

**Settings → Account → Delete Account** permanently deletes your account record and its daily-active rows. Because your content was never uploaded, there is nothing else of yours to erase — your recordings, transcripts, and notes simply stay on your device, and you can delete them by deleting the app.

Two things survive deletion, and we would rather say so than surprise you: a feedback message you sent stays in our support queue so an open report remains actionable, and deleting your account does not cancel your subscription — cancel that in the App Store, under Settings → your name → Subscriptions.

## Children

Miimo is not directed at children and does not knowingly collect information from anyone, of any age, beyond what is described here.

## Changes

If this policy changes, the updated version ships inside the app and the date above is revised.

## Contact

Questions about privacy, or a request to see or delete what we hold? Reach us at **raysonlim77@gmail.com**.
