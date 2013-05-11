## Purpose

This package provides configuration for uim(-vi).

This package should be used with the package `uim-vi-xtelex` from `TheSLinux`.

## Target users

* Telex users (VNI users need a [minor changes](#vni-users))
* Users who often type English and Vietnamese in the same documentation
* Traditional Vietnamese users who want `hòa` not `hoà`

## Installation

Replace your directory `~/.uim.d/` with the directory `./uim.d/`
that is in this repository. Please make a backup of your data first.

## Profile details

* Enabled IMs: `XTelex`, `XVNI`
* Default IM: direct input
* Available IMs: `XTelex`, `XVNI`, `m17n-vi-{telex,vni,tcvn}`, ...
  (ther are also the `-IPA` versions, for example,
    `XTelex-IPA`, `m17n-vi-telex-IPA`, `XNI-IPA`, ...)
* Hotkeys:
  * Switch between IMs (`xtelex`, `xvni`): `^ Alt \`
  * Toggle between current and direct input: `^ Alt Space`
  * Toggle state of the current IM: `Super Escape`
  * Commit a state : `^ Return`
  * Undo the last state: `Backspace`
* UIM settings:
  * Candidate window: disable by default
  * m17n IMs: default state is `on`
  * Generic IMs: default state is `on`

## VNI Users

This profile can be used by `VNI` users with a minor change. The key
is to change the order of enabled `IM`s and put `XVNI` on the top of the
list. To do that, please run the program `uim-setup`, and

* Go to `Global settings`
* Go to `Edit enabled input methods`
* Select `XVNI` and select the up arrow to move it to the top of the list
* After you can see `XVNI` on the top of the list of enabled IMS, select `Close`
* Select `Apply` to update the settings, and select `OK` to exit.

In the future we possibly provide a tool to do the above steps from
a single command.

## Documentation. Support

The following documentations are in Vietnamese

* http://theslinux.org/doc/uim-vi/vim/
* http://theslinux.org/doc/uim-vi/woman/

## Author

Ky-Anh Huynh

## License

GPL version 2.
