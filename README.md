# ParadeDB Cursor plugin

Teach agents how to use ParadeDB effectively.

## Structure

- `.cursor-plugin/plugin.json`: plugin metadata
- `.cursor-plugin/marketplace.json`: marketplace metadata pointing at this plugin
- `mcp.json`: ParadeDB docs MCP server
- `assets/logo.svg`: marketplace logo

The plugin files live at the repository root. The marketplace manifest points to `"."` so the template validator checks the same root plugin layout. To add more plugins later, see `docs/add-a-plugin.md`.

## Submission checklist

- The plugin has a valid `.cursor-plugin/plugin.json`.
- `.cursor-plugin/marketplace.json` maps to the root plugin.
- Plugin names are unique, lowercase, and kebab-case.
- All frontmatter metadata is present in rule, skill, agent, and command files.
- Logos are committed and referenced with relative paths.
- `node scripts/validate-template.mjs` passes.
- Repository link is ready for submission to the Cursor team (Slack or `kniparko@anysphere.com`).
