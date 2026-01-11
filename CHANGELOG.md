# Changelog

All notable changes to MetaPhotoAI will be documented in this file.

## [3.0.15] - 2025-01-11

### Added
- User Guide: Interactive standalone window with collapsible sidebar, image/video support, and detailed pricing information
- User Guide: Button in header bar for quick access
- Category Override: Folder-level category override functionality with improved UI and multi-language support
- System Prompt Selector: New selector in folder settings with improved layout
- Metadata Templates: Apply mode with 'all' and 'positive-only' options
- Workflow: Notification method options for workflow completion
- Workflow: Duplicate workflow functionality and execution scope settings
- FTP Settings: Duplicate host action button with improved visibility
- FTP Settings: Enhanced delete host functionality with danger action button
- Video Files: Automatic detection to skip unsupported metadata operations
- Auto-write Verification: Stats display and UI updates
- Thumbnail Processing: Status indicators and error handling
- Error Handling: Centralized showErrorToast utility for consistent error notifications
- Metadata Panel: "No changes to save" message and improved save button tooltip
- Localization: Metadata verification translations

### Changed
- Filters: Enhanced dropdown UI with sections and improved layout
- Logging: Increased default log line count to 2500 for better debugging
- Logging: Changed logger level from info to debug for onboarding events and thumbnail processing
- Styling: Window controls hover background now uses selection color variable
- Performance: Optimized useAppStore access in callbacks to prevent duplicate event listeners

### Fixed
- Preview: Submenu positioning in context menu for better alignment
- Verification: Count discrepancy resolved
- EXIF: Prevented category batch EXIF writes for video files
- Image Processing: Skip failed/rejected items when processing video files

## [3.0.14] - 2025-01-04

### Added
- FTP: Duplicate host functionality to easily clone FTP/SFTP configurations
- Categories: Shutterstock video categories support with improved media type handling
- Search: Helper text field for searching images by helper text content
- Filters: Helper text filters in the BottomToolbar for filtering by helper text status
- Filmstrip: Enhanced tooltip to display video-specific metadata (duration, resolution, codec)
- Filmstrip: Improved metadata tooltip visibility logic accounting for context menu and color tag picker

### Changed
- Menu: "Check for Updates" action now handled by renderer for better UX feedback
- Localization: Updated Ollama model reference from gemma3:12b to gemma3:4b

### Removed
- Skip options functionality and related hooks from BottomToolbar

## [3.0.13] - 2025-01-04

- Initial release

---

[3.0.15]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.15
[3.0.14]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.14
[3.0.13]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.13
