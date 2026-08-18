# License — Teslatlas

## This Project

Teslatlas is **proprietary software** owned by Magrathean UK Ltd.

> See [`LICENSE`](./LICENSE) for the full proprietary licence text.
> Copyright © 2026 Magrathean UK Ltd. All rights reserved.

This file (`license.md`) is the **third-party notice and component inventory** for Teslatlas. It does not grant any licence to the Teslatlas source itself; the Teslatlas source is governed exclusively by [`LICENSE`](./LICENSE).

---

## TeslaMate interoperability

TeslaMate is a separate open-source project maintained by its community. We
appreciate the work of its maintainers and contributors.

TeslaMate is not a bundled Teslatlas component or dependency. Teslatlas does not
copy, contain, modify, or redistribute TeslaMate. It interoperates with a
separately installed, user-controlled source through read-only access and stores
an independent on-device mirror. References to TeslaMate are descriptive
compatibility notices.

> This project is an unofficial community tool and is not affiliated with, endorsed by, or supported by the official TeslaMate project.

- [Official TeslaMate project](https://github.com/teslamate-org/teslamate)
- [Official documentation](https://docs.teslamate.org/)
- [AGPLv3 licence](https://github.com/teslamate-org/teslamate/blob/main/LICENSE)
- [Trademark policy](https://github.com/teslamate-org/teslamate/blob/main/TRADEMARK.md)

---

## Third-Party Dependencies

### Rust core — `teslatlas-core/Cargo.toml`

| Package | License | Declared in |
|---------|---------|-------------|
| `tokio` | MIT | `teslatlas-core/Cargo.toml` |
| `futures-util` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `tokio-postgres` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `postgres-native-tls` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` (optional) |
| `native-tls` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` (optional) |
| `rusqlite` (bundled SQLite) | MIT + Public Domain (SQLite) | `teslatlas-core/Cargo.toml` |
| `r2d2` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `serde` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `serde_json` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `chrono` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `chrono-tz` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `trtz` | **MPL-2.0** | `teslatlas-core/Cargo.toml` |
| `thiserror` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `libc` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `log` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` |
| `proptest` | MIT OR Apache-2.0 | `teslatlas-core/Cargo.toml` (development only) |

> **⚠ MPL-2.0 notice:** `trtz` is licensed under the Mozilla Public License 2.0.
> MPL-2.0 is a file-level copyleft licence; modifications to `trtz`'s own source
> files must be released under MPL-2.0. Code that merely calls `trtz` as a library is
> not required to be MPL-2.0. Binary redistribution must include the MPL-2.0 licence
> text and source offers per section 3.2.

> **SQLite note:** `rusqlite` is compiled with the `bundled` feature, which embeds the
> SQLite amalgamation. SQLite itself is in the **public domain** with no licence
> obligations; the `rusqlite` Rust bindings are MIT.

### Swift application — `Teslatlas.xcodeproj`

The Swift app layer uses Apple system frameworks only (MapKit, CoreLocation, etc.)
under the Apple SDK licence agreement. No external SPM dependencies are declared.

---

## License Obligations Summary

| License | Action required on redistribution |
|---------|-----------------------------------|
| MIT | Retain copyright notice and licence text |
| Apache-2.0 | Retain NOTICE file (if any) and licence text |
| MPL-2.0 | Include MPL-2.0 text; offer source of any modified MPL files |
| Public Domain (SQLite) | No obligation |
