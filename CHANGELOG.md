<!-- Keep a Changelog guide -> https://keepachangelog.com -->

# intellij-platform-plugin-open-in-cursor Changelog
# Open in Cursor Changelog

## [Unreleased]
### Changed
- Update IntelliJ platform version constraints in build.gradle.kts to support since build 243
- Update plugin.xml to set require-restart attribute to false

## [0.6.0] - 2026-04-27
### Added
- Initial scaffold created from [IntelliJ Platform Plugin Template](https://github.com/JetBrains/intellij-platform-plugin-template)
- `Cursor` action added under IDEA's standard **Open In** submenu (`RevealGroup`) — appears in the editor popup, editor tab popup, project view popup, and navigation-bar popup alongside "Reveal in Finder".
- Chained `cursor://` launch: project folder URL is fired first, then the file URL ~350 ms later, so the file lands in the correct Cursor window.
- Folder targets (project root, sub-directories) open via a single project URL with no line number.
- Cursor logo icon (16×16 with transparent background, plus `@2x` HiDPI variant) shown next to the `Cursor` action item.
