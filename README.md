# LuckyCharms

LuckyCharms is a local-first AI meeting companion for macOS.

It helps you stay focused during a meeting and come back afterward to a clean record of what happened: transcript, notes, action items, search, and long-term meeting memory.

This repository is the public download and auto-update channel for signed LuckyCharms releases.

## What LuckyCharms Does

LuckyCharms is built around a simple workflow:

- capture the meeting without adding a bot participant
- transcribe the conversation locally on your Mac
- generate a structured AI recap after the meeting
- keep that meeting searchable and useful later

Core capabilities include:

- microphone + system-audio capture so both sides of a conversation are included
- live on-device transcription
- AI-generated meeting recaps
- inline personal notes during the meeting
- reusable meeting tags
- full-text search across meetings, notes, transcripts, and tags
- cross-meeting questions over your past conversations
- Outlook calendar awareness
- automatic app updates

## Why It Feels Different

LuckyCharms is designed as an ambient desktop tool, not a meeting bot.

It lives on your Mac, runs locally, and is meant to help you be present in the conversation instead of managing a note-taking workflow in real time.

That makes it a better fit for:

- sensitive internal meetings
- customer and partner calls
- recruiting and interview workflows
- operators, founders, consultants, and anyone who spends a large part of the week in meetings

## Download

To install LuckyCharms:

1. Open the latest release in this repository.
2. Download the `.dmg` asset.
3. Open the DMG.
4. Drag `LuckyCharms.app` into `Applications`.

If you are already running LuckyCharms, future stable releases can also arrive through the in-app update flow.

## First Launch

When you open LuckyCharms for the first time, macOS and the app will guide you through the setup needed for a working meeting workflow.

### 1. Open the app from Applications

Launch `Applications/LuckyCharms.app`.

If macOS warns that the app was downloaded from the internet, choose `Open`.

### 2. Grant Microphone permission

LuckyCharms needs microphone access to capture your side of the meeting.

### 3. Grant Screen Recording permission

macOS uses Screen Recording permission for system-audio capture. LuckyCharms uses that permission to capture remote participants from your computer’s playback audio.

### 4. Configure your AI provider

If you want AI-generated meeting notes, add an API key for your preferred provider in the setup flow or later in Settings.

### 5. Optionally connect Outlook calendar

If you use Outlook, you can connect calendar access so LuckyCharms can better identify and title meetings.

### 6. Allow the transcription model to download

The first recording downloads the local speech model. That is a one-time setup step, so the first run can take longer than later recordings.

## What You Get After a Meeting

LuckyCharms is built to turn a finished meeting into something useful immediately:

- a transcript of the conversation
- AI recap with summary, decisions, and action items
- your own in-meeting notes stored with the meeting
- role attribution such as `You`, `Remote`, or `Mixed` for transcript segments
- tags for organizing meeting history
- searchable long-term meeting memory

## Privacy and Local Processing

LuckyCharms is intentionally local-first.

- transcription runs on-device
- meeting data is stored locally on your Mac
- audio is processed for transcription rather than uploaded as a permanent cloud recording
- API keys are stored in macOS Keychain

AI recap generation depends on the provider you configure, but the core transcription path is local.

## Requirements

- Apple Silicon Mac
- macOS 14 or later

## Notes

- The first time you download the Parakeet model can take up to 5 minutes depending on your network speed. Transcription won't work until the model is downloaded. 
- Auto-updates use the assets published in this repository.
- For the latest signed build, always use the most recent stable release in this repo.
