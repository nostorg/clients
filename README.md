WIP compilation of nostr clients and supported features.

Contributions welcome. Recommend editing/formatting with [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables).

### Similar projects

- <https://github.com/aljazceru/awesome-nostr>
- <https://github.com/vishalxl/Nostr-Clients-Features-List>
- [Nostr Client Comparison Sheet (Google Docs)](https://docs.google.com/spreadsheets/d/1GjfN_eMiEywqXfKFHZMw4rLnoQLBXYEyl2NCEtsCXWw/edit)
- <https://www.nostrapps.com/>
- <https://nostrapp.link/>

### Legend

- ✅ : mostly supported
- 🟡 : partially supported
- ❌ : mostly not supported
- `?` : checked but unclear
- <code>&nbsp;</code> : not yet checked
- [NIPs](https://github.com/nostr-protocol/nips)

### Table

| Feature (NIP) [Kind] | Open Source | Last Known Version | Web App | Windows App | Linux App | macOS App | iOS App | Android App | Integrated Wallet | Multi Account | View Event Relays | View User Relays | Access Raw/JSON | Follow Hashtags | Global Feed | Trending Feed | Rebroadcast | Translation | Push Notifications | Event Deletion (9) | Report (56) | Mute (~~51~~) [30000] | Mute (51) [10000] | Zaps (57) | Reactions (25) | Microblogging [1] | Direct Message (4) | Chat Rooms (28) | Communities (172) | Long-form Content (23) | Pins (51) [10001] | Bookmarks (51) [30001] | Classifieds (99) | Live Streaming (53) | Badges (58) | Search (12, 50) | Content Warning (36) | Subject Tag (14) | Calendar Events (52) | Marketplaces (15) | Wallet Connect (47) | Nostr Connect (46) | Mnemonic Seed (6) | Proof of Work (13) | Relay Info (11) | Labeling & Reviews (32) |
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
| Gossip | [github](https://github.com/mikedilger/gossip) | 0.7.0 | ❌ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | 🟡 | 🟡 |  | ❌ |  |  |  |  |  | ✅ | ❌ | ? | ? | 🟡 | 🟡 | ✅ | ❌ | ❌ | ❌ | 🟡 |  | ❌ | ? | ❌ | ❌ | 🟡 | ✅ | ✅ |  |  |  |  |  |  |  |  |
| [Lume](https://lume.nu/) | [github](https://github.com/luminous-devs/lume) | 1.1.1 | ❌ | ✅ | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ | ? | ? |  |  |  |  |  |  |  |  | ? | ? |  | 🟡 | ✅ | ✅ | ✅ | ❌ | ? | ? |  | ? | ? | ❌ | ? |  |  |  |  |  |  |  |  |  |  |  |
| Amethyst | [github](https://github.com/vitorpamplona/amethyst) | 0.72.2 | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ | ? | ? |  | ✅ |  |  |  |  |  | ✅ | ✅ | ✅ |  | ✅ | ✅ | ✅ | ✅ | ❌ | ✅ | ✅ |  | ❌ | ✅ | ✅ | ✅ |  | ✅ | ✅ |  | ❌ |  |  | ❌ | ❌ | ✅ |  |
| Nostros | [github](https://github.com/KoalaSat/nostros) | 0.3.2.5 | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ | ❌ | ? | ? | ? |  |  |  |  |  |  |  |  | ? | ? |  | ✅ | ? | ✅ | ✅ | ❌ | ? | ? |  | ✅ | ? | ? | ? |  |  |  |  |  |  |  |  |  |  |  |
| [Plebstr](https://plebstr.com/) | ? | 0.7.6 (56) | ❌ | ❌ | ❌ | 🟡 | ✅ | ✅ | ❌ | ❌ | ❌ | ✅ |  |  |  |  |  | ❌ | ❌ |  | ✅ | ✅ |  | 🟡 | 🟡 | ✅ | ✅ | ❌ | ❌ | ? |  | ❌ | ? | ❌ | ❌ |  |  |  |  |  |  |  |  |  |  |  |
| [Current](https://app.getcurrent.io/) | [github](https://github.com/starbackr-com/current) | 0.0.9 (14) | ❌ | ❌ | ❌ | 🟡 | ✅ | ✅ | ✅ | ❌ | ? | ? |  | ❌ |  |  |  | ? | ✅ |  | ✅ | ✅ |  | ✅ | 🟡 | ✅ | ✅ | ❌ | ❌ | ? |  | ❌ | ? | ❌ | ✅ |  |  |  |  |  |  |  |  |  |  |  |
| [Damus](https://damus.io/) | [github](https://github.com/damus-io/damus) | 1.6 (11) | ❌ | ❌ | ❌ | 🟡 | ✅ | ❌ | ❌ | ❌ | ❌ | ✅ |  | ✅ |  |  |  | ✅ | 🟡 | ❌ | ✅ | ✅ |  | 🟡 | ✅ | ✅ | ✅ | ❌ | ❌ | ✅ |  | ✅ | ? | ❌ | ? | 🟡 | ❌ | ❌ |  |  |  |  |  |  | ✅ |  |
| [Nos](https://www.nos.social/) | [github](https://github.com/planetary-social/nos) | 0.1 (65) | ❌ | ❌ | ❌ | 🟡 | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ |  |  |  |  | ❌ | ? |  | ✅ | ✅ |  | ? | 🟡 | ✅ | ❌ | ❌ | ❌ | ? |  | ❌ | ? | ❌ | ❌ | ? |  |  |  |  |  |  |  |  |  |  |
| [Nostur](https://nostur.com/) | [github](https://github.com/nostur-com/nostur-ios-public) | 1.5.0 (147) | ❌ | ❌ | ❌ | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ | ? | ? |  |  |  |  | ❌ | ❌ |  | ✅ | ✅ |  | 🟡 | 🟡 | ✅ | ✅ | ❌ | ❌ | ✅ |  | ✅ | ? | ❌ | ✅ | ✅ |  |  |  |  |  |  |  |  |  |  |
| [Primal](https://primal.net/) | [github](https://github.com/PrimalHQ) | varies | ✅ | ❌ | ❌ | 🟡 | ✅ | ✅ | ❌ | ❌ | ❌ | ❌ |  |  |  | ✅ | ✅ | ❌ | ❌ | ❌ | ✅ | ❌ | ✅ | 🟡 | 🟡 | ✅ | 🟡 | ❌ | ❌ | ? |  | ❌ | ? | ❌ | ❌ | ✅ | ❌ | ❌ |  |  |  |  |  |  |  |  |
| [Nostrmo](https://github.com/haorendashu/nostrmo_faq) | [github](https://github.com/haorendashu/nostrmo) | 1.8.0 | 🟡 | ✅ | ❌ | ✅ | ✅ | ✅ | ❌ | ✅ | ? | ✅ | ✅ | ✅ | ? | ? | ✅ | 🟡 | ❌ |  | ? | ✅ |  | ✅ | 🟡 | ✅ | ✅ | ❌ | ? | ? |  | ❌ | ? | ❌ | ❌ | 🟡 |  |  |  |  |  |  |  |  |  |  |
| [Iris](https://iris.to/) | [github](https://github.com/irislib/iris-messenger) | 0.2.1 | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ❌ | ❌ | 🟡 | ❌ | ✅ |  |  | ✅ | ✅ | ❌ | ❌ | ✅ | ✅ | ✅ |  | ✅ | 🟡 | ✅ | ✅ | ❌ | ? | ? |  | ❌ | ? | ❌ | ? | ✅ | ❌ | ❌ |  |  |  |  |  |  |  |  |
| [Arcade](https://thearcapp.com/) | [github](https://github.com/ArcadeLabsInc/arcade) | 0.3.2 (1) | ❌ | ❌ | ❌ | ❌ | ✅ | ✅ | ❌ | ❌ | ❌ | ? |  |  |  |  |  |  |  |  | ❌ | ❌ |  | ❌ | ❌ | ❌ | ✅ | ✅ | ? | ? |  | ? | ? | ? |  |  |  |  |  |  |  |  |  |  |  |  |
| [0xchat](https://0xchat.com/) | [github](https://github.com/0xchat-app/0xchat-core) | 1.1.4 | ❌ | ❌ | ❌ | 🟡 | ✅ | ✅ | ❌ | ❌ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | ❌ | ✅ | ✅ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| [ZBD Social](https://blog.zebedee.io/zbd-social-app/) | ? |  |  |  |  |  |  |  | ✅ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| [Snort](https://snort.social/) | [github](https://github.com/v0l/snort) | 0.1.12 | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | N/A | ❌ | ✅ |  |  | ✅ | ✅ |  | ? |  | ✅ | ❌ | ✅ |  | ✅ | 🟡 | ✅ | ✅ | ❌ | ? | ❌ | ✅ | ✅ | ? | ? | ✅ | ✅ | ✅ | ❌ |  |  |  |  |  |  | ✅ |  |
| [Coracle](https://coracle.social/) | [github](https://github.com/coracle-social/coracle) | 0.3.1 | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | N/A | 🟡 | ✅ |  |  | ✅ | ? | ❌ | ❌ |  | ❌ | ❌ | ✅ |  | ✅ | 🟡 | ✅ | ✅ | ✅ | ? | ✅ |  | ? | ? | ❌ | ❌ | 🟡 | ❌ | ❌ |  |  |  |  |  |  | ? | ✅ |
| [Satellite](https://satellite.earth/) | [github](https://github.com/lovvtide/satellite-web) | ? | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | N/A | ? | ? | ✅ |  |  |  |  | ❌ |  |  | ❌ | ❌ |  | 🟡 | 🟡 | ✅ | ✅ | ❌ | ✅ | ❌ |  | ❌ | ? | ❌ | ❌ | 🟡 |  |  |  |  |  |  |  |  |  |  |
| [Zapddit](https://zapddit.com/) | [github](https://github.com/vivganes/zapddit) | ? | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | N/A | ? | ? |  |  |  |  |  |  |  |  | ? | ? |  | ✅ | 🟡 | ✅ | ? | ❌ | ✅ | ? |  | ? | ? | ? |  |  |  |  |  |  |  |  |  |  |  |  |
| [Habla](https://habla.news/) | [github](https://github.com/verbiricha/habla.news) | ? | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | N/A | ? | ? |  |  | ✅ |  |  |  |  |  | ? | ? |  | 🟡 | ? | ✅ | ? | ❌ | ? | ✅ |  | ? | ? | ❌ | ❌ | ? |  |  |  |  |  |  |  |  |  |  |
| [zap.stream](https://zap.stream/) | ? | ? | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | N/A | ? | ? |  |  |  |  |  |  |  |  | ? | ✅ |  | ✅ | ✅ | ❌ | ✅ | ❌ | ? | ❌ |  | ? | ? | ✅ |  |  |  |  |  |  |  |  |  |  |  |  |
| [nostr.band](https://nostr.band/) | [github](https://github.com/nostrband/nostr-band-app) | ? | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | N/A | ✅ | ✅ | ✅ |  |  | ✅ | ❌ |  |  | ❌ |  |  |  | ✅ |  |  |  |  |  | 🟡 |  |  |  | ❌ |  | ✅ | ❌ | ❌ |  |  |  |  |  |  |  |  |
| [YakiHonne](https://yakihonne.com/) | ? | ? | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | ✅ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| [Flycat](https://flycat.club/) | [github](https://github.com/digi-monkey/flycat-web) | 0.2.0 | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | ✅ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
| [noStrudel](https://nostrudel.ninja/) | [github](https://github.com/hzrd149/nostrudel) | ? | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  | ❌ |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |  |
