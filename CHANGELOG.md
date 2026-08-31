# Changelog

All notable changes to MetaPhotoAI will be documented in this file.

## [3.1.0] - 2026-08-31

### Added
- Controlled Vocabulary: Generate keywords drawn from the Getty Images / iStock controlled vocabulary, with a toggle in Settings > Keywords and in the metadata panel
- Controlled Vocabulary: Per-image shield badge showing full or partial vocabulary match, with unmatched terms marked directly in the keyword list
- Controlled Vocabulary: Library filter by vocabulary match status (matched, not matched, all)
- Controlled Vocabulary: Pre-upload warning when selected files carry keywords that weren't generated against the controlled vocabulary
- Controlled Vocabulary: Prompt for a default IPTC Country value, applied wherever the field is unset, to satisfy Getty/iStock submission requirements
- Controlled Vocabulary: Independent per-workflow Controlled Vocabulary setting for automated workflows
- Image Quality Check: Local blur and exposure scoring with warning badges, grid filters, and a pre-upload quality callout
- Image Quality Check: Grain and noise detection, including high-ISO noise-reduction artifacts, running as a separate background check
- Image Quality Check: Configurable sensitivity (low / balanced / high) with a separate sensitivity selector for grain
- Crop Editor: Save Cropped Copy and Export Cropped Copy actions, with source metadata preserved on the copy
- Crop Editor: Choice of what happens to the original photo when saving a cropped copy
- Crop Editor: Hold Shift while resizing a free crop to lock its aspect ratio
- Import: Import dialog opens automatically when removable media is attached
- Import: Non-blocking background imports with a floating progress card
- Import: Drag-and-drop file import in grid view
- Missing Folders: Offline state for images whose root folder is unavailable, with sidebar warning tooltips and automatic exclusion from generation, FTP upload, and CSV export
- Updates: Status bar version becomes an Update button with checking state and live download progress when an update is available
- Updates: Newer-release notice and Update Now button in the feedback window
- Categories: On-device fallback for category suggestions when the connection is unavailable
- Categories: Supporting model now ships with the app so semantic features work without an extra download
- Toolbar: Reveal or hide CSV templates and FTP hosts inline from the toolbar dropdowns
- Account: Reserved credits shown in the account menu
- Queue: Run-type labels distinguishing metadata and category runs
- Workflows: Failure toasts open the workflow queue directly, with clearer recovery for failed runs

### Changed
- Performance: Import throughput up to 4x faster and thumbnail scrolling dramatically smoother in large folders
- Performance: Collections open much faster, and folder opening no longer blocks on background reconciliation
- Performance: Immediate feedback when starting generation from any entry point, with clearer queued / processing / uploading progress
- Performance: Thumbnail loading with skeleton shimmer, fade-in, and a blurred base layer while previews generate
- Performance: Faster video metadata batches and workflow thumbnail readiness
- Thumbnails: Filmstrip and grid thumbnails preserve the image's aspect ratio
- Upload: Cloud upload progress phase renamed to image preparation for clarity
- Similar Images: Open-in-Finder buttons replaced with show-in-library navigation
- Feedback: Bug reports now include a compact diagnostic summary to help resolve issues faster, with personal details removed automatically before sending
- Security: Strengthened connection security for FTP, FTPS, and SFTP uploads, with clearer connection-security details in FTP settings
- Stability: Updated core framework and key components to current stable versions
- Localization: Translations added for controlled vocabulary, quality check, crop copies, and other new workflows across all supported languages

### Fixed
- Selection: Shift-select no longer ranges over images hidden by active filters
- Similarity: Images without metadata are excluded from metadata similarity
- Import Dialog: Fixed stale checkmark when toggling a file via its checkbox
- Selection: Warning popover clicks no longer clear the image selection
- Context Menus: Native edit menu no longer doubles up with custom context menus
- Folders: Moving an already-missing folder to Trash is handled gracefully
- Collections: Fixed stale membership counts after collection changes
- Controlled Vocabulary: Shield badge hidden when an image has no keywords, and fixed a badge selection regression
- FTP: Fixed upload verification issues and settings form flashing default values before hosts load
- Updater: Fixed races between updating and quitting the app

