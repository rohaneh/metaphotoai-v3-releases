# Changelog

All notable changes to MetaPhotoAI will be documented in this file.

## [3.0.19] - 2026-03-07

### Added
- Similarity Detection: Perceptual hash (pHash) processing to detect similar and duplicate images
- Cross-Device Sync: Sync settings and data across devices with background sync and conflict resolution UI
- Image Moving: Drag-and-drop support to move images between folders
- Keyboard Shortcuts: New shortcut engine with chord bindings, command bus, and shortcut hints on buttons and dialogs
- What's New Modal: In-app version changelog with collapsible version groups shown automatically after updates
- CSV Export: Export selected metadata templates to CSV
- Live Credits: Real-time credit balance display and management in the UI
- Resizable Left Panel: Drag to resize the sidebar with state persistence
- Background Task Indicator: Status tracking and UI indicator for background operations
- History Tab: Image generation and upscale history tracking with cache-first loading and cross-device name resolution
- Copy Metadata from History: Copy and restore metadata directly from history items
- Email Privacy: Toggle to mask email address in the user menu
- Confirmation Prompts: Configurable confirmation dialogs for metadata generation and save actions
- Upscale History: Detailed upscale job tracking with folder path and device information

### Changed
- Batch Processing: Faster category endpoint with configurable concurrent sub-batch processing
- Right Panel: Increased minimum and default width to 530px for better metadata visibility
- Metadata Panel: Improved copyright display with clickable elements
- Video Speed Selector: Refactored to dropdown for cleaner UI
- Filmstrip & Thumbnails: Enhanced scrollbar visibility on hover
- Sidebar: Improved button visibility and interaction states
- Bottom Toolbar: Enhanced button disable logic for empty folders
- Preview Pane: Dynamic media styling and video play button workaround
- Performance: Speculative prefetching for metadata loading and non-blocking cache setup
- Localization: Added translations for similarity detection, history, sync, confirmation prompts, and queue labels across all supported languages

### Fixed
- Layout: Disabled hover effects and transitions on panels during resize to prevent layout thrashing
- Reconciliation: Improved category request filtering and not-found retry management
- Metadata Panel: Fixed null check for primary editing image in selection metadata map
- Keyboard: Prevented metadata generation trigger for single video images

## [3.0.18] - 2026-02-26

### Added
- Image Upscaling: Standalone 4x upscaling via Runware.ai Real-ESRGAN with context menu integration
- Image Upscaling: Progress indicators in Filmstrip and Thumbnail Grid views
- Image Upscaling: Format validation (JPG, PNG, WEBP) and size limit enforcement
- Inline Metadata Suggestions: AI-powered suggestions for title, description, and keywords within the metadata panel
- Spellcheck: Built-in spellcheck with context menu integration and keyword suggestions
- Spellcheck: Dictionary support and keyboard navigation for suggestions
- Metadata Versioning: Full edit history tracking with version restore capability
- Metadata Versioning: Restore from context menu across all view components
- System Prompts: Custom system prompts for AI metadata generation with per-folder assignment
- Copyright Management: Configurable copyright text, creator, business, and date source in global and folder settings
- Copyright Management: Automatic copyright application during metadata write
- Import Embedded Metadata: Auto-import IPTC/XMP metadata from image files on add, with toggle in General Settings
- Multi-Select Metadata Editing: Edit title, description, keywords, and categories across multiple selected images
- Multi-Select Metadata Editing: Mixed-value indicators and keyword merge/replace toggle
- Keyword Drag-and-Drop: Reorder keywords by dragging within the keywords field
- FTP Quick Upload: One-click upload to selected FTP/SFTP host from the bottom toolbar
- FTP Hosts: Preset configurations for Alamy, Deposit Photos, and Pond5
- Activity Queue Tab: Consolidated queue view for FTP, workflow, EXIF, and batch operations
- Image Info Tab: Multi-selection summary with aggregated information display
- Onboarding: Enhanced steps with detailed descriptions and CSV export step

### Changed
- Metadata Tab: Refactored tab management with consolidated queue handling into single Activity Queue Tab
- Sidebar: Improved header action button visibility on hover and focus
- Root Directories: Deduplication and upsert logic for adding folders
- Root Directories: Enhanced folder name extraction and validation
- Tooltips: Improved TooltipBubble positioning and rendering logic
- Dialogs: Added auxiliary button support and improved image switching confirmation flow
- Image Switching: Improved pending state handling with layout effects
- Background Previews: Paged sweep for directory images for better performance
- Error Messages: User-friendly error formatting across batch processors
- Character Limits: Helper text and prompt limits increased to 1000 characters
- Processing: OpenRouter processing enabled by default
- Localization: Added translations for upscale, spellcheck, metadata versioning, copyright, system prompts, and multi-select features across all 12 languages

