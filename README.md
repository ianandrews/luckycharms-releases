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

## Quick Start

If you want the fastest path to understanding the product, do this:

1. Install LuckyCharms and complete the first-run setup.
2. Start or record one real meeting.
3. Let the transcript run during the meeting.
4. Add a few personal notes while the meeting is happening.
5. Stop recording and generate the AI recap.
6. Create a tag like `Customer` or `Interview` and assign it to the meeting.
7. Come back later and search for that meeting or ask a question across your meeting history.

That single workflow exercises most of what makes LuckyCharms useful.

## Configure AI Meeting Summaries

LuckyCharms separates transcription from summarization:

- transcription runs locally on your Mac
- AI meeting recaps use the provider you configure in Settings

To set up summaries:

1. Open `Settings` in LuckyCharms.
2. Choose an AI provider.
3. Enter the required API key if that provider needs one.
4. Pick the model you want to use for meeting notes.
5. Save your changes.

Notes:

- Keys are stored locally in macOS Keychain.
- You can change providers or models later.
- If you only want local transcription and not AI summaries yet, you can still use LuckyCharms without generating recaps.

## Connect Outlook Calendar

Outlook calendar integration helps LuckyCharms recognize and title meetings more intelligently.

When Outlook is connected, LuckyCharms can:

- identify scheduled meetings more accurately
- use calendar titles and metadata to improve meeting organization
- make the day-to-day workflow smoother if your calendar is already the source of truth

To connect Outlook:

1. Open `Settings`.
2. Find the `Outlook Calendar` section.
3. Start the connection flow.
4. Follow the Microsoft sign-in steps shown by the app.

After setup, LuckyCharms will use that calendar context automatically.

## Organize Meetings with Tags

Tags are the simplest way to turn meeting history into something useful over time.

Examples:

- `Customer`
- `Interview`
- `Private`
- `Board`
- `Tesla`

Typical tag workflow:

1. Create reusable tags in `Settings`.
2. Open a meeting detail page.
3. Assign one or more tags to that meeting.
4. Use the sidebar to filter meetings by a tag later.

Tags also participate in:

- meeting search
- dashboard filtering
- cross-meeting AI retrieval

That means a question like "action items from customer meetings this week" can use tag information to focus the answer on the right subset of meetings.

## Search and Ask Questions

LuckyCharms gives you two different ways to find information:

### Search

Use search when you want to find a specific meeting or phrase quickly.

Search covers:

- meeting titles
- attendees
- tags
- personal notes
- transcripts
- AI summaries

Good examples:

- `tesla`
- `pricing`
- `customer`
- `roadmap`

### Cross-meeting questions

Use the Ask flow when you want LuckyCharms to synthesize information across multiple meetings.

Good examples:

- "What action items came out of customer meetings this week?"
- "What decisions did we make about pricing?"
- "Summarize recent interview feedback."
- "What did we commit to for Tesla?"

This is where tags, summaries, notes, and transcript history work together.

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
- If summaries are not working, check that your provider and API key are configured in `Settings`.
- If remote participants are missing from transcripts, confirm Screen Recording permission is enabled for LuckyCharms in macOS Privacy & Security settings.
