# SwimStructuredWorkout — Support

Thanks for using SwimStructuredWorkout! This page covers the most common questions and how to get in touch if you need help.

## Contact

**Email:** [nilssupport@gmail.com](mailto:nilssupport@gmail.com)

I read every message and try to respond within a few days. When you write in, please include:

- Your iPhone model and iOS version (Settings → General → About)
- The app version (Settings → SwimStructuredWorkout)
- A short description of what you were doing and what went wrong
- If a workout parsed incorrectly, the exact text you pasted

The more I can reproduce, the faster I can fix.

## Frequently asked

### Why does the app need to download ~1.8 GB the first time?

SwimStructuredWorkout uses a local language model (Qwen 2.5) to interpret coach-written workout text. The model lives entirely on your device so your workouts stay private. The download only happens once; after that the app works fully offline.

### Where do my workouts go?

Nowhere unless you send them. Parsing is on-device. When you tap **Send to Apple Watch** or **.FIT**, the workout is handed to Apple's WorkoutKit or saved as a file you can share via AirDrop, Files, Garmin Connect, etc. Nothing is uploaded to a server we control.

See the [Privacy Policy](./privacy.md) for the full picture.

### A workout parsed incorrectly. What should I do?

Tap any row in the preview to edit it directly — every interval is one tap away from the editor. You can also rename or reorder blocks with the `⋯` menu on each section header.

If a particular coach format trips up the parser repeatedly, please email me the raw text so I can improve the parser.

### Can I export to Garmin?

Yes — tap **.FIT** in the preview, then choose how to share the file. Garmin's mobile share extension currently imports `.FIT` files as activities rather than structured workouts; the most reliable way to get a structured workout onto a Garmin watch is to upload the `.FIT` file via [Garmin Connect on the web](https://connect.garmin.com).

### The model says "Failed to load." What now?

Most failures are caused by low device storage or a flaky network during the initial model download. Try:

1. Free up at least 3 GB on your device.
2. Switch to Wi-Fi.
3. Force-quit the app and tap **Load local LLM** again.

If it still fails, email me with your device model and iOS version.

### Does the app collect analytics or crash data?

No. There are no analytics SDKs, no advertising frameworks, and no crash reporters embedded in the app.

## Feature requests and feedback

I'd love to hear what would make the app more useful for your training. Email **[nilssupport@gmail.com](mailto:nilssupport@gmail.com)** with the subject line "Feature request" and a sentence or two on what you'd like to see.
