---
"@googleworkspace/cli": minor
---

Switch MCP tool names from underscore to hyphen separator (e.g., `drive-files-list` instead of `drive_files_list`). This resolves parsing ambiguity for services/resources with underscores in their names like `admin_reports`. Also fixes the alias mismatch where `tools/list` used Discovery doc names instead of configured service aliases.

**Breaking:** MCP tool names have changed format. Well-behaved clients that discover tools via `tools/list` will pick up new names automatically.
