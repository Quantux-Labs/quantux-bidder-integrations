# Quantux Bidder integrations

Public integration metadata and connection instructions for [Quantux Bidder](https://quantux-bidder.quantuxlabs.com).

Quantux Bidder helps you find Freelancer projects, assess opportunities and prepare applications with your AI assistant. Applications follow your direction; submission requires approval of the exact current content and commercial terms.

## Connect

Use an assistant that supports remote MCP servers and OAuth authorization. Add:

    https://quantux-bidder.quantuxlabs.com/mcp

Sign in to Quantux Bidder and authorize the connection when prompted. [Account setup and access](https://quantux-bidder.quantuxlabs.com/account) belong to the website.

## Integrations

- [MCP Registry](mcp-registry/README.md): metadata for the existing hosted server, published as [com.quantuxlabs/quantux-bidder](https://registry.modelcontextprotocol.io/v0.1/servers/com.quantuxlabs%2Fquantux-bidder/versions/latest).
- [OpenAI plugin](openai/README.md): the portable package and review procedure. The public ChatGPT plugin is coming soon.

Each integration has its own manifest and release process. Registry publication provides discovery metadata; provider directories have their own submission and review.

## Source and license

Quantux Labs maintains these files in its private product monorepo and automatically exports this public repository after successful main qualification. Make integration changes in that source; support is available on the [website](https://quantux-bidder.quantuxlabs.com/support).

This repository contains integration material for a separately hosted service. Its files are available under the [MIT License](LICENSE). Registry metadata is additionally subject to the registry's [CC0 dedication](https://modelcontextprotocol.io/registry/terms-of-service).
