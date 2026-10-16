# OpenAI plugin package

This integration prepares Quantux Bidder for the public plugin directory. Its portable source is in [quantux-bidder/](quantux-bidder/). It connects to the existing hosted MCP service through normal OAuth authorization; it does not deploy the server.

The publisher selected for this submission is **Quantux Labs LLC**. The intended availability is all countries OpenAI permits. Work tools use the account's existing Quantux Bidder trial or subscription purchased on the website.

## Package contents

```text
quantux-bidder/
  LICENSE
  plugin.json
  mcp.json
  assets/
    quantux-bidder-logo.svg
    quantux-bidder-logo.png
```

The ZIP must contain this single plugin directory. Keep the MCP Registry's `server.json`, these preparation notes, Git metadata, backend source, credentials, and recorded account details outside the ZIP.

Version `0.1.0` is the first public plugin release. The plugin name is `quantux-bidder`. Its version is independent of the hosted service and the MCP Registry metadata version.

## Preparation status

- Publisher name, country availability, and website subscription model: confirmed by the publisher.
- Website, support, privacy, and terms destinations: inspected publicly on 2026-10-15.
- Logo: the exact `products/quantux-bidder/public/quantux-bidder-logo.svg` supplied by the publisher is included in `assets/`. The listing and composer icon use a 512 x 512 transparent PNG rendered from that SVG, with its aspect ratio and geometry preserved.
- Five positive and three negative review cases: drafted in `plugin.json` from the supported MCP interface; **not run** against a reviewer account.
- Release notes, commerce explanation, and country availability: declared in `plugin.json`.
- Demo recording and accessible recording URL: **not completed**. Follow the [recording guide](review-walkthrough.md).
- Dedicated reviewer account, working Freelancer connection, sample work, and continuing entitlement: **not verified**. Enter credentials and private instructions only in the portal's secure reviewer-access fields.
- Selected verified identity, actual imported OAuth connection, automated scans, saved review metadata, and legal attestations: **not verified in the submission portal**.

The missing demo URL is intentionally absent from the manifest. Do not substitute a script, placeholder URL, or unverified recording. A structurally valid ZIP is a draft package until the remaining preparation and portal checks are complete. No public review or publication is established by this source.

## Build on Oracle

From the integrations repository root, choose an output path outside `integrations/openai/quantux-bidder/`:

```sh
python3 -m zipfile -c /absolute/output/quantux-bidder-openai-0.1.0-draft.zip integrations/openai/quantux-bidder
```

Inspect the resulting ZIP to confirm its only root is `quantux-bidder/` and that the manifest, MCP connection, and referenced icon are included. Validate the JSON against the exact declared schemas and the OpenAI-specific submission requirements.

After the recording has been verified, add its actual accessible URL to `extensions.com.openai.review.demo_recording_url` and rebuild. Keep test results in preparation evidence, not invented manifest fields.

## Submission sequence

Finish the recording and reviewer account setup first. Then select the intended OpenAI organization, project, and verified publisher; upload the ZIP as a draft; connect and authorize the actual MCP endpoint; inspect imported metadata and run the review cases against the saved version. Complete required scans and have the authorized developer supply legal attestations. Submission for review and publication after approval are separate actions.

The package does not declare an existing private app ID or authentication overrides. Preserve bindings the portal generates in its saved draft and finalized release. Never copy private installed-app configuration into the public author-supplied ZIP.

## References

- [Package your plugin](https://developers.openai.com/plugins/build/plugins)
- [Upload and submit your plugin](https://developers.openai.com/plugins/deploy/submission)
- [Remote MCP review requirements](https://developers.openai.com/plugins/deploy/app-review)
- [Plugin guidelines](https://developers.openai.com/plugins/plugin-guidelines)
