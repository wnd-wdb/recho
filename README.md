Recho
====

A personal project of learning Java by forking the *Time travelling recorder for Android* **(echo)**.

Download the Original
---

* [F-Droid](https://f-droid.org/repository/browse/?fdid=eu.mrogalski.saidit)

Architecture
---

**SaidItFragment** the main view of the app.

**SaidItService** manages a high priority thread that records audio. The thread is a state machine that can be accessed by sending it tasks using Android's Handler (`audioHandler`).

**AudioMemory** (not thread-safe) manages the in-memory ring buffer of audio chunks.
