# What's New in MetaPhotoAI

## [3.1.0] August 2026

### Controlled Vocabulary Keywords for Getty & iStock
Getty Images and iStock only accept keywords from their controlled vocabulary — a fixed list of approved terms — and silently drop everything else at submission. Turn on Controlled Vocabulary in Settings > Keywords and MetaPhotoAI generates keywords drawn from that vocabulary, so the terms you write are the terms that count. MetaPhotoAI is an independent application and is not affiliated with or endorsed by Getty Images or iStock.

### Vocabulary Match Badges & Filtering
A shield badge on each image shows whether its keywords are fully or partially vocabulary-matched, and unmatched terms are marked right in the keyword list — your manual edits are never removed, only flagged. Filter your whole library by match status to isolate a Getty/iStock submission set in seconds.

### Pre-Upload Vocabulary Check
Before you upload to a Getty/iStock destination, MetaPhotoAI warns you if selected files carry keywords that weren't generated with Controlled Vocabulary, so you can regenerate first instead of finding out after submission. Missing the required IPTC Country field? MetaPhotoAI prompts for a default and fills it in wherever it's unset. Automated workflows get their own independent Controlled Vocabulary setting.

### Image Quality Check
MetaPhotoAI now scores your images locally for blur, exposure problems, and grain or noise — including the blotchy artifacts high-ISO noise reduction leaves behind. Flagged images get warning badges, can be filtered in the grid, and are called out before upload. Choose low, balanced, or high sensitivity, with a separate sensitivity control just for grain.

### Cropped Copies
Save or export a cropped copy of any image straight from the crop editor, with the original's metadata carried over to the copy. Choose what happens to the source photo when you save, pick aspect presets from a compact dropdown, and hold Shift while resizing a free crop to lock its ratio.

### Faster Everywhere
Importing large batches is up to 4x faster, scrolling long filmstrips and grids is dramatically smoother, and collections open in a fraction of the time. Generation now gives instant feedback from every entry point, thumbnails load with a smooth shimmer-and-fade, and batch progress is easier to follow while work is queued, processing, or uploading.

### Background Imports from Cards & Drives
Attach a memory card or external drive and the import dialog opens automatically. Imports now run in the background with a floating progress card, so you can keep working while files copy in.

### Missing Folders Handled Gracefully
If a drive is unplugged or a folder disappears, its images now show as offline instead of causing errors. The sidebar warns you with a tooltip, and offline images are automatically excluded from generation, uploads, and exports until the folder comes back.

### One-Click Updates
When an update is ready, the version number in the status bar becomes an Update button with live download progress. The feedback window also lets you know when a newer release is available, with an Update Now button right there.

### Category Suggestions, Even Offline
Category suggestions now fall back to on-device processing when you're offline or the connection drops, and the supporting model ships with the app — so semantic features work out of the box, no extra download needed.

### Actionable Workflow Failures
When a workflow fails, the failure toast now takes you straight to the queue, and queue cards are labeled as metadata or category runs so you can see at a glance what ran and what needs attention.

### Quality of Life
Reveal or hide CSV templates and FTP hosts directly from the toolbar dropdowns, see your reserved credits in the account menu, drag and drop files to import in grid view, and enjoy thumbnails that keep their true aspect ratio in the filmstrip and grid.

## [3.0.28] June 2026

