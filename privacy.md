# Privacy Policy

_Last updated: 2026-04-20_

SwimStructuredWorkout is built around a simple promise: **your workouts never leave your device unless you choose to share them.**

## What we collect

**Nothing.** SwimStructuredWorkout does not collect, transmit, or store any personal information. We do not operate any backend servers, we do not use analytics SDKs, and we do not embed advertising or tracking frameworks.

## How your data is used

Everything happens on-device:

- **Workout text you paste** is parsed locally by an on-device language model. It is never sent to Anthropic, OpenAI, or any other third party.
- **The parsed workout** is held in memory while the app is open and discarded when you close it. Nothing is written to iCloud or any remote storage.
- **Pool length preference** is saved locally in `UserDefaults` and stays on your device.

## The on-device language model

The first time you tap "Load local LLM," the app downloads a Qwen 2.5 4-bit model (~1.8 GB) directly from Hugging Face's CDN to your device. After that download:

- The model lives in your device's app storage and runs entirely offline.
- All inference happens on your iPhone's Neural Engine / GPU. No prompts, no completions, and no parsed results ever leave the device.
- Hugging Face may log the initial model download as a normal HTTPS request (their privacy policy applies to that single request). We do not control or observe that log.

## Sharing your workouts

When you tap **Send to Apple Watch** or **.FIT**:

- Apple Watch export hands the workout to Apple's WorkoutKit framework. Apple's privacy policy governs how the workout is synced to your watch.
- `.FIT` export writes a file to a temporary location on your device and opens the standard iOS share sheet. You decide where it goes (AirDrop, Files, Garmin Connect, etc.). The destination app's privacy policy applies once you hand the file off.

We do not see, log, or transmit anything during these handoffs.

## Permissions

SwimStructuredWorkout does not request access to your location, contacts, photos, microphone, camera, HealthKit data, or notifications.

## Changes to this policy

If the app's data handling ever changes — for example, if we add an opt-in cloud sync feature — this document will be updated and the change will be called out in the app's release notes.

## Contact

Questions about this policy: nilssupport@gmail.com 
