# Devices

| Phone | SoC | OS | Status |
|---|---|---|---|
| Ruio F286 | Unisoc UMS9117 (T107) | MocorOS | Main target. Everything in this org was developed on it. |
| Nokia 3210 (TA-1618) | Unisoc T107 | MocorOS | Not run on. Its mmi_app build keeps trace strings ours strips, so it was used as a reference for naming functions. |

Addresses in mocor-sdk and mocor-emu are for one specific F286 firmware build. The patcher checks
the hash of your dump and refuses to touch anything else. A different build or a sibling phone
will need its own address table; the method for finding the addresses is written up in
[ruio-f286](https://github.com/openfeaturephone/ruio-f286).

If you get something working on another phone, a PR adding a row here is welcome. Please say
which firmware build you have (the hash of mmi_app is enough) and what you tested.
