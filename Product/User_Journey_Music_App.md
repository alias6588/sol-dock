
**User Journey Map - Music Learning App**

---

# Introduction

This document outlines the user journey for a music learning application that allows users to take a photo of a sheet music, convert it into playable audio with adjustable tempo, and practice interactively with real-time feedback.

# User Role

**Student (Learner)**

# Main User Journey

## 1. App Launch

- Open the app.
- First-time setup: Choose language, allow microphone access.
- Log in or register (Email, Google, Apple ID).

## 2. Class Enrollment (Optional)

- Enter a class code provided by a teacher.
- Alternatively, browse and select from available practice exercises.

## 3. Capture Sheet Music

- Access the camera through the app.
- Take a photo of sheet music with guidelines for a good capture.

## 4. Image Processing

- System processes the photo.
- Display digitized sheet music.
- Allow user to adjust playback tempo before starting.

## 5. Practice with Real-time Feedback

- Press play to start practicing.
- Microphone listens to user's playing.
- Compare live pitch and rhythm to expected notes.

### Real-time Visual Feedback

| Execution Status                           | Feedback on Staff                  |
| ------------------------------------------ | ---------------------------------- |
| Wrong Note (Pitch error)                   | Note turns **Red**                 |
| Right Note but Timing Error (Rhythm error) | Note turns **Gray**                |
| Played too early                           | Gray speech bubble: **"Too fast"** |
| Played too late                            | Gray speech bubble: **"Too slow"** |
| Correct pitch and rhythm                   | Note remains **Normal color**      |

## 6. End of Practice

- Display session results:
  - Pitch Accuracy %
  - Rhythm Accuracy %
  - Overall Score
  - Highlight trouble areas.
- Suggest replay or proceed to next exercise.

## 7. (Optional) Submit to Teacher

- Send the recorded result or score to assigned teacher for grading and feedback.

## 8. Track Progress

- View completed exercises.
- Earn badges and achievements.
- Access teacher's assigned tasks if enrolled.

---

# Notes

- The app is designed to be **instrument-agnostic** and assumes users have **basic sheet music reading ability**.
