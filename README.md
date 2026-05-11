# Spatio Go SDK

The official Go client for the [SpatioAPI](https://www.spatio.app/developers). Notes, sheets, slides, tasks, mail, calendar, channels, DMs, files, contacts, repos, agents, and federated search.

```bash
go get github.com/spatio-labs/spatio-go
```

```go
package main

import (
    "context"
    "fmt"
    "os"

    spatio "github.com/spatio-labs/spatio-go"
)

func main() {
    cfg := spatio.NewConfiguration()
    cfg.Servers = spatio.ServerConfigurations{{URL: "https://api.spatio.app"}}
    cfg.AddDefaultHeader("Authorization", "Bearer "+os.Getenv("SPATIO_PAT"))

    client := spatio.NewAPIClient(cfg)
    envelope, _, err := client.NotesAPI.ListNotes(context.Background()).Execute()
    if err != nil {
        panic(err)
    }
    fmt.Println(envelope.Items)
}
```

## Authentication

Two paths.

**Personal Access Token.** Mint one at *Settings → Tokens* in [Spatio Desktop](https://www.spatio.app) and pass it as a bearer header. The right choice for scripts, automations, and your own backend services.

**OAuth 2.1 + OpenID Connect.** Build a "Sign in with Spatio" flow for your own product. The OIDC discovery document at [`/.well-known/openid-configuration`](https://api.spatio.app/.well-known/openid-configuration) drops into go-oidc, ory/fosite, and every other conformant RP library.

## What you can build

Spatio's API is designed to be the substrate someone could build their own Spatio Desktop on top of. See [CLONE-PARITY.md](https://github.com/spatio-labs/spatio/blob/main/packages/api-spec/CLONE-PARITY.md) for the full surface: realtime collaboration via Yjs, federated cross-platform search, OAuth 2.1 dynamic client registration, self-hosted agent runtime.

## Links

- [SpatioAPI reference](https://www.spatio.app/developers/docs/api)
- [OpenAPI spec](https://api.spatio.app/openapi.json)
- [Clone parity guide](https://github.com/spatio-labs/spatio/blob/main/packages/api-spec/CLONE-PARITY.md)
- [Spatio on the web](https://www.spatio.app)

## About this package

Generated from the SpatioAPI OpenAPI spec on every release. Source mirrored from the [spatio-labs/spatio](https://github.com/spatio-labs/spatio) monorepo: PRs against generated files will be overwritten by the next release. File issues here; open spec changes against the upstream repo.

Licensed under [MIT](LICENSE).
