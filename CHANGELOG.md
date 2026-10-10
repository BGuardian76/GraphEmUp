# Changelog

All notable changes to GraphEmUp will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- First public release of GraphEmUp, a desktop workbench for Neo4j.
- Connections: save several named connection profiles and open them side by side. Passwords are encrypted, with the key kept in the OS keychain (Windows Credential Manager, Linux Secret Service).
- Schema viewer: see each database's labels, relationship types and properties as a graph, query the schema itself with Cypher, and save schema snapshots to compare versions.
- Cypher notebooks: write and run queries in cells, organised in folders and tabs, with results as a graph, a table or JSON, plus export.
- Query performance: execution plans, a query history and a Performance window.
- AI assistant (optional, uses Claude Code): ask about a database's schema and get suggested queries, which you review and run yourself.
- Keyboard shortcuts list in every window.
