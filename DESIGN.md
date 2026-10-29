# Istighfar — Design Notes

## Product
A private, low-distraction counter to help a person keep track of Astaghfirullah / istighfar without making counting the point of the practice.

## Interaction priorities
- The primary task is one tap to add one count.
- The current count and daily intention must be visible immediately.
- Undo is reversible; reset-today requires confirmation and preserves the all-time total.
- Goals are optional presets: 33, 100, 300, and 1,000.
- Seven-day history, all-time count, and completed-day streak support reflection without a competitive feed.
- No login, cloud sync, advertising, analytics, or external runtime dependencies.

## Visual system
- Warm ivory page, near-white surfaces, dark forest-green actions/data, restrained brass accent.
- Editorial serif for the product name and key count; system sans-serif for controls.
- Quiet borders instead of heavy shadows; use color on the important count and progress, not every surface.
- Designed for both one-handed mobile use and desktop.
- Visible keyboard focus, reduced-motion support, real button labels, and live count announcements.

## Data and privacy
Counts and preferences live in localStorage on the current browser/device. Clearing browser site data clears that data. The app does not send personal counter data to a server. Offline support is available after hosting on HTTPS and the service worker has installed.

## References consulted
- UI UX Pro Max: token hierarchy and state-aware components.
- Taste Skill: app-screen hierarchy, purposeful content, and avoidance of generic dashboard decoration.
- Impeccable: task-first Operate mode, responsive layout, accessibility, and finished state behavior.
- gstack: product/quality review and test-oriented implementation.
- Diagram Design and PPT Master were reviewed; neither suggests a diagram or slide surface for this simple counting interaction, so neither was added to the UI.
