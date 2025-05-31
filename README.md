# Is Rust GUI ready?

Fun-made collection like [`areweguiyet`](https://areweguiyet.com/), but mainly for desktop application development.

## Stable

[gtk]: https://docs.rs/gtk/
[relm]: https://docs.rs/relm/
[gtk4]: https://docs.rs/gtk4/
[relm4]: https://docs.rs/relm4/

[^1]: https://www.fltk.org/COPYING.php

[FLTK]: https://fltk-rs.github.io/fltk-book/

| Crate           | License   | Backend | Windows | MacOS | Linux | Web |
| --------------- | --------- | ------- | ------- | ----- | ----- | --- |
| [gtk], [relm]   | LGPLv2.1+ | GTK3    | Yes     | Yes   | Yes   | No  |
| [gtk4], [relm4] | LGPLv2.1+ | GTK4    | Yes     | Yes   | Yes   | No  |
| [FLTK]          | LGPL[^1]  | --      | Yes     | Yes   | Yes   | No  |

## Pure-Rust

[egui]: https://www.egui.rs/
[iced]: https://iced.rs/
[slint]: https://slint.dev/
[native-windows-gui]: https://gabdube.github.io/native-windows-gui/native-windows-docs/index.html
[cacao]: https://github.com/ryanmcgrath/cacao
[gpui]: https://www.gpui.rs/
[Freya]: https://freyaui.dev/
[makepad]: https://makepad.dev/
[winio]: https://github.com/compio-rs/winio

[^2]: https://github.com/slint-ui/slint?tab=License-1-ov-file#slint-license

| Crate                | License               | Backend      | Windows | MacOS | Linux | Web |
| -------------------- | --------------------- | ------------ | ------- | ----- | ----- | --- |
| [slint]              | GPL-3.0 or custom[^2] | --/GTK3      | Yes     | Yes   | Yes   | Yes |
| [egui]               | Apache-2.0 or MIT     | Glow/GTK3    | Yes     | Yes   | Yes   | Yes |
| [iced]               | MIT                   | --           | Yes     | Yes   | Yes   | No  |
| [gpui]               | Apcache-2.0           | --           | Yes     | Yes   | Yes   | No  |
| [Freya]              | MIT                   | --/GTK3      | Yes     | Yes   | Yes   | No  |
| [makepad]            | MIT                   | --           | Yes     | Yes   | Yes   | Yes |
| [native-windows-gui] | MIT                   | Win32 API    | Yes     | --    | --    | --  |
| [cacao]              | MIT or MPL-2.0+       | Appkit/UIkit | --      | Yes   | --    | --  |
| [winio] (WIP)        | MIT                   | --/GTK4/Qt6  | Yes     | Yes   | Yes   | No  |

## Other

[imgui]: https://docs.rs/imgui
[libui-ng]: https://github.com/libui-rs/libui

| Crate      | License           | Backend | Windows | MacOS | Linux | Web |
| ---------- | ----------------- | ------- | ------- | ----- | ----- | --- |
| [imgui]    | MIT or Apache-2.0 | --      | Yes     | Yes   | Yes   | No  |
| [libui-ng] | MIT or Apache-2.0 | --/GTK3 | Yes     | Yes   | Yes   | No  |