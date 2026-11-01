# Contributing

Issues and PRs are welcome on any of the repos. A few rules that apply everywhere:

**No vendor material.** Don't attach or commit firmware dumps, patched images, PAC files, FDL
loaders, DSP blobs, decompiled vendor code or anything from a vendor SDK. Addresses, register
values, hashes and your own notes are fine. If a bug needs a firmware file to reproduce, give
the hash of the file and the steps.

**No personal data.** Logs from a real phone can contain your IMEI, IMSI, phone number, cell
IDs, SMS text and contacts. Telegram logs can contain your account details and messages. Strip
them before posting, or post a minimal excerpt.

**Hardware testing.** Some of these tools write to flash or poke registers on a live phone. Say
in your PR what you tested on hardware and what only ran in the emulator. Never flash anything
without a backup of your own partitions first.

**Licences.** Our code is MIT unless the repo says otherwise. Linux kernel code in fplinux is
GPL-2.0-only. The Telegram code includes parts ported from TDLib (Boost Software Licence 1.0),
and its notice has to stay.
