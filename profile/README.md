# WormholeSystems

A real-time wormhole mapper for EVE Online, live at [wormhole.systems](https://wormhole.systems/). Shared chain maps, signature tracking, mass and lifetime per hole, routing through the chain, live pilot locations and Discord alerts for corporations and alliances living in wormhole space.

## Repositories

| Repository | What it is | Status |
|---|---|---|
| [wormholesystems](https://github.com/wormholesystems/wormholesystems) | The app: Rust (axum, Postgres) and SvelteKit, plus `wsctl` for self-hosting. In beta. | [![CI](https://github.com/wormholesystems/wormholesystems/actions/workflows/ci.yml/badge.svg)](https://github.com/wormholesystems/wormholesystems/actions/workflows/ci.yml) [![last commit](https://img.shields.io/github/last-commit/wormholesystems/wormholesystems)](https://github.com/wormholesystems/wormholesystems/commits) |
| [wormholesystems-legacy](https://github.com/wormholesystems/wormholesystems-legacy) | The original Laravel, Inertia and Vue app, still running at [legacy.wormhole.systems](https://legacy.wormhole.systems/) | [![last commit](https://img.shields.io/github/last-commit/wormholesystems/wormholesystems-legacy)](https://github.com/wormholesystems/wormholesystems-legacy/commits) |
| [wormholesystems-containers](https://github.com/wormholesystems/wormholesystems-containers) | Docker stack for self-hosting the legacy app | |
| [wormholesystems-cli](https://github.com/wormholesystems/wormholesystems-cli) | The legacy `wsctl` that sets that stack up | |

New work happens in [wormholesystems](https://github.com/wormholesystems/wormholesystems). The legacy repositories are kept running but only get fixes.

## Run your own instance

```bash
curl --proto '=https' --tlsv1.2 -sSf https://install-next.wormhole.systems | sh
wsctl setup
```

You need Docker, a domain pointed at the machine and an EVE application from the [developer portal](https://developers.eveonline.com/). `wsctl setup` asks for the rest, runs Postgres and Caddy itself or uses ones you already have, and `wsctl update` keeps the instance current. See the [self-hosting docs](https://github.com/wormholesystems/wormholesystems/blob/main/docs/deployment.md).

## Community and contact

- **Discord**: [Join our Discord](https://discord.gg/rpfWCzVJS7)
- **Email**: [nicolaskion07@gmail.com](mailto:nicolaskion07@gmail.com)
- **Developer**: [NicolasKion](https://github.com/NicolasKion), [nicolaskion.dev](https://nicolaskion.dev)

Bug reports, feature ideas and pull requests are welcome.

## License

MIT, see the individual repositories.
