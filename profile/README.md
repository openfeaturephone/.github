## openfeaturephone

Tools and notes for cheap Unisoc feature phones, starting with the Ruio F286 (UMS9117, MocorOS).
Most of it came out of trying to get Linux running properly on that phone, which meant first
working out how the stock firmware drives the hardware.

What's here:

- [mocor-sdk](https://github.com/openfeaturephone/mocor-sdk): run your own native apps on stock
  MocorOS. A patcher for your own mmi_app dump, the API headers and some example apps.
- [f286dbg](https://github.com/openfeaturephone/f286dbg): a debug agent that runs on the phone
  and a PC client. Read and write memory, call firmware functions, move files, take screenshots
  over USB.
- [mocor-emu](https://github.com/openfeaturephone/mocor-emu): a Unicorn-based emulator that boots
  a stock MocorOS dump to the idle screen and runs apps against it.
- [tinymtproto](https://github.com/openfeaturephone/tinymtproto): a small Telegram (MTProto 2.0)
  client library in C. No libc, fits in about 128 KB of RAM.
- [f286-telegram](https://github.com/openfeaturephone/f286-telegram): the Telegram app for the
  F286, built on tinymtproto.
- [ruio-f286](https://github.com/openfeaturephone/ruio-f286): everything we know about the phone.
  Memory map, boot chain, flashing, firmware format, API addresses.

None of the repos contain vendor firmware. Where a tool needs firmware it expects a dump from
your own phone.

If you have a different MocorOS phone and want to try any of this, open an issue with the model
and chipset. See [DEVICES.md](https://github.com/openfeaturephone/.github/blob/main/DEVICES.md)
for what's been tried so far.
