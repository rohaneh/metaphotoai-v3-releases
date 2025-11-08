# Changelog

All notable changes to MetaPhotoAI will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- Auto-update system with GitHub Releases
- Background update downloads
- User-controlled update installation

### Changed
- Improved update notification UI

### Fixed
- Various bug fixes and performance improvements

## [3.0.0] - 2024-01-XX

### Added
- Initial public release
- AI-powered metadata generation
- Batch processing support
- Multi-platform export (EXIF, CSV, FTP)
- Folder-based organization
- Custom metadata templates
- Advanced filtering and search
- Device activation system
- Secure credential storage
- Real-time notification system

### Features

#### Core Functionality
- Generate titles, descriptions, keywords, and categories using AI
- Process multiple images simultaneously
- Background processing with progress tracking
- Resume interrupted batches

#### Export Options
- Write metadata to EXIF tags
- Export to CSV with customizable templates
- Direct FTP/SFTP upload to stock agencies
- Platform-specific formatting (Adobe Stock, Shutterstock, Getty, etc.)

#### Workflow Tools
- Per-folder settings overrides
- Editorial vs. commercial content handling
- Color tagging for organization
- Helper text for context-specific generation
- Custom metadata templates
- Find and replace across metadata fields

#### Platform Support
- macOS (Universal binary - Intel & Apple Silicon)
- Windows (64-bit)
- Linux (AppImage)

---

## Version History

### Understanding Version Numbers

MetaPhotoAI follows [Semantic Versioning](https://semver.org/):
- **Major (X.0.0)** - Breaking changes, major overhauls
- **Minor (3.X.0)** - New features, non-breaking changes
- **Patch (3.0.X)** - Bug fixes, minor improvements

### How to Update

MetaPhotoAI includes automatic updates:
1. The app checks for updates on startup
2. Downloads updates in the background
3. Notifies you when ready to install
4. Installs on next app restart (or immediately if you choose)

You can also manually check: **Help → Check for Updates**

---

[Unreleased]: https://github.com/rohaneh/metaphotoai-v3-releases/compare/v3.0.0...HEAD
[3.0.0]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.0
