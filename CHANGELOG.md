# CHANGELOG

All notable changes to this project will be documented in this file.
---

## [v2.3.1] - 2026-01-31

### ✨ New Features (Added)

* **Professional Table Management:** Significantly expanded the **Table Widget** capabilities, including native support for adding/deleting columns and a modernized rendering style for industrial data sets.
* **Expanded Command Set:** Updated the native engine to support a broader range of hardware commands, strengthening the integration between the UI layer and the underlying system.
* **AI Guardrails:** Implemented safety guards for the **AI Event Handler generation** to ensure more consistent and error-free code output for complex interactions.

### ⚙️ Improvements (Changed)

* **HMI Aesthetic Overhaul:** Comprehensive UI update to deliver a more professional and modern aesthetic across all generated components, aligning with high-end industrial design standards.
* **Widget Optimization:** * Refined the **Button** widget for a cleaner, minimalist footprint.
    * Renamed `layoutDescriptor` to `buttonWeights` for better API clarity and intent.
    * Renamed **Flex Box** to **Flex** for industry-standard nomenclature.
* **Property Panel Refinement:** Overhauled the Widget Properties Panel with improved native bindings, ensuring real-time feedback and better state synchronization.
* **Architecture Cleanup:** Removed several incomplete container widgets to maintain a stable, production-ready build environment.

### 🐞 Fixes

* **Critical Widget Hardening:** Resolved functional and rendering issues across a wide array of core widgets:
    * **Data & Inputs:** Fixed Chart (resolved crash issues), Table, Dropdown, Roller, Slider, and Bar widgets.
    * **Indicators & Controls:** Fixed Arc, Meter, Message Box, and Button Matrix widgets.
    * **Geometry & Tools:** Fixed Line, QR Code, and Window widget rendering inconsistencies.
* **Simulator Stability:** Resolved a critical issue where the simulator would experience "duplicate booting," ensuring a cleaner development workflow.
* **Engine Native:** Fixed engine-level versioning mismatches and optimized native command processing.
---

## [v2.3.0] - 2026-01-25

### ✨ New Features (Added)

* **Artok Connect & AtkLink:** Introduced a comprehensive live-sync ecosystem. Artok Studio can now communicate directly with hardware via the `AtkLink` protocol, supporting real-time remote commands and status monitoring.
* **AI Design Suite:** Significant expansion of our AI-driven workflow tools:
    * **AI Appearance:** Automatically generate and apply professional visual styles and themes.
    * **AI Interactions:** Generate behavioral logic and interactive component responses using natural language prompts.
* **Professional Widget Expansion:** Massive update to the component library, including high-performance **Charts (with dynamic scaling), ColorWheels, LEDs, Spinners, and advanced Navigation Views (Tabs/Tiles).**
* **Universal Display Support (Beta):** Preliminary support for resolution-independent layouts, ensuring UI designs scale accurately across different screen densities.
* **Enhanced Localization:** Added native support for **Chinese typography** and improved system-level font integration.

### ⚙️ Improvements (Changed)

* **Artok Core Engine:** Upgraded the underlying framework to a more robust "Engine-first" architecture, significantly improving stability and simulation accuracy.
* **High-Performance Object Management:** Refactored internal object tracking to improve lookup speeds and memory efficiency for complex, high-widget-count projects.
* **Integrated Resource Management:** Optimized asset handling for fonts and images, reducing the final export size and improving runtime loading speeds.
* **Professional Debugging Tools:** Overhauled the **Output** and **Terminal** consoles to provide actionable feedback and detailed telemetry during the design process.
* **Workflow Optimization:** Improved canvas responsiveness with smart geometry debouncing and optimized data transfer speeds.

### 🐞 Fixes

* **Stability & Performance:** Eliminated critical memory leaks and resolved issues where the simulator could become unresponsive during extended sessions.
* **Visual Fidelity:** Fixed various rendering glitches related to 16-bit color depth and asset path resolution.
* **Logic Precision:** Resolved inconsistencies in event triggers and script execution logic.
* **Asset Loading:** Fixed multiple issues involving font compilation and binary data packing.

### ⚠️ Important Updates

* **API Refinement:** Standardized internal logic registration. Custom scripts using legacy handlers may require a minor update to the new naming convention.
* **Unified Branding:** Finalized the transition of all internal components under the **Artok Runtime** brand.

## [v2.2.1] - 2025-11-26 

### ✨ New Features (Added)

* **AI Inspire Feature:** The AI design drafting tool has been significantly enhanced to focus on generating graceful, impressive, and professional UI design concepts. It now intelligently extracts only the screen count and domain context, giving the AI greater creative freedom to invent aesthetically superior content and layouts.

### ⚙️ Improvements (Changed)

* **AI Prompting Strategy:** Refactored the internal AI prompt construction to prioritize pure inspiration, allowing the AI to invent compelling UI content and aesthetics based on screen count and domain, rather than rigidly adhering to provided widget details.
* **Frontend UX for Aesthetic Selection:** Replaced the free-text input for "Design Description (Aesthetic)" with a dropdown of predefined aesthetic styles (e.g., 'modern', 'futuristic', 'minimalist', 'dark mode'). This guides users towards more effective inputs, leading to more consistent and higher-quality AI-generated design drafts.

### 🐞 Fixes

* **AI Image Generation API:** Addressed an issue with the AI image generation API call that resulted in a "model not found" error when attempting to use an incorrect model identifier. (This refers to the `gemini-2.5-flash-image` error and the fix to use `imagen-4.0-generate-001`).

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
[v2.3.1]: https://github.com/Dualturb/artok-studio-releases/releases/tag/v2.3.1
[v2.3.0]: https://github.com/Dualturb/artok-studio-releases/releases/tag/v2.3.0
[v2.2.1]: https://github.com/Dualturb/artok-studio-releases/releases/tag/v2.2.1
[v2.2.0]: https://github.com/Dualturb/artok-studio-releases/releases/tag/v2.2.0
[v2.1.1]: https://github.com/Dualturb/artok-studio-releases/releases/tag/v2.1.1

