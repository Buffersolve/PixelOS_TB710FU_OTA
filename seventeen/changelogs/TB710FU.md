# TB710FU changelog

## PixelOS 17.0 - 20261025-1822

- StrongBox: the secure processor (SPU) services from the stock firmware are back,
  so apps get a hardware StrongBox keystore
- Key attestation works: keys the TEE cannot attest are attested in StrongBox,
  with the stock device IDs
- The certified props for Play Integrity are fetched again (system_server could
  not read the PixelOS version), and their Build.VERSION fields are applied
- Play Integrity still fails without root: Google does not pass this unlocked
  device even for BASIC

## PixelOS 17.0 - 20261025-1428

First public build. Signed with release keys: coming from another ROM or from
the stock firmware, flash the recovery from the same folder and format data.

- Android 17 (PixelOS), October 2026 security patch, stock ZUXOS 1.5.04.470 firmware and blobs
- OTA updates through the PixelOS Updater
- Microphone works for every app: voice recorders, video recording and voice search were silent
- Stock Lenovo thermal limits (skin temperature and charging) are applied
- Pixel Launcher: tapping the weather in At a Glance opens Pixel Weather; dock, taskbar and search bar animation fixes
- Flashlight tile is a plain on/off toggle (the LED has no brightness levels)
- Radio info is hidden from About tablet (Wi-Fi only device)
- Pen, keyboard, folio cover and double tap to wake
- zram swap
- Dolby Atmos (on/off; profiles and equalizer have little effect for now)
- No half-screen flicker at 144 Hz

Known issues:
- Dolby profiles and equalizer do not change the sound noticeably
- Play Integrity: no BASIC/DEVICE/STRONG without root
