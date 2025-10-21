🎉 Artok Studio v2.1.0 Release Notes: The "Asset Packer" Update

Artok Studio v2.1.0 is a monumental release that completely revamps the build and export pipeline. The major focus of this version is the introduction of the Optimized Binary Structure and the ability to package all user assets—images, fonts, and event scripts—into a single, optimized binary file for deployment.

🚀 Key New Features

1. Optimized Binary Output & Asset Packaging

The entire project export system has been upgraded to utilize an efficient, new binary structure, making your HMI file size smaller and load times faster on target hardware.

Optimized Binary Format: Core implementation of an optimized and efficient binary export structure (de86248).

Image Packaging: Images and their corresponding assets are now packed directly into the binary file (32b0845, 283b666).

Animated Image Support: Full support for packing and generating animated image sequences (d9c1a11).

Font Assets: Font files are now properly packed into the UI binary (632a47f).

Style and Event Packaging: Widget style properties and event handler code are successfully packed into the final output binary (dcad069, 4c76b02, abf6238).

2. Widget & Customization Enhancements

We've integrated new widgets and dramatically expanded font customization options.

New Widgets: Integrated support for three essential widgets:

Image Widget (cbc7ed5, 7e20716).

Image Button Widget (ccdc182).

Animated Image Widget (1a7ec11).

Advanced Font Support: You can now fully control typography across your project:

Support for Custom Fonts (2ea0389).

Support for Built-in Fonts (ac9ad84).

Added the ability to edit Font BPP (Bits Per Pixel) (cd819c5).

Updated the Style Panel to allow easy font selection (2f78661).

Lua Event System: Implemented core mechanisms for Lua scripting and event handling, including identifier and handler code pools (8c45dfa, 8159943).

3. Feature Gating & User Plan Limits

The application now enforces limitations based on the user's plan tier, ensuring fair feature access.

Initial implementation of Feature Gating draft alpha (db00563).

Implemented hard limits on the number of screens, images, fonts, and keyboard resources available (1861682).

Updated internal plan limit values (f0c9ba6).

🛠 Stability and Performance Improvements

This release includes numerous critical fixes that improve stability, especially in complex projects and specific operating systems.

Critical Fixes

Platform Compatibility: Fixed issues that prevented font conversion and building in specific Windows environments (924cfd7, 7f92c86, 5e956d7).

Memory and Performance: Resolved a critical memory leak issue (ef7fa28) and combined the string pool for faster memory access (f794e82).

Rendering Stability: Addressed multiple crashes and display bugs:

Fixed crashes related to switching screens and customized fonts (ed7ed3a, 32dfb9, dbec05d, c8cc2ab).

Resolved issues causing image blur, stripes, or widgets failing to display (93a6ac2).

General Improvements & Refactoring

Project Flow: Fixed an issue where image previews failed to display when loading a project (cb92423).

Serial Communication: Updated the serial protocol to support ACK per chunk for more reliable transfers (cd997a3) and fixed a serial port connection issue (54c41d9).

Code Quality: Extensive refactoring to decouple store state management (056548a), rename core internal files from lvgl_ to atk_ (43ef03e), and clean up debug logs across the codebase (21d47cf, e2c4be5).

We believe v2.1.0 delivers a massive leap forward in making your projects robust and ready for deployment. Thank you for your continued support!