# Review walkthrough

This is a recording plan, not a recorded demo or evidence that the review cases passed. The actual test cases and expected tools live in the packaged [plugin manifest](quantux-bidder/plugin.json).

OpenAI requires a reviewer-accessible video demonstrating the MCP plugin's functionality and review cases. The recording should show real interactions and results in ChatGPT. Include the website setup that explains how the plugin becomes usable, then spend most of the recording on the supported ChatGPT workflow.

## Prepare a dedicated account

Use a dedicated review account with sample data, working email/password sign-in, active Quantux Bidder entitlement, a valid authorized Freelancer connection, and realistic professional context. Prepare the account before asking reviewers to use it. Reviewers should not need to create an account, buy a subscription, generate a Freelancer token, obtain a verification code from the publisher, or access a private network.

Prepare at least one saved session and application for the read-only browsing case. Rehearse discovery with genuine accessible Freelancer opportunities. For the application case, the test user must supply truthful professional evidence, select a real eligible project, and confirm complete feasible commercial terms. An empty discovery result, a fictitious project, or invented eligibility does not demonstrate a successful application workflow.

Use the existing development installation or connection in ChatGPT. Its working state still needs to be confirmed. Do not create a duplicate private plugin or upload an incomplete submission merely to start recording.

## Show the website briefly

1. Open the Quantux Bidder website and identify the product and publisher.
2. Show the prepared account's readiness: existing active entitlement, Freelancer connection status, and sample professional context. Keep unrelated data off screen.
3. Show the plugin connection from ChatGPT, its redirect to Quantux Bidder for sign-in and consent, and the return to ChatGPT.

The official requirements call for functioning review cases and a prepared account; they do not specifically require filming every registration, verification, or checkout form. Prepare those prerequisites beforehand. Keep password entry, verification codes, Freelancer tokens, OAuth tokens, checkout details, and payment cards out of the recording.

The plugin uses an existing subscription entitlement. It must not sell or initiate a digital subscription or promote an upgrade within ChatGPT. Demonstrate access using the prepared account rather than a purchase flow.

## Record the actual cases

Show prompts and returned results clearly. This sequence follows the five positive cases in the manifest:

1. **Read context.** Ask for a summary of saved professional context without changes. Show the actual returned information and the assistant's grounded summary.
2. **Browse saved work.** List saved sessions and applications without acquiring a checkout or changing records.
3. **Discover and assess.** Supply the intended session preferences, create the `OpenAI review` session, read its attention, discover actual Freelancer opportunities, and explain the recorded recommendations and bounded coverage.
4. **Prepare an application.** Select a real eligible opportunity and provide the necessary user decisions and commercial terms. Ask explicitly for an application, show its actual saved content and terms, and release the session. Do not submit a real bid for this demonstration.
5. **Resume the work.** Open a fresh ChatGPT conversation connected to the same dedicated account. Resume the now-unheld session, display the same saved application and current status, and release the checkout.

Demonstrate the three negative cases as separate prompts:

- Request unsupported Upwork work. The assistant explains the supported marketplace without claiming to act there.
- Request invented professional experience. The assistant declines to fabricate credentials and does not write false context or applications.
- Request automatic submission of unseen applications without approval. The assistant explains exact-content approval and does not submit.

Show genuine outcomes, including clarifications or failures. Rehearse and resolve any failed positive case before calling it demonstrated. Do not edit footage or captions to imply an operation succeeded when it did not.

## Record and verify

Use a screen recorder that captures the browser and the relevant ChatGPT conversation. Browser control or screenshots alone do not produce a video. If supported computer control is available, it can help perform the visible steps while the creator records.

Play the saved recording to verify readable prompts and results, successful playback, complete case coverage, and no exposed secrets. Host it at a reviewer-accessible destination chosen by the publisher. Verify actual playback and permissions, then add the real URL to the manifest's `extensions.com.openai.review.demo_recording_url` field and rebuild the ZIP.

Supply reviewer credentials and private sign-in instructions only through the secure submission dashboard. Do not put them in this public guide, the manifest, a GitHub issue, or the recording.
