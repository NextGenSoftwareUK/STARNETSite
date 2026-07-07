# STARNET — The Decentralized App Store of the OASIS Omniverse

**Holon Registry · Asset Store · OASIS Omniverse**

STARNET is the decentralized holon registry and asset store of the OASIS Omniverse. Publish OAPPs, Quests, Missions, NFTs, GeoHotSpots, Worlds, Templates and more — versioned, Avatar-signed, and live in every connected world via the WEB5 STAR API.

## What is STARNET?

STARNET is to the OASIS Omniverse what the App Store is to iOS — but decentralized, permissionless and governed by karma:

- **OAPP Registry** — publish and discover OASIS Applications (OAPPs)
- **Quest & Mission Store** — cross-game quests published by developers and community members
- **GeoHotSpot Registry** — physical GPS locations registered for real-world AR discovery
- **NFT Asset Store** — weapons, skins, pets, templates and world assets for all OASIS games
- **World Templates** — reusable world building blocks for Our World, One World and OGEngine
- **Avatar Signing** — every published asset is cryptographically signed by its creator's OASIS avatar

## Publishing to STARNET

```bash
# via STAR CLI
star publish ./my-oapp --network starnet
star publish-quest ./my-quest.json
star register-hotspot --lat 51.5074 --lng -0.1278 --type keycard
```

## Karma Gate

Publishing to STARNET requires a minimum karma threshold — protecting the registry from spam and ensuring quality contributors.

| Asset Type | Min Karma to Publish |
|---|---|
| OAPP | 5,000 |
| Quest / Mission | 2,500 |
| NFT Asset | 1,000 |
| GeoHotSpot | 500 |
| World Template | 10,000 |

## Related

- [`STARNET`](../STARNET) — the TypeScript source for the STARNET backend
- [`STARWebsite`](../STARWebsite) — the STAR Web5 developer hub
- [`OASIS2`](../OASIS2) — the OASIS API platform

## Tech Stack (Site)

| Layer | Detail |
|---|---|
| Site | Single-file `index.html` — inline CSS + vanilla JS |
| OASIS API | `@oasisomniverse/web4-api@2.0.2` via esm.sh |
| Fonts | Orbitron, Rajdhani, Share Tech Mono (Google Fonts) |

## Running the Site Locally

```bash
npx serve .
# or
python -m http.server 8080
```

---

*Part of the [OASIS Omniverse](https://oasisomniverse.one) · The Decentralized OASIS App Store*
