# Meeting Assistant — Engineering Take-Home

Build and deploy a Web meeting assistant that records or accepts audio, transcribes it, and turns it into useful meeting notes in Chinese and English.

This assignment is for **full-stack engineers and AI application engineers**. Product delivery, AI implementation quality, and engineering quality are equally important.

- **Suggested effort:** 1–2 hours. AI-assisted development is welcome.
- **Submission deadline:** within 2 days of receiving the assignment.
- **Partial submissions are welcome:** clearly explain unfinished features and your tradeoffs.

Preserve any co-author attribution your AI development tools automatically add to Git commits, such as `Co-authored-by` trailers.

## Core requirements

### 1. Audio input and transcription

- Support uploading existing audio files and recording through the browser microphone.
- Transcribe after recording stops. Displaying a live transcript during recording is not required.
- Support Mandarin Chinese, English, and mixed Chinese–English speech.
- Display the transcript and distinguish different speakers, for example, “Speaker 1” and “Speaker 2.”
- Find and process your own multi-speaker audio recording, approximately 90 minutes long. See [Test Audio](TEST_RECORDING.md).
- **Optional:** timestamps for individual utterances.

### 2. Meeting notes in Chinese and English

Generate **both Chinese and English versions** of:

- A brief summary.
- Main discussion topics.
- Confirmed decisions.
- Action items: the task, owner, and deadline, when mentioned in the recording.
- Unresolved questions.

Only include information supported by the recording. **If something was not mentioned, omit it. Do not let the AI invent missing content, owners, or deadlines.** Opinions, predictions, and proposals should retain their meaning rather than becoming confirmed decisions or commitments.

Let users manually edit the generated notes in either language. Changes to one language version must automatically update the other version.

### 3. Bilingual interface

The Web interface must let users switch between Chinese and English. The generated meeting notes must provide both language versions regardless of the selected interface language.

### 4. Access codes and meeting history

- No registration or login flow is required.
- **One access code represents one user.** Entering the same code on another device must retrieve that user’s meeting history.
- Save the original recordings, transcripts, and meeting notes, including edits.
- Support playing back saved recordings in the Web application.

The implementation and storage choices are yours.

## Bonus: real-time AI assistance

During a meeting, let the user ask questions or request ideas from an AI assistant that uses **what has already been discussed in the current meeting**.

The bonus feature should support:

- Both a spoken wake phrase and a button to activate the assistant.
- Both visible text and spoken audio for the assistant’s replies.
- Replies in the language of the user’s question.

This is a bonus feature, separate from the core requirement to transcribe after recording stops.

## Technology and AI services

Choose your own frontend and backend stack, speech models, language models, and APIs. **Explain why you selected the models and services you used.**

You are responsible for your own provider accounts, API keys, and usage costs. Keep API keys out of the repository and browser-exposed code.

Automated tests are not required.

## Test Audio

Find a **multi-speaker audio recording approximately 90 minutes long** and use the full recording to test your application. Include the **original audio file** with your submission, as an attachment or an accessible download link.

## How to submit

See [SUBMISSION.md](SUBMISSION.md). In short: click **"Use this template"** to create your own **private repo**, build and deploy your app, invite **`AIDevSkyVision`**, and email us your repo link, README, deployed app URL, access code, original test audio, and a **face-visible introduction video of no more than 2 minutes**.

Send your submission to [aidevelopment@skyvisioninsurance.com](mailto:aidevelopment@skyvisioninsurance.com). [Loom](https://www.loom.com/) is recommended for recording.

See [Evaluation Focus](EVALUATION.md) for what we look for.
