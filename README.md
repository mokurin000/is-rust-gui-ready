# Is Rust GUI ready?

Fun-made collection like [`areweguiyet`](https://areweguiyet.com/), but mainly for desktop application development.

NOTE: unmaintained libraries are unconsidered.

## Stable

[gtk]: https://docs.rs/gtk/
[relm]: https://docs.rs/relm/
[gtk4]: https://docs.rs/gtk4/
[relm4]: https://docs.rs/relm4/

[^1]: https://www.fltk.org/COPYING.php

[FLTK]: https://fltk-rs.github.io/fltk-book/

| Crate           | License   | Backend | Cross | Web |
| --------------- | --------- | ------- | ----- | --- |
| [gtk], [relm]   | LGPLv2.1+ | GTK3    | Yes   | No  |
| [gtk4], [relm4] | LGPLv2.1+ | GTK4    | Yes   | No  |
| [FLTK]          | LGPL[^1]  | --      | Yes   | No  |

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
[azul]: https://azul.rs/
[xilem]: https://github.com/linebender/xilem

[^2]: https://github.com/slint-ui/slint?tab=License-1-ov-file#slint-license

| Crate                | License               | Backend      | Cross | Web |
| -------------------- | --------------------- | ------------ | ----- | --- |
| [slint]              | GPL-3.0 or custom[^2] | --/GTK3      | Yes   | Yes |
| [egui]               | Apache-2.0 or MIT     | Glow/GTK3    | Yes   | Yes |
| [gpui]               | Apache-2.0            | --           | Yes   | No  |
| [xilem]              | Apache-2.0            | --           | Yes   | Yes |
| [iced]               | MIT                   | --           | Yes   | No  |
| [makepad]            | MIT                   | --           | Yes   | Yes |
| [azul]               | MIT                   | --           | Yes   | No  |
| [Freya]              | MIT                   | --/GTK3      | Yes   | No  |
| [winio] (WIP)        | MIT                   | --/GTK4/Qt6  | Yes   | No  |
| [native-windows-gui] | MIT                   | Win32 API    | No    | --  |
| [cacao]              | MIT or MPL-2.0+       | Appkit/UIkit | No    | --  |

## Webview-based

[tauri]: https://tauri.app/
[dioxus]: https://dioxuslabs.com/
[sciter]: https://sciter.com/
[async-ui]: https://github.com/wishawa/async_ui

[^3]: https://sciter.com/prices/

| Crate      | License              | Mobile |
| ---------- | -------------------- | ------ |
| [tauri]    | Apacha-2.0 or MIT    | Yes    |
| [dioxus]   | Apacha-2.0 or MIT    | Yes    |
| [sciter]   | Freeware or Paid[^3] | No     |
| [async-ui] | MPL-2.0              | No     |

## Other

[imgui]: https://docs.rs/imgui
[libui-ng]: https://github.com/libui-rs/libui
[rinf]: https://github.com/cunarist/rinf

| Crate      | License           | Backend | Cross | Web | Mobile |
| ---------- | ----------------- | ------- | ----- | --- | ------ |
| [imgui]    | Apache-2.0 or MIT | --      | Yes   | No  | No     |
| [libui-ng] | Apache-2.0 or MIT | --/GTK3 | Yes   | No  | No     |
| [rinf]     | MIT / BSD-3       | Flutter | Yes   | Yes | Yes    |
