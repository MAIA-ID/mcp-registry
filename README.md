# Maia MCP Registry

This repository maintains a list of Model Context Protocol (MCP) servers that are compatible with [Maia](https://maia.id).

The registry is stored in [`entries.json`](entries.json) and is divided into **official** and **community** entries.

## Contributing

We welcome community contributions! To add or update an entry:

1. **Fork** this repository and create a branch for your changes.
2. Edit [`entries.json`](entries.json) by adding or modifying an entry within the `officialEntries` or `communityEntries` array.
3. Each entry must include the following fields:
   - `name`: unique identifier (lowercase, no spaces)
   - `title`: human-readable name
   - `description`: short description of the MCP server
   - `icon`: URL pointing to an SVG or image representing the service
   - `homepage`: website or repository for the service
   - `configuration`: object containing at least a `type` and `url`
4. Submit a pull request explaining your changes.

Please keep entries sorted alphabetically by `name` within their respective arrays.

## Example Entry

```json
{
  "name": "example",
  "title": "Example MCP",
  "description": "An example entry demonstrating the required fields.",
  "icon": "https://example.com/icon.svg",
  "homepage": "https://example.com",
  "configuration": {
    "type": "sse",
    "url": "https://example.com/sse",
    "headers": {}
  }
}
```

## License

This project is released under the MIT License.
