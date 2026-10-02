# Fork for Claude

Fork connects Claude to sandboxes that your Fork account is authorized to use. You can ask Claude to list those sandboxes, inspect their status and files, make requested file changes, and check a running website preview. The bundled skill guides Claude to identify the right sandbox, read before editing, and verify changes afterward.

## Connect

Install the plugin in Claude and open its **Connectors** tab. Connect **Fork**, then sign in to your Fork account and approve the requested read, write, and browser-preview permissions. You need a Fork account with access to at least one sandbox. Each person connects their own account through OAuth; this package contains no credentials.

The remote connector is `https://agent.fork.site/mcp/public`. Its tools operate on authorized Fork sandboxes, and may send your Fork account identifier and email, sandbox identifiers and hostnames, file paths and contents, edit requests, and website-preview results between Claude and Fork. File edits change the selected sandbox. The plugin contains no local server, executable, hook, or background process. It does not give Fork access to files on your own computer.

## Try it

- “Show the Fork sandboxes I can access.”
- “Read `review-notes.txt` in my Fork sandbox and summarize it.”
- “Change one line in my Fork sandbox, read the file back, and check the website preview.”

Choose a sandbox if Claude finds more than one match. Do not provide passwords, API keys, or environment files in chat. Fork's public file tools exclude secret paths.

## Support and policies

Support: https://fork.site/support  
Privacy: https://fork.site/privacy  
Terms: https://fork.site/terms
