# Evaluation Focus

[Assignment](README.md) · [Test Audio](TEST_RECORDING.md)

We give equal importance to the following three areas, considering the recommended **1–2 hours** of effort, the scope you deliver, and your tradeoffs. Incomplete submissions are welcome; explain the missing parts and tradeoffs in your submission.

### Product delivery

- The deployed web app is accessible by URL. Audio upload and browser microphone recording both lead through transcription, note generation, and result review.
- The Chinese/English UI switch, simultaneous bilingual notes, and automatic synchronization after editing either language form a coherent, usable experience.
- One access code represents one user and retrieves all their historical meetings across devices. Original audio is saved and playable, alongside saved transcripts and notes.
- GitHub source and run instructions make the implementation accessible and understandable.

### AI implementation quality

- Transcription handles Mandarin, English, and mixed speech, with different speakers distinguished. Processing after recording stops is sufficient; timestamps are optional.
- Notes accurately capture a brief summary, main discussion, confirmed decisions, action items, and open questions. Action tasks, owners, and deadlines must be supported by the recording. Omit unsupported categories, items, and fields without placeholders or invented details.
- Both note languages convey the same meaning, and synchronization preserves the intent of manual edits. Explain your model selection and its suitability.

### Engineering quality

- Code is understandable, and technical choices suit the delivered scope. Recording, model calls, saved data, and bilingual synchronization work together sensibly.
- Handling of access codes, API keys, and meeting data demonstrates sound engineering judgment.
- Configuration and run instructions work, with important limitations and incomplete parts explained. **Automated tests are not required.**

### Optional real-time assistant

If implemented, we look at whether it helps using the meeting discussion so far, supports both a wake phrase and a button, provides both text and spoken replies, and follows the question's language. Keep assistant suggestions distinguishable from decisions confirmed by participants.
