# OpenCtx for VS Code

<!-- Published to https://marketplace.visualstudio.com/items?itemName=sourcegraph.openctx -->

Contextual info about code from your dev tools, in your editor. See [openctx.org](https://openctx.org).

![Screenshot of OpenCtx annotations for Storybook in a code file](https://storage.googleapis.com/sourcegraph-assets/blog/screencast-vscode-storybook-v0.gif)

_Hover over a UI component in code to see what it looks like_

## Usage

_Status: experimental_

<!-- Keep in sync with web/content/docs/start.mdx -->

1. Install [OpenCtx for VS Code](https://marketplace.visualstudio.com/items?itemName=sourcegraph.openctx) (`sourcegraph.openctx`).
1. Add the following to your VS Code settings:
      ```json
      "openctx.providers": {
          "https://openctx.org/npm/@openctx/provider-hello-world": true,
      },
      ```
1. Open a code file and look for the "Hello World" items from OpenCtx.
1. Add other OpenCtx providers to see more contextual info about your code:
   - [Links](https://openctx.org/docs/providers/links)
   - [Storybook](https://openctx.org/docs/providers/storybook)
   - [Prometheus](https://openctx.org/docs/providers/prometheus)
   - For more and to write your own, see "[OpenCtx docs](https://openctx.org/docs/start)".

### For extension authors

Use [`@openctx/vscode-lib`](https://www.npmjs.com/package/@openctx/vscode-lib) to incorporate OpenCtx functionality into your own VS Code extension.

## Development

- [Source code](https://sourcegraph.com/github.com/sourcegraph/openctx/-/tree/client/vscode)
- [Docs](https://openctx.org/docs/clients/vscode)
- License: Apache 2.0
