# Quantux Bidder integrations

Public integration metadata and connection instructions for [Quantux Bidder](https://quantux-bidder.quantuxlabs.com).

Published MCP Registry entry: [`com.quantuxlabs/quantux-bidder`](https://registry.modelcontextprotocol.io/v0.1/servers/com.quantuxlabs%2Fquantux-bidder/versions/0.1.0), version `0.1.0`.

Quantux Bidder helps you find freelance work, assess opportunities, and prepare applications with your AI assistant. Freelancer is the currently supported marketplace. Application work follows your direction, and submission requires your approval.

## Connect to the hosted MCP server

Use an assistant that supports remote MCP servers and OAuth authorization. Add this server address, then sign in to Quantux Bidder and authorize the connection when prompted:

```text
https://api-quantux-bidder.quantuxlabs.com/mcp
```

The server uses Streamable HTTP. Account setup and product information are available on the [Quantux Bidder website](https://quantux-bidder.quantuxlabs.com).

## Repository layout

```text
integrations/
  mcp-registry/
    README.md
    server.json
  openai/
    README.md
    review-walkthrough.md
    quantux-bidder/
      LICENSE
      plugin.json
      mcp.json
      assets/
        icon.png
```

Each integration owns its own files and release process. The [MCP Registry integration](integrations/mcp-registry/README.md) describes the existing hosted server. The [OpenAI plugin package](integrations/openai/README.md) is being prepared for public review and has its own manifest, assets, and recording guide. It does not depend on the registry manifest.

Publishing metadata to the MCP Registry makes it available to registry consumers. Availability in a provider's official directory requires that provider's own publication process.

## Scope and license

This repository contains public integration files for a separately hosted service. The hosted server implementation is maintained separately.

Files in this repository are available under the [MIT License](LICENSE). Metadata submitted to the official MCP Registry is additionally subject to the registry's [CC0 dedication](https://modelcontextprotocol.io/registry/terms-of-service).