## [3.0.28] - 2026-06-01

### Added
- Collections: Create manual collections and smart collections to organize work across folders without moving files
- Smart Collections: Build dynamic collections with advanced rules for ratings, metadata status, folders, and other image attributes
- Collection Actions: Add selected images to collections, remove images from collections, navigate back to source folders, and run batch actions from collection views
- IPTC Metadata Editor: New structured IPTC tab for editing contact, creator, rights, licensing, event, location, and administrative metadata
- IPTC Reusable Entries: Save and reuse structured IPTC location entries, with copy/paste actions for faster repeated metadata entry
- Location Editing: Map picker, coordinate paste, copy coordinates, and reset controls for GPS metadata
- Image Review: Rating controls, rating filters, and optional rating display in the preview pane and image info panel
- Rejection Workflow: Mark images as rejected, show rejected state in the preview, and skip rejected items during confirmation-based actions
- Similar Image Audit: Review visually similar images, compare groups with previews, adjust scan sensitivity, and act on matches from the audit dialog
- Image Info: RGB and luminance histogram views, color profile metadata, expanded file details, and derived asset rotation controls
- History Window: Dedicated history window for generation and upscale history
- Folder Automation: Per-folder automatic keyword generation settings with folder indicators
- File Support: Adobe Illustrator file support
- Command Palette: More actions for folders, context actions, image selection, preview controls, tab controls, export, upload, copyright, and accessibility workflows
- Add Files to Folder: Add files directly to the current folder from the app workflow

### Changed
- Preview Pane: Metadata now overlays the preview image with improved spacing, shadows, centered fit behavior, and clearer rejected/rating indicators
- Preview Zoom: Zoom controls are docked below the image area, exposed in the View menu, and available through command palette actions
- Right Panel: Tabs can be customized from a dropdown so each workflow can keep the most relevant panels visible
- Thumbnail Grid: Quick actions, status overlays, rating display, selection behavior, and matched-image audit previews were refined
- Folder Browser: Collection controls, folder settings indicators, drag-and-drop behavior, context menus, and empty states were improved
- History and Prompt Views: Saved prompts render more efficiently and history is easier to access from a separate window
- Notifications and Dialogs: Close buttons, notification surfaces, upload/export language, and workflow discovery were normalized for clearer feedback
- Accessibility: Main regions, controls, command workflows, focus states, announcements, and keyboard-accessible actions were expanded across the app
- Localization: User guide, tooltips, IPTC fields, collection language, review actions, and new workflows were translated across supported languages
- Startup and Performance: App startup, thumbnail loading, folder scans, idle work, and prompt rendering were optimized

### Fixed
- Collections: Fixed stale counts, empty states, filter clearing, rating filters, drag-and-drop into collections, source labels, and delete behavior
- Folder Trash: Fixed stale image state after deleting a folder
- Preview: Fixed selection render loops, rejected badge positioning, title tooltips, and location overlay readability
- IPTC: Fixed grouped editor layout, tab switching, shared fields, multiline values, save behavior, and structured metadata writes
- Similar Image Audit: Fixed preview lookup, dialog stacking, group display, scan progress, and audit thumbnails
- Thumbnail Grid: Fixed stale rating overlays and refreshed filtered thumbnail records
- Shortcuts: Fixed Option-key shortcut normalization and updated rating shortcuts
- Import and File Handling: Improved file import behavior, embedded metadata import, folder add actions, and image rotation handling
- History: Improved access to history from the app workflow

## [3.0.27] - 2026-04-05

