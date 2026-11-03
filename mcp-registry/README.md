# MCP Registry

[server.json](server.json) describes the hosted Quantux Bidder MCP server. Its registry identity is [com.quantuxlabs/quantux-bidder](https://registry.modelcontextprotocol.io/v0.1/servers/com.quantuxlabs%2Fquantux-bidder/versions/latest).

The transport is Streamable HTTP at:

    https://quantux-bidder.quantuxlabs.com/mcp

Domain authentication establishes control of the Quantux Labs namespace. The public integration repository is independent of that ownership proof. The standard repository field is omitted because the hosted implementation is private; publisher-provided metadata links the public integration files.

## Validate and publish from Windows

Use the official [mcp-publisher](https://github.com/modelcontextprotocol/registry/tree/main/cmd/publisher) Windows executable from a private operator directory outside Git. Keep signing keys and authentication state there.

After [authenticating for quantuxlabs.com](https://modelcontextprotocol.io/registry/authentication), validate and publish using the manifest's absolute path:

    mcp-publisher validate C:\path\to\quantux-bidder-integrations\mcp-registry\server.json
    mcp-publisher publish C:\path\to\quantux-bidder-integrations\mcp-registry\server.json

[Published metadata is immutable](https://modelcontextprotocol.io/registry/versioning). Choose a new version before publishing a correction, then read the resulting registry record back and verify its name, version and remote address.

The registry version tracks this metadata. Updating the public Git repository neither publishes it to the registry nor deploys the hosted service or provider plugins.
