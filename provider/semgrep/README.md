# Semgrep context provider for OpenCtx

This is a sample context provider for [OpenCtx](https://openctx.org) that fetches the contents of a Semgrep finding from a given URL.

## Usage

Add the following to your settings in any OpenCtx client:

```json
"openctx.providers": {
    // ...other providers...
    "https://openctx.org/npm/@openctx/provider-semgrep": {
        "token": "Your <SEMGREP_APP_TOKEN>",
        "repo": "Semgrep repository or project filter"
    }
},
```

You can create and download a `SEMGREP_APP_TOKEN` from <https://semgrep.dev/orgs/-/settings/tokens> under the "API tokens" tab menu option.

The `repo` setting, if provided, filters all the findings in your organization using the provided value.

## Development

- [Source code](https://sourcegraph.com/github.com/sourcegraph/openctx/-/tree/provider/semgrep)
- [Docs](https://openctx.org/docs/providers/semgrep)
- License: Apache 2.0
