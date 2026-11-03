# OpenAI plugin

The public ChatGPT plugin is coming soon. Its portable source is [quantux-bidder/](quantux-bidder/), which connects to the hosted MCP service through OAuth.

The plugin name and publisher remain Quantux Bidder and Quantux Labs LLC. Its release version lives in the manifest and is independent of the hosted service and MCP Registry version.

## Package from committed source on Windows

From the public integrations repository root, choose a ZIP path outside the plugin directory:

    git archive --format=zip --prefix=quantux-bidder/ --output=C:\path\to\quantux-bidder.zip HEAD:openai/quantux-bidder
    & "$env:SystemRoot\System32\tar.exe" -tf C:\path\to\quantux-bidder.zip

The only archive root is quantux-bidder/. Include its plugin.json, mcp.json, LICENSE and referenced assets. Keep registry files, review instructions, Git metadata, backend code, credentials and account details outside the archive. Validate the JSON against its declared schemas and check the OpenAI-specific requirements.

The packaged SVG is the product logo; the listing and composer use the accompanying transparent PNG. Keep their geometry consistent with the product artwork.

## Private connection

Import the reviewed package into the intended OpenAI host and connect the existing Bidder account through normal OAuth authorization. Use the host's supported authorization flow without manual scope overrides. Private installed bindings and account credentials stay outside the author-supplied package.

An import or schema check does not establish successful account access or token renewal. Verify the actual connection, tool discovery and a bounded saved read; natural expiry and renewal require their own observation.

## Public review

The manifest owns the review cases. They describe the current tool interface, including shared sessions, user-directed opportunity moves and explicit approval before submission.

Eligible accounts can use the one-time free allowance; paid access is optional and confirmed on the website. Saved reads, professional-context setup and submission recovery remain available without remaining calls or paid access. Public listing descriptions describe functionality; reviewer commerce information explains access. The plugin does not sell or initiate upgrades within ChatGPT.

Prepare a dedicated review account, real sample work and a functioning Freelancer connection. Follow the [recording procedure](review-walkthrough.md), verify the actual recording and add its accessible URL to the review metadata before uploading the final package.

Continue through the existing portal draft, preserving its generated plugin and MCP bindings. Connect and authorize the actual endpoint, inspect imported metadata, run the cases against the saved version and complete scans. Reviewer credentials belong only in the portal's secure access fields. The authorized developer supplies legal attestations. Submission and publication are separate actions.

Source cases and packaging checks are preparation, not evidence of a completed review.

## Official references

- [Package your plugin](https://developers.openai.com/plugins/build/plugins)
- [Upload and submit](https://developers.openai.com/plugins/deploy/submission)
- [Remote MCP review](https://developers.openai.com/plugins/deploy/app-review)
- [Plugin guidelines](https://developers.openai.com/plugins/plugin-guidelines)
