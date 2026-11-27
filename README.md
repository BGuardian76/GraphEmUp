<img src="./assets/icon.png" width="128" height="128" alt="GraphEmUp">

# GraphEmUp

A desktop workbench for Neo4j: explore database schemas, write and run Cypher in notebooks, and inspect query results and plans.

This repository hosts **installers and release notes only**. It is the public download point for GraphEmUp. Source code is developed elsewhere; builds are published here as [GitHub Releases](../../releases).

## Features

- **Connections:** several named connection profiles, open side by side, with environment tags (e.g. Dev, Prod). Passwords are encrypted, with the key in the OS keychain.
- **Schema viewer:** each database's labels, relationship types and properties as a graph. Query the schema itself with Cypher, save snapshots, and compare versions or two connections (Dev against Prod).
- **Cypher notebooks:** queries in cells, organised in folders and tabs, with results as a graph, table or JSON. Parameters with inputs above each query, and cells that take values from earlier cells' results.
- **Graph exploration:** expand and hide nodes, find paths, search, many layouts, and analyse results (PageRank, bridges, communities) without any server plugin.
- **Query performance:** execution plans, query history and a Performance window.
- **AI assistant (optional, uses Claude Code):** ask about a database's schema and get suggested queries, which you review and run yourself.
- **Read-only friendly:** notebooks run read-only unless you allow writes, and nothing in GraphEmUp changes a database on its own.
- **Themes:** light and dark, Dracula, Nord, Solarized and Catppuccin.

## Download

Grab the newest installer for your platform from the [Releases page](../../releases):

| Platform | File |
|---|---|
| Windows | `GraphEmUp_<version>_x64-setup.exe` |
| Linux | `GraphEmUp_<version>_amd64.deb`, `.rpm`, or `.AppImage` |

## Changelog

See [CHANGELOG.md](CHANGELOG.md) for release history.

## License

[MIT](LICENSE)
