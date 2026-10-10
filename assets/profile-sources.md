# Profile sources

Checked on 2026-10-10. The README remains one self-contained SVG. Source files are read for descriptions and branding; they are not executed.

## Design

The initial palette came from the dark tokens in [ThreadMap](https://github.com/xheavy0/Threadmap), `packages/viewer/src/styles.css`. The user subsequently requested livelier colors, so the current version uses deeper graphite, brighter coral and blue accents, and the colored Thread icon-system reference they supplied.

| Role | Color |
| --- | --- |
| App / sidebar | `#151715` / `#0d1211` |
| Card / sunken / raised | `#252b29` / `#191f1d` / `#303a35` |
| Strong / body / muted / faint text | `#faf9f5` / `#e8e6dc` / `#c2c0b6` / `#9c9a92` |
| Coral / cool highlight | `#ff9866` / `#78c9ed` |
| Spectrum glow | `#ff9866` / `#ffc489` / `#82dce5` / `#65afff` |
| Canvas dots | `#788b81` |

Fonts: Inter for body text, Source Serif 4 for headings, JetBrains Mono for annotations. The same self-hosted WOFF2 files used by ThreadMap are embedded in the SVG. Their OFL licenses are in `font-licenses/`. No external font requests are needed.

The existing card drawing style, technology-logo toolbox and 400 × 400 portrait size are retained. The portrait is now at x=584, y=83, lowered 15 pixels from the previous preview. Hero tags read GRC, Desktop & Mobile and Connected Tools. The HUD now has stronger coral/blue ambient light, a drifting background glow, travelling featured-card edge highlights, and a moving hero signal. All new motion respects reduced-motion preferences. Aegis GRC, Trellis, Aegis Helpdesk and Aegis Website now share the dedicated four-card **Security Tool Development** section. Thread tools follow in their own section: four featured apps and 17 additional projects. Thread Releases moves into that ecosystem, while Toolbox becomes a featured app. HUD circuits follow the regrouped sections. Reduced-motion handling is retained. The portrait source PNG is unchanged.

## Project inventory

All 18 current GitHub repositories whose names begin with Thread were inspected: Threadforge, Thread-Releases, ThreadToolbox, Threadmap, Threadshot, Threadbots, ThreadAccount, Threadplan, Threadstorage, ThreadVoice, Threadnote, ThreadforgeMobile, ThreadstorageIOS, ThreadstorageAndroid, ThreadOS, ThreadAura, ThreadCalendar and ThreadMail.

Added: ThreadToolbox, ThreadMap, ThreadAccount, ThreadBots, ThreadStorage Android, ThreadStorage iOS and Thread Releases. Local projects also added: ThreadLens, Threadspace Website and Threadforge's Stream Deck plugin. Existing ThreadSpace remains included.

Trellis is described only as a GRC project for a private company with development ongoing in parallel, based on the user's statement. `trellis-logo.svg` recreates the supplied reference as eight rounded diagonal bars; it contains no phone screenshot, company name or invented product features.

Threadplan now mentions Android and Windows; its README documents the Tauri Windows foundation. ThreadOS remains explicitly research/planning, with Debian 13 / Xfce rather than the previous KDE description. Threadforge Rust and Aegis-2 remain excluded as requested.

## Logos

The user supplied `ThreadSpace_Icon_System_Reference.png` after the repository audit and explicitly requested these new colored icons, excluding Aegis. That reference is now authoritative for matching Thread products. `thread-icon-system-reference.png` is a byte-for-byte project copy, SHA-256 `1ace78cf3d604c90df6832ea18e652089cb5ca417303afc46972cc6067444776`.

The SVG embeds the reference once and uses clipped SVG viewports for each icon. The original PNG is not cropped, resampled, repainted or otherwise edited. Labels and neighboring icons are excluded from the icon viewports. Aegis keeps its eagle asset, Trellis keeps its lattice mark, and the portrait keeps its grayscale filter. The supplied AEGIS tile is intentionally unused.

| Current project | Supplied icon |
| --- | --- |
| Threadforge / Mobile | TF orange-red / FM amber |
| Threadshot / Threadnote / Threadplan | TS pink-red / TN yellow / TP green |
| ThreadVoice / ThreadCalendar | TV purple / TC blue |
| ThreadMail / ThreadStorage including Android and iOS | TM blue / TS cyan |
| ThreadAura / Threadlendar Dock | TA purple / TL blue (ThreadLander tile) |
| ThreadToolbox / Thread Releases | TB orange (ThreadBox tile, shared with the download hub) |
| ThreadAccount / ThreadBots | TA pink (ThreadAccounts tile) / TB purple |
| ThreadMap / ThreadOS | TM amber-orange / TO teal |
| ThreadSpace / Threadspace Website | The silver T from the reference header |
| iOS Simulator | TS blue-purple from ThreadSim, mapped to the existing simulator card |

ThreadLens uses its current approved lilac **TL** master from `F:/coding/Github_Repos/ThreadLens/public/brand/threadlens.svg`, copied unchanged to `threadlens-logo.svg` and embedded with namespaced SVG IDs. Threadforge Stream Deck, AI Usage and WoW Control keep their existing marks because they have no matching tile in the supplied sheet. ThreadAlert and ThreadDiscovery are not added as projects: the sheet supplies icons but no project descriptions, and neither is part of the inspected project inventory.

### Repository assets used before the supplied branding

The prior audit below records the repository assets that were checked before the user's newer icon sheet superseded the matching Thread logos. The unlisted project marks above and Aegis still use their existing assets.

| Project | Asset |
| --- | --- |
| Aegis GRC / Helpdesk / Website | `public/aegis-eagle.png`; remote GRC, remote Helpdesk and local Website files have matching SHA-256 hashes |
| Threadforge | `public/threadforge-emblem.webp`, referenced by `APP_LOGO` |
| Threadforge Mobile | `app/src/main/res/drawable-nodpi/threadforge_logo.png` |
| Threadnote | 128px PNG in `resources/icon.ico`, generated from the same logo used by `BrandMark` |
| ThreadVoice | `src/renderer/logo-symbol.png`, referenced by its main and overlay interfaces |
| ThreadCalendar | `src/renderer/assets/calendar-logo.png`, the current renderer asset |
| Threadplan | 128px PNG in `src-tauri/icons/icon.ico`; current supplied calendar/ribbon logo validated for Android and Windows |
| ThreadMail | `public/app-icon.png`, identical to the active `app-logo.png` blob |
| ThreadStorage / Android / iOS | `src-tauri/icons/128x128.png`; all three checked trees share this branding asset |
| Threadshot | 128px PNG in `build/threadshot.ico`, generated from `build/threadshot-logo.png` |
| ThreadAura | `src-tauri/icons/128x128.png`, packaged from the current logo |
| ThreadSpace | Local `apps/threadspace-web/src/assets/threadspace-logo.png` |
| ThreadToolbox | `build/icon.png`, generated from the current `public/branding/toolbox.png` |
| ThreadAccount | 128px PNG in `public/assets/app-icon.ico`; the active app uses the matching PNG, rather than the placeholder SVG |
| ThreadBots | `src-tauri/icons/128x128.png`, generated from `src/assets/logo.png` |
| ThreadMap | `packages/desktop/build/icon.svg`; internal SVG IDs are namespaced |
| ThreadLens | Superseded magnifying-glass mark; now uses the approved lilac TL master documented above |
| Threadspace Website | The two crossed ellipses from `src/components/Brand.tsx` |
| Threadforge Stream Deck | `com.threadforge.streamdeck.sdPlugin/imgs/plugin.png`, referenced by its manifest |
| AI Usage / WoW Control | Existing embedded images match the current manifest category-icon PNGs byte-for-byte |
| Thread Releases | Uses the Toolbox catalog icon as a distribution-hub illustration, not a separate claimed application logo |

Threadlendar Dock and iOS Simulator now use the supplied ThreadLander and ThreadSim tiles. Their project names and descriptions remain unchanged. Aegis Website's remote repository is unavailable, so its local interface asset was checked instead.

The historical Phosphor MIT license is retained in `font-licenses/`; the profile now uses ThreadLens's branded TL master.

## Additional languages and scripting

The toolbox adds JavaScript, Rust, Kotlin, Go, Swift, Lua, Python and Bash, plus HTML and CSS. Java and TypeScript remain in the original row. Languages were checked against local application and support-script source; Python and Bash represent automation/deployment, while HTML and CSS represent web UI. No language was inferred from a dependency name or a downloaded library.

| Language / format | Evidence |
| --- | --- |
| JavaScript | `ThreadLens/server/index.mjs`; `ios-simulator-for-windows/electron/store.js` |
| Rust | `Threadstorage/src-tauri/src/settings.rs`; `ThreadAura/src-tauri/src/winrt.rs` |
| Kotlin | Threadforge Mobile `app/src/main`; Threadplan `modules/threadplan-system/android/src/main/java/com/threadplan/system/WidgetModel.kt` |
| Go | `ThreadstorageIOS/mobile-engine/peerclient/client.go`, also shared with Android |
| Swift | `ThreadstorageIOS/src-tauri/mobile-runtime/ios/Sources/ExamplePlugin.swift`, actual native storage/keychain/transfer implementation |
| Lua | `Elgato WOW Plugin/wow-addon/StreamDeckWoW/StreamDeckWoW.lua` |
| Python | `Threadforge/scripts/package-vscode.py`; `ThreadstorageIOS/scripts/verify-ios-ipa.py` |
| Bash | `Threadspace/scripts/backup-postgres.sh`; `cee-grc-tool/deploy/release.sh` |
| HTML / CSS | ThreadLens `index.html`, `src/styles.css`; Thread web interfaces |

The new colored tiles use the same [Skill Icons](https://github.com/tandpfun/skill-icons) family as the original technology row, read as SVG source from its official repository's `icons/` directory. They are embedded as data URLs, with no network requests when viewing the README. Its MIT license is at `font-licenses/skill-icons-MIT.txt`. Claude's starburst uses `#D97757`, matching the existing `Threadforge/public/providers/claude-color.svg` asset; its original outline is retained.
