# Is Rust GUI ready?

Fun-made collection like [`areweguiyet`](https://areweguiyet.com/), but mainly for desktop application development.

If you dislike a quick glance, you can look deeper at
[this documentation](https://github.com/Chaoses-Ib/Rust/blob/main/Libraries/GUI/).

NOTE: unmaintained libraries are unconsidered.

## Stable

[gtk]: https://docs.rs/gtk/
[relm]: https://docs.rs/relm/
[gtk4]: https://docs.rs/gtk4/
[relm4]: https://docs.rs/relm4/

[FLTK]: https://fltk-rs.github.io/fltk-book/

[native-windows-gui]: https://gabdube.github.io/native-windows-gui/native-windows-docs/index.html
[cacao]: https://github.com/ryanmcgrath/cacao

[^1]: https://www.fltk.org/COPYING.php

| Crate                | License         | Backend      | Cross | Web |
| -------------------- | --------------- | ------------ | ----- | --- |
| [gtk], [relm]        | LGPLv2.1+       | GTK3         | Yes   | No  |
| [gtk4], [relm4]      | LGPLv2.1+       | GTK4         | Yes   | No  |
| [FLTK]               | LGPL[^1]        | --           | Yes   | No  |
| [native-windows-gui] | MIT             | Win32 API    | No    | --  |
| [cacao]              | MIT or MPL-2.0+ | Appkit/UIkit | No    | --  |

## Desktop-first

[egui]: https://www.egui.rs/
[iced]: https://iced.rs/
[slint]: https://slint.dev/
[gpui]: https://www.gpui.rs/
[Freya]: https://freyaui.dev/
[makepad]: https://makepad.dev/
[winio]: https://github.com/compio-rs/winio
[azul]: https://azul.rs/
[xilem]: https://github.com/linebender/xilem
[Ribir]: https://github.com/RibirX/Ribir

[^2]: https://github.com/slint-ui/slint?tab=License-1-ov-file#slint-license

| Crate     | License               | Backend                 | Cross | Web |
| --------- | --------------------- | ----------------------- | ----- | --- |
| [slint]   | GPL-3.0 or custom[^2] | --/GTK3                 | Yes   | Yes |
| [egui]    | Apache-2.0 or MIT     | winit                   | Yes   | Yes |
| [gpui]    | Apache-2.0            | --                      | Yes   | No  |
| [xilem]   | Apache-2.0            | --                      | Yes   | Yes |
| [iced]    | MIT                   | --                      | Yes   | No  |
| [Ribir]   | MIT                   | winit                   | Yes   | No  |
| [makepad] | MIT                   | --                      | Yes   | Yes |
| [Freya]   | MIT                   | --/GTK3                 | Yes   | No  |
| [azul]    | MIT                   | --                      | Yes   | No  |
| [winio]   | MIT                   | Win32/WinUI<br>GTK4/Qt6 | Yes   | No  |


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
[flutter_rust_bridge]: https://github.com/fzyzcjy/flutter_rust_bridge

| Crate                 | License           | Backend | Cross | Web | Mobile |
| --------------------- | ----------------- | ------- | ----- | --- | ------ |
| [imgui]               | Apache-2.0 or MIT | --      | Yes   | No  | No     |
| [libui-ng]            | Apache-2.0 or MIT | --/GTK3 | Yes   | No  | No     |
| [rinf]                | MIT / BSD-3       | Flutter | Yes   | Yes | Yes    |
| [flutter_rust_bridge] | MIT               | Flutter | Yes   | Yes | Yes    |


## Most mature cross-platform toolkits

[`gobley`]: https://github.com/gobley/gobley
[`slint`]: https://docs.rs/slint/
[`uniffi`]: https://github.com/jhugman/uniffi-bindgen-react-native

[kick]: https://github.com/bartwell/kick
[flutter-hot-reload]: https://docs.flutter.dev/tools/hot-reload
[rn-fast-refresh]: https://reactnative.dev/docs/fast-refresh
[slint-live-reload]: https://slint.dev/blog/slint-1.13-released
[kmp-hot-reload]: https://www.jetbrains.com/help/kotlin-multiplatform-dev/compose-hot-reload.html
[slint-a11y-issue]: https://github.com/slint-ui/slint/issues/2895

|                 Name |     Inspector      |         Hot Reload         |           Live Reload           |          a11y           | Bridge     |
| -------------------: | :----------------: | :------------------------: | :-----------------------------: | :---------------------: | :--------- |
|              flutter |        Best        | [Yes][flutter-hot-reload]  |               --                |           Yes           | See above  |
|         React Native |       Great        | [Limited][rn-fast-refresh] |               --                |           Yes           | [`uniffi`] |
| Kotlin Multiplatform | [Unofficial][kick] |   [Beta][kmp-hot-reload]   |               --                |           Yes           | [`gobley`] |
|                slint |       Basic        |             No             | [Since 1.13][slint-live-reload] | [WIP][slint-a11y-issue] | [`slint`]  |
