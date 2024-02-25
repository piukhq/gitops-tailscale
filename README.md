# tailscale-acls

This repo contains our Tailscale ACLs which are modified using a GitOps methodology.

## Visual Studio Code

Visual Studio Code supports a similar `jsonc` (JSON with comments) format. To
treat all `*.hujson` files as `jsonc` with trailing commas allowed, you can add
the following snippet to your Visual Studio Code configuration:

```json
"[jsonc]": {
    "editor.formatOnSave": false
},
"files.associations": {
    "*.hujson": "jsonc"
},
"json.schemas": [
    {
        "fileMatch": [
            "*.hujson"
        ],
        "schema": {
            "allowTrailingCommas": true
        }
    }
]
```
