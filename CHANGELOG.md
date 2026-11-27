# Changelog

All notable changes to GraphEmUp will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Added
- Themes: Dracula, Nord, Solarized Dark, EmUp Light and EmUp Dark, plus the four Catppuccin flavours (Latte, Frappé, Macchiato, Mocha), each with matching graph canvas and Cypher colours.
- Schema comparison across connections: in the schema window, "Compare with" also lists other connections' live schemas and their snapshots, so you can compare Dev with Prod. Differences read "only in Prod / only in Dev / different", in the summary bar, legend, changes panel, details and the exported report.
- Parameter inputs in notebook cells: each `$parameter` a query uses gets an input above the query (text, number, yes/no or JSON). The notebook's parameters are defaults, and a cell can have its own value (↺ goes back to the default) or parameters only it has. Enter runs the cell, and a parameter without a value is pointed out before the query is sent.
- Cells that use each other's results: a parameter can take its value from an earlier cell, from the nodes picked in its graph (Ctrl- or Shift-click picks several), the rows ticked in its table, a whole column or the first row's value. With Follow on, the cell runs again when that selection or result changes, for drill-down notebooks.
- Analyse result graphs: PageRank, Most connected and Bridges size the nodes by importance, with a ranking panel (pick the top nodes, save it as CSV). Communities and Separate islands colour the nodes by group, listed in the legend, with "Arrange by group". It runs in the app on the graph you're looking at, so it works with any Neo4j server (no plugins needed) and never changes the database.
- Cypher editor: typing `$` suggests the parameters a cell can use with their values, and `$parameters` are shown in italics.

### Changed
- Result graph layouts fill the cell's shape: wide cells get wide layouts and tall cells tall ones (up to 2.5 times). When a cell is resized, the graph offers to fit it again; × keeps the current layout. App Settings → Graphs → "Fit layouts to the cell" turns it off.

## [0.1.18] - 2026-10-10
### Added
- First public release of GraphEmUp, a desktop workbench for Neo4j.
- Connections: save several named connection profiles and open them side by side. Passwords are encrypted, with the key kept in the OS keychain (Windows Credential Manager, Linux Secret Service).
- Schema viewer: see each database's labels, relationship types and properties as a graph, query the schema itself with Cypher, and save schema snapshots to compare versions.
- Cypher notebooks: write and run queries in cells, organised in folders and tabs, with results as a graph, a table or JSON, plus export.
- Query performance: execution plans, a query history and a Performance window.
- AI assistant (optional, uses Claude Code): ask about a database's schema and get suggested queries, which you review and run yourself.
- Keyboard shortcuts list in every window.
