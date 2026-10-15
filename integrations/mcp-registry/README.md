# MCP Registry

[server.json](server.json) is the publication manifest for the hosted Quantux Bidder MCP server.

| Field | Value |
| --- | --- |
| Registry name | `com.quantuxlabs/quantux-bidder` |
| Display name | Quantux Bidder |
| Transport | Streamable HTTP |
| Endpoint | `https://api-quantux-bidder.quantuxlabs.com/mcp` |
| Publisher identity | Control of `quantuxlabs.com` |

The manifest lives in this directory because it belongs to the MCP Registry integration. Other integration packages have independent formats and publication processes.

## Ownership and source

Domain authentication authorizes publication under the `com.quantuxlabs/*` namespace. The public integrations repository is independent of that ownership proof. GitHub organization authentication is an alternative for names under `io.github.quantux-labs/*`; it is not required for this listing.

The standard `repository` field is omitted because the hosted server's implementation is maintained separately. The public integrations repository is linked through the custom publisher-provided `integrationsRepository` metadata field; consumers may choose whether to display custom fields.

## Publish a version

Use the official [`mcp-publisher`](https://github.com/modelcontextprotocol/registry/tree/main/cmd/publisher) CLI from a private operator directory outside this repository. Keep the domain signing key and publisher authentication state outside Git.

After [authenticating for `quantuxlabs.com`](https://modelcontextprotocol.io/registry/authentication), publish the manifest by its absolute path:

```sh
mcp-publisher publish /path/to/quantux-bidder-integrations/integrations/mcp-registry/server.json
```

Published version metadata is immutable. Change the manifest's `version` before publishing updated metadata. This version tracks the registry metadata; publishing it does not deploy the hosted service or publish provider plugins.

## References

- [Registry overview](https://modelcontextprotocol.io/registry/about)
- [Remote server manifests](https://modelcontextprotocol.io/registry/remote-servers)
- [Publisher authentication](https://modelcontextprotocol.io/registry/authentication)
- [Publishing automation](https://modelcontextprotocol.io/registry/github-actions)
- [Registry metadata and versions](https://modelcontextprotocol.io/registry/faq)
