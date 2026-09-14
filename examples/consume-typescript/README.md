# consume-typescript

Minimal example: consume `traverse-embedder-web` from plain Node.js + TypeScript — no React, no browser.

## Target

**Node.js**, using `NodeFsBundleLoader`. This does *not* run in a browser — the browser path uses `FetchBundleLoader` instead (see `packages/web/TraverseEmbedder/examples/react-integration/` for that).

## Install & run

\`\`\`bash
npm install
npm start
\`\`\`

## Expected output

Prints the events emitted while loading and executing the checked-in `traverse-starter` bundle (`examples/applications/traverse-starter/`), then the final submit status:

\`\`\`
[capability_invoked] {...}
[capability_result] {"status":"completed","output":{...}}

submit status: accepted
\`\`\`
