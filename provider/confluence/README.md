# Confluence context provider for OpenCtx

[OpenCtx](https://openctx.org) context provider for bringing Confluence context into code AI and editors.

## Usage

1. [Create an API token](https://id.atlassian.com/manage-profile/security/api-tokens)
2. Configure your OpenCtx client

```json
"openctx.providers": {
    // ...other providers...
    "https://openctx.org/npm/@openctx/provider-confluence": {
        "url": "https://some-org.atlassian.net/wiki",
        "email": "<email-address>",
        "apiToken": "<api-token>",
    }
},
```

## Mention support

- Searches page titles

## Context included

- Page body

## Configuration

- `url` — Confluence URL — Required (e.g. `"https://some-org.atlassian.net/wiki"`)
- `email` — Email — Required
- `apiToken` — API token — Required

## Development

- [Source code](https://sourcegraph.com/github.com/sourcegraph/openctx/-/tree/provider/confluence)
- [Docs](https://openctx.org/docs/providers/confluence)
- License: Apache 2.0

### Local Testing

1. Clone the repo
1. `pnpm install`
1. `pnpm -C provider/confluence bundle --watch` to automatically recompile on changes
1. Run `echo file://$(pwd)/provider/confluence/dist/bundle.js` and use that URL in your OpenCtx instead of `"https://openctx.org/npm/@openctx/provider-confluence"`
1. Reload your OpenCtx client
