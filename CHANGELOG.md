# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

- Nothing added yet!

## [3.3.2] - 2026-05-31

- Improved README.md layout and formatting.
- Changed the upcoming features in README.
- Fixed a bug where essential files and folders were not being made during the initialization of the tool.
- Changed the error handling when HTTP requests fail in builder.py.
- Changed the icon filename in assets/ from exe-icon to mcdl-icon.

## [3.3.1] - 2026-05-21

- Changed the name from `minecraft-mods-downloader` to `MCDL`.
- Changed the filepaths in `constants.py` and import statements to match with the new name.

## [3.3.0] - 2026-05-19

- Added logging and made `verbose_mode` (originally `show_detailed_logs`) configuration functional.
- Added a style for the `questionary` menus to increase contrast for important elements.
- Improved the UX by making incompatible mods with the mod loader disabled.
- Made the manual path prompt a more modern directory window for a more user-friendly experience.
- Added the functionality to set the default directory path to `None`.
- Fixed the behavior settings not being able to be disabled.
- Fixed mods being corrupted or not being downloaded.
- Heavily refactored the main functions in `main.py`
- Improved documentation in the code in general.
- Made private functions in `builder.py` actually private.
- Modified the configuration menu to handle `CTRL + C` cancellation in their submenus.

## [3.2.0] - 2026-05-13

- Added a feature that filters the mods that are incompatible with your launcher in the main selection mods screen.
- Added Multi-OS Compatibility, this tool now allows Linux, macOS and other OSes to download mods as well. However, the smart pathfind system only works on Windows so other OSes have to manually type in their filepaths to download mods.
- Added a new module to help with the development of this tool: `platformdirs`
- Added Dependabot to help resolve project dependency security vulnerabilities.
- Removed the `max_workers` during download, allowing for further concurrency.
- Updated `README.md` information to go along with the latest changes in this version.
- Fixed some minor bugs present in older versions.

## [3.1.1] - 2026-05-04

- Polished the `MCDL.exe` icon.

## [3.1.0] - 2026-05-04

- Removed `bandit` dev dependency.
- Added compatibility for multiple OSes.
- Added a placeholder icon for the `.exe`.
- Made it a `.zip` folder to prevent security warnings.
- Slightly polished code on all files.

## [3.0.0] - 2026-04-03

- Huge code polishing and refactor, removed the need for global variables, put constants in `constants.py`, and so much more.
- Uses `rich.live` to improve and polish the progress bars during downloading.
- Polished the UX of getting the user's download folder path.
- Added a summary table for the failed/incompatible mods at the end.
- Added a MIT License.
- Added `bandit`, `radon` and `vulture` dev dependencies to speed up the future development of this project.
- Now uses the `hatchling` build system for packaging.

## [2.0.0] - 2026-03-26

- Introduced multithreading to significantly speed up the tools moddata fetching and downloading processes.
- Added progress bars to visualize the progress during the downloading section.
- Changed library mods in `mods.json` to be a list of slugs, as it wasn't required to be in the main menu anymore.
- Slightly changed and improved documentation across `main.py`.

## [1.2.0] - 2026-03-23

- Now uses persistent API Sessions to make this tool significantly faster by removing the need to do a TCP handshake at the beginning of each.

## [1.1.0] - 2026-03-22

- Added more mod and more mod categories.
- Polished and cleaned up the overall code.
- Added core features for the tool such as the main menu, settings/configs, initial fetching and downloading process of mods.

## [1.0.0] - 2026-03-22

- Added configuration settings and the core features of the tool.
- The initial release of the tool.

[Unreleased]: https://github.com/nerrader/MCDL/compare/v3.3.1...HEAD
[3.3.2]: https://github.com/nerrader/MCDL/releases/tag/v3.3.2
[3.3.1]: https://github.com/nerrader/MCDL/compare/v3.3.0...v3.3.1
[3.3.0]: https://github.com/nerrader/MCDL/compare/v3.2.0...v3.3.0
[3.2.0]: https://github.com/nerrader/MCDL/compare/v3.1.1...v3.2.0
[3.1.1]: https://github.com/nerrader/MCDL/compare/v3.1.0...v3.1.1
[3.1.0]: https://github.com/nerrader/MCDL/compare/v3.0.0...v3.1.0
[3.0.0]: https://github.com/nerrader/MCDL/compare/v2.0.0...v3.0.0
[2.0.0]: https://github.com/nerrader/MCDL/compare/v1.2.0...v2.0.0
[1.2.0]: https://github.com/nerrader/MCDL/compare/v1.1.0...v1.2.0
[1.1.0]: https://github.com/nerrader/MCDL/compare/v1.0.0...v1.1.0
[1.0.0]: https://github.com/nerrader/MCDL/releases/tag/v1.0.0
