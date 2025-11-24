# CHANGELOG

All notable changes to this project will be documented in this file.

---

## [v2.2.0] - 2025-11-24

### ✨ New Features (Added)

* **AI Draft Feature:** Integrated the core AI drafting functionality.
* **AI Generate Event Code:** Implemented the feature to generate event-handling code using AI.
* **Multi-Screen Support:** Integrated support for managing and rendering multiple screens within the editor.
* **Widget Pack Integration:** Integrated the `dropdown` and `table` widget packs into the build binary (`bin`).

### ⚙️ Improvements (Changed)

* **AI Backend Integration:** Integrated the AI generate feature with the backend API.
* **UI/Aesthetic Updates:** Cleaned up the UI layout and updated the Aesthetic placeholder.
* **Refactoring:** Significant refactoring of widget properties and removal of `CommonProperties`.
* **Configuration:** Updated configuration name from `.artok` to `artok`.
* **Development:** Initial draft implementation of the AI credit feature.
* **UI Color:** Updated login / sign up button color.
* **Hotfix:** Optimized build binary UI speed.

### 🐞 Fixes

* Fixed TS2307 error after dependency cleanup.
* Fixed an unknown hotfix issue.
* Resolved image asset loading issues.

---

## [v2.1.1] - 2025-11-06

### Fixed

* **Hotfix:** Resolved a critical issue that caused application crashes when **reopening or recreating a project**.
* **Fixed:** Addressed a conflict that occurred during the creation process of new UI projects.
* **Resolved:** Issues related to **font loading, rendering, and management**.
* **Addressed:** Serialization and deserialization errors that could lead to data inconsistency.
* **Fixed:** Load status handling for image assets, resolving various resource loading issues.
* **Hotfix:** Resolved an unexpected issue related to the application's operating mode.

### Added

* New functionality to **delete font resources** to help users clean up and manage project assets more effectively.

### Changed

* Updated the internal mechanism for **handling font loading**.

---

[v2.2.0]: https://github.com/Dualturb/artok-studio-releases/releases/tag/v2.2.0
[v2.1.1]: https://github.com/Dualturb/artok-studio-releases/releases/tag/v2.1.1