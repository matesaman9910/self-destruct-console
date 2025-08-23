# LCARS Self-Destruct Console

A Star Trek–inspired **LCARS self-destruct control console**.  
Built with **Firebase Realtime Database** backend (EU region) and **GitHub Pages** frontend.

### Features
- **Countdown view (public)** with voice alarms, sounds, event log.
- **Control view (restricted)** with:
  - Operator PIN (one-time set, cannot be changed).
  - Two-officer authorization (names + secret PINs, stored hashed).
  - Arming, countdown, abort (T-15 lockout), reset.
- **Firebase connectivity watchdog** — if the system is offline, a red banner displays.
- Production hardened:
  - PIN and officer setup can only be done once.
  - Officer data never displayed after setup.
  - Abort disabled within the last 15s before detonation.