### Fixed
- Metadata History: Corrected version count display logic in MetadataActions
- CSV Templates: Removed extra padding from checkbox styles
- Image Switching: Fixed pending state and layout effect handling
- Context Menu: Upscale text updated for clarity across all locales

## [3.0.17] - 2026-02-17

### Added
- AI Image Generation: Full Runware.ai integration with model selection, target folder, and queue management
- AI Image Generation: "Generate Similar" functionality to create variations of existing images
- AI Image Generation: Random base prompt generation with UI controls
- AI Image Generation: Auto-attach generation prompt as helper text for metadata
- AI Image Generation: Workflow support with cancellation logic, cascading deletes, and status tracking
- AI Image Generation: History tab with job cards showing AI model, clipboard actions, and improved UI
- AI Image Generation: Prompts tab with multi-select, bulk delete, move, filter, sort, and usage count display
- AI Image Generation: Multi-image generation counter with persistence
- AI Image Generation: Batched toast notifications for generation events
- Thumbnail Grid View: New grid layout inspired by Lightroom with adaptive metadata display
- Thumbnail Grid View: Status badges, color tag borders, and responsive compact mode
- Thumbnail Grid View: Keyboard shortcuts for thumbnail size control and bulk color tagging
- Thumbnail Grid View: Editorial status toggle, double-click to switch views, and empty state
- Thumbnail Grid View: Animated border glow for items with generating metadata
- Breadcrumb Navigation: New component with multi-language support
- Folder Management: Rename, delete, sorting, and create directory functionality
- Folder Management: Folder creation dialog and management options in image generation
- Image Reporting: Report issue feature for AI-generated images with local hash verification and duplicate prevention
- Media Deletion: Delete functionality with confirmation dialog and telemetry tracking
- Capture Datetime: Enhanced dialog with separate date and time inputs
- Resizable Right Panel: With localStorage persistence and accessibility support
- View Toggle: Icons in BottomToolbar to switch between filmstrip and thumbnail views
- Category Validation: Retry system for stock photo categories
- EPS Files: Enhanced handling to skip title verification in ExifTool and metadata verification
- Telemetry: Tracking for folder creation, renaming, deletion, and image generation events
- AI Metadata: Display for generated images with watermark indicators and keyboard shortcut toggles

### Changed
- State Management: Refactored app store into modular slices for improved maintainability
- CSS Architecture: Split into modular stylesheets for faster loading
- Localization: Reorganized locale files into namespace-based structure
- Localization: Added translations for PT, RU, and UK languages for new features
- Performance: Memory optimization improvements
- Security: Strengthened input validation and data parsing across the application
- Stability: Updated core framework to latest stable version
- Window Management: Main window recreation logic and window existence checks for menu actions
- Notification System: Improved notification handling for better reliability
- Reconciliation: Filesystem reconciliation to remove stale database records and sync deletions
- Sidebar: Updated button styles for improved responsiveness and visibility
- Code Quality: Replaced native alerts/confirms with custom dialogs in settings tabs

### Fixed
- Preview: Datetime tooltip repositioned for improved visibility
- Filmstrip: Tooltip positioning with below state and animations
- Filmstrip: Component updated to use div-based button with keyboard accessibility
- VideoSpeedSelector: Corrected HTML structure
- Thumbnails: Race condition between file watcher and workflow thumbnail processing
- Thumbnails: Status handling in Filmstrip component for improved rendering
- Context Menu: Submenu positioning and active state indication
- Workflow: Fixed issue where workflow actions could target the wrong workflow
- Search: Updated hover border color for global search input wrapper
- Errors: Handled errors in directoryHasChildren function to prevent crashes
- Errors: Improved error handling in reconciliation service and polling timeout logic
- Bottom Toolbar: Fixed overlap in thumbnail view and dynamic filter dropdown positioning

### Removed
- Deprecated AI model 'FLUX.2 [klein] 9B Base' removed from all locales and types

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
- Error Handling: Centralized error notifications for a consistent user experience
- Metadata Panel: "No changes to save" message and improved save button tooltip
- Localization: Metadata verification translations

### Changed
- Filters: Enhanced dropdown UI with sections and improved layout
- Logging: Increased default log output for better debugging
- Styling: Improved window controls hover styling
- Performance: Optimized state access in callbacks to prevent duplicate event listeners

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
- Menu: "Check for Updates" action now provides better UX feedback
- Localization: Updated default local AI model recommendation

### Removed
- Skip options functionality and related hooks from BottomToolbar

## [3.0.13] - 2025-01-04

- Initial release

---

[3.0.19]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.19
[3.0.18]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.18
[3.0.17]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.17
[3.0.15]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.15
[3.0.14]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.14
[3.0.13]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.13
