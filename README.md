# Anima iPad runtime — experimental source build

This repository contains the source package and a manual Mac build workflow for an experimental, interpreter-based iPad runtime. It adapts pinned UTM SE and QEMU sources with a legacy Android framebuffer, input devices, and local data preservation code.

**This is a development project, not a working game release.** Compilation, Android boot, performance, audio, touch controls, and save/reload behavior must be verified on the actual target device. A successful build alone does not establish those results.

The source ZIP contains no game APK, Android system images, personal saves, Apple signing material, or account credentials. Its exact SHA-256 is checked before extraction, followed by a per-file source manifest check. Upstream source versions and hashes are pinned inside the package.

The workflow runs only when manually started. It tests the storage package and new QEMU devices, then builds unsigned iPad code without personal game data. The output is not installable or playable on its own. Private data must be assembled locally and the app must be signed before device testing.

Upstream license texts are included under `LICENSES` in the source ZIP, with applicable notices in individual source files.