### Collections & Smart Collections
![](https://metaphotoai.io/whats-new/3.0.28/collections-smart-collections.jpeg)
Organize images across folders without moving the original files. Create hand-picked collections for client sets, reviews, or uploads, or build smart collections that update automatically from rules such as ratings, folders, and metadata status.

### Full IPTC Metadata Editing
![](https://metaphotoai.io/whats-new/3.0.28/iptc-metadata-editor.jpeg)
The new IPTC tab gives you structured controls for creator, contact, rights, licensing, event, location, and administrative metadata. Reusable entries and copy/paste actions make repeated location and rights metadata much faster to apply.

### Map-Based Location Tools
![](https://metaphotoai.io/whats-new/3.0.28/location-map-tools.jpeg)
Set GPS metadata with a map picker, paste coordinates from another source, copy existing coordinates, or reset the location fields from the same workflow.

### Image Review Tools
![](https://metaphotoai.io/whats-new/3.0.28/image-review-tools.jpeg)
Rate images, filter by rating, show ratings in the preview, and mark files as rejected when they should be skipped from review or batch actions.

### Similar Image Audit
![](https://metaphotoai.io/whats-new/3.0.28/similar-image-audit.jpeg)
Find visually similar images in a folder, compare matched groups with previews, adjust scan sensitivity, and take action on duplicates or near-duplicates before export.

### Richer Image Info
![](https://metaphotoai.io/whats-new/3.0.28/richer-image-info.jpeg)
The Image Info panel now includes RGB and luminance histograms, color profile details, expanded file information, and rotation controls for derived assets.

### Preview & Workspace Polish
![](https://metaphotoai.io/whats-new/3.0.28/preview-workspace-polish.jpeg)
Preview metadata now overlays the image with cleaner spacing and shadows, zoom controls sit below the image area, and right-panel tabs can be customized from a compact dropdown.

### Faster Startup & Smoother Large Folders
MetaPhotoAI now opens sooner and handles large folders more smoothly with improved thumbnail loading, folder scanning, and background work scheduling.

### More Keyboard & Command Palette Coverage
More folder, image, selection, export, upload, copyright, preview, and tab actions are available from the command palette and keyboard-friendly workflows.

## [3.0.27] April 2026

### Dark, Light & Auto Themes
![](https://metaphotoai.io/whats-new/3.0.27/theme-management.gif)
Switch between dark, light, and auto theme modes. Auto mode follows your system appearance. All panels, dialogs, and child windows update seamlessly with consistent styling throughout.

### Preview Zoom Controls
![](https://metaphotoai.io/whats-new/3.0.27/preview-zoom.gif)
Zoom in and out on your preview images with new zoom controls. Toggle between zoom levels with a single click and see a loading indicator while high-resolution images load.

### Tip of the Day
![](https://metaphotoai.io/whats-new/3.0.27/tip-of-the-day.gif)
Discover useful features and workflow tips with a daily tip notification. Each tip includes a description and optional media to help you get the most out of MetaPhotoAI. Available in all supported languages.

### Offline Status Indicator
![](https://metaphotoai.io/whats-new/3.0.27/offline-indicator.jpeg)
A visual indicator lets you know when your internet connection is unavailable, so you can switch to local processing or wait to sync.

### Quit & Navigation Guards
![](https://metaphotoai.io/whats-new/3.0.27/quit-guard.jpeg)
MetaPhotoAI now warns you before quitting during active tasks or when you have unsaved metadata changes. No more accidentally losing work when switching folders or closing the app.

### History Search & Export
![](https://metaphotoai.io/whats-new/3.0.27/history-search.gif)
Search through your generation history and export batches to CSV. You can also apply metadata from any history item directly to your currently selected images.

### Keyword Display Size
![](https://metaphotoai.io/whats-new/3.0.27/keyword-display-size.gif)
Adjust the display size of keyword tags in the metadata panel to match your preference — helpful when working with many keywords on smaller screens.

### New Ollama Models
Added support for the latest Ollama models for local AI processing, with updated display names.

### Enhanced Onboarding
![](https://metaphotoai.io/whats-new/3.0.27/onboarding.jpeg)
A refreshed onboarding experience in the empty state helps new users get started faster with clear guidance and improved visuals.

## [3.0.23] March 2026

### Metadata Shortening
![](https://metaphotoai.io/whats-new/3.0.23/metadata-shortening.jpeg)
Right-click any title or description field to shorten it with AI. MetaPhotoAI intelligently condenses your text to fit within stock agency character limits while preserving the meaning and key details.

### Folder Pinning
![](https://metaphotoai.io/whats-new/3.0.23/folder-pinning.jpeg)
Pin your most-used folders to the top of the sidebar for instant access. Pin up to 6 folders so your active projects are always one click away, no matter how many folders you have.

### Filmstrip Sequence Numbers
![](https://metaphotoai.io/whats-new/3.0.23/filmstrip-numbers.jpeg)
Filmstrip items now display sequence numbers so you can quickly reference and communicate about specific images. Toggle this on or off in General Settings.

### Ghost Keyword Suggestions
![](https://metaphotoai.io/whats-new/3.0.23/ghost-keyword-tags.jpeg)
Keyword suggestions now appear as subtle ghost tags inline with your existing keywords. Accept suggestions with a single click for a faster, more intuitive tagging workflow.

## [3.0.22] March 2026

### Folder Completion Requirements
![](https://metaphotoai.io/whats-new/3.0.22/folder-completion-requirements.jpeg)
Define what makes an image "ready" in each folder. Choose from title, description, keywords, categories, and no-warnings as completion criteria. The status bar shows a live ready count so you always know how many images are complete.

### Completion Breakdown
![](https://metaphotoai.io/whats-new/3.0.22/completion-breakdown.jpeg)
Click the ready count in the status bar to see a detailed breakdown of which completion requirements your images are meeting. Each field shows how many images pass, so you can quickly identify what needs attention.

### Upload Readiness Validation
![](https://metaphotoai.io/whats-new/3.0.22/upload-readiness.jpeg)
Before uploading via FTP/SFTP, a confirmation dialog now shows your folder's completion stats and lets you choose to upload the entire folder, only visible items, or your current selection. Enable "Upload only ready items" in upload settings to automatically filter out incomplete images.


## [3.0.19] March 2026

### Cross-Device Sync
![](https://metaphotoai.io/whats-new/3.0.19/cross-device-sync.jpeg)
Sync your settings and data across multiple devices. Sync runs automatically in the background after sign-in, with a built-in conflict resolution UI when changes collide.

### Image Moving with Drag-and-Drop
![](https://metaphotoai.io/whats-new/3.0.19/image-moving.jpeg)
Move images between folders by dragging and dropping them in the sidebar. Image references are automatically updated so nothing breaks.

### Keyboard Shortcuts & Shortcut Hints
![](https://metaphotoai.io/whats-new/3.0.19/keyboard-shortcuts.jpeg)
A new shortcut engine with support for chord bindings (multi-key sequences). Shortcut hints now appear on buttons and in dialogs so you can learn the shortcuts as you work.

### What's New Modal
![](https://metaphotoai.io/whats-new/3.0.19/whats-new-modal.jpeg)
After each update, a What's New modal automatically shows you what changed. Browse collapsible version groups to catch up on recent and past releases.

### Generation & Upscale History
![](https://metaphotoai.io/whats-new/3.0.19/history-tab.jpeg)
A dedicated History tab tracks all your AI image generation and upscale jobs with cache-first loading for instant access. Copy metadata or restore previous versions directly from history items.

### Resizable Left Panel
![](https://metaphotoai.io/whats-new/3.0.19/resizable-left-panel.jpeg)
Drag to resize the sidebar to your preferred width. Your setting persists across sessions.

### Live Credits
![](https://metaphotoai.io/whats-new/3.0.19/live-credits.jpeg)
Your credit balance now updates in real time as you use AI features, so you always know where you stand.

### CSV Template Export
![](https://metaphotoai.io/whats-new/3.0.19/csv-export.jpeg)
Export selected metadata templates to CSV for use in external tools or bulk upload workflows.

### Confirmation Prompts
![](https://metaphotoai.io/whats-new/3.0.19/confirmation-prompts.jpeg)
Configure when MetaPhotoAI asks for confirmation before generating or saving metadata. Customize the prompts to match your preferred workflow.

### Email Privacy Toggle
![](https://metaphotoai.io/whats-new/3.0.19/email-privacy.jpeg)
Mask your email address in the user menu with a single click for added privacy when screen sharing or recording.

### Upscaling Queue
![](https://metaphotoai.io/whats-new/3.0.18/upscaling-queue.jpeg)
Queue multiple upscaling jobs and monitor their progress in real time. Pause, resume, or cancel jobs as needed with detailed status information.

## [3.0.18] February 2026

### Image Upscaling
![](https://metaphotoai.io/whats-new/3.0.18/upscaling.jpeg)
Upscale your images up to 2x resolution directly from the context menu. Supports JPG, PNG, and WEBP formats with progress indicators in both Filmstrip and Thumbnail Grid views.

### Inline Metadata Suggestions
![](https://metaphotoai.io/whats-new/3.0.18/inline-suggestions.jpeg)
Get AI-powered inline suggestions for titles, descriptions, and keywords right inside the metadata panel. Accept, dismiss, or refine suggestions without leaving your workflow.
#### Contextual Keyword Suggestions
![](https://metaphotoai.io/whats-new/3.0.18/contextual-keyword-suggestions.jpeg)
Get intelligent keyword suggestions based on your existing metadata.

### Spellcheck
![](https://metaphotoai.io/whats-new/3.0.18/spellcheck.jpeg)
Built-in spellcheck with context menu integration for metadata fields. Catch typos in titles, descriptions, and keywords with one-click corrections and dictionary support.

### Metadata Versioning & History
![](https://metaphotoai.io/whats-new/3.0.18/metadata-history.jpeg)
Every metadata change is now versioned. Browse your full edit history and restore any previous version with a single click from the metadata panel or context menu.

### Multi-Select Metadata Editing
![](https://metaphotoai.io/whats-new/3.0.18/multi-select.jpeg)
Select multiple images and edit their metadata simultaneously. Merge or replace keywords across selections, with clear indicators when fields have mixed values.

### Copyright Templates
![](https://metaphotoai.io/whats-new/3.0.18/copyright.jpeg)
Configure copyright text, creator name, and business information in global or folder-level settings. Copyright is automatically applied when writing metadata with support for capture date or write time.

### Keyword Drag-and-Drop
![](https://metaphotoai.io/whats-new/3.0.18/drag-and-drop-keywords.jpeg)
Reorder keywords by dragging them into your preferred position. Fine-tune keyword relevance ordering before exporting or writing to files.

### Import Embedded Metadata
![](https://metaphotoai.io/whats-new/3.0.18/import-embedded-metadata-on-import.jpeg)
Automatically import existing IPTC/XMP metadata from image files when adding them to your library. Toggle this behavior in General Settings.

### New Default Stock Agencies For Quick FTP Upload
![](https://metaphotoai.io/whats-new/3.0.18/new-stock-agencies-for-upload.jpeg)
Upload directly to any configured FTP/SFTP host from the bottom toolbar with a single click. New preset configurations for Alamy, Deposit Photos, and Pond5.

## [3.0.17] February 2026

### AI Image Generation
Generate stock photos directly within MetaPhotoAI using Runware.ai models. Choose from multiple AI models, set a target folder, and queue up batch generations. Create variations of existing images with "Generate Similar", and auto-attach generation prompts as helper text for metadata.

### AI Image Generation History & Prompts
Browse your full generation history with job cards showing AI model details and clipboard actions. Manage your prompts library with multi-select, bulk delete, move, filter, sort, and usage count tracking.

### Thumbnail Grid View
A new Lightroom-inspired grid layout with adaptive metadata display. Includes status badges, color tag borders, responsive compact mode, keyboard shortcuts for thumbnail sizing, and animated border glow for items with generating metadata.

### Breadcrumb Navigation
Navigate your folder hierarchy with a new breadcrumb component supporting all 12 languages.

### Folder Management
Rename, delete, sort, and create directories directly from the sidebar. Includes folder creation within the image generation workflow.

### Resizable Right Panel
Drag to resize the right panel to your preferred width. Your setting persists across sessions via localStorage.

### Image Reporting
Report issues with AI-generated images using local hash verification and duplicate prevention.

## [3.0.15] January 2025

### User Guide
An interactive standalone window with collapsible sidebar, image and video support, and detailed pricing information. Access it anytime from the header bar.

### Category Override
Override stock photo categories at the folder level. Assign categories per folder so all images within inherit the correct category automatically.

### Metadata Templates
Apply metadata templates with new modes — apply all fields or only positive (non-empty) fields — giving you finer control over template behavior.

### Workflow Enhancements
Choose notification methods for workflow completion, duplicate existing workflows, and configure execution scope settings for more flexible automation.

### FTP Settings Improvements
Duplicate FTP/SFTP host configurations with one click. Enhanced delete host functionality with clear danger action buttons.

## [3.0.14] January 2025

### Helper Text Search & Filters
Search images by their helper text content using the global search. Filter by helper text status in the bottom toolbar to quickly find images with or without helper text.

### Shutterstock Video Categories
Full support for Shutterstock video categories with improved media type handling for video files.

### Enhanced Filmstrip Tooltips
Filmstrip tooltips now display video-specific metadata including duration, resolution, and codec information. Improved tooltip visibility when context menus or color tag pickers are open.

### FTP Host Duplication
Quickly clone existing FTP/SFTP configurations to set up similar hosts without re-entering all connection details.