### Added
- Local Processing: Support for local AI processing with updated credit calculations and confirmation messages
- Offline Status Indicator: Visual indicator when the app has no internet connection, with automatic network status detection
- Theme Management: Full dark, light, and auto theme modes with CSS variable theming across all components and child windows
- Preview Zoom: Zoom controls in the Preview Pane with toggle between zoom levels, loading indicators, and localization support
- Tip of the Day: Daily tips displayed as toast notifications with localization and media support, including keyboard navigation
- History Search: Search functionality for history batches to quickly find past generation jobs
- History CSV Export: Export history batches to CSV for external use
- Apply Metadata from History: Apply metadata from history items directly to selected images
- Quit Guard: Confirmation dialog when quitting during active tasks to prevent data loss
- Unsaved Changes Guard: Navigation guard to prevent losing unsaved metadata when switching directories
- Keyword Display Size: Configurable keyword tag display size settings
- Clear Recent Searches: Ability to clear recent search history with a dedicated button
- New Ollama Models: Support for additional Ollama AI models with updated display names
- Enhanced Onboarding: Improved empty state onboarding experience with new UI and translations
- Drag-and-Drop Folders: Drop folders onto the sidebar to add them as root directories
- Directory Subtree Management: Utilities for detecting and removing subtree duplicates when adding folders

### Changed
- Status Bar Messages: Replaced toast notifications with less intrusive status bar messages for user feedback
- Preview Background: Dynamic preview background color based on effective theme with manual override for light mode
- Windows Compatibility: Improved cross-platform file handling and compatibility
- Preview Performance: Optimized panning and zooming for smoother interactions on all platforms
- Filmstrip Numbers: Version-gated filmstrip number default setting with migration support
- Category Generation: Improved category generation handling and user feedback
- Process Management: Cleaner shutdown behavior when closing the application
- Thumbnail Handling: Improved thumbnail loading reliability with cache management
- Localization: Refined tip descriptions across all supported languages for clarity and usability

### Fixed
- EXIF Data: Improved image dimension retrieval from file metadata
- Metadata Import: Fixed duplicated description after metadata re-import
- Filter Dropdown: Fixed filter dropdown not opening from external triggers
- Tip of the Day: Corrected navigation behavior for tip actions

## [3.0.23] - 2026-03-10

### Added
- Metadata Shortening: AI-powered shortening for titles and descriptions via the metadata field context menu to meet stock agency character limits
- Folder Pinning: Pin up to 6 frequently used folders to the top of the sidebar for quick access
- Pin Indicator: Visual pin icon on pinned directories in the sidebar
- Filmstrip Sequence Numbers: Configurable sequence number overlay on filmstrip items, enabled by default
- Ghost Keyword Tags: Streamlined keyword suggestion display with ghost tag styling for inline suggestions

### Changed
- Filmstrip Numbers: Show filmstrip sequence numbers by default for new installations
- Metadata Panel: Improved textarea dimensions and layout for better editing experience
- Sidebar: Adjusted directory header font opacity for improved visibility
- Filmstrip: Adjusted sequence number color opacity for better readability
- Localization: Added translations for metadata shortening and filmstrip number settings across all 12 supported languages

## [3.0.22] - 2026-03-08

### Added
- Folder Completion Requirements: Configurable per-folder completion criteria including title, description, keywords, categories, and no-warnings checks
- Completion Breakdown: Detailed per-field completion stats in the status bar popover showing exactly which requirements each image is missing
- Upload Readiness Filter: Option to upload only "ready" items that meet all folder completion requirements during FTP/SFTP upload
- Choice Confirmation for Uploads: Confirmation dialog before uploading that shows completion stats and lets you choose to upload the full folder, visible items, or selected items
- No-Warnings Completion Requirement: New completion field that marks images as incomplete if they have metadata rule warnings

### Changed
- Status Bar: Redesigned popover with interactive completion requirement checkboxes and live breakdown stats
- Status Bar: Improved popover styling and layout for better readability
- Dropdown Menus: Adjusted menu item alignment for consistency
- Default Settings: Categories completion requirement now defaults to off for new installations
- Localization: Added translations for folder completion requirements, upload readiness, and completion breakdown across all 12 supported languages

### Fixed
- Default folder completion requirement for categories changed to false to avoid requiring categories for all users by default

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

[3.1.0]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.1.0
[3.0.28]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.28
[3.0.27]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.27
[3.0.23]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.23
[3.0.22]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.22
[3.0.19]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.19
[3.0.18]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.18
[3.0.17]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.17
[3.0.15]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.15
[3.0.14]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.14
[3.0.13]: https://github.com/rohaneh/metaphotoai-v3-releases/releases/tag/v3.0.13
