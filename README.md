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
[wxDragon]: https://github.com/AllenDang/wxDragon/

[native-windows-gui]: https://gabdube.github.io/native-windows-gui/native-windows-docs/index.html
[cacao]: https://github.com/ryanmcgrath/cacao

[^1]: https://www.fltk.org/COPYING.php

| Crate                | License           | Backend      | Cross | a11y       |
| -------------------- | ----------------- | ------------ | ----- | ---------- |
| [gtk], [relm]        | LGPLv2.1+         | GTK3         | Yes   | Linux-only |
| [gtk4], [relm4]      | LGPLv2.1+         | GTK4         | Yes   | Yes        |
| [FLTK]               | LGPL[^1]          | --           | Yes   | Yes        |
| [wxDragon]           | Apache-2.0 or MIT | wxWidgets    | Yes   | Yes        |
| [native-windows-gui] | MIT               | Win32 API    | No    | Yes        |
| [cacao]              | MIT or MPL-2.0+   | Appkit/UIkit | No    | Yes        |

## Desktop-first

[egui]: https://www.egui.rs/
[iced]: https://iced.rs/
[slint]: https://slint.dev/
[gpui]: https://www.gpui.rs/
[Freya]: https://freyaui.dev/
[winio]: https://github.com/compio-rs/winio
[xilem]: https://github.com/linebender/xilem
[Ribir]: https://github.com/RibirX/Ribir
[Floem]: https://lap.dev/floem/
[vizia]: https://github.com/vizia/vizia/
[agg-gui]: https://github.com/larsbrubaker/agg-gui
[mirui]: https://github.com/W-Mai/mirui
[wabou]: https://github.com/SunDoge/wabou
[rosin]: https://github.com/sailbrush/rosin

[^2]: https://github.com/slint-ui/slint?tab=License-1-ov-file#slint-license
[^3]: https://github.com/lapce/winit
[^4]: https://github.com/vizia/vizia/tree/main/crates/vizia_winit
[^5]: https://github.com/RibirX/Ribir#support-platform
[^6]: https://github.com/iced-rs/iced/issues/302
[^7]: https://github.com/lapce/floem/issues/619#issuecomment-2408729839
[^8]: https://github.com/zed-industries/zed/issues/12039#issuecomment-2119357583
[^9]: https://github.com/compio-rs/winio#platform-support

| Crate     | License               | Backend    | Mobile  | Web | a11y  |
| --------- | --------------------- | ---------- | ------- | --- | ----- |
| [slint]   | GPL-3.0 or custom[^2] | --/GTK3    | Yes     | Yes | Yes   |
| [egui]    | Apache-2.0 or MIT     | winit      | Yes     | Yes | Yes   |
| [rosin]   | Apache-2.0 or MIT     | AppKit     | No      | No  | Yes   |
| [xilem]   | Apache-2.0            | winit      | Yes     | Yes | Yes   |
| [wabou]   | Apache-2.0            | winit      | No      | No  | Yes   |
| [gpui]    | Apache-2.0            | --         | No[^8]  | No  | No    |
| [iced]    | MIT                   | --         | WIP[^6] | No  | No    |
| [mirui]   | MIT                   | SDL2/embed | No      | WIP | No    |
| [agg-gui] | MIT                   | winit      | No      | Yes | No    |
| [Ribir]   | MIT                   | winit      | WIP[^5] | No  | No    |
| [Floem]   | MIT                   | winit*[^3] | WIP[^7] | No  | No    |
| [vizia]   | MIT                   | winit*[^4] | No      | No  | Crash |
| [Freya]   | MIT                   | --/GTK3    | Yes     | No  | No    |
| [winio]   | MIT                   | native[^9] | Yes     | No  | Yes   |


## Webview-based

[tauri]: https://tauri.app/
[dioxus]: https://dioxuslabs.com/
[sciter]: https://sciter.com/
[async-ui]: https://github.com/wishawa/async_ui

[^9]: https://sciter.com/prices/

| Crate      | License              | Mobile |
| ---------- | -------------------- | ------ |
| [tauri]    | Apacha-2.0 or MIT    | Yes    |
| [dioxus]   | Apacha-2.0 or MIT    | Yes    |
| [sciter]   | Freeware or Paid[^9] | No     |
| [async-ui] | MPL-2.0              | No     |

## Web Apps

[leptos]: https://github.com/leptos-rs/leptos
[MoonZoon]: https://github.com/MoonZoon/MoonZoon
[sycamore]: https://github.com/sycamore-rs/sycamore

|   Crate    | License |
| :--------: | :-----: |
|  [leptos]  |   MIT   |
| [MoonZoon] |   MIT   |
| [sycamore] |   MIT   |


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


## Note

### Slint

In Android, with some Chinese OEM fonts.xml and system fonts,
parley may insufficiently handle glyth fallback, resulting tofu
for some CJK characters.

What make it even worse, slint does not support custom fonts in non-software renderer, while the software renderer is
not available to the `android-activity` backend.

To workaround this, **before** the slint initialization, hack [`shared_collection`](https://docs.rs/slint/latest/slint/fontique_010/fn.shared_collection.html).
