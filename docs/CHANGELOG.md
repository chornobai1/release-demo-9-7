# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0] - 2026-11-27

### Added

- Filter notes by tag with `NoteBook.filter_by_tag`
- Full-text search across note titles and bodies, ignoring letter case
- Export a notebook to a JSON string without writing a file

### Fixed

- Opening a notes file that does not exist yet no longer has to fail: `storage.load_or_empty` returns an empty notebook instead
- Repeated tags on a note can be collapsed with `dedupe_tags`, keeping the order they were first added

## [0.1.0] - 2026-01-15

### Added

- Initial release of the `notes` library
- In-memory notebook with add / get / list / remove / find
- JSON persistence via `storage.save` and `storage.load`
