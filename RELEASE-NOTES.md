# SCE — Release Notes

Every release, newest first. Each links to its full notes below.

<a name="versions"></a>
## Versions

- **[2.1.1](#v2-1-1)** — 2026-11-15
  - Fixes a channel that could come out silent, and makes the plug-in report its delay and reset correctly in every host.

---

<a name="v2-1-1"></a>
## 2.1.1 — 2026-11-15

Fixes a channel that could come out silent, and makes the plug-in report its delay and reset correctly in every host.

### Fixes

- **First (left) channel silent.** In an offline export, or sometimes when the
  plug-in was opened in a DAW and played straight away, the first channel
  could come out silent while the others played. Every channel now has its
  settings before the host processes any audio.
- **Delay compensation at every sample rate.** The plug-in now reports its
  real delay for the session's sample rate, so the host lines it up with the
  other tracks at 88.2, 96 kHz and above, not only at 44.1/48 kHz.
- **Reset.** When the host resets the plug-in, it now starts clean, so a
  passage processed again (played back, or exported) comes out the same as
  the first time.

Everything else is as in 2.1.0.

[Back to the list of versions](#versions)

---
